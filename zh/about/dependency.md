---
layout: zh/default
---
<h3>项目依赖</h3>
<h3>项目软件</h3>

<table border="0" class="table table-striped table-bordered ">
    <thead>
        <tr>
            <th>SoftWare</th>
			<th>Version</th>
            <th>Introduction</th>
            <th>Home</th>
            <th>License</th></tr>
    </thead>
    <tbody>
        <tr>
            <td>MySQL Community Server</td>
			<td>8.0.*</td>
            <td>
			MySQL is the most trusted and widely used open source database platform in use today. 10 out of the top 10 most popular and highly-trafficked websites in the world rely on MySQL. 
			</td>
            <td>https://www.mysql.com/</td>
            <td>GNU General Public License v2.0</td>
		</tr>
		<tr>
            <td>PostgreSQL </td>
			<td>13.6.*</td>
            <td>
			PostgreSQL is a powerful, open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.
			</td>
            <td>https://www.postgresql.org/</td>
            <td>PostgreSQL License</td>
		</tr>
		<tr>
            <td>OpenJDK</td>
			<td>14</td>
            <td>
			The place to collaborate on an open-source implementation of the Java Platform, Standard Edition, and related projects,open-source JDK for most popular Linux distributions. Oracle's free, GPL-licensed, production-ready OpenJDK JDK 14 binaries are at jdk.java.net/14; Oracle's commercially-licensed JDK 14 binaries for Linux, macOS, and Windows, based on the same code
			</td>
            <td>http://openjdk.java.net/</td>
            <td>GNU General Public License v2.0</td>
		</tr>
		<tr>
            <td>Node.js</td>
			<td>Node.js v16.13.1</td>
            <td>
			Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.

			</td>
            <td>https://nodejs.org/</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>Tomcat/Tomcat-embed</td>
			<td>9.0.*</td>
            <td>
			The Apache Tomcat® software is an open source implementation of the Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket technologies. The Java Servlet, JavaServer Pages, Java Expression Language and Java WebSocket specifications are developed under the Java Community Process.
			</td>
            <td>https://tomcat.apache.org/</td>
            <td>Apache License 2.0</td>
		</tr>
		<tr>
            <td>nginx</td>
			<td>1.21.*</td>
            <td>
			nginx [engine x] is an HTTP and reverse proxy server, a mail proxy server, and a generic TCP/UDP proxy server, originally written by Igor Sysoev.
			</td>
            <td>http://nginx.org/</td>
            <td>2-clause BSD-like license</td>
		</tr>
		
		<tr>
            <td>Redis</td>
			<td>6.0.*</td>
            <td>
			Redis is an open source (BSD licensed), in-memory data structure store, used as a database, cache and message broker. It supports data structures such as strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, geospatial indexes with radius queries and streams. Redis has built-in replication, Lua scripting, LRU eviction, transactions and different levels of on-disk persistence, and provides high availability via Redis Sentinel and automatic partitioning with Redis Cluster
			</td>
            <td>https://redis.io/</td>
            <td>BSD licensed</td>
		</tr>
		<tr>
            <td>OpenLDAP</td>
			<td>4.4.*</td>
            <td>
			OpenLDAP Software is an open source implementation of the Lightweight Directory Access Protocol.
			</td>
            <td>https://www.openldap.org/</td>
            <td>OpenLDAP Public License</td>
		</tr>
		<tr>
            <td>Apache Kafka</td>
			<td>2.5.0</td>
            <td>
			Kafka® is used for building real-time data pipelines and streaming apps. It is horizontally scalable, fault-tolerant, wicked fast, and runs in production in thousands of companies.

			</td>
            <td>https://kafka.apache.org/</td>
            <td>Apache License 2.0</td>
		</tr>
		<tr>
            <td>Apache RocketMQ</td>
			<td>4.9.*</td>
            <td>
			Apache RocketMQ™ is a unified messaging engine, lightweight data processing platform.

			</td>
            <td>https://rocketmq.apache.org/</td>
            <td>Apache License 2.0</td>
		</tr>
		<tr>
            <td>Gradle</td>
			<td>7.*</td>
            <td>
			Gradle is an open-source build automation tool focused on flexibility and performance. Gradle build scripts are written using a Groovy or Kotlin DSL. Read about Gradle features to learn what is possible with Gradle.

			</td>
            <td>https://gradle.org/</td>
            <td>Apache License 2.0</td>
		</tr>
		<tr>
            <td>Eclipse</td>
			<td>eclipse-jee-2020-06</td>
            <td>
			The Eclipse IDE is famous for our Java Integrated Development Environment (IDE), but we have a number of pretty cool IDEs, including our C/C++ IDE, JavaScript/TypeScript IDE, PHP IDE, and more.

			</td>
            <td>https://www.eclipse.org/</td>
            <td>Eclipse Public License - v 2.0</td>
		</tr>
		<tr>
            <td>Visual Studio Code</td>
			<td>VSCode Version 1.66</td>
            <td>
			Visual Studio Code is a lightweight but powerful source code editor which runs on your desktop and is available for Windows, macOS and Linux

			</td>
            <td>https://code.visualstudio.com/</td>
            <td>MIT license </td>
		</tr>
		
    </tbody>
