---
title: "Java Networking #1: Hiểu về Socket và ServerSocket"
date: 2023-12-20
draft: false
tags: ["Java", "Network"]
description: "Khái niệm cơ bản nhất trong lập trình mạng mà sinh viên IT cần nắm."
author: "Lê Quốc Trọng"
---

Trong đồ án môn Lập trình mạng lần này, khái niệm đầu tiên mình tiếp cận là **Socket**.

## Socket là gì?
Hiểu đơn giản, Socket giống như một cái "cổng" để hai chương trình (Client và Server) có thể nói chuyện với nhau qua mạng. Trong Java, chúng ta dùng gói `java.net`.

## Code ví dụ tạo Server
Dưới đây là đoạn code mình viết để tạo một Server lắng nghe ở cổng 5000:

```java
import java.net.*;
import java.io.*;

public class SimpleServer {
    public static void main(String[] args) {
        try {
            // Tạo Server lắng nghe tại port 5000
            ServerSocket server = new ServerSocket(5000);
            System.out.println("Server của Trọng đang chạy...");
            
            // Chấp nhận kết nối từ Client
            Socket socket = server.accept();
            System.out.println("Có người kết nối!");
            
            server.close();
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}