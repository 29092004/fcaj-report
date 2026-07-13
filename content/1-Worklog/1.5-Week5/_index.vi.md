---
title: "Worklog Tuần 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu tuần 5:
* Tìm hiểu kiến trúc Serverless trên AWS với Lambda, S3, và DynamoDB.
* Thiết lập một quy trình xử lý ảnh tự động và ghi dữ liệu log vào cơ sở dữ liệu NoSQL DynamoDB.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2-3 | - Giới thiệu Serverless: Tìm hiểu khái niệm Serverless, vai trò của Lambda, S3, DynamoDB | 18/05/2026 | 19/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4-5 | - Thiết lập DynamoDB: Tạo bảng DynamoDB và định nghĩa Partition Key | 20/05/2026 | 21/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Cấu hình IAM Role: Cấp quyền truy cập tối thiểu (Least Privilege) cho Lambda vào S3/DynamoDB | 22/05/2026 | 22/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 7-CN | - Serverless Lab: Thực hành chạy toàn bộ luồng xử lý ảnh và dọn dẹp tài nguyên | 23/05/2026 | 24/05/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 5:
* Hiểu tổng quan về kiến trúc Serverless và cơ chế hoạt động của Lambda.
* Viết thành công hàm Lambda tự động resize/tối ưu kích thước ảnh khi upload lên S3.
* Khởi tạo bảng DynamoDB thành công và thiết kế cấu trúc dữ liệu NoSQL cơ bản.
* Tích hợp thành công SDK trong Lambda để lưu metadata ảnh vào DynamoDB.
* Áp dụng bảo mật phân quyền IAM Role tối thiểu (Least Privilege) cho Lambda function.
* Vận hành thử nghiệm thành công toàn bộ luồng Event-driven (S3 trigger Lambda -> ghi DB).
* Hiểu cách dọn dẹp tài nguyên để tối ưu hóa chi phí AWS.
