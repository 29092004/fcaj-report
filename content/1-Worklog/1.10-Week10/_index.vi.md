---
title: "Worklog Tuần 10"
date: 2026-06-22
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu tuần 10:
* Truy vấn và hiển thị động dữ liệu từ DynamoDB lên giao diện danh sách của ứng dụng.
* Xây dựng trang chi tiết Job, triển khai Lambda function xử lý API chi tiết và hoàn thiện kiểm thử.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 - 4 | - Đổ dữ liệu lên UI: Gọi API để hiển thị danh sách Job động từ DynamoDB lên giao diện | 22/06/2026 | 24/06/2026 | AWS Console |
| 5 - 6 | - Xây dựng trang chi tiết: Thiết kế giao diện và xử lý logic lọc Job theo ID trên URL | 25/06/2026 | 26/06/2026 | Figma / UI Design |
| 7 - CN | - Deploy Lambda API: Viết và deploy Lambda function hỗ trợ lấy thông tin chi tiết Job theo ID | 27/06/2026 | 28/06/2026 | AWS Console / SAM |
| 2 | - Kiểm thử toàn diện: Chạy thử luồng người dùng click chọn Job -> gọi Lambda -> lấy DB -> hiển thị | 29/06/2026 | 29/06/2026 | AWS Console |

### Kết quả đạt được tuần 10:
* Đổ dữ liệu thành công từ DynamoDB để hiển thị động danh sách Job trên giao diện người dùng.
* Hoàn thiện thiết kế và luồng xử lý nhận diện ID của trang chi tiết Job.
* Viết và triển khai thành công Lambda API phục vụ truy vấn thông tin chi tiết của một Job cụ thể.
* Deploy thành công API chi tiết Job lên AWS.
* Hoàn thành kiểm thử toàn diện tích hợp luồng xử lý từ Frontend đến Database trên Cloud.
* Đảm bảo ứng dụng chạy mượt mà, không phát sinh lỗi liên quan đến dữ liệu động.
