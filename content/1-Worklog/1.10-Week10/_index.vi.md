---
title: "Worklog Tuần 10"
date: 2026-11-09
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### MỤC TIÊU TRONG WEEK 10:
- Làm chủ kiến trúc Serverless toàn diện: Từ xử lý sự kiện (S3 triggers), lưu trữ (DynamoDB) đến xây dựng API (API Gateway).
- Xây dựng quy trình CI/CD tự động cho ứng dụng Serverless bằng AWS CodePipeline.
- Thực hành giám sát (Monitoring) và truy vết (Tracing) ứng dụng Serverless chuyên sâu với CloudWatch và X-Ray.
- Rà soát kế hoạch test2020, lượt Rolling Accuracy đầu tiên ngày 12/11 và hoàn thành Blog 1.

### CÁC ĐẦU VIỆC CỦA WEEK 10:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Họp team project: rà soát baseline, challenger và kế hoạch test2020**<br>+ Tổng hợp các thử nghiệm DLinear, CEEMDAN–DLinear/K3, K3b, S1a và giới hạn của validation 2019<br>+ Đối chiếu tiêu chí `pinball_skill`, bootstrap CI, benchmark `baseline-q252` và quyết định giữ champion hiện tại<br>+ Review runbook/runner test2020: walk-forward, mask hợp lệ, kiểm định DM-HAC, hiệu chỉnh Holm và nguyên tắc chạy official một lần<br>**- Thực hành Lab 22: Serverless - Tương tác giữa Lambda với S3 và DynamoDB**<br>+ Giới thiệu<br>+ Xử lý và Tối ưu Kích thước Ảnh trên AWS<br>* Tạo Lambda Function Xử Lý Ảnh<br>* Tạo S3 Bucket<br>* Tạo IAM Policy cho Lambda Function<br>* Kiểm tra hoạt động của Lambda Function<br>+ Ghi dữ liệu vào Amazon DynamoDB<br>* Tạo và Quản lý Bảng trong AWS DynamoDB<br>* Tạo Lambda Function để Ghi dữ liệu<br>+ Dọn dẹp tài nguyên | 09/11/2026 | 09/11/2026 | [DLinear Paper](https://arxiv.org/abs/2205.13504)<br>[Lab 22 Intro](https://000078.awsfcaj.com/vi/1-introduce/)<br>[Resize Function](https://000078.awsfcaj.com/vi/2-resize-image-function/)<br>[DynamoDB Write](https://000078.awsfcaj.com/vi/3-write-data-to-dynaomodb/) |
| **3** | **- Blog 1 (song song với Lab):** Hoàn thiện bài giới thiệu huấn luyện robot hình người với Isaac Lab trên Amazon SageMaker AI; nội dung tổng hợp tài liệu AWS, không thực hành GPU.<br>**- Thực hành Lab 23: Serverless - Hướng dẫn viết Front-end gọi API Gateway**<br>+ Giới thiệu API Gateway / DynamoDB<br>+ Triển khai front-end<br>+ Triển khai Lambda function<br>* Tạo bảng trong DynamoDB<br>* Triển khai Lambda function<br>Lambda function ghi dữ liệu<br>Lambda function đọc dữ liệu<br>Lambda function xoá dữ liệu<br>+ Thiết lập API Gateway<br>* Tạo các method<br>* Cài đặt và kích hoạt CORS<br>+ Kiểm tra API với Postman<br>+ Kiểm tra API với front-end<br>+ Dọn dẹp tài nguyên | 10/11/2026 | 10/11/2026 | [Lab 19 Intro](https://000038.awsfcaj.com/vi/1-introduce/)<br>[CDK Basic](https://000038.awsfcaj.com/vi/3-cdkbasic/)<br>[Create Template](https://000038.awsfcaj.com/vi/4-createcdktemplate/)<br>[Lab 23 Intro](https://000079.awsfcaj.com/vi/1-introduction/)<br>[Deploy Frontend](https://000079.awsfcaj.com/vi/2-front-end-deployment/)<br>[API Gateway](https://000079.awsfcaj.com/vi/4-config-api-gw/)<br>[Postman Test](https://000079.awsfcaj.com/vi/5-test-api-by-postman/) |
| **4** | **- CPAWS (song song với Lab):** Đối chiếu kế hoạch báo cáo Chương 2, phương pháp thống kê và điều kiện khóa trước khi chạy official test2020.<br>**- Thực hành Lab 24: Serverless - CI/CD với CodePipeline**<br>+ Chuẩn bị<br>+ Xây dựng pipeline SAM<br>* Tạo kho Git<br>* Tạo SAM pipeline<br>+ Xây dựng pipeline cho front-end<br>* Tạo kho Git<br>* Tạo pipeline<br>+ Kiểm tra hoạt động web<br>+ Dọn dẹp | 11/11/2026 | 11/11/2026 | [Lab 20 Intro](https://000076.awsfcaj.com/vi/1-introduction/)<br>[ECS & ALB](https://000076.awsfcaj.com/vi/3-ecs-alb-and-api-gateway/)<br>[Nested Stack](https://000076.awsfcaj.com/vi/5-nested-stack/)<br>[Lab 24 Intro](https://000084.awsfcaj.com/vi/1-preparation/)<br>[SAM Pipeline](https://000084.awsfcaj.com/vi/2-build-sam-pipeline/) |
| **5** | **- Họp team project: rà soát lượt Rolling Accuracy đầu tiên và giao thức đánh giá**<br>+ Đối chiếu trạng thái job 4/4 asset `COMPLETED` với API còn `collecting` 9/20; làm rõ `COMPLETED` không đồng nghĩa đủ mẫu để công bố metric<br>+ Review cách tính các base date hợp lệ, provenance và đường đi dữ liệu phục vụ báo cáo<br>+ Thống nhất `baseline-q252` vẫn là champion; S1a chỉ chạy shadow, không tự động được promote | 12/11/2026 | 12/11/2026 | [DynamoDB Query](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/Query.html) |
| **6** | **- Tìm hiểu chủ đề AWS mới (song song với Lab):** Đọc về EKS, AWS Batch, SageMaker và Terraform trong Physical AI Toolchain; ghi chú vai trò các thành phần NVIDIA để chuẩn bị Blog 2.<br>**- Thực hành Lab 25: Serverless - Giám sát ứng dụng Serverless với CloudWatch và X-Ray**<br>+ Chuẩn bị<br>+ Giám sát với CloudWatch<br>* Gỡ lỗi với nhật ký CloudWatch<br>* Tạo số liệu tùy chỉnh<br>* Tạo cảnh báo với CloudWatch Alarm<br>+ Theo dõi với X-ray<br>+ Dọn dẹp | 13/11/2026 | 13/11/2026 | [Lab 21 Intro](https://000102.awsfcaj.com/vi/1-introduction/)<br>[Create Lambda](https://000102.awsfcaj.com/vi/3-createlambda/)<br>[Three Tier](https://000102.awsfcaj.com/vi/5-threetierweb/)<br>[Lab 25 Intro](https://000085.awsfcaj.com/vi/1-preparation/)<br>[CloudWatch](https://000085.awsfcaj.com/vi/2-cloudwatch-monitor/)<br>[X-Ray](https://000085.awsfcaj.com/vi/3-x-ray-trace/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 10:

1. Xây dựng hoàn chỉnh luồng xử lý Serverless Backend: Tự động hóa xử lý ảnh với S3 Trigger và quản lý dữ liệu NoSQL với DynamoDB.
2. Triển khai thành công Full-stack Serverless App: Kết nối Frontend với Backend thông qua API Gateway và Lambda, xử lý tốt vấn đề CORS.
3. Thiết lập quy trình DevOps tự động (CI/CD) cho ứng dụng Serverless, giúp việc deploy Code và Frontend trở nên nhanh chóng và ít lỗi.
4. Tổng hợp kết quả validation 2019 và kế hoạch kiểm định test2020 (bootstrap, DM-HAC, Holm, validity mask); review lượt Rolling Accuracy 12/11 và tiếp tục giữ `baseline-q252` champion.
5. Hoàn thiện Blog 1 ngày 10/11 về Isaac Lab trên SageMaker AI; tiếp tục tìm hiểu các mảnh ghép Physical AI Toolchain.

