---
layout: zh/default
---
<h2>JWT应用集成</h2>
本文介绍JWT应用如何与MaxKey进行集成。

<h2>应用注册</h2>

应用在MaxKey管理系统进行注册，注册的配置信息如下

<img src="{{ "/static/images/sso/sso_jwt_conf.png" | prepend: site.baseurl }}?{{ site.time | date: "%Y%m%d%H%M" }}"  alt=""/>

<h2>JWT客户端集成</h2>

本文使用JAVA WEB程序为例

<h3> 第一步，引入客户端所需包</h3>

<pre><code class="ini hljs">
gson-2.2.4.jar
maxkey-client-sdk.jar
nimbus-jose-jwt-8.10.jar
commons-codec-1.9.jar
commons-io-2.2.jar
commons-logging-1.1.1.jar
</code></pre>


<h3> 第二步，获取令牌和用户信息及验证签名</h3>

<pre><code class="jsp hljs">
&lt;%@ page language="java" import="java.util.*" pageEncoding="utf-8"%&gt;
&lt;%@ page language="java" import="org.maxkey.client.oauth.model.*" %&gt;
&lt;%@ page language="java" import="org.maxkey.client.utils.*" %&gt;
&lt;%@ page language="java" import="com.nimbusds.jwt.JWTClaimsSet" %&gt;
&lt;%@ page language="java" import="com.nimbusds.jose.*" %&gt;
&lt;%@ page language="java" import="com.nimbusds.jwt.*" %&gt;
&lt;%@ page language="java" import="com.connsec.oidc.jose.keystore.*" %&gt;
&lt;%@ page language="java" import="com.nimbusds.jose.jwk.*" %&gt;
&lt;%@ page language="java" import="java.io.File" %&gt;
&lt;%@ page language="java" import="com.nimbusds.jose.crypto.*" %&gt;
&lt;%@ page language="java" import="com.google.gson.*" %&gt;
&lt;%
String path = request.getContextPath();
String basePath = request.getScheme()+"://"+request.getServerName()+":"+request.getServerPort()+path+"/";
String token=request.getParameter("jwt");
System.out.println("jwt "+token);
SignedJWT signedJWT=null;
File jwksFile=new File(PathUtils.getInstance().getClassPath()+"jwk.jwks");
JWKSet jwkSet=JWKSet.load(jwksFile);
RSASSAVerifier rsaSSAVerifier = new RSASSAVerifier(((RSAKey) jwkSet.getKeyByKeyId("maxkey_rsa")).toRSAPublicKey());
try {
    signedJWT = SignedJWT.parse(token);
} catch (java.text.ParseException e) {
    // Invalid signed JWT encoding
}
System.out.println("signedJWT "+signedJWT);
JWTClaimsSet jwtClaims =signedJWT.getJWTClaimsSet();
%&gt;
&lt;!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"&gt;
&lt;html&gt;
  &lt;head&gt;
    &lt;base href="&lt;%=basePath%&gt;"&gt;
   &lt;title&gt;JWT 1.0 Demo&lt;/title&gt;
	&lt;meta http-equiv="pragma" content="no-cache"&gt;
	&lt;meta http-equiv="cache-control" content="no-cache"&gt;
	&lt;meta http-equiv="expires" content="0"&gt;    
	&lt;meta http-equiv="keywords" content="keyword1,keyword2,keyword3"&gt;
	&lt;meta http-equiv="description" content="JWT 1.0 Demo"&gt;
	&lt;link rel="shortcut icon" type="image/x-icon" href="&lt;%=basePath %&gt;/images/favicon.ico"/&gt;
	&lt;script type="text/javascript" src="&lt;%=basePath %&gt;/jquery-3.5.0.min.js"&gt;&lt;/script&gt;
	&lt;script type="text/javascript" src="&lt;%=basePath %&gt;/jsonformatter.js"&gt;&lt;/script&gt;
	&lt;link   type="text/css" rel="stylesheet"  href="&lt;%=basePath %&gt;/demo.css"/&gt;	
  &lt;/head&gt;
  &lt;body&gt;
  		&lt;div class="container"&gt;
	  		&lt;table class="datatable"&gt;
	  			&lt;tr&gt;
	  				&lt;td colspan="2" class="title"&gt;JSON Web Token (JWT) 1.0 Demo&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;JWT 1.0 Logo&lt;/td&gt;
	  				&lt;td&gt; &lt;img src="&lt;%=basePath %&gt;/images/jwt.png"  width="124px" height="124px"/&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;Issuer&lt;/td&gt;
	  				&lt;td&gt;&lt;%=jwtClaims.getIssuer() %&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;Subject&lt;/td&gt;
	  				&lt;td&gt;&lt;%=jwtClaims.getSubject()%&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;Audience&lt;/td&gt;
	  				&lt;td&gt;&lt;%=jwtClaims.getAudience() %&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;ExpirationTime&lt;/td&gt;
	  				&lt;td&gt;&lt;%=jwtClaims.getExpirationTime() %&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;JWTID&lt;/td&gt;
	  				&lt;td style="word-wrap: break-word;"&gt;&lt;%=jwtClaims.getJWTID() %&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;IssueTime&lt;/td&gt;
	  				&lt;td style="word-wrap: break-word;"&gt;&lt;%=jwtClaims.getIssueTime() %&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
				&lt;tr&gt;
	  				&lt;td&gt;Verify&lt;/td&gt;
	  				&lt;td style="word-wrap: break-word;"&gt;&lt;%=signedJWT.verify(rsaSSAVerifier) %&gt;&lt;/td&gt;
	  			&lt;/tr&gt;
	  			&lt;tr&gt;
	  				&lt;td&gt;JWTClaims&lt;/td&gt;
	  				&lt;td style="word-wrap: break-word;"&gt;
						&lt;textarea cols="68" rows="20" v-model="text2"&gt;&lt;%=signedJWT.getPayload() %&gt;&lt;/textarea&gt;
					&lt;/td&gt;
	  			&lt;/tr&gt;
	  		&lt;/table&gt;
  		&lt;/div&gt; 
		&lt;script type="text/javascript"&gt;
			FormatTextarea();
		&lt;/script&gt;
  &lt;/body&gt;
