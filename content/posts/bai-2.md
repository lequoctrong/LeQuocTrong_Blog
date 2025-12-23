### File 2: `content/posts/bai-2.md`
*(Chủ đề: Client kết nối Server)*

```markdown
---
title: "Java Networking #2: Xây dựng mô hình Client - Server đơn giản"
date: 2023-12-20
draft: false
tags: ["Java", "Tutorial"]
author: "Lê Quốc Trọng"
---

Ở bài trước mình đã tạo Server. Hôm nay mình sẽ viết code cho phía **Client** để kết nối vào Server đó.

## Code Client
Client cần biết 2 thứ:
1. IP của Server (đang chạy máy mình nên là `localhost`).
2. Port của Server (bài trước mình đặt là `5000`).

```java
import java.net.*;
import java.io.*;

public class SimpleClient {
    public static void main(String[] args) {
        try {
            // Kết nối đến Server
            Socket s = new Socket("localhost", 5000);
            
            System.out.println("Đã kết nối thành công tới Server!");
            
            s.close();
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}