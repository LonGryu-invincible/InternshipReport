---
title: "Worklog Tuần 5"
date: 2026-10-12
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### MỤC TIÊU TRONG WEEK 5:
- Hiểu và ứng dụng kiến trúc Serverless (AWS Lambda) để tự động hóa vận hành (Cost Optimization) và xử lý sự kiện (Event-driven).
- Nắm vững cách tương tác giữa Lambda với các dịch vụ lưu trữ (S3) và cơ sở dữ liệu NoSQL (DynamoDB).
- Làm chủ công cụ dòng lệnh AWS CLI để quản lý tài nguyên nhanh chóng và chuyên nghiệp thay vì chỉ dùng Console.
- Rà soát bản nháp Proposal và định nghĩa target trong API contract ở các buổi trao đổi ngày 14–15/10.

### CÁC ĐẦU VIỆC CỦA WEEK 5:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | - Ôn luồng xử lý AWS Lambda theo sự kiện, quyền IAM và CloudWatch cơ bản để chuẩn bị Lab 13 và Lab 14. | 12/10/2026 | 12/10/2026 | [Lab 13 Intro](https://000022.awsfcaj.com/vi/1-introduce/)<br>[Create Role](http://000022.awsfcaj.com/vi/4-createroleforlambda/)<br>[Lambda Function](https://000022.awsfcaj.com/vi/5-createlambdafunction/) |
| **3** | **- Thực hành Lab 13: Tối ưu chi phí EC2 với Lambda**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Tạo VPC<br>* Tạo Security Group<br>* Tạo EC2 instance<br>* Incoming Web-hooks slack<br>+ Tạo Tag cho Instance<br>+ Tạo Role cho Lambda<br>+ Tạo Lambda Function<br>* Function stop instance<br>* Function start instance<br>+ Kiểm tra kết quả<br>+ Dọn dẹp tài nguyên | 13/10/2026 | 13/10/2026 | [Lab 13 Intro](https://000022.awsfcaj.com/vi/1-introduce/)<br>[Create Role](http://000022.awsfcaj.com/vi/4-createroleforlambda/)<br>[Lambda Function](https://000022.awsfcaj.com/vi/5-createlambdafunction/) |
| **4** | **- Họp team project: Tiến hành viết proposal, xác định problem statement, các main flow của web app**<br>+ Đọc problem statement, phạm vi bốn tài sản, luồng xem dự báo USD/VND và chức năng chatbot để hiểu yêu cầu hệ thống<br>+ Góp ý phần Modeling & Evaluation: target log return, chia dữ liệu theo thời gian, baseline, pinball loss và yêu cầu tránh leakage<br>+ Trao đổi với nhóm để bảo đảm đề xuất mô hình có thể đánh giá khách quan và triển khai được theo lịch phát hành | 14/10/2026 | 14/10/2026 | [Proposal Guide](https://workshop-sample.fcjuni.com/2-proposal/) |
| **5** | **- CPAWS (song song với Lab):** Review `docs/api/contract.md` về target theo phiên giao dịch, khoảng thiếu, quy tắc chuẩn hóa phân vị và `prob_up`; tổng hợp góp ý Modeling & Evaluation.<br>**- Thực hành Lab 14: Serverless - Tương tác giữa Lambda với S3 và DynamoDB**<br>+ Giới thiệu<br>+ Xử lý và Tối ưu Kích thước Ảnh trên AWS<br>* Tạo Lambda Function Xử Lý Ảnh<br>* Tạo S3 Bucket<br>* Tạo IAM Policy cho Lambda Function<br>* Kiểm tra hoạt động của Lambda Function<br>+ Ghi dữ liệu vào Amazon DynamoDB<br>* Tạo và Quản lý Bảng trong AWS DynamoDB<br>* Tạo Lambda Function để Ghi dữ liệu<br>+ Dọn dẹp tài nguyên | 15/10/2026 | 15/10/2026 | [Lab 11 Intro](https://000005.awsfcaj.com/vi/1-introduce/)<br>[Create RDS](https://000005.awsfcaj.com/vi/4-create-rds/)<br>[Backup](https://000005.awsfcaj.com/vi/6-backup/)<br>[Lab 14 Intro](https://000078.awsfcaj.com/vi/1-introduce/)<br>[Resize Function](https://000078.awsfcaj.com/vi/2-resize-image-function/)<br>[DynamoDB Write](https://000078.awsfcaj.com/vi/3-write-data-to-dynaomodb/) |
| **6** | **- Tìm hiểu chủ đề AWS mới (song song với Lab):** Bắt đầu đọc tổng quan về Physical AI, mô phỏng robot và Reinforcement Learning; ghi chú vai trò của cloud trong việc huấn luyện chính sách điều khiển.<br>**- Thực hành Lab 15: Làm quen với AWS CLI**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>+ Cài đặt AWS CLI<br>+ Kiểm tra tài nguyên qua CLI<br>+ AWS CLI với Amazon S3<br>+ AWS CLI với Amazon SNS<br>+ AWS CLI với IAM<br>+ AWS CLI với VPC<br>* AWS CLI với VPC<br>* AWS CLI với Internet Gateway<br>+ Tạo EC2 sử dụng AWS CLI<br>+ Khắc phục lỗi<br>+ Dọn dẹp tài nguyên | 16/10/2026 | 16/10/2026 | [Lab 12 Intro](https://000006.awsfcaj.com/vi/1-introduction/)<br>[Launch Template](https://000006.awsfcaj.com/vi/3-create-launch-template/)<br>[ASG](https://000006.awsfcaj.com/vi/6-create-auto-scaling-group/)<br>[Test Solutions](https://000006.awsfcaj.com/vi/7-test-solutions/)<br>[Lab 15 Intro](https://000011.awsfcaj.com/vi/1-introduce/)<br>[Install CLI](https://000011.awsfcaj.com/vi/3-installcli/)<br>[CLI with EC2](https://000011.awsfcaj.com/vi/9-ec2/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 5:

1. Triển khai thành công giải pháp tiết kiệm chi phí tự động (Lab 13): Sử dụng Lambda để Stop/Start EC2 theo lịch trình và tích hợp thông báo qua Slack.
2. Xây dựng ứng dụng Serverless xử lý ảnh (Lab 14): Kết hợp Lambda, S3 và DynamoDB để tự động resize ảnh và lưu metadata.
3. Sử dụng thành thạo AWS CLI (Lab 15) để thao tác với các dịch vụ cốt lõi (S3, EC2, VPC, IAM) mà không cần giao diện Console.
4. Đọc và góp ý bản nháp Proposal CPAWS; nắm rõ problem statement, luồng web/chatbot và các yêu cầu Modeling & Evaluation. Review hợp đồng API để thống nhất định nghĩa target, phân vị và xác suất.
5. Bước đầu tìm hiểu Physical AI và vai trò của AWS trong mô phỏng, huấn luyện robot thông qua tài liệu; chưa thực hành trên GPU.

