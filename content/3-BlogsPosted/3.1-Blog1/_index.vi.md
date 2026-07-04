---
title: "AI Gateway – Giải pháp quản lý AI trên AWS"
date: 2026-06-29
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# AI Gateway – Giải pháp quản lý AI trên AWS với Amazon Bedrock và Amazon API Gateway

Khi các ứng dụng AI tạo sinh ngày càng được sử dụng rộng rãi trong doanh nghiệp, việc cho phép mọi hệ thống truy cập trực tiếp vào mô hình AI có thể dẫn đến nhiều vấn đề như khó kiểm soát chi phí, thiếu cơ chế phân quyền và khó theo dõi mức độ sử dụng.

Để giải quyết vấn đề này, AWS đề xuất mô hình AI Gateway, sử dụng Amazon API Gateway làm lớp trung gian giữa người dùng và Amazon Bedrock. Kiến trúc này giúp doanh nghiệp kiểm soát quyền truy cập, giới hạn số lượng yêu cầu, theo dõi chi phí và tăng cường bảo mật khi triển khai các ứng dụng Generative AI.

Mô hình này sử dụng Amazon API Gateway làm lớp truy cập phía trước Amazon Bedrock. Giải pháp hỗ trợ nhiều tính năng quan trọng như xác thực và phân quyền người dùng thông qua các hệ thống nhận dạng hiện có (ví dụ: JWT), quản lý hạn mức sử dụng, điều tiết lưu lượng truy cập, quản lý vòng đời API, triển khai thử nghiệm (Canary Release) và tăng cường bảo mật thông qua AWS WAF.

Ngoài ra, API Gateway còn hỗ trợ cơ chế truyền phản hồi theo thời gian thực (Streaming Response), cho phép kết quả từ mô hình AI được gửi trực tiếp đến người dùng ngay khi được tạo ra thay vì phải chờ hoàn tất toàn bộ quá trình xử lý.

Nhờ những khả năng này, AI Gateway không chỉ đóng vai trò là cổng truy cập vào Amazon Bedrock mà còn giúp doanh nghiệp kiểm soát chi phí, tăng cường bảo mật và quản lý việc sử dụng AI hiệu quả hơn ở quy mô lớn.

## Kiến trúc của cổng AI

Kiến trúc tham chiếu cung cấp cho bạn khả năng kiểm soát chi tiết quyền truy cập LLM bằng cách sử dụng các dịch vụ AWS được quản lý hoàn toàn. Nó hoạt động minh bạch đối với các ứng dụng khách và tích hợp liền mạch vào môi trường doanh nghiệp hiện có.

![Kiến trúc tham chiếu của cổng AI](/images/3-BlogsPosted/3.1-Blog1/ai-gateway-diagram.png)
*Hình 1. Kiến trúc tham chiếu của cổng AI.*

Giải pháp bao gồm bốn thành phần cốt lõi:

* **Amazon Route 53:** Chịu trách nhiệm quản lý Custom Domain Routing, cho phép người dùng truy cập AI Gateway thông qua tên miền riêng của doanh nghiệp thay vì sử dụng domain mặc định của Amazon API Gateway. Điều này giúp hệ thống chuyên nghiệp hơn và dễ dàng tích hợp vào hạ tầng hiện có của tổ chức.
* **Amazon API Gateway:** Đóng vai trò là Entry Point cho toàn bộ request gửi đến hệ thống AI. Dịch vụ này cung cấp nhiều tính năng quan trọng như Authorization, Request Throttling, Lifecycle Management, Rate Limiting và Monitoring, giúp doanh nghiệp kiểm soát quyền truy cập, quản lý lưu lượng request, theo dõi hoạt động của hệ thống và đảm bảo tính ổn định, bảo mật cho các ứng dụng AI.
* **AWS Lambda Authorizer:** Chịu trách nhiệm xử lý Authorization cho các request, trong đó ở triển khai của Dynatrace, thành phần này thực hiện việc xác thực JWT Token với các hệ thống Authentication hiện có. Đối với từng nhu cầu triển khai cụ thể, bạn có thể xây dựng Authorization Logic riêng trong Lambda Authorizer, tích hợp với Amazon Cognito User Pools hoặc sử dụng các API Gateway Authorization Mechanisms khác.
* **Lambda Integration:** Là một Dynamic Request Forwarder có nhiệm vụ ký các request đến bằng AWS Credentials và định tuyến chúng đến các Amazon Bedrock Endpoints phù hợp. Thành phần này giữ nguyên toàn bộ thông tin của request ban đầu, bao gồm API Action và Parameters, nhằm hỗ trợ các Amazon Bedrock APIs hiện tại cũng như trong tương lai mà không cần thay đổi mã nguồn. Toàn bộ phần triển khai được cung cấp trong Integration Lambda Function.
* **Amazon Bedrock:** Cung cấp quyền truy cập đến các Foundation Models và các khả năng AI.

Ưu điểm của kiến trúc này là tính minh bạch đối với các Client Applications và thiết kế có khả năng đáp ứng các nhu cầu trong tương lai (Future-Proof Design). Các ứng dụng khách có thể sử dụng AWS SDKs (chẳng hạn như Boto3) để truy cập các chức năng của Amazon Bedrock (như LLMs và Knowledge Bases) tương tự như khi gọi trực tiếp Amazon Bedrock API. Trong khi đó, AI Gateway xử lý Authorization, Quota Management và các khả năng khác ở phía sau hệ thống.

## Phần kết luận

Mô hình cổng AI được trình bày trong bài viết này cung cấp một cách thức có khả năng mở rộng để quản lý quyền truy cập vào các mô hình nền tảng và công cụ tác nhân thông qua Amazon Bedrock. Ban đầu được phát triển và triển khai bởi Dynatrace để phục vụ cơ sở người dùng toàn cầu của họ, mô hình này đã chứng minh hiệu quả ở quy mô doanh nghiệp. Bằng cách sử dụng các tính năng doanh nghiệp của Amazon API Gateway, các tổ chức có thể triển khai các biện pháp kiểm soát cần thiết trong khi vẫn duy trì được lợi ích của kiến trúc không máy chủ.

---

* **Link bài viết gốc:** [Building an AI Gateway to Amazon Bedrock with Amazon API Gateway](https://aws.amazon.com/blogs/architecture/building-an-ai-gateway-to-amazon-bedrock-with-amazon-api-gateway/)