### File 6: `content/posts/bai-6.md`
*(Chủ đề: Multithreading)*

```markdown
---
title: "Java Networking #3: Xử lý đa luồng cho Server"
date: 2023-12-22
draft: false
tags: ["Java", "Advanced"]
author: "Lê Quốc Trọng"
---

Vấn đề của bài 1 là Server chỉ phục vụ được 1 người tại 1 thời điểm. Để phục vụ hàng trăm người cùng lúc, ta cần **Multithreading** (Đa luồng).

## Cách thực hiện
Mỗi khi có Client kết nối (`accept()`), ta sẽ ném Client đó cho một `Thread` riêng để xử lý.

```java
while (true) {
    Socket socket = server.accept();
    System.out.println("Client mới kết nối: " + socket);
    
    // Tạo luồng mới cho client này
    Thread t = new Thread(new ClientHandler(socket));
    t.start();
}