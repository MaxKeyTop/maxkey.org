---
layout: zh/default
---

<h2>基本配置</h2>

<h3>修改端口号</h3>

默认端口是443

1、脚本中修改端口

start_maxkey.bat/start_maxkey.sh

以下示例把端口从443改为9090

<pre><code class="ini hljs">
%JAVA_EXEC% %JAVA_OPTS%  -classpath %JAVA_CLASSPATH% %JAVA_MAINCLASS%  --server.port=9090

</code></pre>

2、配置文件修改端口

MaxKey-v*GA/maxkey/application.properties和在maxkey-web-maxkey*.jar中的application.properties

<pre><code class="ini hljs">
#server port
#server.port=80
server.port=443

</code></pre>


<h3>修改上下文</h3>

MaxKey-v*GA/maxkey/application.properties和在maxkey-web-maxkey*.jar中的application.properties

<pre><code class="ini hljs">
#web app context path
server.servlet.context-path=/maxkey

</code></pre>

修改相关的配置

MaxKey-v*GA/maxkey/maxkey.properties和在maxkey-web-maxkey*.jar中的maxkey.properties

<pre><code class="ini hljs">

############################################################################
#                        MaxKey
############################################################################
#                domain name configuration
config.server.basedomain=maxkey.top
config.server.domain=sso.${config.server.basedomain}
config.server.name=https://${config.server.domain}
config.server.uri=${config.server.name}/maxkey
</code></pre>

<h3>https停用</h3>

MaxKey-v*GA/maxkey/application.properties和在maxkey-web-maxkey*.jar中的application.properties，注释掉以下的内容

<pre><code class="ini hljs">
#ssl
server.ssl.key-store=classpath:maxkeyserver.keystore
server.ssl.key-alias=maxkey
server.ssl.enabled=true
server.ssl.key-store-password=maxkey
server.ssl.key-store-type=JKS
</code></pre>


修改以下文件中的https改为http

MaxKey-v*GA/maxkey/maxkey.properties和在maxkey-web-maxkey*.jar中的maxkey.properties