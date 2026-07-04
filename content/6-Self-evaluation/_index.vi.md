---
title: "Tự đánh giá"
date: 2026-07-03
weight: 6
chapter: false
pre: " <b> 6. </b> "
---


Trong suốt thời gian thực tập tại **Công ty TNHH Amazon Web Services Việt Nam** từ **17/04/2026** đến **12/07/2026**, tôi đã có cơ hội học hỏi, rèn luyện và áp dụng kiến thức đã được trang bị tại trường vào môi trường làm việc thực tế.

Cụ thể, quá trình tham gia hoạt động và đóng góp của tôi bao gồm:
* **Học tập và nghiên cứu các dịch vụ đám mây AWS:** Tiếp cận và làm quen với các khái niệm hạ tầng cốt lõi như cấu hình mạng riêng tư ảo (**VPC**), quản lý phân quyền bảo mật tối giản (**IAM**), mô hình kiến trúc serverless (**Serverless**), công cụ triển khai mã nguồn dưới dạng hạ tầng (**AWS SAM**), và nền tảng hỗ trợ lưu trữ - phân phối ứng dụng (**AWS Amplify**).
* **Phát triển dự án Jobs-Matching-Platform:** 
  * Thiết kế và xây dựng giao diện ứng dụng phía người dùng sử dụng framework Next.js hiện đại, đảm bảo tính responsive, giao diện trực quan và trải nghiệm mượt mà.
  * Tích hợp cơ chế gọi API để lấy và hiển thị dữ liệu động từ cơ sở dữ liệu **DynamoDB** lên trang chủ (**Home Page**) và trang thông tin chi tiết (**Job Detail Page**).
  * Tính năng tìm kiếm, lọc công việc nhanh chóng (**Search Jobs**) để tăng tính tương tác và tiện ích tối đa cho người dùng.
  * Thiết kế hạ tầng và triển khai Backend thông qua **AWS SAM**: viết tệp cấu hình **template** (`template.yaml`) để định nghĩa các tài nguyên AWS đám mây (API Gateway, Lambda, DynamoDB) và thực hiện triển khai dự án lên Cloud.
  * Thực hiện **Host Frontend** sử dụng **AWS Amplify Hosting**, cấu hình liên kết repository Git, thiết lập pipeline triển khai tự động CI/CD và cài đặt các **biến môi trường** (`NEXT_PUBLIC_API_BASE_URL`, v.v.) trong Amplify Console để kết nối an toàn tới Backend.
  * Thiết lập và quản lý hệ thống xác thực người dùng sử dụng **Amazon Cognito**: tích hợp luồng Đăng ký/Đăng nhập qua Cognito Managed Login, quản lý Token để bảo vệ an toàn các tuyến đường dẫn tĩnh (Routing Protection) trên Next.js như `/favorites`, `/upload-cv`.
  * Cấu hình phân quyền bảo mật API bằng cách thiết lập bộ xác thực **Cognito JWT Authorizer** trên **API Gateway**, đồng thời quản lý cấu hình chia sẻ tài nguyên nguồn gốc chéo (**CORS**) cho **Amazon S3** phục vụ tải lên CV của ứng viên một cách an toàn.

Thông qua các hoạt động thực hành thực tế trong suốt kỳ thực tập, tôi đã cải thiện và củng cố vững chắc các nhóm kỹ năng cốt lõi sau:

* **Kỹ năng chuyên môn (Technical Skills):**
  * **Lập trình và xây dựng giao diện người dùng:** Làm chủ framework **Next.js** và ngôn ngữ **JavaScript** để phát triển các trang giao diện tối ưu (Home Page, Job Detail Page), tối ưu cấu trúc DOM, hiểu rõ cơ chế Server-Side Rendering (SSR) và Client-Side Rendering (CSR).
  * **Xử lý và tích hợp dữ liệu hệ thống:** Nắm vững cách tích hợp các hàm API Endpoint để gọi và truy xuất dữ liệu động từ cơ sở dữ liệu **Amazon DynamoDB**, biết cách ánh xạ (mapping) và xử lý JSON Response phức tạp hiển thị chính xác lên giao diện.
  * **Kiến trúc phi máy chủ (Serverless Architecture) & Triển khai mã nguồn:** Hiểu sâu về cách viết và quản lý tệp cấu hình hạ tầng `template.yaml` của **AWS SAM** để định nghĩa tài nguyên (Lambda, API Gateway, DynamoDB), thực hiện câu lệnh đóng gói (`sam package`) và triển khai (`sam deploy`) lên Cloud.
  * **Lưu trữ và phân phối tự động (Hosting & CI/CD):** Hiểu quy trình thiết lập Continuous Integration / Continuous Deployment (CI/CD) qua **AWS Amplify Hosting**, biết cách kết nối nhánh Git để tự động kích hoạt tiến trình Build, đồng thời cấu hình quản lý bảo mật các **biến môi trường (Environment Variables)** hệ thống.

