## 1. Định dạng văn bản

In đậm: Sử dụng hai dấu sao \*\* hoặc gạch dưới \_\_.

**In đậm**

**In đậm**

In nghiêng: Sử dụng một dấu sao \* hoặc gạch dưới \_.

_In nghiêng_

_In nghiêng_

Gạch ngang (cross out): Dùng dấu ~~.

~~Gạch ngang~~

## 2. Tiêu đề

Tiêu đề trong Markdown được tạo bằng dấu #, từ 1 đến 6 dấu # tương ứng với các cấp độ tiêu đề (h1-h6).

# Tiêu đề cấp 1

## Tiêu đề cấp 2

### Tiêu đề cấp 3

#### Tiêu đề cấp 4

##### Tiêu đề cấp 5

###### Tiêu đề cấp 6

## 3. Danh sách

Danh sách không có thứ tự (bullet points): Sử dụng dấu -, + hoặc \*.

- Món ăn 1
- Món ăn 2
  - Món ăn phụ 1
  - Món ăn phụ 2

* Món ăn 3

- Món ăn 4
  Danh sách có thứ tự: Dùng số và dấu chấm.

1. Món ăn 1
2. Món ăn 2
3. Món ăn 3

## 4. Định dạng liên kết

Liên kết nội bộ (URL): Dùng dấu ngoặc vuông [] và ngoặc tròn ().

[Google](https://www.google.com)
Liên kết với văn bản có title: Thêm tiêu đề trong dấu ngoặc đơn sau URL.

[Google](https://www.google.com "Trang chủ của Google")

## 5. Định dạng hình ảnh

Hình ảnh cũng sử dụng cú pháp tương tự như liên kết, nhưng bắt đầu bằng dấu !.

```
![Alt text](URL_hình_ảnh)
```

Ví dụ:

![Logo](https://example.com/logo.png)

## 6. Đoạn mã (Code)

Mã trong dòng: Đặt mã trong dấu backticks (`).

Đây là một đoạn `mã` trong dòng.
Mã đa dòng: Đặt mã trong ba dấu backticks (```).

```
code
```

## 7. Bảng

Để tạo bảng, sử dụng dấu gạch dọc | và dấu gạch ngang - để phân cách các cột và dòng.

| Tiêu đề 1 | Tiêu đề 2 | Tiêu đề 3 |
| --------- | --------- | --------- |
| Dữ liệu 1 | Dữ liệu 2 | Dữ liệu 3 |
| Dữ liệu 4 | Dữ liệu 5 | Dữ liệu 6 |

## 8. Trích dẫn

Sử dụng dấu > để tạo trích dẫn.

> Đây là một trích dẫn.
>
> Đây là dòng thứ hai của trích dẫn.

## 9. Thêm dòng ngắt (Line Break)

> Để tạo một dòng ngắt (dòng mới) trong Markdown, bạn cần phải có ít nhất hai dấu cách ở cuối dòng trước khi nhấn Enter.

Đây là dòng 1.  
Đây là dòng 2.

## 10. Chèn Emoji

Markdown hỗ trợ chèn emoji bằng cách sử dụng cú pháp :tên_emoji:. Ví dụ:

:tada: Đây là một emoji mừng!

## 11. Thêm mã nhúng (HTML)

Markdown hỗ trợ nhúng mã HTML trực tiếp. Ví dụ:

<p>Đoạn văn bản này là mã HTML</p>
