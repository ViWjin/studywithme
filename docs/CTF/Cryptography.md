---
sidebar_position: 3
---

# CTF - CRYPTOGRAPHY

> _"Trang này chủ yếu lấy những chủ đề CTF về Cryptography đến từ Pico CTF. Từ easy -> medium -> hard."_

[CTF from picoCTF](https://play.picoctf.org/)

## ⚙️ Các công cụ được sử dụng để làm bài

- WSL

## 1️⃣ Các bài mức dễ

### Mod 26

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/144?page=5)

***Kết thúc!***

### The Numbers

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/68?page=6)

***Kết thúc!***

### 13

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/62?page=6)

***Kết thúc!***

### hashcrack

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/475?page=1)

**Bước 1:** Theo yêu cầu đề bài cần chạy lệnh *"nc verbal-sleep.picoctf.net 51759"*, mà lệnh này thì chạy bằng *Ubuntu* nên tôi sẽ dùng *WSL* để chạy.

![Pic1](../CTF/img/Cryptography/hashcrack/1.png)

**Bước 2:** Sau khi kết nối thành công, bài sẽ gửi về đoạn mã **482c811da5d5b4bc6d497ffa98491e38**, tiến hành giải băm vì nó khá đơn giản.

![Pic2](../CTF/img/Cryptography/hashcrack/2.png)

**Bước 3:** Sau khi giải băm đoạn này, tiếp tục có đoạn băm **b7a875fc1ea228b9061041b7cec4bd3c52ab3ce3**, tiến hành giải băm (trang web gợi ý đoạn mã được băm theo dạng MD5).

![Pic3](../CTF/img/Cryptography/hashcrack/3.png)

**Bước 4:** Bài làm lại yêu cầu giải băm theo định dạng SHA-1 có mã là **916e8c4f79b25028c9e467f1eb8eee6d6bbdff965f9928310ad30a8d88697745**, tiến hành giải băm.

![Pic4](../CTF/img/Cryptography/hashcrack/4.png)

**Bước 5:** Sau khi làm hết các nội dung băm trên, ta có mã CTF Flag cần tìm

![Pic5](../CTF/img/Cryptography/hashcrack/5.png)

Đoạn Flag: **picoCTF\{UseStr0nG_h@shEs_&PaSswDs!_ce730f64\}**

***Kết thúc!***

## 2️⃣ Các bài mức trung bình

## 3️⃣ Các bài mức khó

