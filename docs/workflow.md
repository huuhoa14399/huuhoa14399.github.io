---
id: workflow
title: Datagrin API
---

# Project Work Flow


1. API kiểm tra trạng thái có dữ liệu hay không.

```
METHOD: GET
URL: /:project_id/check-data

RESPONSE:
{
    uid-info: false,
    page: false,
    group: true,
}

NOTE:
- Nếu có dữ liệu rồi thì chạy theo luồng cũ.
- Nếu chưa có gọi API kiểm tra xem có queue chưa.
```

2. API Kích hoạt và kiểm tra trạng thái queue.

```
METHOD: POST
URL: /:project_id/queue

RESPONSE:
{
    status: -1
}

NOTE:
- -1 là dã có queue
- 0 là kích hoạt queue thất bại.
- 1 là kích hoạt queue thành công.