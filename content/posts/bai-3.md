### File 3: `content/posts/bai-3.md`
*(Chủ đề: TCP và UDP)*

```markdown
---
title: "Lý thuyết: Khi nào dùng TCP, khi nào dùng UDP?"
date: 2023-12-21
draft: false
tags: ["Network", "Theory"]
author: "Lê Quốc Trọng"
---

Trong quá trình học Lập trình mạng, mình hay bị nhầm lẫn giữa hai giao thức này. Đây là cách mình nhớ chúng:

## TCP (Transmission Control Protocol)
* **Đặc điểm:** Tin cậy, đảm bảo dữ liệu đến nơi và đúng thứ tự. Có bước "bắt tay 3 bước".
* **Ứng dụng:** Web (HTTP), Email, File Transfer.
* **Java Class:** `Socket`, `ServerSocket`.

## UDP (User Datagram Protocol)
* **Đặc điểm:** Nhanh, "bắn và quên" (fire and forget), không quan tâm dữ liệu có đến nơi hay không.
* **Ứng dụng:** Game online, Video call, Livestream.
* **Java Class:** `DatagramSocket`, `DatagramPacket`.

> **Kết luận:** Nếu viết ứng dụng chat, mình chọn TCP. Nếu viết game bắn súng, mình chọn UDP.