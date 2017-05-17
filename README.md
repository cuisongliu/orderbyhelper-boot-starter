[![Build Status](https://travis-ci.org/cuisongliu/orderbyhelper-boot-starter.svg?branch=master)](https://travis-ci.org/cuisongliu/orderbyhelper-boot-starter)
[![Dependency Status](https://www.versioneye.com/user/projects/5916d430e1638f00530324f9/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/5916d430e1638f00530324f9)
[![license](https://img.shields.io/badge/gradle-3.3-brightgreen.svg)](https://gradle.org)
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/mit-license.php)

# MyBatis [OrderByHelper](https://github.com/abel533/OrderByHelper)  integration  with springboot

OrderbyHelper-Spring-Boot-Starter 帮助你集成通用 [OrderByHelper](https://github.com/abel533/OrderByHelper) 到 Spring Boot。

OrderbyHelper-Spring-Boot-Starter will help you use [OrderByHelper](https://github.com/abel533/OrderByHelper) with Spring Boot.

## How to use

### maven

在pom.xml加入nexus资源库（解决中国访问慢的问题,已经加入中央仓库）

Add the following nexus repository(fix china access slow problem,already append to central nexus.) to your pom.xml:

    <repositories>
        <repository>
            <id>nexus</id>
            <name>nexus</name>
            <url>http://maven.cuisongliu.com/content/groups/public</url>
            <releases>
                <enabled>true</enabled>
            </releases>
            <snapshots>
                <enabled>false</enabled>
            </snapshots>
        </repository>
    </repositories>

在pom.xml加入依赖

Add the following dependency to your pom.xml:

    <dependency>
       <groupId>com.cuisongliu</groupId>
       <artifactId>orderbyhelper-spring-boot-starter</artifactId>
       <version>1.0</version>
     </dependency>

### gradle

在build.gradle加入nexus资源库（解决中国访问慢的问题,已经加入中央仓库）

Add the following nexus repository(fix china access slow problem,already append to central nexus.) to your build.gradle:

    allprojects {
        repositories {
            mavenLocal()
            maven { url "http://maven.cuisongliu.com/content/groups/public" }
            mavenCentral()
            jcenter()
        }
    }
    

在build.gradle加入依赖

Add the following dependency to your build.gradle:
    
    compile "com.cuisongliu:orderbyhelper-spring-boot-starter:1.0"
    
## Acknowledgments

 [OrderByHelper](https://github.com/abel533/OrderByHelper).