</table>	


<h3>项目依赖包</h3>

以下是此项目的项目依赖中的编译依赖项列表。这些依赖项可以包含在子模块中，以编译和运行子模块：

<table border="0" class="table table-striped table-bordered ">
    <thead>
        <tr>
            <th>Dependency</th>
            <th>GroupId</th>
            <th>ArtifactId</th>
            <th>Version</th>
            <th>Type</th>
            <th>License</th></tr>
    </thead>
    <tbody>
        <tr>
            <td>test</td>
            <td>junit</td>
            <td>junit</td>
            <td>{{site.junitVersion}}</td>
            <td>jar</td>
            <td>EPL 1.0</td></tr>
        <tr>
            <td>test</td>
            <td>javax.servlet</td>
            <td>javax.servlet-api</td>
            <td>3.0.1</td>
            <td>jar</td>
            <td>GPL 2.0</td></tr>
        <tr>
            <td>test</td>
            <td>org.mockito</td>
            <td>mockito-all</td>
            <td>{{site.mockitoallVersion}}</td>
            <td>jar</td>
            <td>MIT</td></tr>
        <tr>
            <td>test</td>
            <td>xmlunit</td>
            <td>xmlunit</td>
            <td>{{site.xmlunitVersion}}</td>
            <td>jar</td>
            <td>BSD</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-beanutils</td>
            <td>commons-beanutils</td>
            <td>{{site.commonsbeanutilsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-codec</td>
            <td>commons-codec</td>
            <td>{{site.commonscodecVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-collections</td>
            <td>commons-collections</td>
            <td>{{site.commonscollectionsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-collections4</td>
            <td>{{site.commonscollections4Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-compress</td>
            <td>{{site.commonscompressVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>	
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-csv</td>
            <td>{{site.commonscsvVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>org.apache.commons </td>
            <td>commons-text</td>
            <td>{{site.commonstextVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-dbcp2</td>
            <td>{{site.commonsdbcp2Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-dbutils</td>
            <td>commons-dbutils</td>
            <td>{{site.commonsdbutilsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-digester3</td>
            <td>{{site.commonsdigester3Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-digester</td>
            <td>commons-digester</td>
            <td>{{site.commonsdigesterVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-io</td>
            <td>commons-io</td>
            <td>{{site.commonsioVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-lang</td>
            <td>commons-lang</td>
            <td>{{site.commonslangVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-lang3</td>
            <td>{{site.commonslang3Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-logging</td>
            <td>commons-logging</td>
            <td>{{site.commonsloggingVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-pool2</td>
            <td>{{site.commonspool2Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-httpclient</td>
            <td>commons-httpclient</td>
            <td>{{site.commonshttpclientVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>commons-fileupload</td>
            <td>commons-fileupload</td>
            <td>{{site.commonsfileuploadVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>commons-email</td>
            <td>{{site.commonsemailVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.httpcomponents</td>
            <td>httpclient</td>
            <td>{{site.httpcomponentsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.httpcomponents</td>
            <td>fluent-hc</td>
            <td>{{site.httpcomponentsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.httpcomponents</td>
            <td>httpclient-cache</td>
            <td>{{site.httpcomponentsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.httpcomponents</td>
            <td>httpmime</td>
            <td>{{site.httpcomponentsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.httpcomponents</td>
            <td>httpcore</td>
            <td>{{site.httpcoreVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.velocity</td>
            <td>velocity</td>
            <td>{{site.velocityVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>velocity</td>
            <td>velocity-dep</td>
            <td>{{site.velocitydepVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.freemarker</td>
            <td>freemarker</td>
            <td>{{site.freemarkerVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.commons</td>
            <td>not-yet-commons-ssl</td>
            <td>0.3.9</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td> org.apache.poi</td>
            <td>
				poi              <br/>
				poi-scratchpad   <br/>
				poi-ooxml        <br/>
				poi-ooxml-schemas
				</td>
            <td>{{site.poiVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>	

		<tr>
            <td>compile</td>
            <td> org.apache.xmlbeans</td>
            <td>xmlbeans</td>
            <td>{{site.xmlbeansVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>	

        <tr>
            <td>compile</td>
            <td>org.apache.logging.log4j</td>
            <td>
				log4j-1.2-api    <br/>
				log4j-api        <br/>
				log4j-core       <br/>
				log4j-jcl        <br/>
				log4j-jul        <br/>
				log4j-slf4j-impl <br/> 
				log4j-web
			</td>
            <td>{{site.log4jVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.slf4j</td>
            <td>slf4j-api</td>
            <td>{{site.slf4jVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.jboss.logging</td>
            <td>jboss-logging</td>
            <td>{{site.jbossloggingVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.springframework</td>
            <td>
				spring-aop                  <br/>
				spring-aspects              <br/>
				spring-beans                <br/>
				spring-core                 <br/>
				spring-context              <br/>
				spring-context-indexer      <br/>
				spring-context-support      <br/>
				spring-expression           <br/>
				spring-instrument           <br/>
				spring-jcl                  <br/>
				spring-jdbc                 <br/>
				spring-jms                  <br/>
				spring-messaging            <br/>
				spring-orm                  <br/>
				spring-oxm                  <br/>
				spring-tx                   <br/>
				spring-web                  <br/>
				spring-webflux              <br/>
				spring-webmvc               <br/>
				spring-websocket            <br/>
				spring-test
			</td>
            <td>{{site.springVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.kafka</td>
            <td>kafka-clients</td>
            <td>{{site.kafkaclientsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.springframework.kafka</td>
            <td>spring-kafka</td>
            <td>{{site.springkafkaVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.springframework.retry</td>
            <td>spring-retry</td>
            <td>{{site.springretryVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.springframework.security</td>
            <td>
				spring-security-core<br/>
				spring-security-web<br/>
				spring-security-crypto
			</td>
            <td>{{ site.springSecurityVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.springframework.boot</td>
            <td>
				spring-boot<br/>
				spring-boot-starter<br/>
				spring-boot-actuator<br/>
				spring-boot-autoconfigure<br/>
				spring-boot-starter-freemarker<br/>
				spring-boot-starter-log4j2<br/>
				spring-boot-starter-web<br/>
				spring-boot-starter-tomcat<br/>
				spring-boot-starter-test
			</td>
            <td>{{ site.springBootVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td>
		</tr>
		
		<tr>
            <td>compile</td>
            <td>org.springframework.security</td>
            <td>spring-security-oauth</td>
            <td>2.5.1</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td>
		</tr>	
		<tr>
            <td>compile</td>
            <td>org.springframework.data</td>
            <td>
				spring-data-commons<br/>
				spring-data-keyvalue<br/>
				spring-data-redis
				</td>
            <td>{{ site.springDataVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>	
		
		<tr>
            <td>compile</td>
            <td>org.springframework.plugin</td>
            <td>spring-plugin-core</td>
            <td>{{ site.springplugincoreVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>		
		<tr>
            <td>compile</td>
            <td>org.springframework.plugin</td>
            <td>spring-plugin-metadata</td>
            <td>{{ site.springpluginmetadataVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>org.springframework.session</td>
            <td>spring-session-core</td>
            <td>{{ site.springSessionVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
	    <tr>
            <td>compile</td>
            <td>org.springframework.session</td>
            <td>spring-session-data-redis</td>
            <td>{{ site.springSessionVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.opensaml</td>
            <td>opensaml</td>
            <td>{{site.opensamlVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.opensaml</td>
            <td>openws</td>
            <td>{{site.openwsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.opensaml</td>
            <td>xmltooling</td>
            <td>{{site.xmltoolingVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>net.shibboleth.utilities</td>
            <td>java-support</td>
            <td>{{site.javasupportVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>	
        <tr>
            <td>compile</td>
            <td>com.nimbusds</td>
            <td>nimbus-jose-jwt</td>
            <td>{{site.nimbusjosejwtVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>net.jcip</td>
            <td>jcip-annotations</td>
            <td>{{site.jcipannotationsVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>net.minidev</td>
            <td>json-smart</td>
            <td>{{site.minidevjsonsmartVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>net.minidev</td>
            <td>asm</td>
            <td>{{site.minidevasmVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.xkcoding.http</td>
            <td>simple-http</td>
            <td>{{site.simplehttpVersion}}</td>
            <td>jar</td>
            <td>LGPL 3.0</td></tr>
        <tr>
            <td>compile</td>
            <td>me.zhyd.oauth</td>
            <td>JustAuth</td>
            <td>{{site.JustAuthVersion}}</td>
            <td>jar</td>
            <td>MIT</td></tr>
        <tr>
            <td>compile</td>
            <td>org.javassist</td>
            <td>javassist</td>
            <td>{{site.javassistVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.owasp.esapi</td>
            <td>esapi</td>
            <td>{{site.esapiVersion}}</td>
            <td>jar</td>
            <td>BSD 2-clause</td></tr>
        <tr>
            <td>compile</td>
            <td>com.sun.mail</td>
            <td>javax.mail</td>
            <td>{{site.javaxmailVersion}}</td>
            <td>jar</td>
            <td>GPL 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.eclipse.persistence</td>
            <td>javax.persistence</td>
            <td>{{site.javaxpersistenceVersion}}</td>
            <td>jar</td>
            <td>Eclipse Public License v. 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.activation</td>
            <td>activation</td>
            <td>{{site.activationVersion}}</td>
            <td>jar</td>
            <td>CDDL 1.0</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.annotation</td>
            <td>javax.annotation-api</td>
            <td>{{site.javaxannotationapiVersion}}</td>
            <td>jar</td>
            <td>GPLv2</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.transaction</td>
            <td>jta</td>
            <td>{{site.jtaVersion}}</td>
            <td>jar</td>
            <td>GPLv2</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.transaction</td>
            <td>javax.transaction-api</td>
            <td>{{site.javaxtransactionapiVersion}}</td>
            <td>jar</td>
            <td>GPLv2</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.validation</td>
            <td>validation-api</td>
            <td>{{site.validationapiVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.xml</td>
            <td>jsr173</td>
            <td>{{site.jsr173Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>javax.xml.bind</td>
            <td>jaxb-api</td>
            <td>{{site.jaxbapiVersion}}</td>
            <td>jar</td>
            <td>CDDL 1.1</td></tr>
        <tr>
            <td>compile</td>
            <td>com.sun.xml.bind</td>
            <td>jaxb-core</td>
            <td>{{site.jaxbcoreVersion}}</td>
            <td>jar</td>
            <td>Eclipse Distribution License - v 1.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.sun.xml.bind</td>
            <td>jaxb-impl</td>
            <td>{{site.jaxbimplVersion}}</td>
            <td>jar</td>
            <td>Eclipse Distribution License - v 1.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.sun.xml.bind</td>
            <td>jaxb-xjc</td>
            <td>{{site.jaxbxjcVersion}}</td>
            <td>jar</td>
            <td>Eclipse Distribution License - v 1.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.bouncycastle</td>
            <td>bcpkix-jdk15on</td>
            <td>{{site.bouncycastleVersion}}</td>
            <td>jar</td>
            <td>Bouncy Castle Licence</td></tr>
        <tr>
            <td>compile</td>
            <td>org.bouncycastle</td>
            <td>bcprov-jdk15on</td>
            <td>{{site.bouncycastleVersion}}</td>
            <td>jar</td>
            <td>Bouncy Castle Licence</td></tr>
        <tr>
            <td>compile</td>
            <td>org.bouncycastle</td>
            <td>bcprov-ext-jdk15on</td>
            <td>{{site.bouncycastleVersion}}</td>
            <td>jar</td>
            <td>Bouncy Castle Licence</td></tr>
        <tr>
            <td>compile</td>
            <td>com.google.crypto.tink</td>
            <td>tink</td>
            <td>{{site.tinkVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.jhlabs</td>
            <td>filters</td>
            <td>{{site.jhlabsfiltersVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.github.penggle</td>
            <td>kaptcha</td>
            <td>{{site.kaptchaVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.google.code.gson</td>
            <td>gson</td>
            <td>{{site.gsonVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.fasterxml.jackson.core</td>
            <td>
				jackson-annotations <br/>
				jackson-core        <br/>
				jackson-databind
			</td>
            <td>{{site.jacksonVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
       
        <tr>
            <td>compile</td>
            <td>com.fasterxml</td>
            <td>classmate</td>
            <td>{{site.classmateVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.alibaba</td>
            <td>fastjson</td>
            <td>{{site.fastjsonVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.reactivestreams</td>
            <td>reactive-streams</td>
            <td>{{site.reactivestreamsVersion}}</td>
            <td>jar</td>
            <td>CC0 1.0</td></tr>
        <tr>
            <td>compile</td>
            <td>io.projectreactor</td>
            <td>reactor-core</td>
            <td>{{site.reactorcoreVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>eu.tekul</td>
            <td>szxcvbn_2.9.2</td>
            <td>{{site.szxcvbnVersion}}</td>
            <td>jar</td>
            <td>MIT</td></tr>
        <tr>
            <td>compile</td>
            <td>org.quartz-scheduler</td>
            <td>quartz</td>
            <td>{{site.quartzVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>mysql</td>
            <td>mysql-connector-java</td>
            <td>{{site.mysqlconnectorjavaVersion}}</td>
            <td>jar</td>
            <td>GPL 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>org.postgresql</td>
            <td>postgresql</td>
            <td>{{site.postgresqlVersion}}</td>
            <td>jar</td>
            <td>BSD-2-Clause</td></tr>	
        <tr>
            <td>compile</td>
            <td>com.alibaba</td>
            <td>druid</td>
            <td>{{site.druidVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.alibaba</td>
            <td>druid-spring-boot-starter</td>
            <td>{{site.druidspringbootstarterVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>redis.clients</td>
            <td>jedis</td>
            <td>{{site.jedisVersion}}</td>
            <td>jar</td>
            <td>MIT</td></tr>
        <tr>
            <td>compile</td>
            <td>org.ehcache</td>
            <td>ehcache</td>
            <td>{{site.ehcacheVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.mybatis</td>
            <td>mybatis</td>
            <td>{{site.mybatisVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.mybatis</td>
            <td>mybatis-spring</td>
            <td>{{site.mybatisspringVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.hibernate.validator</td>
            <td>hibernate-validator</td>
            <td>{{site.hibernateVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.hibernate</td>
            <td>hibernate-validator-cdi</td>
            <td>{{site.hibernateVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.hibernate.validator</td>
            <td>hibernate-validator-annotation-processor</td>
            <td>{{site.hibernateVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>joda-time</td>
            <td>joda-time</td>
            <td>{{site.jodatimeVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.yaml</td>
            <td>snakeyaml</td>
            <td>1.26</td>
            <td>{{site.snakeyamlVersion}}</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>net.sourceforge.nekohtml</td>
            <td>nekohtml</td>
            <td>{{site.nekohtmlVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.jdom</td>
            <td>jdom</td>
            <td>{{site.jdomVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.google.zxing</td>
            <td>core</td>
            <td>{{site.zxingcoreVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.google.guava</td>
            <td>guava</td>
            <td>{{site.guavaVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>ognl</td>
            <td>ognl</td>
            <td>{{site.ognlVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>cglib</td>
            <td>cglib</td>
            <td>{{site.cglibVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.ow2.asm</td>
            <td>asm</td>
            <td>{{site.asmVersion}}</td>
            <td>jar</td>
            <td>BSD 3-clause</td></tr>
        <tr>
            <td>compile</td>
            <td>aopalliance</td>
            <td>aopalliance</td>
            <td>{{site.aopallianceVersion}}</td>
            <td>jar</td>
            <td>Public</td></tr>
        <tr>
            <td>compile</td>
            <td>org.aspectj</td>
            <td>aspectjtools</td>
            <td>{{site.aspectjtoolsVersion}}</td>
            <td>jar</td>
            <td>EPL 1.0</td></tr>
        <tr>
            <td>compile</td>
            <td>dom4j</td>
            <td>dom4j</td>
            <td>{{site.dom4jVersion}}</td>
            <td>jar</td>
            <td>BSD</td></tr>
        <tr>
            <td>compile</td>
            <td>xalan</td>
            <td>serializer</td>
            <td>{{site.serializerVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>xml-resolver</td>
            <td>xml-resolver</td>
            <td>{{site.xmlresolverVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.santuario</td>
            <td>xmlsec</td>
            <td>{{site.xmlsecVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.ogce</td>
            <td>xpp3</td>
            <td>{{site.xpp3Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>com.thoughtworks.xstream</td>
            <td>xstream</td>
            <td>{{site.xstreamVersion}}</td>
            <td>jar</td>
            <td>BSD 3-clause</td></tr>
		<tr>
            <td>compile</td>
            <td>org.passay</td>
            <td>passay</td>
            <td>{{site.passayVersion}}</td>
            <td>jar</td>
            <td>Apache 2.0 & LGPL 3.0</td></tr>	
		<tr>
            <td>compile</td>
            <td>io.micrometer</td>
            <td> micrometer-core</td>
            <td>{{site.micrometercoreVersion}}</td>
            <td>jar</td>
            <td>Apache 2.0 </td></tr>	
		<tr>
            <td>compile</td>
            <td>org.latencyutils</td>
            <td> LatencyUtils</td>
            <td>{{site.LatencyUtilsVersion}}</td>
            <td>jar</td>
            <td>CC0 1.0 </td></tr>	
		<tr>
            <td>compile</td>
            <td>org.codehaus.woodstox</td>
            <td> stax2-api</td>
            <td>{{site.stax2apiVersion}}</td>
            <td>jar</td>
            <td>	BSD 2-clause </td></tr>	
		<tr>
            <td>compile</td>
            <td>org.mapstruct</td>
            <td> mapstruct</td>
            <td>{{site.mapstructVersion}}</td>
            <td>jar</td>
            <td>Apache 2.0 </td></tr>	
        <tr>
            <td>compile</td>
            <td>com.aliyun</td>
            <td>aliyun-java-sdk-core</td>
            <td>{{site.aliyunjavasdkcoreVersion}}</td>
            <td>jar</td>
            <td>Aliyun </td></tr>
        <tr>
            <td>compile</td>
            <td>com.tencentcloudapi</td>
            <td>tencentcloud-sdk-java</td>
            <td>{{site.tencentcloudsdkjavaVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.tomcat.embed</td>
            <td>tomcat-embed-core</td>
            <td>{{site.tomcatVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
        <tr>
            <td>compile</td>
            <td>org.apache.tomcat.embed</td>
            <td>tomcat-embed-logging-juli</td>
            <td>{{site.tomcatembedloggingjuliVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		 <tr>
            <td>compile</td>
            <td>mybatis-jpa-extra</td>
            <td>mybatis-jpa-extra</td>
            <td>2.3</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>mybatis-jpa-extra</td>
            <td>mybatis-jpa-extra-spring-boot-starter</td>
            <td>6.0.4.jre8</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>com.highgo</td>
            <td>HgdbJdbc</td>
            <td>2.3</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>gradle.plugin.com.google.cloud.tools</td>
            <td>jib-gradle-plugin</td>
            <td>{{site.jibGradlePluginVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>io.swagger</td>
            <td>swagger-annotations<br/>
				swagger-models</td>
            <td>{{site.swaggerVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>
		<tr>
            <td>compile</td>
            <td>io.swagger.core.v3</td>
            <td>
				swagger-annotations<br/>
				swagger-core<br/>
				swagger-integration<br/>
				swagger-models<br/>
			</td>
            <td>{{site.swaggerV3Version}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>	
		<tr>
            <td>compile</td>
            <td>io.springfox</td>
            <td>
				springfox-bean-validators<br/>
				springfox-core<br/>
				springfox-data-rest<br/>
				springfox-spi<br/>
				springfox-oas<br/>
				springfox-schema<br/>
				springfox-swagger2<br/>
				springfox-swagger-ui<br/>
				springfox-swagger-common<br/>
				springfox-spring-webmvc<br/>
				springfox-spring-web<br/>
				springfox-spring-webflux<br/>
				springfox-boot-starter
			</td>
            <td>{{site.springfoxVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td></tr>		
		<tr>
            <td>compile</td>
            <td>com.github.xiaoymin</td>
            <td>
				knife4j-annotations<br/>
				knife4j-core<br/>
				knife4j-spring-mvc<br/>
				knife4j-spring<br/>
				knife4j-spring-ui<br/>
				knife4j-spring-boot-starter<br/>
				knife4j-spring-boot-autoconfigure
			</td>
            <td>{{site.knife4jVersion}}</td>
            <td>jar</td>
            <td>The Apache License, Version 2.0</td>
		</tr>	
		
		
    </tbody>
</table>

前端组件依赖

<table border="0" class="table table-striped table-bordered ">
    <thead>
        <tr>
            <th>Dependency</th>
            <th>Component</th>
            <th>Version</th>
            <th>Type</th>
            <th>License</th></tr>
    </thead>
    <tbody>
		<tr>
            <td><b>~v3.5.0+</b></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
		</tr>
		<tr>
            <td>compile</td>
            <td>Angular</td>
            <td>13.3.3</td>
            <td>typescript</td>
            <td>MIT-style License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>Ant Design of Angular(NG-ZORRO)</td>
            <td>v13.1.1</td>
            <td>typescript</td>
            <td>MIT</td>
		</tr>	
		<tr>
            <td>compile</td>
            <td>NG ALAIN</td>
            <td>v13.4.2</td>
            <td>typescript</td>
            <td>MIT</td>
		</tr>	
		<tr>
            <td>compile</td>
            <td>ng-ant-admin</td>
            <td>v12.2+</td>
            <td>typescript</td>
            <td>MIT License</td>
		</tr>	
		<tr>
            <td>compile</td>
            <td>CryptoJS</td>
            <td>4.1.1</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td><b>~pre v3.5.0</b></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
		</tr>
		<tr>
            <td>compile</td>
            <td>jQuery</td>
            <td>v3.6.0</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>Bootstrap</td>
            <td>v5.1.2</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>bootstrap-table</td>
            <td>1.18.3</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>zTree</td>
            <td>3.5.46</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>metisMenu</td>
            <td>3.0.7</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>datetimepicker</td>
            <td>2.5.20</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>font-awesome</td>
            <td>4.7.0</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>CKEditor</td>
            <td>5</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>artDialog</td>
            <td>5.0.4</td>
            <td>javascript</td>
            <td>GNU GPL</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>popperjs</td>
            <td>v2.10.2</td>
            <td>javascript</td>
            <td>MIT License</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>jQuery serializeObject</td>
            <td>2.4.3</td>
            <td>javascript</td>
            <td>BSD</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>jQuery Form Plugin</td>
            <td>3.51.0</td>
            <td>javascript</td>
            <td>LGPLv2.1 (or later) or MIT</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>jQuery blockUI plugin</td>
            <td>2.70.0</td>
            <td>javascript</td>
            <td>MIT</td>
		</tr>
		<tr>
            <td>compile</td>
            <td>jQuery Cookie</td>
            <td>v1.4.1</td>
            <td>javascript</td>
            <td>MIT</td>
		</tr>
		
		<tr>
            <td>compile</td>
            <td>Chart.js</td>
            <td>v3.4.1</td>
            <td>javascript</td>
            <td>MIT</td>
		</tr>
		 
		
		
    </tbody>
</table>
