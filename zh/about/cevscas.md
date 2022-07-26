---
layout: zh/default
---

<h2>MaxKey和Keycloak/CAS对比</h2>

<table border="0" class="table table-striped table-bordered ">
	<thead>
		<th>模块</th><th>功能</th><th>MaxKey</th><th>Keycloak</th><th>Apereo CAS</th>
	</thead>
	<tbody>
		<tr>
			<td>标准协议</td>
			<td>OpenID Connect 1.0</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>插件</td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>OAuth v2.0/2.1</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>插件</td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>SAML V2.0</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>插件</td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>CAS 1.0/2.0/3.0</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>JWT</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>定制</td>
			<td>定制</td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>TOKEN令牌支持</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>密码代填(FORMBASED)支持</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>API扩展支持</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>标准协议</td>
			<td>扩展定制支持</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>定制</td>
			<td>定制</td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-图片验证码</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>定制</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-短信验证码</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-TOTP动态令牌</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>定制</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-邮件验证码</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-社交账号登陆</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-企业微信、钉钉扫码登陆</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-双因素认证</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>定制</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-Active Directory用户登录</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-OpenLDAP用户登录</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户登录-Windows域认证</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>登录注销</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td> 应用访问权限控制</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>定制</td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>密码修改</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>密码过期修改</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>首次登陆密码修改</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>找回密码</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>安全配置</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>用户信息修改</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>社交账号绑定</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>主题切换</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td>时间令牌</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>插件</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td> 应用账号管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td> 多种设备支持</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td> 用户登录日志</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td> 应用访问日志</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>认证服务</td>
			<td> 管理日志</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>机构管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>用户管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>账号管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>应用管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>访问控制-角色管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>访问控制-角色成员管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>访问控制-访问控制管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>权限管理-资源管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>权限管理-权限管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>配置管理-同步器管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>配置管理-适配器管理</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>配置管理-密码策略</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>管理服务</td>
			<td>管理端单点登录</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>REST接口机构和用户同步</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>SCIM2接口机构和用户同步</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>KAFKA同步支持</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td >生命周期管理</td><td colspan="5">同步器把存在上游系统的机构和账号同步到MaxKey</td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>Active Directory同步器</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>标准LDAP同步器</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>企业微信同步器</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>钉钉同步器</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td >生命周期管理</td><td colspan="5">连接器把MaxKey的机构和账号同步到下游系统</td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>Active Directory连接器</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>标准LDAP连接器</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>企业微信连接器</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>钉钉连接器</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>飞书连接器</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>生命周期管理</td>
			<td>华为WeLink连接器</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>日志审计</td>
			<td>统计报表</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>日志审计</td>
			<td>管理日志审计</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>日志审计</td>
			<td>登录日志审计</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>日志审计</td>
			<td>应用访问日志审计</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>日志审计</td>
			<td>连接器日志审计</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td>日志审计</td>
			<td>同步器日志审计</td>
			<td><div class="icon"><i class="fa fa-lock" style="color:red;"></i></div></td>
			<td></td>
			<td></td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>其他</td>
			<td>JAVA SDK<br/>.NET SDK</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>其他</td>
			<td>支持多平台<br/>Windows<br/>LINUX<br/>UNIX</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>其他</td>
			<td>支持主流浏览器：<br/>Google Chrome <br/>Mozilla Firefox <br/> Internet Explorer 10 <br/>Microsoft Edge <br/>等</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>其他</td>
			<td>支持PC、平板PAD、手机Moblie</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td>其他</td>
			<td>开发集成指南</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>产品文档及安装配置(集群)</td>
			<td><div class="icon">开源社区</div></td>
			<td><div class="icon">开源社区</div></td>
			<td><div class="icon">开源社区</div></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>版本升级及BUG修复</td>
			<td>开源社区</td>
			<td>开源社区</td>
			<td>开源社区</td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>在线技术支持</td>
			<td>官方QQ</td>
			<td><div class="icon"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>集成解决方案咨询</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>技术培训</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>定制开发支持</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>客户化界面定制</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td>客户服务</td>
			<td>紧急故障修复</td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
			<td><div class="icon"><i class="fa fa-window-close" style="color:red;"></i></div></td>
		</tr>
		<tr>
			<td colspan="5"></td>
		</tr>
		<tr>
			<td>团队</td>
			<td>研发团队</td>
			<td>国内<div class="icon" style="float: left;"><i class="fa fa-check-square" style="color:#009999;"></i></div></td>
			<td>国外</td>
			<td>国外</td>
		</tr>
		<tr>
			<td>授权标识</td>
			<td><a href="{{site.baseurl}}/zh/about/licenses.html">许可证声明</a></td>
			<td><div class="icon">不可忽略</div></td>
			<td><div class="icon">不可忽略</div></td>
			<td><div class="icon">不可忽略</div></td>
		</tr>
	</tbody>
</table>
