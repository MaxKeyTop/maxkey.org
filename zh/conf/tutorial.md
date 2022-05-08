---
layout: zh/default
---
<h2>介绍</h2>
为了你更好的使用MaxKey，本教程介绍在Windows中如何快速配置和使用MaxKey，在开始本文档前，请先<a href="https://www.maxkey.top/zh/about/download.html" target="_blank">下载MaxKey</a>并解压到C:盘。

<h2>目录结构</h2>
<table border="0" class="table table-striped table-bordered ">
    <thead>
        <tr>
            <th>序号</th><th>目录/文件</th><th>备注</th>
        </tr>
    </thead>
    <tbody>
                    <tr>
                        <td>1</td>
                        <td>MaxKey单点登陆认证系统介绍-CE-***.pdf</td>
                        <td>系统介绍</td>
                    </tr>
                    <tr>
                        <td>2</td>
                        <td>getting-started.html</td>
                        <td>快速使用文档</td>
                    </tr>
                    <tr>
                        <td>3</td>
                        <td>LICENSE</td>
                        <td>许可证</td>
                    </tr>
                    <tr>
                        <td>4</td>
                        <td>NOTICE</td>
                        <td>许可证NOTICE</td>
                    </tr>
                    <tr>
                        <td>5</td>
                        <td>jdk/jre</td>
                        <td>运行时JDK</td>
                    </tr>
                    <tr>
                        <td>6</td>
                        <td>lib</td>
                        <td>公共包</td>
                    </tr>
                    <tr>
                        <td>7</td>
                        <td>maxkey</td>
                        <td>认证服务,端口9527</td>
                    </tr>
                    <tr>
                        <td>8</td>
                        <td>maxkey_frontend</td>
                        <td>认证前端服务,端口8527</td>
                    </tr>
                    <tr>
                        <td>9</td>
                        <td>maxkey_mgt</td>
                        <td>管理服务,端口9526</td>
                    </tr>
                    <tr>
                        <td>10</td>
                        <td>maxkey_mgt_frontend</td>
                        <td>管理前端服务,端口8526</td>
                    </tr>
                    <tr>
                        <td>11</td>
                        <td>nginx-1.20.1-proxy</td>
                        <td>nginx反向代理服务,端口80</td>
                    </tr>
                    <tr>
                        <td>12</td>
                        <td>maxkey_monitor</td>
                        <td>监控平台,端口9528</td>
                    </tr>
                    <tr>
                        <td>13</td>
                        <td>mysql_***</td>
                        <td>MySQL数据库,端口3306</td>
                    </tr>
                    <tr>
                        <td>14</td>
                        <td>maxkey_demo</td>
                        <td>样例,端口9521</td>
                    </tr>
                    <tr>
                        <td>15</td>
                        <td>start_maxkey.bat</td>
                        <td>启动认证服务器</td>
                    </tr>
                    <tr>
                        <td>16</td>
                        <td>start_maxkey_frontend.bat</td>
                        <td>启动认证前端服务器</td>
                    </tr>
                    <tr>
                        <td>17</td>
                        <td>start_maxkey_mgt.bat</td>
                        <td>启动管理服务器</td>
                    </tr>
                    <tr>
                        <td>18</td>
                        <td>start_maxkey_mgt_frontend.bat</td>
                        <td>启动管理前端服务器</td>
                    </tr>
                    <tr>
                        <td>19</td>
                        <td>start_maxkey_db.bat</td>
                        <td>启动数据库</td>
                    </tr>
                    <tr>
                        <td>20</td>
                        <td>start_maxkey_proxy.bat</td>
                        <td>启动代理服务器</td>
                    </tr>
                    <tr>
                        <td>21</td>
                        <td>start_maxkey_monitor.bat</td>
                        <td>启动监控服务器</td>
                    </tr>
                    <tr>
                        <td>22</td>
                        <td>start_maxkey_demo.bat</td>
                        <td>启动样例</td>
                    </tr>
                    <tr>
                        <td>23</td>
                        <td>set_maxkey_env.bat</td>
                        <td>环境设置脚本</td>
                    </tr>
                </tbody>
    </table>
    