&lt;/html&gt;
</code></pre>


<h2>PHP客户端集成</h2>

<h3> 第一步，引入firebase/php-jwt</h3>
<pre><code>composer require firebase/php-jwt
</code></pre>

<h3> 第二步，验证签名</h3>
<pre><code class="php hljs">
&lt;?php
require 'vendor/autoload.php';
use \Firebase\JWT\JWT;
use \Firebase\JWT\Key;

$publicKey = &lt;&lt;&lt;EOD
-----BEGIN PUBLIC KEY-----
MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAvyfZwQuBLNvJDhmziUCF
uAfIv+bC6ivodcR6PfanTt8XLd6G63Yx10YChAdsDACjoLz1tEU56WPp/ee/vcTS
sEZT3ouWJYghuGI2j4XclXlEj0S7DzdpcBBpI4n5dr8K3iKY+3JUMZR1AMBHI50U
aMST9ZTZJAjUPIYxkhRdca5lWBo4wGUh1yj/80+Bq6al0ia9S5NTzNLaJ18jSxFq
Z79BAkBm+KjkP248YUk6WBGtYEAV5Fws4dpse4hrqJ3RRHiMZV1o1iTmPHz/l55Z
SDP3vpYf6iKqKzoK2RmdjfH5mGpbc4+PclTs4GKfwZ7cWfrny6B7sMnQfzujCH99
6QIDAQAB
-----END PUBLIC KEY-----
EOD;

$jwt = $_POST["jwt"];
echo "jwt:\n" .$jwt. "\n";

$decoded = JWT::decode($jwt, new Key($publicKey, 'RS256'));

/*
 * NOTE: This will now be an object instead of an associative array. 
 *	   To get an associative array, you will need to cast it as such:
 */
$decoded_array = (array) $decoded;
echo "Decode:\n" . print_r($decoded_array, true) . "\n";
?&gt;
</code></pre>