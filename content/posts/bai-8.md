### File 8: `content/posts/bai-8.md`
*(Chủ đề: Các lỗi thường gặp)*

```markdown
---
title: "Chia sẻ kinh nghiệm: Các lỗi thường gặp khi code Socket"
date: 2023-12-23
draft: false
tags: ["Java", "Tips"]
author: "Lê Quốc Trọng"
---

Trong quá trình làm đồ án này, mình đã gặp (và fix) vô số lỗi. Dưới đây là những lỗi phổ biến:

1. **BindException: Address already in use**
   * *Nguyên nhân:* Cổng (Port) bạn định chạy đã có chương trình khác chiếm dụng.
   * *Cách sửa:* Đổi số port khác (VD: từ 5000 sang 5001).

2. **ConnectException: Connection refused**
   * *Nguyên nhân:* Client cố kết nối nhưng Server chưa chạy.
   * *Cách sửa:* Luôn nhớ chạy file Server trước, Client sau.

3. **Lỗi Encoding (Tiếng Việt bị lỗi)**
   * *Cách sửa:* Luôn sử dụng `UTF-8` khi đọc/ghi dữ liệu qua Stream.