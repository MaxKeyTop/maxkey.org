---
layout: zh/default
---
<h1>MaxKey概述</h1>
<b>MaxKey</b>单点登录认证系统，谐音为马克思的钥匙寓意是最大钥匙，是<b>业界领先的IAM身份管理和认证产品</b>；支持OAuth 2.x/OpenID Connect、SAML 2.0、JWT、CAS、SCIM等标准协议；提供<i>安全、标准和开放</i>的用户身份管理(IDM)、身份认证(AM)、单点登录(SSO)、资源管理和权限管理等。

官方QQ：<b>1054466084</b> 

邮箱EMAIL: <b>support@maxsso.net</b>
<br/>

代码托管 <a href="https://github.com/dromara/MaxKey" target="_blank"><b>GitHub</b></a> | <a href="https://gitee.com/dromara/MaxKey" target="_blank"><b>码云(Gitee)</b></a>
<br/>


><i>**单点登录(Single Sign On)**简称为**SSO**</i>
>
>用户只需要登录认证中心一次就可以访问所有相互信任的应用系统，无需再次登录，主要功能：
>  
>1.所有应用系统共享一个身份认证系统
>
>2.所有应用系统能够识别和提取ticket信息



<h2>标准协议</h2>

<table border="0" class="table table-striped table-bordered ">
	<tbody>
		<tr class="a">
			<th>序号</th>
			<th>协议</th>
			<th>支持</th>
		</tr>
				
		<tr class="b">
			<td>1 </td>
			<td>OAuth 2.x/OpenID Connect</td>
			<td> 高 </td>
		</tr>
		<tr class="a">
			<td>2 </td>
			<td>SAML 2.0 </td>
			<td>高 </td>
		</tr>  
		<tr class="b">
			<td>3 </td>
			<td>JWT</td>
			<td> 高 </td>
		</tr>
		<tr class="a">
			<td>4 </td>
			<td>CAS</td>
			<td>高 </td>
		</tr>  
		<tr class="b">
			<td>5 </td>
			<td>FormBased</td>
			<td> 中 </td>
		</tr>
		<tr class="a">
			<td>6 </td>
			<td>TokenBased(Post/Cookie)</td>
			<td> 中</td>
		</tr>  
		<tr class="b">
			<td>7 </td>
			<td>ExtendApi</td>
			<td> 低 </td>
		</tr>
		<tr class="a">
			<td>8 </td>
			<td>EXT</td>
			<td> 低</td>
		</tr>  
	</tbody>
</table>
<img src="{{ "/static/images/authz.png" | prepend: site.baseurl }}?{{ site.time | date: "%Y%m%d%H%M" }}"  alt=""/>

<h2>登录支持</h2>

<table border="0" class="table table-striped table-bordered ">
	<tbody>
		<tr class="a">
			<th>序号</th>
			<th>登录方式</th>
			<th>类型</th>
		</tr>
		<tr class="b">
			<td>1 </td>
			<td>图片验证码</td>
			<td>字母/数字/算术</td>
		</tr>
		<tr class="a">
			<td>2 </td>
			<td>双因素认证 </td>
			<td>短信或者邮件动态验证码</td>
		</tr>  
		<tr class="b">
			<td>3 </td>
			<td>短信认证</td>
			<td>腾讯云短信/阿里云短信/网易云信 </td>
		</tr> 
		<tr class="a">
			<td>4 </td>
			<td>TOTP或者HOTP动态口令</td>
			<td>Google/Microsoft Authenticator/FreeOTP/支持TOTP或者HOTP</td>
		</tr>
		<tr class="b">
			<td>5 </td>
			<td>Windows域认证</td>
			<td>Kerberos/SPNEGO/AD域</td>
		</tr>  
		<tr class="b">
			<td>6 </td>
			<td>LDAP认证</td>
			<td>OpenLDAP/ActiveDirectory/标准LDAP服务器</td>
		</tr>  
		<tr class="a">
			<td>7 </td>
			<td>社交账号</td>
			<td>微信/QQ/微博/钉钉/Google/Facebook/其他</td>
		</tr>
		<tr class="b">
			<td>8 </td>
			<td>扫码登录</td>
			<td>企业微信/钉钉/飞书扫码登录</td>
		</tr>
	</tbody>
</table>
<img src="{{ "/static/images/authn.png" | prepend: site.baseurl }}?{{ site.time | date: "%Y%m%d%H%M" }}"  alt=""/>

<h2>优势</h2>

1. 提供标准的认证接口以便于其他应用集成SSO，安全的移动接入，安全的API、第三方认证和互联网认证的整合。

2. 提供用户生命周期管理，支持SCIM 2协议；开箱即用的连接器(Connector)实现身份供给同步。

3. 简化微软Active Directory域控、标准LDAP服务器机构和账号管理，密码自助服务重置密码。

4. 认证多租户功能，支持集团下多企业独立管理或企业下不同部门数据隔离的，降低运维成本。

5. 认证中心具有平台无关性、环境多样性，支持Web、手机、移动设备等, 如Apple iOS，Andriod等，将认证能力从B/S到移动应用全面覆盖。

6. 基于Java EE平台，微服务架构，采用Spring、MySQL、Tomcat、Redis、MQ等开源技术，扩展性强。  

7. 开源、安全、自主可控，许可证 Apache 2.0 License & <a href="https://maxkey.top/zh/about/licenses.html" target="_blank">MaxKey版权声明</a>。 


<h2>最有价值开源项目</h2>
Gitee-最有价值开源项目

<img src="{{ "/static/images/gitee_mvp.png" | prepend: site.baseurl }}?{{ site.time | date: "%Y%m%d%H%M" }}"  width="800px"  alt=""/>