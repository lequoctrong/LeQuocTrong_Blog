---
title: "Bài 1: Làm sao biết máy mình đang dùng IP gì trong Java?"
date: 2025-12-15
weight: 1
draft: false
tags: ["Java", "Network", "Lập trình mạng"]
summary: "Hướng dẫn sử dụng class InetAddress để lấy thông tin IP và tên máy tính (Localhost)."
---

Trong lập trình mạng, "địa chỉ nhà" (IP Address) là thông tin cơ bản nhất để các thiết bị có thể tìm thấy và giao tiếp với nhau. Java cung cấp một class cực kỳ mạnh mẽ để xử lý việc này là `java.net.InetAddress`.

Bài viết này sẽ hướng dẫn bạn cách lấy **Tên máy** và **Địa chỉ IP** của chính máy tính bạn đang sử dụng (Localhost).

### 1. Class InetAddress là gì?
`InetAddress` là class đại diện cho một địa chỉ giao thức Internet (IP). Nó có thể xử lý cả IPv4 và IPv6.
Điểm đặc biệt là class này **không có Public Constructor**, nghĩa là bạn không thể tạo đối tượng bằng từ khóa `new`. Thay vào đó, bạn phải dùng các phương thức tĩnh (static methods) như:
* `getLocalHost()`: Lấy thông tin máy hiện tại.
* `getByName(String host)`: Lấy thông tin từ tên miền (ví dụ: "google.com").
* `getAllByName(String host)`: Lấy tất cả IP của một tên miền.

### 2. Code thực hành: Lấy IP của máy (Localhost)

Dưới đây là đoạn code đơn giản để in ra tên máy và địa chỉ IP hiện tại.

```java
import java.net.InetAddress;

public class MyIP {
    public static void main(String[] args) {
        try {
            // Lấy đối tượng InetAddress đại diện cho máy local
            InetAddress myIP = InetAddress.getLocalHost();
            
            // Hiển thị tên máy (Host Name)
            System.out.println("Tên máy: " + myIP.getHostName());
            
            // Hiển thị địa chỉ IP (Host Address)
            System.out.println("Địa chỉ IP: " + myIP.getHostAddress());
            
        } catch (Exception e) {
            // In ra lỗi nếu không lấy được thông tin (ví dụ: lỗi mạng)
            e.printStackTrace();
        }
    }
}