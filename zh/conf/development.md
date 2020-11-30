---
layout: zh/default
---
<h2>开发指南</h2>

<h3>开发工具及相关软件</h3>

<table border="0" class="table table-striped table-bordered ">
	<thead>
		<th  >软件</th><th>版本</th><th>备注</th>
	</thead>
	<tbody>
		<tr>
			<td>JDK</td>
			<td>1.8 +</td>
			<td>JAVA运行及开发工具包</td>
		</tr>
		<tr>
			<td>eclipse-jee</td>
			<td>2020-06 +</td>
			<td>推荐JAVA开发工具</td>
		</tr>
		<tr>
			<td>Gradle</td>
			<td>6.5.1 +</td>
			<td>代码构建</td>
		</tr>
		<tr>
			<td>Tomcat/tomcat-embed</td>
			<td> 9 +</td>
			<td>应用服务器</td>
		</tr>
		<tr>
			<td>MySQL Server</td>
			<td>8.0.21 +</td>
			<td>数据库服务器</td>
		</tr>
		<tr>
			<td>Kafka</td>
			<td>2.5.0 +</td>
			<td>用户生命周期管理同步中间件</td>
		</tr>
		<tr>
			<td>Redis</td>
			<td>6 +</td>
			<td>高速缓存内存数据库</td>
		</tr>
		<tr>
			<td>OpenLDAP</td>
			<td>2.2 +</td>
			<td>企业目录服务器</td>
		</tr>
	</tbody>
</table>		
 
<h3>程序目录</h3>

<table border="0" class="table table-striped table-bordered ">
	<thead>
		<th  >MaxKey</th><th>一级目录</th><th>二级目录</th><th>三级目录</th><th>说明</th>
	</thead>
	<tbody>
		<tr>
			<td></td>
			<td>README.md</td>
			<td></td>
			<td></td>
			<td>关于MaxKey项目</td>
		</tr>
		<tr>
			<td></td>
			<td>LICENSE</td>
			<td></td>
			<td></td>
			<td>许可证</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-authentications</td>
			<td></td>
			<td></td>
			<td>登录认证</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-core</td>
			<td></td>
			<td></td>
			<td>基础包</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-identitys</td>
			<td></td>
			<td></td>
			<td>身份管理</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-identity-kafka</td>
			<td></td>
			<td>kafka身份同步，和连接器Connector配合使用</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-identity-rest</td>
			<td></td>
			<td>REST身份管理接口</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-identity-scim</td>
			<td></td>
			<td>SCIM2.0身份管理接口</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-lib</td>
			<td></td>
			<td></td>
			<td>使用jar包</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-persistence</td>
			<td></td>
			<td></td>
			<td>数据库访问</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-protocols</td>
			<td></td>
			<td></td>
			<td>认证协议实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-authorize</td>
			<td></td>
			<td>认证协议实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-cas</td>
			<td></td>
			<td>CAS认证协议实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-desktop</td>
			<td></td>
			<td>桌面认证实现模拟键盘输入登录</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-extendapi</td>
			<td></td>
			<td>扩展API实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-formbased</td>
			<td></td>
			<td>Formbased实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-oauth-2.0</td>
			<td></td>
			<td>oauth-2.0实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-saml-2.0</td>
			<td></td>
			<td>saml-2.0实现</td>
		</tr>
		<tr>
			<td></td>
			<td></td>
			<td>maxkey-protocol-tokenbased</td>
			<td></td>
			<td>tokenbased实现</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-web-manage</td>
			<td></td>
			<td></td>
			<td>管理系统</td>
		</tr>
		<tr>
			<td></td>
			<td>maxkey-web-maxkey</td>
			<td></td>
			<td></td>
			<td>认证系统</td>
		</tr>
		<tr>
			<td></td>
			<td>shellscript</td>
			<td></td>
			<td></td>
			<td>Window和LINUX启动脚本</td>
		</tr>
		<tr>
			<td></td>
			<td>sql</td>
			<td></td>
			<td></td>
			<td>数据库MYSQL脚步,GA版本对应SQL</td>
		</tr>
		<tr>
			<td></td>
			<td>checkstyle</td>
			<td></td>
			<td></td>
			<td>编码规范配置</td>
		</tr>
		<tr>
			<td></td>
			<td>build.gradle</td>
			<td></td>
			<td></td>
			<td>工程构建及版本控制</td>
		</tr>
		<tr>
			<td></td>
			<td>gradle.properties</td>
			<td></td>
			<td></td>
			<td>版本参数配置</td>
		</tr>
		<tr>
			<td></td>
			<td>settings.gradle</td>
			<td></td>
			<td></td>
			<td>项目引入</td>
		</tr>
		<tr>
			<td></td>
			<td>ReleaseNotes.txt</td>
			<td></td>
			<td></td>
			<td>GA版本描述</td>
		</tr>
		<tr>
			<td></td>
			<td>gradle</td>
			<td></td>
			<td></td>
			<td>gradle的配置</td>
		</tr>
		<tr>
			<td></td>
			<td>setEnvVars.bat</td>
			<td></td>
			<td></td>
			<td>JDK及Gradle路径配置，用于构建脚本，需要开发人员自行配置</td>
		</tr>
		<tr>
			<td></td>
			<td>release.bat</td>
			<td></td>
			<td></td>
			<td>清除历史构建版本</td>
		</tr>
		<tr>
			<td></td>
			<td>eclipsePluginApply.bat</td>
			<td></td>
			<td></td>
			<td>设置IDE</td>
		</tr>
		<tr>
			<td></td>
			<td>eclipsePluginClean.bat</td>
			<td></td>
			<td></td>
			<td>清除IDE的设置</td>
		</tr>		
		</tbody>