* **Kỹ năng bổ trợ (Soft Skills & Professional Work Style):**
  * **Tư duy và kỹ năng giải quyết vấn đề kỹ thuật:** Rèn luyện khả năng phân tích log lỗi (CloudWatch, Console), gỡ lỗi (debugging) hệ thống khi tích hợp API, tự tìm kiếm giải pháp và tối ưu thuật toán tìm kiếm/lọc thông tin.
  * **Nghiên cứu công nghệ độc lập:** Hình thành thói quen và phương pháp tự đọc hiểu tài liệu kỹ thuật chuyên sâu bằng tiếng Anh từ trang chủ AWS (AWS Documentation, Developer Guide) cũng như các diễn đàn công nghệ uy tín để giải quyết độc lập các bài toán kỹ thuật mới khó khăn.
  * **Kỹ năng viết tài liệu kỹ thuật song ngữ:** Học cách biên soạn và trình bày các hướng dẫn kỹ thuật chi tiết theo định dạng Markdown, phân chia bố cục logic và đồng bộ hóa chính xác giữa tiếng Anh và tiếng Việt cho hệ thống tài liệu báo cáo của dự án.
  * **Làm việc nhóm và giao tiếp chuyên nghiệp:** Làm quen với quy trình phát triển Agile/Scrum, cách sử dụng các công cụ quản lý dự án (Jira/Git), chủ động báo cáo tiến độ công việc, chia sẻ khó khăn với Mentor để cùng thảo luận và đưa ra giải pháp tối ưu.  

Về tác phong, tôi luôn cố gắng hoàn thành tốt nhiệm vụ, tuân thủ nội quy, và tích cực trao đổi với đồng nghiệp để nâng cao hiệu quả công việc.

Để phản ánh một cách khách quan quá trình thực tập, tôi xin tự đánh giá bản thân dựa trên các tiêu chí dưới đây:


| STT | Tiêu chí | Mô tả | Đánh giá |
| --- | --- | --- | --- |
| 1 | **Kiến thức và kỹ năng chuyên môn** | Hiểu biết về ngành, áp dụng kiến thức vào thực tế, kỹ năng sử dụng công cụ, chất lượng công việc | Khá |
| 2 | **Khả năng học hỏi** | Tiếp thu kiến thức mới, học hỏi nhanh | Khá |
| 3 | **Chủ động** | Tự tìm hiểu, nhận nhiệm vụ mà không chờ chỉ dẫn | Tốt |
| 4 | **Tinh thần trách nhiệm** | Hoàn thành công việc đúng hạn, đảm bảo chất lượng | Tốt |
| 5 | **Kỷ luật** | Tuân thủ giờ giấc, nội quy, quy trình làm việc | Tốt |
| 6 | **Tính cầu tiến** | Sẵn sàng nhận feedback và cải thiện bản thân | Tốt |
| 7 | **Giao tiếp** | Trình bày ý tưởng, báo cáo công việc rõ ràng | Khá |
| 8 | **Hợp tác nhóm** | Làm việc hiệu quả với đồng nghiệp, tham gia nhóm | Tốt |
| 9 | **Ứng xử chuyên nghiệp** | Tôn trọng đồng nghiệp, đối tác, môi trường làm việc | Tốt |
| 10 | **Tư duy giải quyết vấn đề** | Nhận diện vấn đề, đề xuất giải pháp, sáng tạo | Khá |
| 11 | **Đóng góp vào dự án/tổ chức** | Hiệu quả công việc, sáng kiến cải tiến, ghi nhận từ team | Tốt |
| 12 | **Tổng thể** | Đánh giá chung về toàn bộ quá trình thực tập | Tốt |

### Điểm cần cải thiện và định hướng phát triển

* **Nâng cao tính kỷ luật và phong cách làm việc chuyên nghiệp:** Tiếp tục rèn luyện tác phong làm việc đúng giờ, chủ động lập kế hoạch quản lý thời gian chi tiết hàng ngày để đảm bảo hoàn thành các công việc theo đúng thời hạn (deadlines) đã đề ra.
* **Cải thiện tư duy giải quyết vấn đề kỹ thuật nâng cao:** Tự trau dồi thêm khả năng lập luận logic và tư duy hệ thống. Khi đối mặt với một lỗi kỹ thuật phức tạp (như đồng bộ dữ liệu hoặc phân quyền truy cập), tôi cần rèn luyện cách chia nhỏ bài toán, tìm hiểu kỹ nguyên nhân gốc rễ (Root Cause Analysis) trước khi thử nghiệm các giải pháp.
* **Nâng cao kỹ năng giao tiếp và xử lý tình huống thực tế:** Học hỏi cách diễn đạt và giải thích các vấn đề kỹ thuật phức tạp một cách ngắn gọn, dễ hiểu hơn cho cả các thành viên phi kỹ thuật. Rèn luyện sự bình tĩnh, tính chủ động lắng nghe phản hồi (feedback) từ mentor và đồng nghiệp để học hỏi kinh nghiệm hiệu quả nhất.
* **Rèn luyện kỹ năng quản lý công việc cá nhân:** Sử dụng hiệu quả hơn các công cụ hỗ trợ như Git, Jira, hoặc ghi chú cá nhân để theo dõi chặt chẽ tiến độ công việc, tránh tình trạng quá tải hoặc phân bổ thời gian chưa hợp lý giữa các đầu việc.