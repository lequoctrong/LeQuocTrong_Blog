### File 7: `content/posts/bai-7.md`
*(Chủ đề: JSON)*

```markdown
---
title: "Kiến thức chung: JSON - Ngôn ngữ chung của Internet"
date: 2023-12-23
draft: false
tags: ["Theory", "JavaScript"]
author: "Lê Quốc Trọng"
---

Khi Java Server nói chuyện với JavaScript Client, chúng không hiểu nhau trực tiếp. Chúng cần một định dạng trung gian. Đó là **JSON (JavaScript Object Notation)**.

## Cấu trúc JSON
Nó rất giống Object của JS, nhưng key phải nằm trong dấu ngoặc kép.

```json
{
  "sinh_vien": "Lê Quốc Trọng",
  "mssv": "XXXXXXXX",
  "ky_nang": ["Java", "Network", "Git"]
}