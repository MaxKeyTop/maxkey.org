---
layout: zh/default
---
<h2>高可用性High Availability</h2>

架构Architecture

<img src="{{ "/static/images/maxkey_ha.png" | prepend: site.baseurl }}?{{ site.time | date: "%Y%m%d%H%M" }}"  alt=""/>



<h2>高可用性配置</h2>

1、准备两台服务器，并安装MaxKey

2、准备Redis作为缓存

3、修改配置文件

MaxKey-v*GA/maxkey/application.properties和在maxkey-web-maxkey*.jar中的application.properties。

Redis配置

<pre><code class="ini hljs">
#redis
spring.redis.host=127.0.0.1
spring.redis.port=6379
spring.redis.password=password
spring.redis.timeout=10000
spring.redis.jedis.pool.max-wait=1000
spring.redis.jedis.pool.max-idle=200
spring.redis.lettuce.pool.max-active=-1
spring.redis.lettuce.pool.min-idle=0
</code></pre>

启动Sessions存储在Redis配置

<pre><code class="ini hljs">
# Session store type.
spring.session.store-type=redis
# Session timeout. If a duration suffix is not specified, seconds is used.
server.servlet.session.timeout=1800
# Sessions flush mode.
spring.session.redis.flush-mode=on_save 
# Namespace for keys used to store sessions.
spring.session.redis.namespace=spring:session 
</code></pre>

4、Nginx转发配置

  请参照Nginx官方网站完成配置