</table>

<h3>开发环境应用启动</h3>

MaxKey统一认证系统

maxkey-web-maxkey/src/main/java/org/maxkey/MaxKeyApplication.java 

MaxKey身份安全管理系统

maxkey-web-manage/src/main/java/org/maxkey/MaxKeyMgtApplication.java


<h3>工程构建BuildRelease</h3>

1. 配置环境变量

setEnvVars.bat

set JAVA_HOME=D:\JavaIDE\jdk1.8.0_91

set GRADLE_HOME=D:\JavaIDE\gradle-5.4.1


2. 启动构建

release.bat


3. 构建结果

构建包路径

MaxKey/build/maxkey-jars

依赖包路径

MaxKey/build/maxkey-depjars


<h3>Docker 构建release</h3>

1. Docker 构建配置

maxkey-web-manage/build.gradle增加以下配置

<pre><code class="ini hljs">
plugins {
	id 'com.google.cloud.tools.jib' version '2.6.0'
	id 'org.springframework.boot' version '2.3.4.RELEASE'
}

jib {
	from {
		image = 'adoptopenjdk:11-jre-openj9'
	}
	to {
		image = "maxkey/maxkey-mgt"
		tags = ["${project.version}".toString(), 'latest']
	}
	container {
		jvmFlags = ['-Dfile.encoding=utf-8', '-Dserver.port=80']
		ports = ['80']
	}
}
</code></pre>

maxkey-web-maxkey/build.gradle增加以下配置

<pre><code class="ini hljs">
plugins {
	id 'com.google.cloud.tools.jib' version '2.6.0'
	id 'org.springframework.boot' version '2.3.4.RELEASE'
}

jib {
	from {
		image = 'adoptopenjdk:11-jre-openj9'
	}
	to {
		image = "maxkey/maxkey"
		tags = ["${project.version}".toString(), 'latest']
	}
	container {
		jvmFlags = ['-Dfile.encoding=utf-8', '-Dserver.port=80']
		ports = ['80']
	}
}
</code></pre>

2. 启动构建

release.bat


3. 构建的结果

maxkey-web-manage/

maxkey-web-maxkey/



<h3>问题及解决</h3>
问题1

“A cycle was detected in the build path of project: XXX” 

解决方法：
 
Eclipse Menu -> Window -> Preferences... -> Java -> Compiler -> Building -> Building path problems -> Circular dependencies -> 将Error改成Warning

问题2

Access restriction

解决方案：

Eclipse Menu -> Window -> Preferences... -> Java -> Compiler ->  Errors/Warnings界面的Deprecated and restricted API下。把Forbidden reference (access rules): 的规则由默认的Error改为Warning即可。
