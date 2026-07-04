---
title: "Worklog Tuần 6"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6:
* Tìm hiểu và cấu hình AWS API Gateway để định tuyến và chuyển tiếp các yêu cầu HTTP.
* Tạo REST API tích hợp với Lambda để kết nối và truyền dữ liệu cho ứng dụng Front-end.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 3 | - Tổng quan API Gateway: Học cơ chế định tuyến từ Front-end qua API Gateway tới Lambda | 26/05/2026 | 26/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Triển khai Lambda API: Viết Lambda function truy vấn dữ liệu từ DynamoDB và trả về dạng JSON | 27/05/2026 | 27/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Thiết lập API Gateway: Khởi tạo REST API trên API Gateway, cấu hình GET/POST và bật CORS | 28/05/2026 | 28/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Kiểm tra với Postman: Gửi các request HTTP qua Postman, kiểm tra lỗi CORS và phân quyền | 29/05/2026 | 29/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 7 | - Front-end gọi API: Xây dựng Front-end đơn giản để gọi API Gateway nhận dữ liệu | 30/05/2026 | 30/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| CN | - Kiểm tra hệ thống: Chạy tích hợp toàn bộ luồng Front-to-Back, render dữ liệu ra màn hình | 31/05/2026 | 31/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Dọn dẹp tài nguyên: Ôn tập quy trình tích hợp và xóa các tài nguyên AWS đã tạo | 01/06/2026 | 01/06/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 6:
* Hiểu rõ cơ chế định tuyến và chuyển tiếp API của AWS API Gateway.
* Xây dựng và triển khai thành công Lambda function trả về payload JSON chuẩn.
* Cấu hình thành công REST API trên API Gateway, bật tính năng CORS cho phép domain lạ truy cập.
* Sử dụng thành thạo Postman để debug, test API và xử lý triệt để các lỗi CORS.
* Kết nối thành công mã nguồn Frontend tĩnh với endpoint của API Gateway.
* Hoàn thiện một ứng dụng Full-stack Serverless hoàn chỉnh có tương tác database.
* Nắm vững cách giải phóng tài nguyên AWS để tối ưu ngân sách.
