---
title: "Worklog Tuần 8"
date: 2026-06-08
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8:
* Xây dựng tích hợp luồng trao đổi dữ liệu giữa Frontend và Backend Serverless.
* Triển khai lưu trữ Frontend tĩnh lên AWS S3 và chạy thử nghiệm tích hợp hệ thống.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 - 3 | - Kiến trúc tích hợp: Nghiên cứu cơ chế giao tiếp Frontend (S3) - API Gateway - Lambda | 08/06/2026 | 09/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 - 5 | - Cấu hình & Gọi API: Thiết lập biến môi trường và viết mã nguồn fetch gọi API Gateway từ Frontend | 10/06/2026 | 11/06/2026 | <https://cloudjourney.awsstudygroup.com/>|
| 6 - 7 | - Triển khai lên S3: Đóng gói code Frontend, cấu hình Static Website Hosting trên S3 và CloudFront | 12/06/2026 | 13/06/2026 | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 8:
* Hiểu rõ mô hình phân tách độc lập (decoupled) giữa Frontend và Backend Serverless.
* Cấu hình và kết nối thành công Frontend local gọi đúng các URL API của API Gateway.
* Đóng gói mã nguồn Frontend và deploy thành công lên AWS S3 bucket.
* Cấu hình thành công tính năng Static Website Hosting cho S3.
* Tích hợp thành công toàn bộ hệ thống trên môi trường live AWS Cloud.
* Phát hiện và xử lý thành công một số lỗi kết nối và cấu hình CORS.