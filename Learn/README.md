# Identity Project

Identity Project giúp quản lý dữ liệu tập trung, phân quyền và chuyển hướng. Dự án này nhằm mục đích tạo ra một hệ thống quản lý dữ liệu bảo mật và hiệu quả cho các ứng dụng doanh nghiệp.

## Mục lục

- [Giới thiệu](#giới-thiệu)
- [Yêu cầu hệ thống](#yêu-cầu-hệ-thống)
- [Cài đặt](#cài-đặt)
- [Cách sử dụng](#cách-sử-dụng)
- [Liên hệ](#liên-hệ)

## Giới thiệu

Identity Project giúp quản lý dữ liệu tập trung, phân quyền và chuyển hướng. Dự án này nhằm mục đích tạo ra một hệ thống quản lý dữ liệu bảo mật và hiệu quả cho các ứng dụng doanh nghiệp.

## Yêu cầu hệ thống

### Backend Project

- JDK >= 17 (19 recommended)
- Intellij IDEA >= 2020.3 (MAX-VERSION recomended)
- SQL Server (MAX-VERSION recomended)

### Frontend Project

- Node.js >= 14.0.0 (v20.15.0 recommended)
- npm >= 6.0.0 (v10.7.0 recommended)

Upgrade Yarn

- yarn >= 1.22.10 (v1.22.22 recomended) 

## Cài đặt

Clone repository:

```sh
git clone https://github.com/FPLHN-FACTORY/udpm-identity-java.git
```

### Backend Project

1. Mở IdentityBE với Intellij IDEA (đợi Intellij IDEA load dự án Maven).

2. Sau khi load dự án Maven xong, mở terminal và chạy lệnh sau để tạo file .env:

```sh
  echo  >> .env
   ```

```sh
  ctrl + C
   ```

3. Cấu hình các biến môi trường:

`Your password` cần đổi

```.env
#DATABASE ENVIRONMENT
DATABASE_HOSTNAME=localhost
DATABASE_USERNAME=sa
DATABASE_PASSWORD= `Your password`
DATABASE_DDL_AUTO=update
DATABASE_NAME=identity_project

#EXCEL PATH ENVIRONMENT
EXCEL_FOLDER=src/main/resources/excel/
EXCEL_FOLDER_ROLE=role-saved/

#GOOGLE OAUTH2 ENVIRONMENT
# Apply another GG_ID and GG_SECRET for production
#GOOGLE_CLIENT_ID=
#GOOGLE_CLIENT_SECRET=

#SERVER ENVIRONMENT
SERVER_PORT=5000

#FRONTEND URL
#FRONTEND_URL=http://localhost:3000

#MAIL ENVIRONMENT
HOST_MAIL= # your email
MAIL_TO_SEND=minhhieu8723@gmail.com
````

4. Cấu hình sql:

```SQL Server
CREATE DATABASE identity_project
```

5. Run project Backend and return your SQL SERVER

```SQL Server
UPDATE module SET xoa_mem = 'NOT_DELETED'
```

`yourName _ yourMail@fe.edu.vn _ yourMail@fpt.edu.vn` cần đổi tại `*`

```SQL SERVER
INSERT INTO nhan_vien
(id_bo_mon_theo_co_so, id_co_so, avatar, ho_ten, ma_nhan_vien, so_dien_thoai, tai_khoan_fe, tai_khoan_fpt, xoa_mem)
VALUES(null, null, null, N'*', '*', '*', '*', '*', 'NOT_DELETED')
```

 `id_nhan_vien (id chứa your mail)` cần đổi tại `*`

```
INSERT INTO identity_project.dbo.[nhan_vien-chuc_vu]
(id_chuc_vu, id_modules, id_nhan_vien, xoa_mem)
VALUES(1, 1, *), 'NOT_DELETED');
```

### Frontend Project

1. Mở Identity_fe với Visual Code Studio.
2. Mở terminal và chạy lệnh sau để tạo file .env

```sh
  echo  >> .env
```

```sh
  ctrl + C
```

3. Cấu hình các biến môi trường:

```.env
REACT_APP_BACKEND_DOMAIN=http://localhost:5000
REACT_APP_URL_BACKEND_OAUTH2=http://localhost:5000
REACT_APP_FRONT_DOMAIN=http://localhost:3000
REACT_APP_SECRET_KEY=pFBSx4[O}|7.6h7
REACT_APP_NODE_ENV=development
BROWSER=none
````

4. Chạy project_fe with terminal:
Với npm:

```sh
   npm i
```

Đợi npm load xong và chạy:

```sh
   npm start
```

Với yarn:

```sh
   yarn install
```

Đợi yarn load xong và chạy:

```sh
   yarn start
```

## Liên hệ

Nếu bạn có bất kỳ câu hỏi nào, vui lòng liên hệ qua email [hieunmph42056@fpt.edu.vn] OR [nghiabe.dev@gmail.com].
