---
title: "Worklog Tuần 9"
date: 2026-11-09
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### MỤC TIÊU TRONG WEEK 9:
- Thực hành kiến trúc Serverless toàn diện: Từ xử lý sự kiện (S3 triggers), lưu trữ (DynamoDB) đến xây dựng API (API Gateway).
- Xây dựng quy trình CI/CD tự động cho ứng dụng Serverless bằng AWS CodePipeline.
- Thực hành giám sát (Monitoring) và truy vết (Tracing) ứng dụng Serverless chuyên sâu với CloudWatch và X-Ray.
- Chốt hướng đánh giá mô hình trước official test2020; rà soát lượt Rolling Accuracy đầu tiên ngày 12/11, thống nhất quy tắc công bố metric và giữ champion để làm cơ sở cho tích hợp, vận hành.
- Hoàn thiện bài viết cá nhân về Isaac Lab trên SageMaker AI.

### CÁC ĐẦU VIỆC CỦA WEEK 9:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Họp team project: Xây dựng mốc so sánh và đánh giá mô hình**<br>+ Tổng hợp các thử nghiệm DLinear, CEEMDAN–DLinear/K3, K3b, S1a và giới hạn của validation 2019<br>+ Đối chiếu tiêu chí `pinball_skill`, bootstrap CI, benchmark `baseline-q252` và tiêu chí xác nhận champion hiện tại<br>+ Review runbook/runner test2020: walk-forward, mask hợp lệ, kiểm định DM-HAC, hiệu chỉnh Holm và nguyên tắc chạy official một lần<br>**- Thực hành lại Lab 14 (lượt Lab 22): Serverless - Tương tác giữa Lambda với S3 và DynamoDB**<br>+ Giới thiệu<br>+ Xử lý và Tối ưu Kích thước Ảnh trên AWS<br>* Tạo Lambda Function Xử Lý Ảnh<br>* Tạo S3 Bucket<br>* Tạo IAM Policy cho Lambda Function<br>* Kiểm tra hoạt động của Lambda Function<br>+ Ghi dữ liệu vào Amazon DynamoDB<br>* Tạo và Quản lý Bảng trong Amazon DynamoDB<br>* Tạo Lambda Function để Ghi dữ liệu<br>+ Dọn dẹp tài nguyên | 09/11/2026 | 09/11/2026 | [DLinear Paper](https://arxiv.org/abs/2205.13504)<br>[Lab 22 Intro](https://000078.awsfcaj.com/vi/1-introduce/)<br>[Resize Function](https://000078.awsfcaj.com/vi/2-resize-image-function/)<br>[DynamoDB Write](https://000078.awsfcaj.com/vi/3-write-data-to-dynaomodb/)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **3** | **- Bài viết cá nhân về Isaac Lab (song song với Lab):** Hoàn thiện bài giới thiệu huấn luyện robot hình người với Isaac Lab trên Amazon SageMaker AI; nội dung tổng hợp tài liệu AWS, không thực hành GPU.<br>**- Thực hành Lab 23: Serverless - Hướng dẫn viết Front-end gọi API Gateway**<br>+ Giới thiệu API Gateway / DynamoDB<br>+ Triển khai front-end<br>+ Triển khai Lambda function<br>* Tạo bảng trong DynamoDB<br>* Triển khai Lambda function<br>Lambda function ghi dữ liệu<br>Lambda function đọc dữ liệu<br>Lambda function xoá dữ liệu<br>+ Thiết lập API Gateway<br>* Tạo các method<br>* Cài đặt và kích hoạt CORS<br>+ Kiểm tra API với Postman<br>+ Kiểm tra API với front-end<br>+ Dọn dẹp tài nguyên | 10/11/2026 | 10/11/2026 | [Lab 23 Intro](https://000079.awsfcaj.com/vi/1-introduction/)<br>[Deploy Frontend](https://000079.awsfcaj.com/vi/2-front-end-deployment/)<br>[API Gateway](https://000079.awsfcaj.com/vi/4-config-api-gw/)<br>[Postman Test](https://000079.awsfcaj.com/vi/5-test-api-by-postman/)<br>[Isaac Lab documentation](https://isaac-sim.github.io/IsaacLab/)<br>[SageMaker AI documentation](https://docs.aws.amazon.com/sagemaker/) |
| **4** | **- CPAWS (song song với Lab):** Đối chiếu kế hoạch báo cáo Chương 2, phương pháp thống kê và điều kiện khóa trước khi chạy official test2020.<br>**- Thực hành Lab 24: Serverless - CI/CD với CodePipeline**<br>+ Chuẩn bị<br>+ Xây dựng pipeline SAM<br>* Tạo kho Git<br>* Tạo SAM pipeline<br>+ Xây dựng pipeline cho front-end<br>* Tạo kho Git<br>* Tạo pipeline<br>+ Kiểm tra hoạt động web<br>+ Dọn dẹp | 11/11/2026 | 11/11/2026 | [Lab 24 Intro](https://000084.awsfcaj.com/vi/1-preparation/)<br>[SAM Pipeline](https://000084.awsfcaj.com/vi/2-build-sam-pipeline/)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **5** | **- Họp team project: Chốt mô hình chạy production và viết code Lambda predict**<br>+ Đối chiếu trạng thái job 4/4 asset `COMPLETED` với API còn `collecting` 9/20; làm rõ `COMPLETED` không đồng nghĩa đủ mẫu để công bố metric<br>+ Review cách tính các base date hợp lệ, provenance và đường đi dữ liệu phục vụ báo cáo<br>+ Thống nhất `baseline-q252` vẫn là champion; S1a chỉ chạy shadow, không tự động được promote | 12/11/2026 | 12/11/2026 | [DynamoDB Query](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Query.html)<br>[CPAWS repository](https://github.com/CPAWS-AWS-FCAJ/CPAWS-commodity-forecasting) |
| **6** | **- Tìm hiểu chủ đề AWS mới (song song với Lab):** Đọc về EKS, AWS Batch, SageMaker và Terraform trong Physical AI Toolchain; ghi chú vai trò các thành phần NVIDIA để chuẩn bị bài viết Physical AI Toolchain.<br>**- Thực hành Lab 25: Serverless - Giám sát ứng dụng Serverless với CloudWatch và X-Ray**<br>+ Chuẩn bị<br>+ Giám sát với CloudWatch<br>* Gỡ lỗi với nhật ký CloudWatch<br>* Tạo số liệu tùy chỉnh<br>* Tạo cảnh báo với CloudWatch Alarm<br>+ Theo dõi với X-Ray<br>+ Dọn dẹp | 13/11/2026 | 13/11/2026 | [Lab 25 Intro](https://000085.awsfcaj.com/vi/1-preparation/)<br>[CloudWatch](https://000085.awsfcaj.com/vi/2-cloudwatch-monitor/)<br>[X-Ray](https://000085.awsfcaj.com/vi/3-x-ray-trace/)<br>[AWS Physical AI Toolchain](https://aws.amazon.com/blogs/physical-ai/introducing-aws-physical-ai-toolchain/)<br>[Physical AI for Robotics on AWS](https://aws.amazon.com/solutions/physical-ai-for-robotics-on-aws/) |
| **7** | **- Tham gia Cloud Mastery 1: Amazon Bedrock AgentCore**<br>+ Tìm hiểu các thành phần AgentCore và cách phối hợp chúng trong ứng dụng AI Agent trên AWS. | 14/11/2026 | 14/11/2026 | [Amazon Bedrock AgentCore](https://aws.amazon.com/bedrock/agentcore/)<br>[AgentCore Developer Guide](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/what-is-bedrock-agentcore.html) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 9:

1. Củng cố luồng xử lý Serverless Backend qua lượt thực hành lại: Tự động hóa xử lý ảnh với S3 Trigger và quản lý dữ liệu NoSQL với DynamoDB.
2. Triển khai thành công Full-stack Serverless App: Kết nối Frontend với Backend thông qua API Gateway và Lambda, xử lý tốt vấn đề CORS.
3. Thiết lập quy trình DevOps tự động (CI/CD) cho ứng dụng Serverless, giúp việc deploy Code và Frontend trở nên nhanh chóng và ít lỗi.
4. Chốt hướng đánh giá trước official test2020 (bootstrap, DM-HAC, Holm, validity mask) trên cơ sở validation 2019; giữ `baseline-q252` làm champion.
5. Rà soát lượt Rolling Accuracy ngày 12/11, làm rõ sự khác biệt giữa job `COMPLETED` (4/4 asset) và API `collecting` (9/20); thống nhất nguyên tắc công bố metric và vai trò shadow của S1a, làm cơ sở cho tài liệu bàn giao kỹ thuật ở Week 10.
6. Hoàn thiện bài viết về Isaac Lab trên SageMaker AI ngày 10/11; tiếp tục tìm hiểu các mảnh ghép Physical AI Toolchain.
7. Tham gia Cloud Mastery 1 ngày 14/11, tìm hiểu Amazon Bedrock AgentCore.
