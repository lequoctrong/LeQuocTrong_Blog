### File 5: `content/posts/bai-5.md`
*(Chủ đề: Async/Await)*

```markdown
---
title: "JavaScript: Tại sao phải dùng Async/Await?"
date: 2023-12-22
draft: false
tags: ["JavaScript"]
author: "Lê Quốc Trọng"
---

Trong lập trình mạng, độ trễ (latency) là điều không tránh khỏi. Nếu code chạy tuần tự (synchronous), giao diện web sẽ bị đơ khi chờ server trả lời.

Để giải quyết, ES6 cung cấp `async/await`.

## Viết lại code Fetch API
Đây là cách mình viết code gọn hơn bài trước:

```javascript
async function getUserInfo() {
    try {
        let res = await fetch('[https://api.github.com/users/lequoctrong](https://api.github.com/users/lequoctrong)');
        let data = await res.json();
        console.log("Dữ liệu nhận được: ", data);
    } catch (err) {
        console.log("Có lỗi xảy ra: " + err);
    }
}

getUserInfo();