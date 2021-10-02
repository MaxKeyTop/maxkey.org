---
layout: zh/default
---
<h2>介绍</h2>
为了你更好的使用MaxKey，本教程介绍在Windows中如何快速配置和使用MaxKey，在开始本文档前，请先<a href="https://www.maxkey.top/zh/about/download.html" target="_blank">下载MaxKey</a>并解压到C:盘。

<h2>配置</h2>
hosts配置文件目录
<pre class="prettyprint">
C:\Windows\System32\drivers\etc
</pre>
新增如下内容
<pre><code class="ini hljs">
127.0.0.1  sso.maxkey.top
127.0.0.1  tokenbased.demo.maxkey.top
127.0.0.1  cas.demo.maxkey.top
127.0.0.1  oauth.demo.maxkey.top
</code></pre>

<h2>应用服务启动</h2>
1)启动数据库
<pre><code class="bash hljs">
start_maxkey_db.bat
</code></pre>
2)启动认证服务
<pre><code class="bash hljs">
start_maxkey.bat
</code></pre>
3)启动管理服务
<pre><code class="bash hljs">
start_maxkey_mgt.bat
</code></pre>
4)启动样例及WIKI
<pre><code class="bash hljs">
start_maxkey_wiki.bat
</code></pre>
	
<h2>访问</h2>
打开浏览器，访问以下地址
<table border="0" class="table table-striped table-bordered ">
		<thead>
			<tr>
				<th>序号</th><th>名称</th><th>访问地址</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>1</td><td>认证平台</td><td><a href="https://sso.maxkey.top/maxkey/login" target="blank">https://sso.maxkey.top/maxkey/login</a></td>
			</tr>
			<tr>
				<td>2</td><td>管理平台</td><td><a href="http://sso.maxkey.top:9527/maxkey-mgt/login" target="blank">http://sso.maxkey.top:9527/maxkey-mgt/login</a></td>
			</tr>
			<tr>
				<td>3</td><td>集成指南</td><td><a href="http://sso.maxkey.top:9521/wiki" target="blank">http://sso.maxkey.top:9521/wiki</a></td>
			</tr>
			<tr>
				<td>4</td><td>监控平台</td><td><a href="http://sso.maxkey.top:9528/login" target="blank">http://sso.maxkey.top:9528/login</a></td>
			</tr>
			<tr>
				<td>5</td><td>认证平台接口文档</td><td><a href="https://sso.maxkey.top/maxkey/doc.html" target="blank">https://sso.maxkey.top/maxkey/doc.html</a></td>
			</tr>
			<tr>
				<td>6</td><td>账户密码</td><td>admin/maxkey</td>
			</tr>
			<tr>
				<td>7</td><td>监控账户密码</td><td>monitor/maxkey</td>
			</tr>
		</tbody>
</table>		


<h2>目录结构</h2>
<table border="0" class="table table-striped table-bordered ">
		<thead>
			<tr>
				<th>序号</th><th>目录/文件</th><th>备注</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>1</td><td>MaxKey单点登陆认证系统介绍-CE-***.pdf</td><td>系统介绍</td>
			</tr>
			<tr>
				<td>2</td><td>getting-started.html</td><td>快速使用文档</td>
			</tr>
			<tr>
				<td>3</td><td>LICENSE</td><td>许可证</td>
			</tr>
			<tr>
				<td>4</td><td>NOTICE</td><td>许可证NOTICE</td>
			</tr>
			<tr>
				<td>5</td><td>jdk/jre</td><td>运行时JDK</td>
			</tr>
			<tr>
				<td>6</td><td>lib</td><td>公共包</td>
			</tr>
			<tr>
				<td>7</td><td>maxkey</td><td>认证服务</td>
			</tr>
			<tr>
				<td>8</td><td>maxkey_mgt</td><td>管理服务</td>
			</tr>
			<tr>
				<td>9</td><td>maxkey_monitor</td><td>监控平台</td>
			</tr>
			<tr>
				<td>10</td><td>mysql_***</td><td>MySQL数据库</td>
			</tr>
			<tr>
				<td>11</td><td>maxkey_wiki</td><td>WIKI和样例</td>
			</tr>
			<tr>
				<td>12</td><td>start_maxkey.bat</td><td>启动认证服务器</td>
			</tr>
			<tr>
				<td>13</td><td>start_maxkey_mgt.bat</td><td>启动管理服务器</td>
			</tr>
			<tr>
				<td>14</td><td>start_maxkey_db.bat</td><td>启动数据库</td>
			</tr>
			<tr>
				<td>15</td><td>start_maxkey_monitor.bat</td><td>启动监控服务器</td>
			</tr>
			<tr>
				<td>16</td><td>start_maxkey_wiki.bat</td><td>启动WIKI和样例</td>
			</tr>
			<tr>
				<td>17</td><td>set_maxkey_env.bat</td><td>环境设置脚本</td>
			</tr>
		</tbody>
	</table>

