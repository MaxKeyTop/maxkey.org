---
layout: default
---
<h2>CAS应用集成</h2>
本文介绍CAS应用如何与MaxKey进行集成。

<h2>应用注册</h2>

应用在MaxKey管理系统进行注册，注册的配置信息如下

<img src="{{ "/images/sso/sso_cas_conf.png" | prepend: site.baseurl }}?{{ site.time | date: "%Y%m%d%H%M" }}"  alt=""/>


<h2>CAS客户端配置</h2>

本文使用JAVA WEB程序为例

jar包依赖如下

https://github.com/MaxKeyTop/MaxKey-Demo/tree/master/maxkey-demo-cas/lib

web.xml配置

https://github.com/MaxKeyTop/MaxKey-Demo/blob/master/maxkey-demo-cas/src/main/webapp/WEB-INF/web.xml

JSP实现Code

https://github.com/MaxKeyTop/MaxKey-Demo/blob/master/maxkey-demo-cas/src/main/webapp/index.jsp

<h2>基于SpringBoot CAS客户端配置</h2>

源代码地址

https://github.com/MaxKeyTop/MaxKey-SpringBoot4CAS-demo


demo分别写了三个请求:拦截请求 test1/index,test1/index1 以及不拦截请求test1/index2,

<h3> 第一步，引入cas 客户端所需包</h3>

<pre><code class="xml hljs">
&lt;dependency&gt;
	&lt;groupId&gt;net.unicon.cas&lt;/groupId&gt;
	&lt;artifactId&gt;cas-client-autoconfig-support&lt;/artifactId&gt;
	&lt;version&gt;2.3.0-GA&lt;/version&gt;
&lt;/dependency&gt;
</code></pre>	  

<h3>第二步，配置spring boot 配置文件</h3>

<pre><code class="ini hljs">
server:
  port: 8989
cas:
  # cas服务端地址
  server-url-prefix: http://sso.maxkey.top/maxkey/authz/cas/
  # cas服务端登陆地址
  server-login-url: http://sso.maxkey.top/maxkey/authz/cas/login
  # 客户端访问地址
  client-host-url: http://localhost:8989/
  # 认证方式，默认cas
  validation-type: cas
  #  客户端需要拦截的URL地址
  authentication-url-patterns:
    - /test1/index
    - /test1/index1
</code></pre>	

扩展配置项
<pre><code class="ini hljs">
cas.authentication-url-patterns
cas.validation-url-patterns
cas.request-wrapper-url-patterns
cas.assertion-thread-local-url-patterns
cas.gateway
cas.use-session
cas.redirect-after-validation
cas.allowed-proxy-chains
cas.proxy-callback-url
cas.proxy-receptor-url
cas.accept-any-proxy
server.context-parameters.renew
</code></pre>

<h3>第三步 在application启动类上加上 @EnableCasClient 注解</h3>

<pre><code class="java hljs">
@SpringBootApplication
@EnableCasClient
public class DemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(DemoApplication.class, args);
    }

}
</code></pre>

<h3>第四步 在代码中获取登录用户信息</h3>

<pre><code class="java hljs">
    @GetMapping("test1/index1")
    public String index1(HttpServletRequest request){
        String token =request.getParameter("token");
        System.out.println("token : "+token);
        Assertion assertion = (Assertion) request.getSession().getAttribute(AbstractCasFilter.CONST_CAS_ASSERTION);

        String username=     assertion.getPrincipal().getName();
        System.out.println(username);

        return "test index cas拦截正常,登录账号:"+username;
    }
</code></pre>
