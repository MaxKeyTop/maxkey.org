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

http默认端口为80，https默认端口为443

MaxKey-v*GA/maxkey/和在maxkey-web-maxkey*.jar中的application-(http/https).properties

<pre><code class="ini hljs">
#server port
#server.port=80
server.port=443

</code></pre>

<h3>https停用</h3>

http默认端口为80，https默认端口为443

MaxKey-v*GA/maxkey/application.properties和在maxkey-web-maxkey*.jar中的application.properties，注释掉以下的内容

<pre><code class="ini hljs">
#spring.profiles.active=https
spring.profiles.active=http
</code></pre>


<h3>修改上下文</h3>

MaxKey-v*GA/maxkey/和在maxkey-web-maxkey*.jar中的application-(http/https).properties

<pre><code class="ini hljs">
#web app context path
server.servlet.context-path=/maxkey

</code></pre>

修改相关的配置 /maxkey 为新的路径