<a  name="windows"></a>

<h2>Windows 版本</h2>
<h2>配置</h2>
hosts配置文件目录
<pre class="prettyprint">
C:\Windows\System32\drivers\etc
</pre>
新增如下内容
<pre><code class="ini hljs">
127.0.0.1  sso.maxkey.top
127.0.0.1  mgt.maxkey.top
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

4)启动认证前端服务
<pre><code class="bash hljs">
start_maxkey_frontend.bat
</code></pre>
                
5)启动管理前端服务
<pre><code class="bash hljs">
start_maxkey_mgt_frontend.bat
</code></pre>

6)启动代理
<pre><code class="bash hljs">
start_maxkey_proxy.bat
</code></pre>
				
7)启动样例
<pre><code class="bash hljs">
start_maxkey_demo.bat
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
                            <td>1</td>
                            <td>认证平台</td>
                            <td><a href="http://sso.maxkey.top/maxkey/"
                                    target="blank">http://sso.maxkey.top/maxkey/login</a></td>
                        </tr>
                        <tr>
                            <td>2</td>
                            <td>管理平台</td>
                            <td><a href="http://mgt.maxkey.top/maxkey-mgt/"
                                    target="blank">http://mgt.maxkey.top/maxkey-mgt/login</a></td>
                        </tr>
                        <tr>
                            <td>3</td>
                            <td>集成指南</td>
                            <td><a href="http://doc.maxkey.top/" target="blank">http://doc.maxkey.top/</a></td>
                        </tr>
                        <tr>
                            <td>4</td>
                            <td>监控平台</td>
                            <td><a href="http://sso.maxkey.top:9528/login"
                                    target="blank">http://sso.maxkey.top:9528/login</a></td>
                        </tr>
                        <tr>
                            <td>5</td>
                            <td>账户密码</td>
                            <td>admin/maxkey</td>
                        </tr>
                        <tr>
                            <td>6</td>
                            <td>监控账户密码</td>
                            <td>monitor/maxkey</td>
                        </tr>
                    </tbody>
</table>		


<a name="linux"></a>

<h2>LINUX 7 版本</h2>

1 JDK 安装

<table border="0" class="table table-striped table-bordered ">
	<thead>
		<tr>
			<th>推荐</th><th>版本</th><th>更新至</th><th>地址</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>Oracle JDK 8</td>
			<td>December 2030</td>
			<td><a href="https://www.oracle.com/java/technologies/downloads/#JDK17">访问</a></td>
			
		</tr>
		<tr>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>Eclipse Temurin 8</td>
			<td>December 2030</td>
			<td><a href="https://adoptium.net/?variant=openjdk8&jvmVariant=hotspot">访问</a></td>
			
		</tr>
		<tr>
			<td></td>
			<td>OracleJDK 17</td>
			<td>October 2029</td>
			<td><a href="https://www.oracle.com/java/technologies/downloads/#java8">访问</a></td>
		</tr>
		<tr>
			<td></td>
			<td>Eclipse Temurin 17</td>
			<td>October 2029</td>
			<td><a href="https://adoptium.net/?variant=openjdk17&jvmVariant=hotspot">访问</a></td>
			
		</tr>
	</tbody>
</table>

1.1 下载地址

Eclipse Temurin 8  x64 RPM Package

假设当前安装目录/root
	
<pre><code class="bash hljs">
curl -L "https://github.com/adoptium/temurin8-binaries/releases/download/jdk8u332-b09/OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz" -H "Cookie: oraclelicense=accept-securebackup-cookie"  -H "Connection: keep-alive" -O  
</code></pre>
 
1.2 解压缩及安装

<pre><code class="bash hljs">
tar -zxf OpenJDK8U-jdk_x64_linux_hotspot_8u332b09.tar.gz
</code></pre>

完成后本地目录

