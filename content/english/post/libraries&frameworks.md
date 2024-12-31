+++
author = "Bảo Thi"
title = "Các Thư Viện và Framework Phổ Biến trong Java"
date = "2024-12-22"
description = "Hướng dẫn về các thư viện và framework phổ biến trong Java"
tags = [
    "java",
    "libraries",
    "frameworks",
]
thumbnail = "/images/thumbnail/thuvien.jpg"
+++

Java có một hệ sinh thái phong phú các thư viện và framework giúp đơn giản hóa việc phát triển và nâng cao năng suất. Trong bài viết này, chúng ta sẽ khám phá một số thư viện và framework phổ biến nhất.

<!--more-->

## Spring Framework

[Spring Framework](https://spring.io/projects/spring-framework) là một framework toàn diện cho phát triển Java doanh nghiệp. Nó cung cấp một loạt các tính năng bao gồm tiêm phụ thuộc, quản lý giao dịch và dịch vụ web.

```java
import org.springframework.context.ApplicationContext;
import org.springframework.context.support.ClassPathXmlApplicationContext;

public class SpringExample {
    public static void main(String[] args) {
        ApplicationContext context = new ClassPathXmlApplicationContext("Beans.xml");
        HelloWorld obj = (HelloWorld) context.getBean("helloWorld");
        obj.getMessage();
    }
}
