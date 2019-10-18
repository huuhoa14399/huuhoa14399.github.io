---
id: contributing
title: Datagrin Contributing Guide
---

Hướng dẫn cơ bản để  đóng góp vào project.

## General

- Chắc chắn rằng không có pull request nào đề cập đến vấn đề/feature mà bạn đang thực hiện.
- Đưa ra issue nếu tồn tại vấn đề mới, gán nhãn phù hợp cho từng vấn đề.
- Tạo nhánh issue/feature để giải quyết vấn đề bạn đang giải quyết. 
- Tên nhánh ngắn gọn (dưới 30 ký tự) , nối nhanh giữa các từ bởi dấu `-` theo dạng **type**-**subject**:
    - Issue: `issue-IssueID-desc`. Ví dụ: `issue-12-auth-error`.
    - Feature: `feat-desc`. Ví dụ: `feat-search-product-api`.
    - Docs: `doc-desc`. Ví dụ: `doc-search-product-docs`.

## Commit Message Format

Mỗi commit message có **type** và có mô tả **subject**:

```
 <type>: <subject>
```

Nội dung commit không quá 100 kí tự, ngắn gọn đủ diễn đạt nội dung commit muốn đề cập. Điều này giúp cho 
dev dễ theo dõi git log:

```
 #271 feat(containers): add exposed ports in the containers view
 #270 fix(templates): fix a display issue in the templates view
 #269 style(dashboard): update dashboard with new layout
```

Trong trường hợp có nhiều loại thay đổi, ngăn tách giữa các type bởi `/`. Ví dụ: `feat/fix: something ...` .

### Type

Giá trị **type** có thể nhận một số giá trị:

* **feat**: Feature mới
* **fix**: Fix lỗi bug
* **docs**: Tài liệu, api
* **style**: Thay đổi code style, không ảnh hưởng ý nghĩa của code (dấu, typo,..)
  semi-colons, etc)
* **refactor**: Thay đổi cấu trúc tổ chức của project
* **test**: Thêm các test thiếu
* **chore**: Thay đổi nhỏ liên quan đến build process, tool và thư viện phụ thuộc,...

### Subject

Tiêu đề của commit cần:
* Sử dụng động từ nguyên thể, thì hiện tại đơn.
* Không viết hoa chữ cái đầu
* Không sử dụng dấu (.) ở cuối câu

### Tham khảo
- [Portainer Contributing Guide](https://raw.githubusercontent.com/portainer/portainer/develop/CONTRIBUTING.md)
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.2/)