<pre><code class="bash hljs">
jdk8u332-b09
</code></pre>

2.1 安装MySQL 8.0

假如本地安装过mariadb，请先卸载

2.1.1 安装MySQL官方的yum repository

<pre><code class="bash hljs">
curl -L  "https://dev.mysql.com/get/mysql80-community-release-el7-3.noarch.rpm"  -O 
 </code></pre>
 
2.1.2 下载rpm包：

<pre><code class="bash hljs">
yum -y install mysql80-community-release-el7-3.noarch.rpm
 </code></pre>
 
2.1.3 安装MySQL服务
 
<pre><code class="bash hljs">
yum -y install mysql-community-server
 </code></pre>

2.1.4 安装MySQL问题

<pre><code class="bash hljs">
Failing package is: mysql-community-libs-compat-8.0.28-1.el7.x86_64  GPG Keys are configured as: file:///etc/pki/rpm-gpg/RPM-GPG-KEY-mysql
</code></pre>

解决方案
<pre><code class="bash hljs">
rpm --import https://repo.mysql.com/RPM-GPG-KEY-mysql-2022
</code></pre>

2.2 调整配置

编辑 /etc/my.cnf 文件

<pre><code class="bash hljs">
character-set-server=utf8
lower_case_table_names=1
</code></pre>
 
2.3. 启动mysql服务

    systemctl start mysqld
	
	--停止
	
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

--以下步骤可能要求先修改初始化密码为复杂密码 SET PASSWORD = 'UDF(ez/8Lufi';

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

https://gitee.com/dromara/MaxKey/tree/master/sql/v3.5.0.ga/

登陆LINUX MYSQL并创建schema maxkey，字符集utf8,数据文件导入到maxkey schema中，


<pre><code class="sql hljs">
mysql -u root -p;

输入密码

CREATE DATABASE  IF NOT EXISTS `maxkey` /*!40100 DEFAULT CHARACTER SET utf8 */ /*!80016 DEFAULT ENCRYPTION='N' */;

USE `maxkey`;

-- 使用source命令，后面参数为脚本文件(如这里用到的.sql),其中v3.5.0是对应的版本号

source your sql path/maxkey_v3.5.0.GA.sql;

source your sql path/maxkey_v3.5.0.GA_data.sql

</code></pre>


3.3 配置
hosts配置文件目录
<pre class="prettyprint">
vi /etc/hosts
</pre>
新增如下内容
<pre><code class="ini hljs">
127.0.0.1  sso.maxkey.top
127.0.0.1  mgt.maxkey.top
127.0.0.1  tokenbased.demo.maxkey.top
127.0.0.1  cas.demo.maxkey.top
127.0.0.1  oauth.demo.maxkey.top
</code></pre>

3.4 启动
修改set_maxkey_env.sh以下参数，/root/为安装路径
<pre><code class="bash hljs">
JAVA_HOME=/root/jdk8u332-b09

export JAVA_HOME=/root/jdk8u332-b09
</code></pre>


<pre><code class="bash hljs">
  ./start_maxkey_db.sh & #自行编写
  
  ./start_maxkey.sh &
  
  ./start_maxkey_mgt.sh &
  
  ./start_maxkey_demo.sh &
</code></pre>

<h2>前端服务部署</h2>

安装nginx,参考windows版本配置，再把windows版本前端文件放入对应的nginx目录下

<h2>代理服务部署</h2>

安装nginx,参考windows版本的代理配置

<h2>Docker快速部署</h2>

<a href="https://www.maxkey.top/zh/conf/deploy_docker.html" target="_blank">基于Docker快速部署</a>


<h2>Rainbond应用商店快速安装</h2>

<a href="https://www.maxkey.top/zh/conf/deploy_rainbond.html" target="_blank">Rainbond快速安装</a>，[Rainbond](https://github.com/goodrain/rainbond) 是云原生且易用的云原生应用管理平台。


<h2><a href="./tutorial_v3.3.html">v3.3 部署介绍</a></h2>