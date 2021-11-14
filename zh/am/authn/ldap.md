---
layout: zh/default
---
<h2>LDAP登录集成</h2>
MaxKey支持LDAP包括Active Directory。


<h3>注释默认数据库认证</h3>

配置文件maxkey/application-https(http).properties

<h3>LDAP支持</h3>

<pre><code class="xml hljs">
############################################################################ 
#LDAP Login support configuration                                          #
############################################################################
maxkey.login.ldap.enable=false
maxkey.login.ldap.jit=false
#openldap,activedirectory,normal
maxkey.login.ldap.product=openldap
maxkey.login.ldap.ssl=false
maxkey.login.ldap.providerurl=ldap://localhost:389
maxkey.login.ldap.principal=cn=Manager,dc=maxcrc,dc=com
maxkey.login.ldap.credentials=secret
maxkey.login.ldap.basedn=dc=maxcrc,dc=com
maxkey.login.ldap.filter=(uid=%s)
maxkey.login.ldap.truststore=maxkey
maxkey.login.ldap.truststorepassword=maxkey
</code></pre>

<h3>Active Directory支持</h3>

<pre><code class="xml hljs">
############################################################################ 
#LDAP Login support configuration                                          #
############################################################################
maxkey.login.ldap.enable=false
maxkey.login.ldap.jit=false
#openldap,activedirectory,normal
maxkey.login.ldap.product=activedirectory
maxkey.login.ldap.ssl=false
maxkey.login.ldap.providerurl=ldap://localhost:389
maxkey.login.ldap.principal=cn=Manager,dc=maxcrc,dc=com
maxkey.login.ldap.credentials=secret
maxkey.login.ldap.basedn=dc=maxcrc,dc=com
maxkey.login.ldap.filter=(uid=%s)
maxkey.login.ldap.truststore=maxkey
maxkey.login.ldap.truststorepassword=maxkey
#activedirectory effective
maxkey.login.ldap.activedirectory.domain=MAXKEY.ORG
</code></pre>

