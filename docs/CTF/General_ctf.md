---
sidebar_position: 2
---

# CTF - General Skills

> _"Trang này chủ yếu lấy những chủ đề CTF về General Skill đến từ Pico CTF. Từ easy -> medium -> hard."_

## 📌 Mục lục

- [## ⚙️ Các công cụ được sử dụng để làm bài](#️-các-công-cụ-được-sử-dụng-để-làm-bài)
- [1️⃣ Các bài mức dễ](#1️⃣-các-bài-mức-dễ)
    
- [2️⃣ Các bài mức trung bình](#2️⃣-các-bài-mức-trung-bình)

- [3️⃣ Các bài mức khó](#3️⃣-các-bài-mức-khó)

[CTF from picoCTF](https://play.picoctf.org/)

## ⚙️ Các công cụ được sử dụng để làm bài

- Git (Tôi đã có 1 phần nói về cái này). [Xem tại đây](../Tutorial/Git.md)

## 1️⃣ Các bài mức dễ 

### Commitment Issues

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/411?page=3)

**Bước 1:** Tất nhiên là tải file tài nguyên và giải nén trước. Sau đó ta sẽ thấy file nén chỉ có 1 file .txt và folder .git 

![Pic1](./img/general_skill/Commitment_Issue/1.png)

**Bước 2:** Kiểm tra file .txt, ta sẽ thấy không có kết quả gì cả.

![Pic2](./img/general_skill/Commitment_Issue/2.png)

**Bước 3:** Nhìn lại các folder có, có folder .git, vì vậy ta sẽ nghĩ ngay tới kiểm tra các sự kiện đã xảy ra với git. Lệnh sử dụng trong bài này sẽ là:

```
git log
```

![Pic3](./img/general_skill/Commitment_Issue/3.png)

**Bước 4:** Ta thấy đoạn *commit a6dca68e4310585eac3b5c9caf0f75967dfe972c* đã bị xóa, thử show ra bằng lệnh:

```
git show a6dca68e4310585eac3b5c9caf0f75967dfe972c
```

![Pic4](./img/general_skill/Commitment_Issue/4.png)

***Kết thúc!***

## 2️⃣ Các bài mức trung bình

## 3️⃣ Các bài mức khó