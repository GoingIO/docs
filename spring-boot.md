title: Spring boot入门
notebook: 技术相关
tags: spring, spring-boot

[TOC]

# Getting started
Spring boot方便了用户去创建一个独立的，基于spring的应用，你可以直接运行。大多数的spring boot 应用不需要太多的配置。 

## maven 设置

    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>1.4.2.RELEASE</version>
    </parent>

    <!-- Add typical dependencies for a web application -->
    <dependencies>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>
    </dependencies>

    <!-- Package as an executable jar -->
    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
            </plugin>
        </plugins>
    </build>

并不是所有的应用都需要继承直``spring-boot-starter-parent``, 如果你有自己的parent，你可以使用如下的Maven配置
