+++
author = "Java Authors"
title = "Hướng Dẫn Sử Dụng Icon trong Java"
date = "2024-12-20"
description = "Hướng dẫn cách sử dụng icon trong Java"
tags = [
    "icon",
    "java"
]
thumbnail = "/images/thumbnail/icon-support-thumbnail.jpg"
+++


Trong Java, bạn có thể sử dụng các biểu tượng (icon) bằng cách sử dụng các thư viện như Swing. Dưới đây là cách làm:

<!--more-->

### Sử Dụng Icon trong Java

Trong Java, biểu tượng có thể được sử dụng trong các ứng dụng GUI thông qua thư viện Swing. Dưới đây là một ví dụ về cách thêm biểu tượng vào một nút (button):

```java
import javax.swing.*;
import java.awt.*;

public class IconExample {
    public static void main(String[] args) {
        // Tạo một JFrame
        JFrame frame = new JFrame("Icon Example");
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        frame.setSize(400, 300);

        // Tạo một ImageIcon từ một đường dẫn hình ảnh
        ImageIcon icon = new ImageIcon("path/to/your/icon.png");

        // Tạo một JButton và thêm ImageIcon vào
        JButton button = new JButton("Click Me", icon);
        
        // Thêm nút vào JFrame
        frame.setLayout(new FlowLayout());
        frame.add(button);

        // Hiển thị JFrame
        frame.setVisible(true);
    }
}
