---
title: 23dec_false_folder
description: 23decfalse_folder
tags: [tutorial:product/hana_studio, tutorial:product/sapHana]
---


```markup
    <?xml version="1.0" encoding="UTF-8"?>
    <web-app xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://java.sun.com/xml/ns/javaee" xsi:schemaLocation="http://java.sun.com/xml/ns/javaee http://java.sun.com/xml/ns/javaee/web-app_2_5.xsd" id="WebApp_ID" version="2.5">
    <display-name>cloud-weatherapp</display-name>
    <welcome-file-list>
    <welcome-file>index.html</welcome-file>
    </welcome-file-list>
    <servlet>
    <display-name>HelloWorldServlet</display-name>
    <servlet-name>HelloWorldServlet</servlet-name>
    <servlet-class>
        com.sap.hana.cloud.samples.weatherapp.web.HelloWorldServlet
    </servlet-class>
    </servlet>
    <servlet-mapping>
    <servlet-name>HelloWorldServlet</servlet-name>
    <url-pattern>/hello</url-pattern>
    </servlet-mapping>
    <login-config>
    <auth-method>FORM</auth-method>
    </login-config>
    <security-constraint>
    <web-resource-collection>
        <web-resource-name>Protected Area</web-resource-name>
        <url-pattern>/*</url-pattern>
    </web-resource-collection>
    <auth-constraint>
        <!-- Role Everyone will not be assignable -->
        <role-name>Everyone</role-name>
    </auth-constraint>
    </security-constraint>
    <security-role>
    <description>All SAP HANA Cloud Platform users</description>
    <role-name>Everyone</role-name>
    </security-role>
    </web-app>
```
