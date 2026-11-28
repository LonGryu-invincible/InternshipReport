---
title: "Worklog Tuần 6"
date: 2026-10-19
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### MỤC TIÊU TRONG WEEK 6:
- Tham gia review Well-Architected và giao thức dự báo CPAWS; tổng hợp lựa chọn champion/challenger có căn cứ thực nghiệm.
- Nắm vững dịch vụ In-memory Caching với Amazon ElastiCache (Redis): Tạo cluster, kết nối qua CLI/SDK và thao tác dữ liệu.
- Đọc và góp ý Proposal/API contract, đồng bộ mục tiêu sản phẩm với tiêu chí Modeling & Evaluation.
- Thực hành Networking nâng cao: Transit Gateway, Site-to-Site VPN (với Cisco CSR), ECMP Routing và Hybrid DNS với Route 53.
- Rà soát kiến trúc CPAWS và bằng chứng lựa chọn baseline/challenger trong các buổi trao đổi ngày 19–22/10.
### CÁC ĐẦU VIỆC CỦA WEEK 6:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Họp team project: Xác định, nghiên cứu solution architecture cho web app**<br>+ Đối chiếu API Contract đã rà soát với luồng EventBridge Scheduler → Lambda ingest → S3 → Lambda predict → DynamoDB → API Gateway → web để xác định dữ liệu đầu vào và thời điểm dự báo<br>+ Rà soát EDA, lịch giao dịch NYSE/CME, các mốc giá bất thường (đặc biệt WTI 20/04/2020) và nguyên tắc không dùng dữ liệu tương lai<br>+ Tập trung vào giao diện giữa dữ liệu đã làm sạch, target log return theo phiên và bộ metric đánh giá | 19/10/2026 | 19/10/2026 | [CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **3** | **- Thực hành Lab 16: Amazon ElastiCache - Redis**<br>+ Giới thiệu<br>+ Chuẩn bị<br>* Tạo AWS Access Key<br>* Cài đặt AWS CLI<br>* Cấu hình AWS CLI<br>+ Tạo ElastiCache cluster<br>* Tạo subnet group (Console/AWS CLI)<br>* Tạo cluster (cluster mode disabled) (Console/AWS CLI)<br>* Tạo cluster(cluster mode enabled)<br>* Cấp quyền truy cập vào cluster<br>* Kết nối với node của cluster<br>Cluster Mode Disabled<br>Cluster Mode Enabled<br>Endpoints use AWS CLI<br>* Xóa cluster (Console/AWS CLI) | 20/10/2026 | 20/10/2026 | [Lab 16 Intro](https://000061.awsfcaj.com/vi/1-introduce/)<br>[Prereq](https://000061.awsfcaj.com/vi/2-prerequiste/)<br>[Redis Lab](https://000061.awsfcaj.com/vi/3-amazonelasticacheforredis/) |
| **4** | **- CPAWS (song song với Lab):** Rà soát schema đánh giá với `evaluation_kind`, `target_cutoff_date`, pinball skill và phân biệt validation/test/rolling; đối chiếu các yêu cầu trong ADR-0008.<br>**- Tiếp tục Thực hành Lab 16: Amazon ElastiCache - Redis**<br>+ Sử dụng AWS SDK để ghi và đọc dữ liệu trên ElastiCache<br>* Tạo Elasticache cluster<br>Tạo một cluster (mode disabled cluster)<br>Tạo một cluster (mode enabled cluster)<br>Kiểm tra nhóm người dùng<br>* Kết nối với Elasticache<br>Kết nối tới một cluster (mode disabled cluster)<br>Kết nối tới một cluster (mode enabled cluster)<br>* Set and Get strings<br>* Set and Get a hash with multiple items<br>* Publish (write) and subscribe (read)<br>* Write and read from a stream<br>+ Dọn dẹp tài nguyên | 21/10/2026 | 21/10/2026 | [Lab 14 Intro](https://000078.awsfcaj.com/vi/1-introduce/)<br>[Resize Function](https://000078.awsfcaj.com/vi/2-resize-image-function/)<br>[DynamoDB Write](https://000078.awsfcaj.com/vi/3-write-data-to-dynaomodb/)<br>[SDK Redis](https://000061.awsfcaj.com/vi/4-sdkelasticache/)<br>[Cleanup](https://000061.awsfcaj.com/vi/5.cleanupresource/) |
| **5** | **- Họp team project: Hoàn thiện solution architecture, budget estimation cho web app**<br>+ Đọc phần ước tính chi phí/kiến trúc để hiểu vì sao nhóm chọn Lambda theo lịch thay cho endpoint hoạt động liên tục<br>+ Thực hiện và phân tích validation 2019 cho DLinear MVP so với baseline phân vị 252 phiên; ghi nhận hạn chế của mô hình học sâu trên dữ liệu hiện có<br>+ Đối chiếu thử nghiệm CEEMDAN–DLinear (K3), pinball skill, các trường hợp không vượt baseline và kế hoạch kiểm tra tính ổn định | 22/10/2026 | 22/10/2026 | [AWS Pricing Calculator](https://calculator.aws/#/)<br>[PyEMD (CEEMDAN)](https://pyemd.readthedocs.io/) |
| **6** | **- Tìm hiểu chủ đề AWS mới (song song với Lab):** Đọc tổng quan NVIDIA Isaac Lab và hai phương án SageMaker HyperPod/Training Jobs; tìm hiểu khái niệm GPU job, container và checkpoint, chưa chạy huấn luyện thực tế.<br>**- Thực hành Lab 17: AWS Networking and Content Delivery**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Triển khai VPC<br>* Cisco CSR Agreement<br>+ VPC Components Deep Dive<br>+ Transit Gateway và Site-to-Site VPNs<br>* Transit Gateway và Site-to-Site VPNs<br>* Truy cập Cisco CSR Router với Cloud9<br>* Cài đặt Site-to-site VPN<br>* Thêm ECMP Path<br>* Transit Gateway Routing<br>+ Route53 DNS Endpoints và Internal Hosted Zones<br>* Triển khai DNS<br>* Kiểm tra DNS | 23/10/2026 | 23/10/2026 | [Lab 15 Intro](https://000011.awsfcaj.com/vi/1-introduce/)<br>[Install CLI](https://000011.awsfcaj.com/vi/3-installcli/)<br>[CLI with EC2](https://000011.awsfcaj.com/vi/9-ec2/)<br>[Lab 17 Intro](http://000092.awsfcaj.com/vi/1-introduce/)<br>[VPC Deep Dive](https://000092.awsfcaj.com/vi/3-vpcs/)<br>[TGW & VPN](https://000092.awsfcaj.com/vi/4-transitgatewayandvpn/)<br>[Route53](https://000092.awsfcaj.com/vi/5-route53/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 6:

1. Hoàn thành Lab 16: Nắm được kiến thức về Amazon ElastiCache (Redis), thực hành tạo Cluster, kết nối và thao tác dữ liệu nâng cao (Pub/Sub, Stream) thông qua AWS SDK.
2. Hoàn thành Lab 17: Triển khai mô hình mạng phức tạp sử dụng Transit Gateway kết nối VPN với Router Cisco CSR, cấu hình định tuyến ECMP và phân giải tên miền Hybrid với Route 53.
3. Đọc và góp ý kiến trúc serverless/chi phí CPAWS để xác định vị trí của pipeline Modeling & Evaluation; kiến trúc triển khai do các thành viên Platform phụ trách.
4. Rà soát EDA, quy tắc chất lượng dữ liệu, lịch giao dịch và giá WTI bất thường; tham gia đánh giá DLinear/K3 so với baseline phân vị 252 phiên trên validation 2019.
5. Đọc thêm về Isaac Lab, SageMaker HyperPod và Training Jobs để hiểu các lựa chọn hạ tầng huấn luyện robot.

