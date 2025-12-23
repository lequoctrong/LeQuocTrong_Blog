---
title: "JavaScript: Gọi API bằng Fetch (Thay thế XMLHttpRequest)"
date: 2023-12-21
draft: false
tags: ["JavaScript", "Web"]
author: "Lê Quốc Trọng"
---

Là dân lập trình mạng, việc gửi HTTP Request là chuyện cơm bữa. Trong JavaScript hiện đại, chúng ta không dùng `XMLHttpRequest` nữa mà dùng `fetch`.

## Ví dụ lấy dữ liệu Github
Đoạn code JS này giúp mình lấy thông tin profile Github của chính mình:

```javascript
const url = '[https://api.github.com/users/lequoctrong](https://api.github.com/users/lequoctrong)'; // Thay user

fetch(url)
  .then(response => response.json()) // Chuyển dữ liệu về JSON
  .then(data => {
    console.log("GitHub ID: " + data.login);
    console.log("URL: " + data.html_url);
  })
  .catch(error => console.error('Lỗi:', error));