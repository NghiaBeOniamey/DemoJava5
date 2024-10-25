# Articles Management

## Module Quản lý bài viết

## Mục lục

- [Giới thiệu](#giới-thiệu)
- [Actor](#Actor)
- [Yêu cầu hệ thống](#yêu-cầu-hệ-thống)
- [Cài đặt và sử dụng](#cài-đặt-và-sử-dụng)
- [Liên hệ](#liên-hệ)

## Giới thiệu

Articles Management giúp quản lý thông kê các bài viết. Dự án này nhằm mục đích tạo ra một hệ thống quản lý bài viết cho hệ thống fpt, thông kê các thông tin liên quan đến bài viết.

### Actor

##### Giảng Viên Viết Bài:

<!-- * Viết bài viết theo yêu cầu -->

##### Admin

<!-- * Phê duyệt bài viết -->

##### Trưởng Phòng PR

<!-- * Chọn lọc bài viết từ kho lưu trữ -->

##### Nhân Viên Phòng PR

<!-- * Chọn lọc bài viết từ kho lưu trữ -->

## Yêu cầu hệ thống

### Backend Project

- JDK >= 17 (19 recommended)
- Intellij IDEA >= 2020.3 (MAX-VERSION recomended)
- SQL Server (MAX-VERSION recomended)

## Cài đặt và sử dụng

1. Clone Repository.

   ```sh
   git clone https://github.com/FPLHN-FACTORY/udpm-portal-articles-convert.git
   ```

2. Mở BE với Intellij IDEA (đợi Intellij IDEA load dự án Gradlle).

3. Sau khi load dự án Gradlle xong, mở terminal và chạy lệnh sau để tạo file .env:

   ```sh
   echo  >> .env
   ctrl + C
   ```

4. Cấu hình sql:

   ```MySQL
   CREATE DATABASE article_project
   ```

5. Cấu hình các biến môi trường:

   ```
   Note: Điều kiện cần có:

   - Đã có database name article_project.

   - Điền đẩy đủ các trường trống.

   - Đổi DOMAIN_IDENTITY, IDENTITY_ID, CLIENT_SECRET thành domain và mã được đăng ký tại DOMAIN_IDENTITY đó.

   ```

   ```.env
   DATABASE_USERNAME=
   DATABASE_PASSWORD=
   DATABASE_HOSTNAME=localhost
   DATABASE_DDL=update
   DATABASE_DRIVER=com.mysql.cj.jdbc.Driver
   DATABASE_URL=jdbc:mysql://localhost:3306/article_project
   DOMAIN_IDENTITY=https://authentication.udpm-hn.com/
   IDENTITY_SECRET=keytoken_NVT25102002@123456789abcdefgh
   IDENTITY_CLIENT_ID=f9c4125b0d63f1db8e828aeae9f88fdcc1b0ae2e37397482f572ab95bd2ac085
   IDENTITY_CLIENT_SECRET=P2EF8eDZEiosgvXm8SIjnRy2E9U=
   ```

6. Run Backend Project.

7. Cấu hình sql: (Chạy 1 lần từng câu lệnh)

   ```MySQL
    ALTER TABLE article_project.articles ADD FULLTEXT(title);
   ```

   ```MySQL
   ALTER TABLE article_project.articles ADD FULLTEXT(descriptive);
   ```

   ```MySQL
   ALTER TABLE article_project.articles ADD FULLTEXT(content);
   ```

   ```MySQL
   ALTER TABLE article_project.category ADD FULLTEXT(name);
   ```

   ```MySQL
   ALTER TABLE article_project.users ADD FULLTEXT(name);
   ```

8. Đăng nhập thông qua Identity.

## Liên hệ

Nếu bạn có bất kỳ câu hỏi nào, vui lòng liên hệ qua email nghiabe.dev@gmail.com hoặc truy cập [FPL-HNFACTORY](https://fplhn-factory.github.io/) liên hệ trực tiếp leader.