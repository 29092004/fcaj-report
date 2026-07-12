---
title: "Event 2"
date: 2026-06-06
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Bài thu hoạch "AWS Community Day - 06/06/2026"

### Mục Đích Của Sự Kiện

- Cung cấp các kiến thức chuyên sâu về công nghệ đóng gói container (Docker), tích hợp Machine Learning với AWS WAF để phát hiện tấn công mạng, và xây dựng game multiplayer trên nền tảng đám mây.
- Giới thiệu các giải pháp GraphRAG hiện đại sử dụng cơ sở dữ liệu đồ thị AWS Neptune để lưu trữ cơ sở tri thức (Knowledge Graph).
- Chia sẻ các kỹ năng mềm quan trọng về cách làm việc nhóm hiệu quả và lộ trình thực tế giúp phát triển sự nghiệp từ IT Helpdesk tiến lên vị trí Senior System Administrator.

### Danh Sách Diễn Giả & Đề Tài

1. **Bảo Huỳnh** - Đề tài: *Docker - A containerization technology*
2. **Lê Hoàng Gia Đại** - Đề tài: *Combining AWS WAF with Machine Learning for Cyber Attack Detection*
3. **Nguyễn Quốc Bảo** - Đề tài: *Multiplayer in the Cloud: Connecting Godot Clients with AWS*
4. **Trương Phước** - Đề tài: *Cách làm việc nhóm hiệu quả*
5. **Việt Phát** - Đề tài: *AWS Neptune for Building a Graph Knowledge Base for GraphRAG*
6. **Vinh Trấn** - Đề tài: *Từ IT Helpdesk lên Senior Sysadmin: Hành trình tự học và Lộ trình dịch chuyển*

---

### Nội Dung Nổi Bật Của Các Bài Tham Luận

#### 1. Docker - A containerization technology
**Diễn giả:** Bảo Huỳnh

- **Khái niệm Containerization và Virtualization:** Phân biệt sự khác nhau giữa máy ảo truyền thống (VMs) sử dụng Hypervisor và Container sử dụng chung nhân hệ điều hành.
- **Các thành phần cốt lõi của Docker:** Tìm hiểu chi tiết về Docker Engine, Dockerfile để định nghĩa môi trường, Docker Image làm khuôn mẫu và Docker Container khi chạy thực tế.
- **Quản lý nhiều Container bằng Docker Compose:** Hướng dẫn cách viết file cấu hình `docker-compose.yml` để khởi chạy đồng thời nhiều dịch vụ (frontend, backend, database) một cách dễ dàng và đồng bộ.
- **Giá trị thực tiễn:** Giải quyết triệt để lỗi kinh điển "chạy được trên máy tôi nhưng lỗi trên production", tối ưu hóa tài nguyên phần cứng và tăng tốc độ triển khai ứng dụng (CI/CD).

#### 2. Combining AWS WAF with Machine Learning for Cyber Attack Detection
**Diễn giả:** Lê Hoàng Gia Đại

- **Hạn chế của WAF dựa trên luật cứng (Rule-based WAF):** Phân tích rủi ro khi đối mặt với các cuộc tấn công Zero-day phức tạp hoặc các mẫu tấn công biến thể liên tục.
- **Tích hợp Machine Learning vào AWS WAF:** Giải pháp phân tích lưu lượng truy cập (traffic) thời gian thực bằng mô hình ML để phát hiện hành vi bất thường (Anomaly Detection).
- **Kiến trúc hệ thống tự động bảo vệ:** Sử dụng AWS WAF thu thập logs -> chuyển tiếp qua Amazon Kinesis Data Firehose -> lưu trữ tại Amazon S3 -> chạy AWS Lambda phân tích logs với mô hình ML -> tự động cập nhật danh sách IP bị chặn (IP Set Blocklists) trên AWS WAF.
- **Lợi ích:** Nâng cao khả năng tự vệ chủ động của hệ thống trước các mối đe dọa an ninh mạng nghiêm trọng mà không làm giảm tốc độ xử lý request.

#### 3. Multiplayer in the Cloud: Connecting Godot Clients with AWS
**Diễn giả:** Nguyễn Quốc Bảo

- **Thách thức của trò chơi nhiều người chơi (Multiplayer Game):** Quản lý độ trễ (latency), đồng bộ hóa trạng thái trò chơi (state synchronization) giữa các người chơi khác nhau.
- **Kết nối Game Client phát triển bằng Godot Engine:** Phương pháp sử dụng Godot để giao tiếp với server thông qua các giao thức mạng hiệu năng cao như UDP, TCP hoặc WebSockets.
- **Kiến trúc Cloud Server cho Game:** Triển khai các máy chủ game chuyên dụng (Dedicated Game Servers) sử dụng dịch vụ AWS (như Amazon GameLift, Amazon ECS hoặc AWS App Runner).
- **Live Demo:** Trực quan hóa quá trình người chơi điều khiển nhân vật từ máy client, tín hiệu truyền lên AWS server và đồng bộ hóa tức thời về các client khác.

#### 4. Cách làm việc nhóm hiệu quả
**Diễn giả:** Trương Phước

- **Yếu tố cốt lõi của một nhóm thành công:** Sự thấu hiểu mục tiêu chung, giao tiếp cởi mở, sự tin tưởng lẫn nhau và sự phân công trách nhiệm rõ ràng.
- **Áp dụng quy trình Agile/Scrum:** Hướng dẫn cách tổ chức các buổi Daily Standup, Sprint Planning, Retrospective để tối ưu hóa tiến độ công việc và giải quyết vướng mắc nhanh chóng.
- **Các công cụ hỗ trợ phối hợp:** Sử dụng hiệu quả Jira/Trello để quản lý task, Slack/Discord để trao đổi thông tin, và Git/GitHub để quản lý mã nguồn chung mà không bị xung đột.
- **Quản trị xung đột:** Cách nhìn nhận mâu thuẫn như một cơ hội để cải tiến, kỹ năng lắng nghe tích cực và đưa ra phản hồi mang tính xây dựng.

