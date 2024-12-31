+++
author = "Bảo Thi"
title = "JavaScript và API"
date = "2024-12-25"
description = "Hướng dẫn sử dụng API trong JavaScript"
tags = [
    "JavaScript",
    "API",
    "Web Development"
]
thumbnail = "/images/thumbnail/java-api.jpg"
+++

API (Application Programming Interface) là một tập hợp các quy tắc cho phép các ứng dụng giao tiếp với nhau. Trong JavaScript, chúng ta thường sử dụng API để tương tác với các dịch vụ web.

<!--more-->

### Sử Dụng API trong JavaScript

JavaScript cung cấp nhiều cách để làm việc với API, bao gồm `XMLHttpRequest`, `fetch`, và các thư viện như `axios`. Hãy khám phá cách sử dụng `fetch` để gọi API.

1. ***Sử Dụng fetch***

    `fetch` là một API hiện đại để thực hiện các yêu cầu HTTP. Nó trả về một Promise, cho phép chúng ta xử lý kết quả của yêu cầu một cách dễ dàng.

    ```javascript
    // Gọi API để lấy dữ liệu người dùng
    fetch('https://jsonplaceholder.typicode.com/users')
        .then(response => response.json())
        .then(data => {
            console.log(data);
        })
        .catch(error => {
            console.error('Error:', error);
        });

2. ***Xử Lý Kết Quả API***

    `fetch` là một API hiện đại để thực hiện các yêu cầu HTTP. Nó trả về một Promise, cho phép chúng ta xử lý kết quả của yêu cầu một cách dễ dàng.

    ```javascript
    // Gọi API để lấy dữ liệu người dùng
    fetch('https://jsonplaceholder.typicode.com/users')
        .then(response => response.json())
        .then(users => {
            const userList = document.getElementById('user-list');
            users.forEach(user => {
                const listItem = document.createElement('li');
                listItem.textContent = `${user.name} (${user.email})`;
                userList.appendChild(listItem);
            });
        })
        .catch(error => {
            console.error('Error:', error);
        });
3.