<h2>LINUX 7 版本</h2>

1 OracleJDK 17 安装

1.1 下载地址
https://www.oracle.com/java/technologies/downloads/#JDK17

Java SE Development Kit 17

    x64 RPM Package
	
<pre><code class="bash hljs">	
wget --no-check-certificate --no-cookies wget https://download.oracle.com/java/17/latest/jdk-17_linux-x64_bin.rpm
</code></pre>
 
1.2 解压缩及安装

<pre><code class="bash hljs">
rpm -Uvh jdk-17_linux-x64_bin.rpm
</code></pre>


2.1 安装MySQL 8.0

2.1.1 安装MySQL官方的yum repository

<pre><code class="bash hljs">
wget -i -c https://dev.mysql.com/get/mysql80-community-release-el7-3.noarch.rpm
 </code></pre>
 
2.1.2 下载rpm包：

<pre><code class="bash hljs">
yum -y install mysql80-community-release-el7-3.noarch.rpm
 </code></pre>
 
2.1.3 安装MySQL服务
 
<pre><code class="bash hljs">
yum -y install mysql-community-server
 </code></pre>

 
2.2 调整配置

编辑 /etc/my.cnf 文件

<pre><code class="bash hljs">
character-set-server=utf8
lower_case_table_names=1
</code></pre>
 
2.3. 启动mysql服务

    > systemctl start mysqld
	
	
	停止
	
	systemctl stop mysqld  --无需执行
	
	
2.4 登录MySQL

 第一次启动MySQL后，就会有临时密码，这个默认的初始密码在/var/log/mysqld.log文件中，我们可以用这个命令来查看：
 
 <pre><code class="bash hljs">
 grep "password" /var/log/mysqld.log
 </code></pre>
 
2.5 设置访问权限及密码

<pre><code class="sql hljs">
mysql -u root -p;

输入密码

set global validate_password.policy=0; --改变密码等级

set global validate_password.length=4; --改变密码最小长度

SET PASSWORD = 'maxkey';

use mysql;

alter user 'root'@'localhost' identified with mysql_native_password by 'maxkey';

flush privileges ;

---修改root用户的访问权限为‘%’

update user set host='%' where user='root';

flush privileges ;

</code></pre>
 
2.7. 设置开机启动

<pre><code class="bash hljs">
chkconfig --add mysqld
chkconfig mysqld on
</code></pre>

查看开机启动设置是否成功

<pre><code class="bash hljs">
 chkconfig --list | grep mysql*
 
 # mysqld 0:关闭 1:关闭 2:启用 3:启用 4:启用 5:启用 6:关闭停止
</code></pre>


3 MaxKey安装

3.1 把MaxKey上传到Linux服务器

3.2 数据导入

MaxKey对应的版本SQL文件，参见

https://gitee.com/dromara/MaxKey/tree/master/sql

登陆LINUX MYSQL并创建schema maxkey，字符集utf8,数据文件导入到maxkey schema中，


<pre><code class="sql hljs">
mysql -u root -p;

输入密码

CREATE DATABASE  IF NOT EXISTS `maxkey` /*!40100 DEFAULT CHARACTER SET utf8 */ /*!80016 DEFAULT ENCRYPTION='N' */;

USE `maxkey`;

-- 使用source命令，后面参数为脚本文件(如这里用到的.sql),其中v2.9.0是对应的版本号

source your sql path/maxkey_v3.0.0.GA.sql;

source your sql path/maxkey_v3.0.0.GA_data.sql

</code></pre>


3.3 启动
修改set_maxkey_env.sh以下参数
<pre><code class="bash hljs">
JAVA_HOME=/usr/java/jdk-17

export JAVA_HOME=/usr/java/jdk-17
</code></pre>


<pre><code class="bash hljs">
  ./start_maxkey_db.sh & #自行编写
  
  ./start_maxkey.sh &
  
  ./start_maxkey_mgt.sh &
  
  ./start_maxkey_wiki.sh &
</code></pre>


<h2>Rainbond应用商店快速安装</h2>

[Rainbond](https://github.com/goodrain/rainbond) 是云原生且易用的云原生应用管理平台。通过<a href="https://www.maxkey.top/zh/conf/rainbond.html" target="_blank">Rainbond快速安装</a>
