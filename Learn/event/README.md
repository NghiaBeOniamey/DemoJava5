# Portal Event

## Module Quản lý Sự kiện

## Mục lục

- [Giới thiệu](#giới-thiệu)
- [Actor](#Actor-Mô-tả-quyền-hạn)
- [Yêu cầu hệ thống](#yêu-cầu-hệ-thống)
- [Cài đặt và sử dụng](#cài-đặt-và-sử-dụng)
- [Liên hệ](#liên-hệ)

## Giới thiệu

Portal Event giúp quản lý thông kê các sự kiện. Dự án này nhằm mục đích tạo ra một hệ thống quản lý sự kiện cho hệ thống fpt lưu trữ, thông kê các thông tin liên quan đến sự kiện.

### Actor Mô tả quyền hạn

#### Sinh Viên:
* Đăng ký tham gia sự kiện `đã phê duyệt`.
* Điểm danh sự kiện `đã phê duyệt` tại thời điểm ``người tổ chức`` `mở đăng ký sự kiện`.

#### Giảng Viên:
* `Người đăng ký` tổ chức sự kiện.
* `Xuất` file danh sách điểm danh, danh sách đăng ký tham gia sự kiện
* Có thể quản lý các thông tin sự kiện: danh sách `người tổ chức`, danh sách `agenda`, danh sách `địa điểm`, danh sách `tài nguyên`, danh sách 'điểm danh', `đăng ký` sự kiện, `minh chứng`.

#### Chủ Nhiệm Bộ Môn:
* Thực hiện phê duyệt các sự kiện `chờ phê duyệt` thành sự kiện ` được bộ môn thông qua`.
* `Thống kê` và `xuất` file báo cáo thông tin chi tiết của sự kiện theo Học Kỳ và Cơ Sở, Bộ Môn của `chủ nhiệm bộ môn`.
* `Xuất` file danh sách điểm danh, danh sách đăng ký tham gia sự kiện.
* Xem chi tiết thông tin của 1 sự kiện.
danh sách `người tổ chức`, danh sách `agenda`, danh sách `địa điểm`, danh sách `tài nguyên`, danh sách 'điểm danh', `đăng ký` sự kiện, `minh chứng`.

#### Quản Lý Đào Tạo:
* `Thống kê` và `xuất` file sự kiện theo học kỳ, bộ môn và cơ sở của quản lý đào tạo.
* `Xuất` file danh sách điểm danh, danh sách đăng ký tham gia sự kiện.
* Xem chi tiết thông tin của 1 sự kiện.
danh sách `người tổ chức`, danh sách `agenda`, danh sách `địa điểm`, danh sách `tài nguyên`, danh sách 'điểm danh', `đăng ký` sự kiện, `minh chứng`.
* Quản lý bộ môn theo cơ sở với cơ sở dự liệu tập trung `Identity` bằng cách đồng bộ dữ liệu.

#### Trưởng Ban Đào Tạo
* Thực hiện phê duyệt các sự kiện đã được `bộ môn thông qua` thành sự kiện `đã thông qua TBDTCS` .
* `Thống kê` và `xuất` file sự kiện theo học kỳ, bộ môn và cơ sở của quản lý đào tạo.
* `Xuất` file danh sách điểm danh, danh sách đăng ký tham gia sự kiện.
* Xem chi tiết thông tin của 1 sự kiện 
danh sách `người tổ chức`, danh sách `agenda`, danh sách `địa điểm`, danh sách `tài nguyên`, danh sách 'điểm danh', `đăng ký` sự kiện, `minh chứng`

#### Giám Đốc Cơ Sở
* Thực hiện phê duyệt các sự kiện đã được `TBDTCS thông qua` thành sự kiện `đã phê duyệt` .
* `Thống kê` và `xuất` file sự kiện theo học kỳ, bộ môn và cơ sở của quản lý đào tạo.
* `Xuất` file danh sách điểm danh, danh sách đăng ký tham gia sự kiện.
* Xem chi tiết thông tin của 1 sự kiện
  danh sách `người tổ chức`, danh sách `agenda`, danh sách `địa điểm`, danh sách `tài nguyên`, danh sách 'điểm danh', `đăng ký` sự kiện, `minh chứng`

#### Ban Đào Tạo: (HO)
* `Thống kê` và `xuất file` sự kiện theo học kỳ, bộ môn, cơ sở.
* `Xuất` file danh sách điểm danh, danh sách đăng ký tham gia sự kiện.
* Xem chi tiết thông tin của 1 sự kiện 
danh sách `người tổ chức`, danh sách `agenda`, danh sách `địa điểm`, danh sách `tài nguyên`, danh sách 'điểm danh', `đăng ký` sự kiện, `minh chứng`
* Quản lý thể loại, đối tượng sự kiện. 
* Quản lý bộ môn, cơ sở với cơ sở dự liệu tập trung `Identity` bằng cách đồng bộ dữ liệu

## Yêu cầu hệ thống

### Backend Project

- JDK >= 17 (19 recommended)
- Intellij IDEA >= 2020.3 (MAX-VERSION recomended)
- SQL Server (MAX-VERSION recomended)

### Frontend Project

- Node.js >= 14.0.0 (v20.15.0 recommended)
- npm >= 6.0.0 (v10.7.0 recommended)

## Cài đặt và sử dụng

Clone repository:

```sh
git clone https://github.com/FPLHN-FACTORY/udpm-portal-events.git
```

### Backend Project

1. Mở BE với Intellij IDEA (đợi Intellij IDEA load dự án Gradlle).

2. Sau khi load dự án Gradlle xong, mở terminal và chạy lệnh sau để tạo file .env:

```sh
  echo  >> .env
   ```

```sh
  ctrl + C
   ```

3. Cấu hình các biến môi trường:

`#mysql` và `#yourpassword` cần đổi

```.env
DATABASE_USERNAME=root
DATABASE_PASSWORD=123456
DATABASE_HOSTNAME=localhost
DATABASE_DDL=update
IDENTITY_DOMAIN=http://localhost:5000
COMSUMER_DOMAIN=https://factory.udpm-hn.com/
HONEY_DOMAIN=https://honey.udpm-hn.com
##authen
#IDENTITY_CLIENT_WEB_ID=94d890604c930bf4e018f11b5f8498e1fefea0033e93adbdd601cb14b3bb6360
#IDENTITY_CLIENT_WEB_SECRET=ZVGSakiG++yF0JSyR+ySRAdoRB8=
##local
IDENTITY_CLIENT_LOCAL_ID=87e749c7a2c41e2829de5e5d87460b2b20a449316fd1ff270d3134892433c0c2
IDENTITY_CLIENT_LOCAL_SECRET=1DK5ubuIEntHit+i6XtSI/kv5io=
````

4. Cấu hình sql:

```SQL Server
CREATE DATABASE portal_event
```
5. Run Backend Project

### Frontend Project

1. Mở FE với Visual Code Studio.
2. Mở terminal và chạy lệnh sau để tạo file .env

```sh
  echo  >> .env
```

```sh
  ctrl + C
```

3. Cấu hình các biến môi trường:

```.env
PORT=9999
REACT_APP_IDENTITY_WEB=https://authentication.udpm-hn.com/
REACT_APP_HOST_IP_ADDRESS=http://localhost:1626/
REACT_APP_HOST_IDENTITY_IP_ADDRESS=https://event.udpm-hn.com/
REACT_APP_EVENT_IP_ADDRESS_WEB=http://localhost:9999/
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

## Liên hệ

Nếu bạn có bất kỳ câu hỏi nào, vui lòng liên hệ qua email [hieunmph42056@fpt.edu.vn] OR [nghiabe.dev@gmail.com].
