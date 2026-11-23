---
title: "Worklog Tuần 9"
date: 2026-11-02
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### MỤC TIÊU TRONG WEEK 9:
- Tiếp cận và làm chủ AWS Cloud Development Kit (CDK) để định nghĩa hạ tầng đám mây bằng ngôn ngữ lập trình.
- Thực hành triển khai các kiến trúc phức tạp (ECS, ALB, API Gateway, Serverless) sử dụng CDK và Nested Stacks.
- Củng cố tư duy Infrastructure as Code (IaC) thông qua việc triển khai kiến trúc 3 tầng (Three-Tier Architecture) hoàn chỉnh.
- Rà soát điều kiện eligibility, provenance của Rolling Accuracy và dữ liệu chất lượng trong các ngày 02–05/11.

### CÁC ĐẦU VIỆC CỦA WEEK 9:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Họp team project: đối chiếu hiển thị dự báo với phương pháp đánh giá**<br>+ Kiểm tra ý nghĩa q10/q50/q90, khoảng 80%, `prob_up`, USD/VND để web không diễn giải nhầm thành mức bảo đảm<br>+ Tập trung xây dựng RFC Rolling Accuracy: cửa sổ 56 ngày, `base_date`/`target_date`, eligibility và dữ liệu forecast đã phát hành<br>+ Thảo luận schema `rolling_8w` và tính nhất quán giữa đánh giá nội bộ, DynamoDB và API `/accuracy/{asset}` | 02/11/2026 | 02/11/2026 | [yfinance](https://github.com/ranaroussi/yfinance)<br>[EIA Open Data API](https://www.eia.gov/opendata/) |
| **3** | **- CPAWS (song song với Lab):** Review các cập nhật Rolling Accuracy, bằng chứng cutover, cấu hình champion và yêu cầu truy xuất dữ liệu đúng thời điểm.<br>**- Thực hành Lab 19: CDK cơ bản**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Tạo IAM Role<br>+ CDK cơ bản<br>* Tạo workspace<br>* Cấu hình Cloud9<br>+ Tạo CDK Template<br>+ Cập nhật CDK Template<br>+ Dọn dẹp tài nguyên | 03/11/2026 | 03/11/2026 | [VPC Endpoint](https://000092.awsfcaj.com/vi/6-vpcendpointaws/)<br>[PrivateLink](https://000092.awsfcaj.com/vi/7-vpcendpointonpremise/)<br>[Peering](https://000092.awsfcaj.com/vi/8-vpcpeering/)<br>[Network Manager](https://000092.awsfcaj.com/vi/9-transitgatewaynetworkmanager/)<br>[Lab 19 Intro](https://000038.awsfcaj.com/vi/1-introduce/)<br>[CDK Basic](https://000038.awsfcaj.com/vi/3-cdkbasic/)<br>[Create Template](https://000038.awsfcaj.com/vi/4-createcdktemplate/) |
| **4** | **- Thực hành Lab 20: CDK Cơ bản - 2**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Tạo IAM Role<br>* Chạy một máy chủ EC2<br>* Cấu hình môi trường VSCode<br>+ ECS, ALB và API Gateway<br>+ Lambda và S3<br>+ Nested stack<br>* Tạo các stack lồng với CDK<br>+ Dọn dẹp tài nguyên | 04/11/2026 | 04/11/2026 | [Lab 20 Intro](https://000076.awsfcaj.com/vi/1-introduction/)<br>[ECS & ALB](https://000076.awsfcaj.com/vi/3-ecs-alb-and-api-gateway/)<br>[Nested Stack](https://000076.awsfcaj.com/vi/5-nested-stack/) |
| **5** | **- Họp team project: rà soát nguồn dữ liệu và điều kiện đánh giá rolling**<br>+ Đối chiếu snapshot S3 (`raw/`, `clean/prices/`), lịch NYSE/CME, các phiên thiếu và quality flags với yêu cầu không rò rỉ thông tin tương lai<br>+ Kiểm tra logic provenance, idempotency, run completion và các trạng thái thiếu forecast hoặc upstream failure cho Rolling Accuracy<br>+ Review các cập nhật schema/contract và chuẩn bị kế hoạch test2020; phần Lambda ingest và hạ tầng do các thành viên phụ trách tương ứng triển khai | 05/11/2026 | 05/11/2026 | [pandas_market_calendars](https://github.com/rsheftel/pandas_market_calendars)<br>[Lambda Container Image](https://docs.aws.amazon.com/lambda/latest/dg/images-create.html) |
| **6** | **- Tìm hiểu chủ đề AWS mới (song song với Lab):** Đọc ví dụ Isaac Lab trên SageMaker, so sánh HyperPod và Training Jobs theo cách khởi chạy, theo dõi checkpoint và chi phí; tổng hợp ghi chú để chuẩn bị Blog 1.<br>**- Thực hành Lab 21: Giới Thiệu về Infrastructure as Code**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>+ Tạo Lambda function<br>+ Tạo VPC và EC2<br>+ Triển khai Three-Tier Architecture<br>* Triển khai CloudFormation Stack<br>* Kiểm tra truy cập Web Tier<br>* Kiểm tra truy cập Application Tier<br>* Kiểm tra truy cập Database Tier<br>+ Dọn dẹp tài nguyên | 06/11/2026 | 06/11/2026 | [Lab 19 Intro](https://000037.awsfcaj.com/vi/1-introduce/)<br>[CF Basic](https://000037.awsfcaj.com/vi/3-cloudformationbasic/)<br>[CF Advanced](https://000037.awsfcaj.com/vi/4-cloudformationadvance/)<br>[Lab 21 Intro](https://000102.awsfcaj.com/vi/1-introduction/)<br>[Create Lambda](https://000102.awsfcaj.com/vi/3-createlambda/)<br>[Three Tier](https://000102.awsfcaj.com/vi/5-threetierweb/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 9:

1. Thiết lập thành công môi trường làm việc CDK (Cloud9, VSCode) và triển khai các Template hạ tầng cơ bản.
2. Ứng dụng CDK để xây dựng các tài nguyên nâng cao: ECS Cluster, Application Load Balancer, API Gateway và cấu trúc Nested Stack.
3. Triển khai thành công kiến trúc Three-Tier chuẩn mực (Web, App, Database layers) hoàn toàn bằng mã nguồn (IaC).
4. Xây dựng/review đặc tả Rolling Accuracy (`rolling_8w`), khóa logic evaluation, tiêu chí eligibility/provenance; kiểm tra snapshot S3 và trạng thái pipeline ingest từ góc nhìn đánh giá, không nhận phần triển khai ingest.
5. Tổng hợp kiến thức nhập môn về Isaac Lab/SageMaker làm tài liệu chuẩn bị cho bài blog đầu tiên.

