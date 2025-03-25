---
sidebar_position: 1
---

# CTF - WEB EXPLOTATION

> _"Trang này chủ yếu lấy những chủ đề CTF về Web Explotation. Từ ease -> medium -> hard."_

## 📌 Mục lục

- [1️⃣ Các bài mức dễ](#1️⃣-các-bài-mức-dễ)
    - [Local Authority](#local-authority)

- [2️⃣ Các bài mức trung bình](#2️⃣-các-bài-mức-trung-bình)

- [3️⃣ Các bài mức khó](#3️⃣-các-bài-mức-khó)


[CTF from picoCTF](https://play.picoctf.org/)

## 1️⃣ Các bài mức dễ 

### Inspect HTML

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/275?page=4)

*Note: Bài này tôi làm sau mà nó đơn giản quá nên để lên đầu🐧. Bài này chỉ full cách tra source luôn (để tôi nhớ)*

**Bước 1:** Nhìn vào trang nội dung, ta thấy không có bất kỳ thông tin nào cần để giải bài này.

![Pic1](../CTF/img/web/Inspect_HTML/1.png)

**Bước 2:** Ấn chuột phải, chọn "Kiểm tra phần tử" hoặc "Inspect" (như trong hình).

![Pic2](../CTF/img/web/Inspect_HTML/2.png)

**Bước 3:** Lúc này, đã thấy mã cần tìm, nhưng vì lỡ chỉ rồi nên tôi chỉ cho trót các xem source 🐧. Thì bạn thấy ảnh con bọ không. Đúng rồi, ở cái ô màu đỏ đấy, ấn vào đi.

![Pic3](../CTF/img/web/Inspect_HTML/3.png)

**Bước 4:** Cái nội dung lúc này là file html mà bạn thấy lúc mới vào. Và bài này khá đơn giản nên mã flag cần tìm cũng đã nằm ở phần comment

![Pic4](../CTF/img/web/Inspect_HTML/4.png)

***Kết thúc!***

### Local Authority

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/278?page=4)

***Cách thực hiện:***

**Bước 1:** Kiểm tra source code thì không có gì bất thường. Tiến hành đăng nhập (tài khoản,mật khẩu bất kỳ).

![Pic1](../CTF/img/web/Local_Autho/1.png)

**Bước 2:** Sau khi đăng nhập, thông tin sẽ trả về lỗi. Nhưng lúc này, ở source code đã có 1 file tên là secure.js, tiến hành kiểm tra file này và thấy thông tin đăng nhập hợp lệ.

![Pic2](../CTF/img/web/Local_Autho/2.png)

**Bước 3:** Tiến hành đăng nhập bằng tài khoản đã thấy, ta sẽ thấy có mã CTF flag cần tìm.

![Pic3](../CTF/img/web/Local_Autho/3.png)

***Kết thúc!***

## 2️⃣ Các bài mức trung bình

## 3️⃣ Các bài mức khó