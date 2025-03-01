---
tittle: Git and Github tutorial
sidebar_position: 1
---

# Git and Github tutorial

> _"Chủ đề chính của bài này sẽ là nói về git và github và một số lệnh cơ bản để dùng."_

## 📌 Mục lục

- [1️⃣ Git là gì?](#1️⃣-git-là-gì)

- [2️⃣ Đặc điểm của Git](#2️⃣-đặc-điểm-của-git)

- [3️⃣ Một số thuật ngữ cần biết](#3️⃣-một-số-thuật-ngữ-cần-biết)

- [4️⃣ Cài đặt Git](#4️⃣-cài-đặt-git)

  - [Đối với Windows OS](#đối-với-windows-os)

  - [Đối với MAC OS](#đối-với-mac-os)

  - [Đối với Linux](#đối-với-linux)

- [5️⃣ Github](#5️⃣-github)

  - [Tạo 1 repository căn bản](#tạo-1-repository-căn-bản)

  - [Tạo branch mới trên github](#tạo-branch-mới-trên-github)

  - [Tải nội dung trên github về thiết bị](#tải-nội-dung-trên-github-về-thiết-bị)

### 1️⃣ Git là gì?

**Git** là một hệ thống kiểm soát phiên bản (version control system - VCS) dùng để theo dõi các thay đổi trong các tập tin và cách phối hợp sao cho nhiều người có thể cùng làm việc trên những tập tin đó.

Là hệ thống điều khiển phiên bản phân tán, có tốc độ xử lý nhanh đảm bảo tính toàn vẹn dữ liệu và hỗ trợ cho các workflow phân tán, phi tuyến tính.

Là mã nguồn mở (open source) hoàn toàn miễn phí, và chạy được trên nhiều hệ điều hành khác nhau như là Linux, Windows, MAC OSX, ...

### 2️⃣ Đặc điểm của Git:

- **Branching & Merging:** Git cho phép tạo, gộp và xóa nhánh nhanh chóng, giúp làm việc độc lập và thử nghiệm ý tưởng mới mà không ảnh hưởng đến nhánh chính (main branch). Khi đẩy lên kho remote, ta có thể chọn nhánh cần chia sẻ, tăng tính linh hoạt trong quản lý mã nguồn.

- **Small & Fast:** Git hoạt động cục bộ, giúp tăng tốc độ xử lý so với hệ thống tập trung. Được thiết kế cho Linux kernel, Git tối ưu hiệu suất và hỗ trợ kho lưu trữ lớn hiệu quả.

- **Distributed Distributed:** Git là hệ thống phân tán, cho phép “clone” toàn bộ repository thay vì chỉ “checkout” mã nguồn. Mỗi người dùng đều có bản sao đầy đủ, giúp sao lưu và khôi phục dễ dàng.

- **Data Assurance:** Git đảm bảo tính toàn vẹn dữ liệu bằng cách kiểm tra từng tập tin và commit. Mọi thay đổi đều tạo ID mới, giúp bảo toàn lịch sử dự án.

### 3️⃣ Một số thuật ngữ cần biết:

- **git:** Tiền tố cho lệnh CLI trong Git.

- **repository:** Kho lưu trữ mã nguồn và dữ liệu dự án.

- **branch:** Nhánh phân chia version khi có sự khác biệt.

- **commit:** Điểm trên Work Tree, thể hiện trạng thái mã nguồn.

- **clone:** Sao chép repository về máy để tiếp tục phát triển.

- **fork:** Sao chép repository của người khác về tài khoản Git của mình.

- **tag:** Đánh dấu commit quan trọng.

- **remote:** Điều khiển nhánh từ repository trên Git server.

- **diff:** So sánh sự khác biệt giữa hai phiên bản.

- **.gitignore:** File loại bỏ các thư mục/tệp không muốn push lên Git.

### 4️⃣ Cài đặt Git:

Phần mềm mà ta cần tên là **Git**

Trang cài đặt: [Tại đây](https://git-scm.com/downloads)

#### Đối với Windows OS:

- **Bước 1:** Tại file `.exe` từ trang web trên.

- **Bước 2:** Mở file cài đặt, làm theo hướng dẫn (có thể để mặc định).

- **Bước 3:** Sau khi cài đặt xong, dùng lệnh sau để kiểm tra.

```
git --version
```
#### Đối với MAC OS:

**Cách 1:** Dùng Homebrew *(Khuyến nghị)*

- **Bước 1:** Dùng lệnh sau để cài đặt

```
brew install git
```

- **Bước 2:** Sau khi cài đặt xong, dùng lệnh sau để kiểm tra.

```
git --version
```

**Cách 2:** Tải file về như của Window

- **Bước 1:** Tại file theo định dạng MAC từ trang web trên.

- **Bước 2:** Mở file cài đặt, làm theo hướng dẫn (có thể để mặc định).

- **Bước 3:** Sau khi cài đặt xong, dùng lệnh sau để kiểm tra.

```
git --version
```

#### Đối với Linux:

Mở terminal và chạy các lệnh sau:

```
sudo apt update
sudo apt install git -y
git --version
```

### 5️⃣ Github:

Truy cập: [Tại đây](https://github.com/)

Nói đơn giải, **github** có thể xem như là 1 loại mạng xã hội, đây là hệ thống quản lý các dự án, lưu trữ các source code do người dùng push lên, nơi giúp người trong một nhóm có thể theo dõi các tiến trình trong quy trình xây dựng ứng dụng.

#### Tạo 1 repository căn bản

- **Bước 1:** Truy cập vào trang chủ *github* và tiến hành đăng nhập/đăng ký.

- **Bước 2:** Tạo 1 repository mới khi mới đăng nhập vào.

![ảnh 1](/docs/Tutorial/img/git/1.png)

- **Bước 3:** Cài đặt thông tin cơ bản cho respository.

![ảnh 2](/docs/Tutorial/img/git/2.png)

- **Bước 4:** Để push file lên respository mới tạo, tại folder muốn push, mở terminal và sử dụng các lệnh sau.

*1. Lệnh khởi tạo git*
```
git init
```

*2. Thêm remote các file*
```
git add .
```

*3. Tiến hành commit file*
```
git commit -m "message"
```

*4. Thêm remote respository*
```
git remote add origin https://github.com/username/tên-repository.git
```

*5. Tiến hành push nội dung lên branch*
```
git push -u origin new-branch
```

#### Tạo branch mới trên github

*Hàm kiểm tra các branch hiện có*
```
git branch
```

*Tạo branch mới*
```
git branch new-branch
```

*Chuyển qua branch mới*
```
git checkout new-branch
```

*Vừa tạo vừa chuyển qua branch mới*
```
git checkout -b new-branch
```

#### Tải nội dung trên github về thiết bị

- **Dùng lệnh clone**
```
git clone https://github.com/username/respository_name.git
```

- **Dùng Github desktop**

Tải github desktop: [tại đây](https://github.com/apps/desktop)

- **Dùng git pull**
```
git pull origin branch_name
```