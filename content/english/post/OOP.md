+++
author = "Bảo Thi"
title = "Giới Thiệu về Lập Trình Hướng Đối Tượng trong Java"
date = "2024-12-10"
description = "Hướng dẫn hiểu về lập trình hướng đối tượng trong Java"
tags = [
    "OOP",
    "java"
]
thumbnail = "/images/thumbnail/OOP.jpg"
+++

Lập Trình Hướng Đối Tượng (OOP) là một mô hình sử dụng các đối tượng và lớp để cấu trúc phần mềm theo cách có tính mô-đun, tái sử dụng và dễ bảo trì.

<!--more-->

### Các Khái Niệm Cơ Bản của OOP trong Java

Trong Java, OOP xoay quanh một số khái niệm cốt lõi bao gồm lớp, đối tượng, kế thừa, đóng gói, đa hình và trừu tượng. Hãy khám phá những khái niệm này với một số ví dụ.

#### Lớp và Đối Tượng

**Lớp** là một bản thiết kế để tạo các đối tượng. **Đối tượng** là một thể hiện của lớp. Đây là ví dụ về một lớp đơn giản và cách tạo một đối tượng từ nó:

```java
public class Person {
    private String name;
    private int age;

    // Constructor
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    // Getter cho tên
    public String getName() {
        return name;
    }

    // Setter cho tên
    public void setName(String name) {
        this.name = name;
    }

    // Phương thức để hiển thị thông tin người
    public void displayInfo() {
        System.out.println("Tên: " + name + ", Tuổi: " + age);
    }

    public static void main(String[] args) {
        // Tạo một đối tượng của lớp Person
        Person person = new Person("Alice", 30);
        person.displayInfo();
    }
}