#### 5. AWS Neptune for Building a Graph Knowledge Base for GraphRAG
**Diễn giả:** Việt Phát

- **RAG truyền thống và những giới hạn:** RAG thông thường (dựa trên vector database) gặp khó khăn khi truy vấn thông tin có mối liên kết phức tạp hoặc yêu cầu suy luận đa bước (multi-hop reasoning).
- **Mô hình GraphRAG:** Kết hợp tìm kiếm ngữ nghĩa với Cơ sở dữ liệu đồ thị (Graph Database) để biểu diễn tri thức dưới dạng các thực thể (entities) và mối quan hệ (relationships).
- **Xây dựng Graph Knowledge Base với AWS Neptune:** Khai thác AWS Neptune làm cơ sở dữ liệu đồ thị được quản lý hoàn toàn để lưu trữ Graph Tri thức lớn. Sử dụng ngôn ngữ truy vấn Gremlin hoặc openCypher để truy xuất ngữ cảnh phong phú.
- **Tác động:** Giúp mô hình ngôn ngữ lớn (LLM) đưa ra câu trả lời chính xác hơn, có chiều sâu hơn và giải thích được mối liên hệ logic giữa các dữ liệu.

#### 6. Từ IT Helpdesk lên Senior Sysadmin: Hành trình tự học và Lộ trình dịch chuyển
**Diễn giả:** Vinh Trấn

- **Sự khác biệt về vai trò và tư duy:** Từ hỗ trợ sự cố người dùng (IT Helpdesk - phản ứng thụ động) sang quản trị hạ tầng hệ thống lớn (Sysadmin - chủ động quy hoạch và tối ưu).
- **Lộ trình kỹ năng cần trang bị:**
  - *Mạng & Hệ điều hành:* Nắm vững TCP/IP, DNS, Linux (RedHat/Ubuntu) và Windows Server.
  - *Tự động hóa:* Kỹ năng viết script tự động bằng Bash, PowerShell hoặc Python.
  - *Cloud & IaC:* Thành thạo các dịch vụ đám mây (AWS, Azure) và Infrastructure as Code (Terraform).
- **Phương pháp tự học thực chiến:** Thiết lập Lab tại nhà (Home Lab) sử dụng Proxmox, VMware hoặc AWS Free Tier để thực hành, kết hợp ôn luyện các chứng chỉ uy tín (CCNA, AWS SysOps, MCSA, Linux+).
- **Lời khuyên nghề nghiệp:** Luôn duy trì thái độ tò mò, sẵn sàng nhận các thử thách khó trong dự án thực tế và xây dựng tư duy giải quyết vấn đề có hệ thống.

---

### Những Gì Học Được

- **Về Kỹ thuật & Công nghệ:**
  - Nắm vững quy trình đóng gói container và triển khai ứng dụng đa thành phần với Docker Compose.
  - Hiểu cách thức hoạt động của GraphRAG và tầm quan trọng của cơ sở dữ liệu đồ thị AWS Neptune trong việc nâng cao chất lượng câu trả lời của AI.
  - Nắm rõ kiến trúc kết hợp ML với AWS WAF để bảo mật chủ động và cách triển khai game server trên đám mây.
- **Về Phát triển cá nhân:**
  - Học hỏi được các phương pháp tổ chức làm việc nhóm chuyên nghiệp, tăng hiệu quả phối hợp và giảm thiểu xung đột.
  - Định hình được một lộ trình tự học rõ ràng, thực tế để nâng cao trình độ chuyên môn hệ thống và dịch chuyển nghề nghiệp thành công.

### Ứng Dụng Vào Công Việc

- **Áp dụng Docker:** Tiến hành viết Dockerfile và docker-compose để đóng gói ứng dụng báo cáo thực tập này cùng các dịch vụ liên quan, giúp việc chạy thử và deploy thuận tiện hơn.
- **Xây dựng Lộ trình Tự học:** Thiết lập một roadmap tự học cá nhân hàng tuần tập trung vào kỹ năng Linux Administration và viết script tự động hóa với Python.
- **Phối hợp Teamwork:** Áp dụng các quy tắc giao tiếp rõ ràng và quy trình review code nghiêm túc hơn khi làm việc nhóm trong các bài tập lớn hoặc dự án thực tập.

### Trải nghiệm trong event

- Sự kiện vô cùng bổ ích với lượng kiến thức đa dạng, từ hạ tầng hệ thống cơ bản, an ninh mạng, phát triển game cho đến công nghệ AI thế hệ mới (GraphRAG).
- Các diễn giả trình bày rất tâm huyết, các bài demo trực quan sinh động giúp người nghe dễ dàng hình dung lý thuyết phức tạp.
- Buổi giao lưu định hướng sự nghiệp mang tính thực tế cao, giúp gỡ rối nhiều thắc mắc về con đường phát triển của các kỹ sư IT trẻ.

#### Một số hình ảnh khi tham gia sự kiện
![FCAJ Tech Sharing Event](/images/4-EventParticipated/event2-photo.jpg)

> Sự kiện Demo Day 2 đã trang bị cho tôi những góc nhìn công nghệ sắc bén và nguồn động lực mạnh mẽ để tiếp tục hoàn thiện cả kỹ năng chuyên môn lẫn kỹ năng mềm trong quá trình thực tập.
