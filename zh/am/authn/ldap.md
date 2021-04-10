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
maxkey.support.ldap.enable=false
maxkey.support.ldap.jit=false
#openldap,activedirectory,normal
maxkey.support.ldap.product=openldap
maxkey.support.ldap.ssl=false
maxkey.support.ldap.providerurl=ldap://localhost:389
maxkey.support.ldap.principal=cn=Manager,dc=maxcrc,dc=com
maxkey.support.ldap.credentials=secret
maxkey.support.ldap.basedn=dc=maxcrc,dc=com
maxkey.support.ldap.filter=(uid=%s)
maxkey.support.ldap.truststore=maxkey
maxkey.support.ldap.truststorepassword=maxkey
</code></pre>

<h3>Active Directory支持</h3>

<pre><code class="xml hljs">
############################################################################ 
#LDAP Login support configuration                                          #
############################################################################
maxkey.support.ldap.enable=false
maxkey.support.ldap.jit=false
#openldap,activedirectory,normal
maxkey.support.ldap.product=activedirectory
maxkey.support.ldap.ssl=false
maxkey.support.ldap.providerurl=ldap://localhost:389
maxkey.support.ldap.principal=cn=Manager,dc=maxcrc,dc=com
maxkey.support.ldap.credentials=secret
maxkey.support.ldap.basedn=dc=maxcrc,dc=com
maxkey.support.ldap.filter=(uid=%s)
maxkey.support.ldap.truststore=maxkey
maxkey.support.ldap.truststorepassword=maxkey
#activedirectory effective
maxkey.support.ldap.activedirectory.domain=MAXKEY.ORG
</code></pre>

