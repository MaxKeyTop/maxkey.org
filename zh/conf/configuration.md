---
layout: zh/default
---

<h2>端口配置</h2>

<table border="0" class="table table-striped table-bordered ">
		<thead>
			<tr>
				<th>序号</th><th>服务</th><th>文件目录</th><th>上下文</th><th>端口</th>
			</tr>
		</thead>
		<tbody>
        <tr>
                            <td>1</td>
                            <td>认证服务</td>
                            <td>maxkey</td>
                            <td>/sign</td>
                            <td>9527</td>
                        </tr>
                        <tr>
                            <td>2</td>
                            <td>认证前端服务</td>
                            <td>maxkey_frontend</td>
                            <td>/maxkey</td>
                            <td>8527</td>
                        </tr>
                        <tr>
                            <td>4</td>
                            <td>管理服务</td>
                            <td>maxkey_mgt</td>
                            <td>maxkey_mgt_api</td>
                            <td>9526</td>
                        </tr>
                        <tr>
                            <td>5</td>
                            <td>管理前端服务</td>
                            <td>maxkey_mgt_frontend</td>
                            <td>/maxkey_mgt</td>
                            <td>8526</td>
                        </tr>
                        <tr>
                            <td>6</td>
                            <td>nginx反向代理服务</td>
                            <td>nginx-version-proxy</td>
                            <td>/</td>
                            <td>80</td>
                        </tr>
                        <tr>
                            <td>7</td>
                            <td>监控服务</td>
                            <td>maxkey_monitor</td>
                            <td>/</td>
                             <td>9528</td>
                        </tr>
                        <tr>
                            <td>8</td>
                            <td>MySQL数据库</td>
                            <td>mysql_***</td>
                            <td></td>
                            <td>3306</td>
                        </tr>
                        <tr>
                            <td>9</td>
                            <td>样例</td>
                            <td>maxkey_demo</td>
                            <td>/</td>
                            <td>9521</td>
                        </tr>
                    </tbody>
	</table>

<h3>修改端口号</h3>

认证服务默认端口是9527

1、脚本中修改端口

start_maxkey.bat/start_maxkey.sh

以下示例把端口从9527改为9090

<pre><code class="ini hljs">
%JAVA_EXEC% %JAVA_OPTS%  -classpath %JAVA_CLASSPATH% %JAVA_MAINCLASS%  --server.port=9090

</code></pre>

2、配置文件修改端口

http默认端口为9527，https默认端口为9090

MaxKey-v*GA/maxkey/和在maxkey-web-maxkey*.jar中的application-(http/https).properties

<pre><code class="ini hljs">
#server port
#server.port=9527
server.port=9090

</code></pre>

<h3>环境配置</h3>

MaxKey-v*GA/maxkey/application.properties和在maxkey-web-maxkey*.jar中的application.properties，注释掉以下的内容，其中application-prod.properties是生产配置文件

<pre><code class="ini hljs">
#spring.profiles.active=http
spring.profiles.active=prod
</code></pre>


<h3>修改上下文</h3>

MaxKey-v*GA/maxkey/和在maxkey-web-maxkey*.jar中的application-(http/https).properties

<pre><code class="ini hljs">
#web app context path
server.servlet.context-path=/sign

</code></pre>

修改相关的配置 /sign 为新的路径


<h3>前端及代理服务配置</h3>

请参照Nginx端口配置
