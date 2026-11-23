---
title: "Worklog Tuần 12"
date: 2026-11-23
weight: 12
chapter: false
pre: " <b> 1.12 </b> "
---

### MỤC TIÊU TRONG WEEK 12:
- Phối hợp rà soát trạng thái production và dữ liệu Rolling Accuracy; tổng kết các giới hạn của hệ thống đánh giá.
- Đối chiếu chi phí do nhóm Platform/Security tổng hợp và hoàn thiện phần tổng kết Modeling & Evaluation.
- Làm chủ kỹ năng quản trị chi phí và tuân thủ (Governance) thông qua IAM Policy nâng cao (giới hạn Region, Instance Type).
- Thiết lập hệ thống giám sát toàn diện: Từ tầng mạng (VPC Flow Logs), tầng ứng dụng (Grafana) đến tầng dịch vụ AWS (CloudWatch).

### CÁC ĐẦU VIỆC CỦA WEEK 12:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Thực hành Lab 30: Quản trị Chi phí và Sử dụng tài nguyên với IAM trên AWS**<br>+ Chuẩn bị<br>* Tạo IAM Group<br>* Tạo IAM user<br>+ Giới hạn theo Region<br>* Tạo policy giới hạn<br>* Gán policy vào group<br>* Kiểm tra hiệu quả policy<br>+ Giới hạn theo EC2 family<br>* Tạo policy giới hạn<br>* Gán policy vào group<br>* Kiểm tra hiệu quả policy<br>+ Giới hạn theo instance size<br>* Cập nhật policy giới hạn<br>* Kiểm tra hiệu quả policy<br>+ Giới hạn theo EBS volume<br>* Tạo policy giới hạn<br>* Gán policy vào group<br>* Kiểm tra hiệu quả policy<br>+ Dọn dẹp tài nguyên | 23/11/2026 | 23/11/2026 | [Lab 30 Intro](https://000064.awsfcaj.com/vi/1-preparation/)<br>[Limit Region](https://000064.awsfcaj.com/vi/2-limit-region/)<br>[Limit Family](https://000064.awsfcaj.com/vi/3-limit-family/)<br>[Limit Size](https://000064.awsfcaj.com/vi/4-limit-size/) |
| **3** | **- Thực hành Lab 31: Giám sát hạ tầng mạng với VPC Flow Log**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>+ Kích hoạt VPC Flow Logs<br>+ Giám sát hạ tầng mạng<br>+ Dọn dẹp tài nguyên | 24/11/2026 | 24/11/2026 | [Lab 31 Intro](https://000074.awsfcaj.com/vi/1-introduce/)<br>[VPC Flow Logs](https://000074.awsfcaj.com/vi/4-enablevpcflowlogs/) |
| **4** | **- Thực hành Lab 32: Bắt đầu với Grafana trên AWS**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Tạo VPC và subnet<br>* Tạo Security Group<br>* Tạo EC2 Instance<br>* Tạo IAM User<br>* Tạo IAM Role<br>* Gán IAM Role<br>+ Cài đặt Grafana<br>+ Giám sát với Grafana<br>+ Dọn dẹp tài nguyên | 25/11/2026 | 25/11/2026 | [Lab 32 Intro](https://000029.awsfcaj.com/vi/1-introduce/)<br>[Install Grafana](https://000029.awsfcaj.com/vi/3-installgrafana/) |
| **5** | **- Thực hành Lab 33: AWS CloudWatch Workshop**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>+ CloudWatch Metric<br>* Viewing Metrics<br>* Search expressions<br>* Math expressions<br>* Dynamic Labels<br>+ CloudWatch Logs<br>* CloudWatch Logs<br>* CloudWatch Logs Insights<br>* CloudWatch Metric Filter<br>+ CloudWatch Alarms<br>+ CloudWatch Dashboards<br>+ Dọn dẹp tài nguyên | 26/11/2026 | 26/11/2026 | [Lab 33 Intro](https://000036.awsfcaj.com/vi/1-introduce/)<br>[Metrics](https://000036.awsfcaj.com/vi/3-cloudwatchmetric/)<br>[Logs](https://000036.awsfcaj.com/vi/4-cloudwatchlogs/)<br>[Alarms](https://000036.awsfcaj.com/vi/5-cloudwatchalarm/) |
| **6** | **- CPAWS: rà soát hồ sơ dự án và phối hợp bàn giao báo cáo**<br>+ Đối chiếu bản Proposal, các ADR, kết quả official test2020, Rolling Accuracy và nội dung Chương 1–5 để kiểm tra tính thống nhất<br>+ Trao đổi với Khải về cấu trúc phần Project của workshop FCAJ; chuẩn bị các file Markdown và liên kết/hình minh họa theo yêu cầu đã thống nhất<br>+ Hỗ trợ kiểm tra bản tổng hợp, demo và các tài liệu nộp; không nhận nhiệm vụ deploy hoặc quay video thay thành viên phụ trách<br>**- CPAWS: kiểm tra báo cáo và tổng kết phần Modeling & Evaluation**<br>+ Rà soát trạng thái Rolling Accuracy, champion/challenger và các giới hạn còn cần nêu trong báo cáo cuối kỳ<br>+ Phối hợp với nhóm đối chiếu thông tin vận hành, chi phí đã chốt và tư liệu workshop; không tự nhận trách nhiệm triển khai production<br>+ Tổng hợp đóng góp cá nhân, kết quả học AWS và bài học về kiểm chứng dự báo trong hệ thống thực tế | 27/11/2026 | 27/11/2026 | [GitHub Pages](https://docs.github.com/en/pages)<br>[AWS Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 12:

1. Thiết lập các chính sách IAM chặt chẽ để kiểm soát việc tạo tài nguyên, ngăn chặn vượt ngân sách (Cost Control) và đảm bảo an ninh.
2. Xây dựng hệ thống giám sát đa tầng: Theo dõi lưu lượng mạng với VPC Flow Logs và trực quan hóa Metric ứng dụng trên Grafana/CloudWatch Dashboard.
3. Đối chiếu Proposal, ADR, Chương 1–5 và kết quả official test2020; góp ý nội dung trước khi nhóm chốt bản nộp.
4. Xác nhận với Khải cách đưa báo cáo vào phần Project của workshop; chuẩn bị nội dung Markdown và hỗ trợ kiểm tra liên kết, không mặc định đã deploy website.
5. Tổng hợp checklist đối chiếu bằng chứng dự báo/accuracy hiện có và các trạng thái production cần nhóm xác nhận; không nhận là người trực tiếp triển khai hệ thống.
6. Tổng hợp phương pháp đánh giá mô hình, kiểm toán artifact và giới hạn point-in-time cho báo cáo workshop cá nhân.

