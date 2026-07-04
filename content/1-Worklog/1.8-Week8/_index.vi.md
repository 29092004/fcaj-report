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
| 3 - 4 | - Kiến trúc tích hợp: Nghiên cứu cơ chế giao tiếp Frontend (S3) - API Gateway - Lambda | 09/06/2026 | 10/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 - 6 | - Cấu hình & Gọi API: Thiết lập biến môi trường và viết mã nguồn fetch gọi API Gateway từ Frontend | 11/06/2026 | 12/06/2026 | <https://cloudjourney.awsstudygroup.com/>|
| 7 - CN | - Triển khai lên S3: Đóng gói code Frontend, cấu hình Static Website Hosting trên S3 và CloudFront | 13/06/2026 | 14/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Kiểm thử tích hợp: Deploy toàn bộ hệ thống lên Cloud và chạy thử nghiệm luồng thực tế | 15/06/2026 | 15/06/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 8:
* Hiểu rõ mô hình phân tách độc lập (decoupled) giữa Frontend và Backend Serverless.
* Cấu hình và kết nối thành công Frontend local gọi đúng các URL API của API Gateway.
* Đóng gói mã nguồn Frontend và deploy thành công lên AWS S3 bucket.
* Cấu hình thành công tính năng Static Website Hosting cho S3.
* Tích hợp thành công toàn bộ hệ thống trên môi trường live AWS Cloud.
* Phát hiện và xử lý thành công một số lỗi kết nối và cấu hình CORS.
