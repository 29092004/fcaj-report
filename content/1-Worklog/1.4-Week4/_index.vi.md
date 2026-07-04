---
title: "Worklog Tuần 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4:
* Nắm vững kiến thức IAM Role, phân biệt với IAM User/Access Key.
* Thực hành gán IAM Role cho EC2 instance và thực hiện truy cập an toàn bằng CLI tuân thủ Least Privilege.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 3 | - IAM Role Overview: Học lý thuyết IAM Role, Assume Role và phân biệt với IAM User | 12/05/2026 | 12/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 4 | - Access Key vs IAM Role: So sánh ưu nhược điểm bảo mật của hai phương thức | 13/05/2026 | 13/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - IAM Role trên EC2: Tạo và gán IAM Role cho EC2 để cấp quyền truy cập S3 | 14/05/2026 | 14/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - AWS CLI với IAM Role: Sử dụng AWS CLI kiểm tra các lệnh S3 qua IAM Role của EC2 | 15/05/2026 | 15/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 7 | - Best Practice: Nghiên cứu nguyên tắc Least Privilege trong thiết kế IAM Role | 16/05/2026 | 16/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| CN | - IAM Role Lab: Thực hành tạo nhiều IAM Role và kiểm tra phân quyền | 17/05/2026 | 17/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 2 | - Tổng hợp IAM Role: Ôn tập lại kiến thức IAM Role và quy trình tích hợp EC2 | 18/05/2026 | 18/05/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:
* Hiểu rõ khái niệm IAM Role, Assume Role và sự khác biệt với IAM User thông thường.
* Nhận thức rõ tại sao nên sử dụng IAM Role thay thế cho Access Key truyền thống.
* Cấu hình thành công EC2 instance truy cập S3 một cách an toàn thông qua IAM Role.
* Kiểm tra và chạy thành công lệnh AWS CLI mà không cần cấu hình Access Key trực tiếp.
* Áp dụng nguyên tắc Least Privilege (quyền tối thiểu) vào thiết kế hệ thống phân quyền AWS.
* Thành thạo quy trình tạo, chỉnh sửa và gán IAM Role cho các tài nguyên AWS.
* Nắm vững các Best Practice về bảo mật tài khoản AWS.
