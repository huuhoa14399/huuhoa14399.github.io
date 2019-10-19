---
id: test
title: Datagrin Test
---

T sẽ tạo 1 docs và cho nó lên thanh sidebar
headerLinks: [
    {doc: 'server', label: 'Docs'},
    {doc: 'api', label: 'API'},
    {page: 'help', label: 'Help'},
    {blog: true, label: 'Blog'},
  ],

đây là chỗ cho mn config phần header
```
{
  "docs": {
    "Server": ["server"],
    "WebApp": ["webapp"],
    "Contributing": ["contributing"],
    "Test Docs": ["api"]
  },
  "docs-other": {
    "First Category": ["doc4", "doc5"]
  }
}
```
đây là chỗ mọi người config trên thanh side bar

Khi mn thay đổi gì ở trên side bar thì phải start lại  
Còn sửa trên docs thì ko cần load lại nhé
Mỗi khi mn code xong chỉ cần push code lên nhánh public-gh-pages là Circle CI sẽ tự động build và push lên master và chạy trên github page nha
À quên lúc đầu mn pull code vê fvaf checkout sang nhánh publish-gh-pags để code nhé, chúng t sẽ code trên nhánh này nên đừng push gì lên master nhaa
:v ok thank anh em đã xem