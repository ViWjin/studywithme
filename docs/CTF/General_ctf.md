---
sidebar_position: 2
---

# CTF - General Skills

> _"Trang này chủ yếu lấy những chủ đề CTF về General Skill đến từ Pico CTF. Từ easy -> medium -> hard."_

## 📌 Mục lục

- [⚙️ Các công cụ được sử dụng để làm bài](#️-các-công-cụ-được-sử-dụng-để-làm-bài)
- [1️⃣ Các bài mức dễ](#1️⃣-các-bài-mức-dễ)
    - [Commitment Issues](#commitment-issues)


- [2️⃣ Các bài mức trung bình](#2️⃣-các-bài-mức-trung-bình)

- [3️⃣ Các bài mức khó](#3️⃣-các-bài-mức-khó)

[CTF from picoCTF](https://play.picoctf.org/)

## ⚙️ Các công cụ được sử dụng để làm bài

- Git (Tôi đã có 1 phần nói về cái này). [Xem tại đây](../Tutorial/Git.md)

- Python (Ai học chắc cũng biết đây là 1 nnlt nhỉ). [Tải ứng dụng tại đây](https://www.python.org/downloads/)

## 1️⃣ Các bài mức dễ 

### Commitment Issues

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/411?page=3)

**Bước 1:** Tất nhiên là tải file tài nguyên và giải nén trước. Sau đó ta sẽ thấy file nén chỉ có *1 file .txt* và *folder .git*

![Pic1](./img/general_skill/Commitment_Issue/1.png)

**Bước 2:** Kiểm tra *file .txt*, ta sẽ thấy không có kết quả gì cả.

![Pic2](./img/general_skill/Commitment_Issue/2.png)

**Bước 3:** Nhìn lại các folder có, có *folder .git*, vì vậy ta sẽ nghĩ ngay tới kiểm tra các sự kiện đã xảy ra với *git.* Lệnh sử dụng trong bài này sẽ là:

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

### Collaborative Development

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/410?page=3)

**Bước 1:** Vẫn là tải file về và giải nén tài nguyên. Quan sát thấy chỉ có *1 file flag.py* và *folder .git*

![Pic1](./img/general_skill/Collaborative-Development/1.png)

**Bước 2:** Thử kiểm tra và chạy *file flag.py* bằng lệnh:

![Pic1.5](./img/general_skill/Collaborative-Development/1.5.png)

![Pic2](./img/general_skill/Collaborative-Development/2.png)

**Bước 3:** Chứng tỏ đoạn chương trình này không có flag cần tìm. Vậy nếu sử dụng lệnh log như nãy thì sao?

![Pic3](./img/general_skill/Collaborative-Development/3.png)

*Hoàn toàn không có gì!*

**Bước 4:** Lúc này, ta sẽ thử kiểm tra các yếu tố khác, ví dụ như mình đã kiểm tra các nhánh (branch) bằng lệnh:

```
git branch -a
```

![Pic4](./img/general_skill/Collaborative-Development/4.png)

*Khá may mắn vì thấy có nhiều nhánh phụ trừ nhánh chính (main)!*

**Bước 5:** Thử chuyển qua nhánh phụ và chạy lại *file flag.py* và xem kết quả. Lệnh chạy:

```
git checkout feature/part-1
python flag.py
git checkout feature/part-2
python flag.py
git checkout feature/part-3
python flag.py
```

Hoặc nhanh hơn:

```
git checkout feature/part-1
python flag.py
git checkout feature/part-2
python flag.py
git checkout feature/part-3
python flag.py
```

![Pic5](./img/general_skill/Collaborative-Development/5.png)

*Vì có 3 nhánh nên đoạn Flag đã bị chia thành 3, ta chỉ việc ghép lại là hoàn thành!*

**Lưu ý: có một số thiết bị phải chạy python3 thay vì python như máy tôi!**

***Kết thúc!***

### Blame Game

Bài làm: [Tại đây](https://play.picoctf.org/practice/challenge/405?page=3)

**Bước 1:** Vẫn là tải file về và giải nén tài nguyên. Quan sát thấy chỉ có *1 file message.py* và *folder .git*

![Pic1](./img/general_skill/Blame_game/1.1.png)

**Bước 2:** Thử kiểm tra và chạy *file message.py* bằng lệnh:

![Pic1.5](./img/general_skill/Blame_game/1.png)

![Pic2](./img/general_skill/Blame_game/2.png)

**Bước 3:** Chứng tỏ đoạn chương trình này không có flag cần tìm. Vậy nếu sử dụng lệnh log và branch như nãy thì sao?

![Pic3](./img/general_skill/Blame_game/3.png)

*Hoàn toàn không có gì!*

![Pic4](./img/general_skill/Blame_game/4.png)

*Lệnh log thì chạy liên tục, khiến ta khó quan sát.*

**Bước 4:** Lúc này, ta thử chỉ kiểm tra log của *file message.py*.

```
git log message.py
```

![Pic5](./img/general_skill/Blame_game/5.png)

***Kết thúc!***



## 2️⃣ Các bài mức trung bình

## 3️⃣ Các bài mức khó