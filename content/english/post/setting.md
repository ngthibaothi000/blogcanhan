---
author: Bảo Thi
title: Cài Đặt Môi Trường Phát Triển Java
date: 2024-11-12
description: Hướng dẫn cài đặt môi trường phát triển Java
thumbnail: "/images/thumbnail/setting.jpg"
---

Cài đặt môi trường phát triển Java có thể được thực hiện bằng cách sử dụng Bộ công cụ phát triển Java (JDK). <!--more-->

Trong ví dụ này, chúng tôi sẽ hướng dẫn bạn cách tải xuống JDK và thiết lập các biến môi trường.

1. **Tải xuống JDK**:
   - Truy cập trang web [Oracle JDK] hoặc [OpenJDK] để tải xuống phiên bản JDK mới nhất.

2. **Cài Đặt JDK**:
   - Chạy trình cài đặt đã tải xuống và làm theo hướng dẫn để hoàn tất cài đặt.

3. **Thiết Lập Các Biến Môi Trường**:
   - Trên Windows:
     - Mở **Control Panel** → **System and Security** → **System** → **Advanced System Settings** → **Environment Variables**.
     - Trong phần **System variables**, nhấn **New** và thêm một biến có tên là `JAVA_HOME` với giá trị được đặt là đường dẫn cài đặt JDK (ví dụ: `C:\Program Files\Java\jdk-11.0.1`).
     - Tìm biến `Path` trong danh sách và nhấn **Edit**. Thêm `C:\Program Files\Java\jdk-11.0.1\bin` vào danh sách.

   - Trên macOS hoặc Linux:
     - Mở terminal và thêm các dòng sau vào tệp `.bash_profile` hoặc `.bashrc` của bạn:
       ```bash
       export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-11.0.1.jdk/Contents/Home
       export PATH=$JAVA_HOME/bin:$PATH
       ```
     - Lưu tệp và chạy `source ~/.bash_profile` hoặc `source ~/.bashrc` để áp dụng các thay đổi.

4. **Xác Minh Cài Đặt**:
   - Mở terminal hoặc command prompt và gõ lệnh sau để kiểm tra phiên bản Java:
     ```bash
     java -version
     ```

### Ví dụ
- Kiểm tra phiên bản Java:
  ```bash
  java -version
