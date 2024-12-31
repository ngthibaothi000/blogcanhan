+++
author = "Bảo Thi"
title = "JavaScript Hiện Đại"
date = "2024-12-20"
description = "Hướng dẫn hiểu về các tính năng hiện đại của JavaScript"
tags = [
    "JavaScript",
    "ES6",
    "Modern JavaScript"
]
thumbnail = "/images/thumbnail/hiendai.jpg"
+++

JavaScript hiện đại đã phát triển rất nhiều với sự ra đời của ES6 và các phiên bản sau đó. Các tính năng mới giúp lập trình viên viết mã dễ đọc hơn, hiệu quả hơn và mạnh mẽ hơn.

<!--more-->

### Các Tính Năng Mới trong JavaScript Hiện Đại

JavaScript hiện đại bao gồm nhiều tính năng mới như let, const, arrow functions, template literals, destructuring, và nhiều hơn nữa. Hãy khám phá một số tính năng này với các ví dụ.

1. ***let và const***

    `let` và `const` là các từ khóa mới để khai báo biến trong JavaScript. `let` cho phép khai báo biến có phạm vi khối, trong khi `const` khai báo các hằng số không thể thay đổi.

    ```javascript
    let name = "Alice";
    const age = 30;

    name = "Bob"; // Hợp lệ
    age = 25; // Lỗi: Assignment to constant variable.

2. ***Arrow Functions***

    Arrow functions cung cấp một cú pháp ngắn gọn hơn để viết các hàm.

    ```javascript
    // Hàm thông thường
    function add(a, b) {
    return a + b;
    }
    // Arrow function
    const add = (a, b) => a + b;

3. ***Template Literals***

    Template literals cho phép chèn biến và biểu thức vào chuỗi một cách dễ dàng.

    ```javascript
    const name = "Alice";
    const greeting = `Hello, ${name}!`;
    console.log(greeting); // Output: Hello, Alice!

4. ***Destructuring***

    Destructuring cho phép trích xuất dữ liệu từ mảng hoặc đối tượng và gán chúng vào các biến.
    ```javascript
    const person = {
    name: "Alice",
    age: 30
    };

    const { name, age } = person;
    console.log(name); // Output: Alice
    console.log(age); // Output: 30

