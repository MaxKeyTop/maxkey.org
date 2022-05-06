---
layout: zh/default
---
<h2>介绍</h2>
Docker 是一个开源的应用容器引擎，让开发者可以打包他们的应用以及依赖包到一个可移植的镜像中，然后发布到任何流行的 Linux或Windows操作系统的机器上，也可以实现虚拟化。

本教程介绍在Docker中如何快速配置和部署MaxKey，在此之前请提前<a target="_blank" href="https://docs.docker.com/engine/install/">安装Docker</a>

MaxKey官方镜像仓库：<a href="https://hub.docker.com/u/maxkeytop" target="_blank">访问</a>

<h2>Docker快速部署</h2>
LINUX 7 基于Docker快速部署

1、创建MySQL数据文件和日志文件目录

<pre><code class="bash hljs">
mkdir /root/mysql/data

mkdir /root/mysql/logs
</code></pre>

2、Docker文件下载

把 https://gitee.com/dromara/MaxKey/tree/master/docker 或者https://github.com/dromara/MaxKey/tree/master/docker目录上传到/root目录下

3、启动MySQL服务
<pre><code class="bash hljs">
docker pull mysql:8.0.27

docker 	run -p 3306:3306  \
-v /root/mysql/data:/var/lib/mysql \
-v /root/mysql/logs:/var/log/mysql \
-v /root/docker-mysql:/etc/mysql/conf.d \
-v /root/docker-mysql/sql:/docker-entrypoint-initdb.d \
--name mysql \
-e MYSQL_ROOT_PASSWORD=maxkey \
-d mysql:8.0.27
</code></pre>

4、启动MaxKey服务

请把<b>DATABASE_HOST</b>为实际地址

<pre><code class="bash hljs">
docker pull maxkeytop/maxkey:3.3.3

docker 	run -p 443:443  \
-e DATABASE_HOST=192.168.0.102 \
-e DATABASE_PORT=3306 \
-e DATABASE_NAME=maxkey \
-e DATABASE_USER=root \
-e DATABASE_PWD=maxkey \
--name maxkey \
-d maxkeytop/maxkey:3.3.3
</code></pre>

5、启动MaxKey管理服务

请把<b>DATABASE_HOST</b>为实际地址

<pre><code class="bash hljs">
docker pull maxkeytop/maxkey-mgt:3.3.3

docker 	run -p 9527:9527  \
-e DATABASE_HOST=192.168.0.102 \
-e DATABASE_PORT=3306 \
-e DATABASE_NAME=maxkey \
-e DATABASE_USER=root \
-e DATABASE_PWD=maxkey \
--name maxkey-mgt \
-d maxkeytop/maxkey-mgt:3.3.3
</code></pre>

<h2>Docker Compose快速部署</h2>
LINUX 7 基于Docker Compose快速部署

1、创建MySQL数据文件和日志文件目录

<pre><code class="bash hljs">
mkdir /root/mysql/data

mkdir /root/mysql/logs
</code></pre>

2、上传并修改Docker配置文件

把 https://gitee.com/dromara/MaxKey/tree/master/docker 或者https://github.com/dromara/MaxKey/tree/master/docker目录上传到/root目录下

以下配置文件中<b>DATABASE_HOST</b>为实际地址

	docker-compose.yml
	
	docker-maxkey/Dockerfile
	
	docker-maxkey-mgt/Dockerfile

3、启动MaxKey服务
<pre><code class="bash hljs">
docker-compose up --build -d
</code></pre>
