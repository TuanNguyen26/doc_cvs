---
title: 'API v1'
description: 'Tài liệu hướng dẫn tích hợp API Computer Vision Việt Nam'
---

## Cơ Chế Xác Thực

Chúng tôi sử dụng `Basic Authentication` để cấp quyền truy cập vào API.

Cách hoạt động:

1. API access key là một cặp:

- username (api_key): một mã định danh duy nhất của API access key.
- password (api_secret): một mã bí mật của API access key.

Đội ngũ Computer Vision Việt Nam sẽ tạo username và password cho từng khách hàng trước khi tích hợp.

2. Client gửi một request:

Client gửi HTTP requests cùng với `Authorization` header chứa `Basic` theo sau là một khoảng trắng và một mã hoá Base64 `username:password`.
Ví dụ, `demo:p@55w0rd` client sẽ gửi

```
Authorization: Basic ZGVtbzpwQDU1dzByZA==
```

## Dòng Tương Tác

### Flow 1: OCR

[![ocr](https://static.swimlanes.io/591b6e2fea681de2bf8c1e8e3aee30b6.png)](https://swimlanes.io/d/DpmXjqcrp)

### Flow 2: Face Matching

[![face matching](https://static.swimlanes.io/862fcd7dfc64aabe0d9d8b64676856dd.png)](https://swimlanes.io/d/umDCBbU-d)

### Flow 3: Face Search

[![face search](https://static.swimlanes.io/9012d6bc5b996fb780c1c1abad6d75d6.png)](https://swimlanes.io/d/INlNJtSgY)
