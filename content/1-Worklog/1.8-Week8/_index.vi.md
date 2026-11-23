---
title: "Worklog Tuần 8"
date: 2026-10-26
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### MỤC TIÊU TRONG WEEK 8:
- Hoàn thiện kỹ năng Networking nâng cao: VPC Endpoints (PrivateLink), VPC Peering và quản lý mạng tập trung với Transit Gateway Network Manager.
- Thực hành triển khai hệ thống Web Application thực tế (WordPress) với kiến trúc High Availability (ASG, ALB, RDS, CloudFront).
- Làm chủ tư duy "Infrastructure as Code" (IaC) thông qua AWS CloudFormation để tự động hóa việc khởi tạo hạ tầng.
- Tham gia hoạt động tình nguyện AWS HCM ngày 26/10 và rà soát ngữ nghĩa API/evaluation, S1a shadow của CPAWS.

### CÁC ĐẦU VIỆC CỦA WEEK 8:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Tham gia event tình nguyện: Thú nhồi bông làm STEM cùng AWS HCM**<br>**- Họp team: đánh giá Well-Architected và thống nhất giao thức dự báo**<br>+ Trao đổi phương án Lambda container cho batch inference, chú ý chi phí và tính tái lập<br>+ Rà soát target log return theo h = 1–7 phiên giao dịch, 7 phân vị, điều kiện hợp lệ của endpoint và pinball skill so với `baseline-q252`<br>+ Tổng hợp kết quả DLinear/K3 và tiêu chí phân biệt champion với challenger | 26/10/2026 | 26/10/2026 | [AWS Well-Architected](https://aws.amazon.com/architecture/well-architected/)<br>[Proper Scoring Rules](https://doi.org/10.1198/016214506000001437) |
| **3** | **- Tiếp tục Thực hành Lab 17:**<br>+ VPC Endpoints cho AWS Services<br>* Triển khai VPC Endpoint<br>* Kiểm tra VPC Endpoint<br>+ VPC Endpoint Services<br>* Triển khai VPC Endpoint Services<br>+ VPC Peering<br>* VPC Peering Request<br>* Routing Configuration<br>* Kiểm tra VPC Peering<br>+ Transit Gateway Network Manager<br>* Cài đặt Network Manager<br>* Cấu hình Site<br>* Network Insights<br>+ Dọn dẹp tài nguyên | 27/10/2026 | 27/10/2026 | [VPC Endpoint](https://000092.awsfcaj.com/vi/6-vpcendpointaws/)<br>[PrivateLink](https://000092.awsfcaj.com/vi/7-vpcendpointonpremise/)<br>[Peering](https://000092.awsfcaj.com/vi/8-vpcpeering/)<br>[Network Manager](https://000092.awsfcaj.com/vi/9-transitgatewaynetworkmanager/) |
| **4** | **- CPAWS (song song với Lab):** Rà soát đề xuất chạy shadow S1a (`s1a-l094`), hệ số co giãn độ biến động và phương án theo dõi độc lập với champion.<br>**- Thực hành Lab 18: Triển khai Wordpress trên AWS Cloud**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Chuẩn bị VPC và Subnet<br>* Tạo Security Group cho EC2<br>* Tạo Security Group cho Database Instance<br>* Khởi tạo EC2 Instance<br>* Khởi tạo Database Instance<br>+ Cài đặt wordpress trên EC2<br>+ Thực hiện tạo Autoscaling cho wordpress Instance<br>* Khởi tạo AMI từ Webserver Instance<br>* Khởi tạo Launch Template<br>* Khởi tạo Target Group<br>* Khởi tạo Load Balancer<br>* Khởi tạo Auto Scaling Group<br>+ Sao lưu và phục hồi database<br>* Tạo DB snapshot<br>* Phục hồi bằng DB snapshot<br>+ Khởi tạo Cloudfront cho Web Server<br>+ Dọn dẹp tài nguyên | 28/10/2026 | 28/10/2026 | [SDK Redis](https://000061.awsfcaj.com/vi/4-sdkelasticache/)<br>[Cleanup](https://000061.awsfcaj.com/vi/5.cleanupresource/)<br>[Lab 18 Intro](https://000101.awsfcaj.com/vi/1-introduce/)<br>[Install WP](https://000101.awsfcaj.com/vi/3-installwordpressonec2/)<br>[ASG Setup](https://000101.awsfcaj.com/vi/4-asgforec2/)<br>[CloudFront](https://000101.awsfcaj.com/vi/6-createcloudfront/) |
| **5** | **- Đọc, rà soát Proposal và tài liệu API/evaluation của CPAWS**<br>+ Đối chiếu mục tiêu Proposal với hợp đồng API, các phân vị, quy tắc `normalize_quantiles()` và `prob_up`<br>+ Góp ý về metric, calendar, data provenance và cách đánh giá walk-forward; phối hợp review thay vì nhận phần triển khai API<br>+ Tổng hợp kết quả S1a volatility scaling, giữ `baseline-q252` làm champion và S1a làm challenger chạy shadow | 29/10/2026 | 29/10/2026 | [API Gateway REST API](https://docs.aws.amazon.com/apigateway/latest/developerguide/apigateway-rest-api.html) |
| **6** | **- Tìm hiểu chủ đề AWS mới (song song với Lab):** Đọc bài giới thiệu Physical AI Toolchain của AWS, ghi chú chu trình dữ liệu thực → mô phỏng → huấn luyện → kiểm chứng → triển khai xuống thiết bị.<br>**- Thực hành Lab 19: AWS CloudFormation**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Tạo IAM User<br>* Tạo IAM Role<br>+ CloudFormation cơ bản<br>* Tạo Workspace<br>* Tạo CloudFormation Template<br>+ CloudFormation nâng cao<br>* Các tài nguyên tùy chỉnh<br>Tạo Lambda Function<br>Tạo Stack<br>Kết nối EC2 Instance<br>* Ánh xạ và Stacksets<br>* Drift Detection<br>+ Dọn dẹp tài nguyên | 30/10/2026 | 30/10/2026 | [Lab 17 Intro](http://000092.awsfcaj.com/vi/1-introduce/)<br>[VPC Deep Dive](https://000092.awsfcaj.com/vi/3-vpcs/)<br>[TGW & VPN](https://000092.awsfcaj.com/vi/4-transitgatewayandvpn/)<br>[Route53](https://000092.awsfcaj.com/vi/5-route53/)<br>[Lab 19 Intro](https://000037.awsfcaj.com/vi/1-introduce/)<br>[CF Basic](https://000037.awsfcaj.com/vi/3-cloudformationbasic/)<br>[CF Advanced](https://000037.awsfcaj.com/vi/4-cloudformationadvance/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 8:

1. Triển khai thành công các kết nối mạng bảo mật: VPC Endpoints (kết nối nội bộ đến dịch vụ AWS) và VPC Peering (kết nối giữa các VPC).
2. Xây dựng hoàn chỉnh hệ thống WordPress có khả năng tự động mở rộng (Auto Scaling), cân bằng tải (ALB) và phân phối nội dung toàn cầu (CloudFront).
3. Nắm vững quy trình Backup & Restore cơ sở dữ liệu RDS thông qua Snapshot trong bài toán thực tế.
4. Sử dụng thành thạo AWS CloudFormation để viết Template (Infrastructure as Code), quản lý Stacks và phát hiện sai lệch cấu hình (Drift Detection).
5. Tham gia review kiến trúc và giao thức CPAWS: target theo phiên, 7 phân vị, pinball skill và kiểm soát thông tin tương lai.
6. Rà soát Proposal, hợp đồng API và các ADR đánh giá; tổng hợp kết quả DLinear/K3/K3b/S1a, giữ `baseline-q252` champion và chuẩn bị S1a chạy shadow.
7. Góp sức vào hoạt động thiện nguyện làm thú nhồi bông STEM cho các em nhỏ cùng anh chị ở AWS HCM.
8. Bắt đầu tìm hiểu Physical AI Toolchain và mối liên hệ giữa mô phỏng, huấn luyện và triển khai robot.

