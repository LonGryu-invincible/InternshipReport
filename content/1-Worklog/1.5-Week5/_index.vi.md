---
title: "Worklog Tuần 5"
date: 2026-10-05
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### MỤC TIÊU TRONG WEEK 5:
- Nắm vững kiến thức về các dịch vụ cơ sở dữ liệu trên AWS (RDS, Aurora, Redshift, ElastiCache).
- Làm chủ kỹ năng Hosting Website tĩnh trên S3 kết hợp với CloudFront để tối ưu hiệu năng và bảo mật.
- Thực hành triển khai, quản trị và sao lưu cơ sở dữ liệu quan hệ với Amazon RDS.
- Xây dựng kiến trúc hệ thống có khả năng tự động mở rộng (Scalability) và chịu lỗi cao (High Availability) sử dụng Auto Scaling Group và Load Balancer.
- Tổng kết kết quả thực hành S3 hosting, RDS và Auto Scaling cùng tài liệu tham khảo.

### CÁC ĐẦU VIỆC CỦA WEEK 5:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Học Module 06: Dịch vụ cơ sở dữ liệu trên AWS:**<br>+ 06-01: Database Concepts review<br>+ 06-02: Amazon RDS & Amazon Aurora<br>+ 06-03: Redshift - Elasticache | 05/10/2026 | 05/10/2026 | [06-01](https://youtu.be/OOD2RwWuLRw?si=gUgPzH3nVghQiDQC)<br>[06-02](https://www.youtube.com/watch?v=qbrobQZrokY)<br>[06-03](https://youtu.be/UvdiRW34aNI?si=scib1_YZ27xtdRJY) |
| **3** | **- Thực hành Lab 10: Hosting Website tĩnh với Amazon S3**<br>+ Giới thiệu<br>+ Các Bước Chuẩn Bị<br>* Tạo S3 bucket<br>* Tải dữ liệu<br>+ Bật tính năng static website<br>+ Cấu hình Block Public Access<br>+ Cấu hình public object<br>+ Kiểm Tra Website<br>+ Tăng tốc Static Website với Cloudfront<br>* Chặn tất cả truy cập công cộng vào S3<br>* Cấu hình Amazon CloudFront<br>* Kiểm tra Amazon CloudFront<br>+ Bucket versioning<br>+ Di chuyển Object<br>+ Sao chép S3 Object sang region khác<br>+ Dọn dẹp tài nguyên<br>+ Ghi Chú & Thực Hành Tốt Nhất | 06/10/2026 | 06/10/2026 | [Lab 10 Intro](https://000057.awsfcaj.com/vi/1-introduce/)<br>[Prerequisite](https://000057.awsfcaj.com/vi/2-prerequiste/)<br>[Static Web](https://000057.awsfcaj.com/vi/3-staticwebsite/)<br>[CloudFront](https://000057.awsfcaj.com/vi/7-cloudfront/)<br>[Versioning](https://000057.awsfcaj.com/vi/8-versioning/) |
| **4** | - Rà soát kết quả S3 hosting và CloudFront của Lab 10; chuẩn bị các điều kiện về mạng và security group cho Lab 11 (RDS). | 07/10/2026 | 07/10/2026 | [Lab 10 Intro](https://000057.awsfcaj.com/vi/1-introduce/)<br>[Prerequisite](https://000057.awsfcaj.com/vi/2-prerequiste/)<br>[Static Web](https://000057.awsfcaj.com/vi/3-staticwebsite/)<br>[CloudFront](https://000057.awsfcaj.com/vi/7-cloudfront/)<br>[Versioning](https://000057.awsfcaj.com/vi/8-versioning/) |
| **5** | **- Thực hành Lab 11: Kiến thức cơ bản về cơ sở dữ liệu với Amazon Relational Database Service (RDS)**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Tạo VPC<br>* Tạo EC2 Security Group<br>* Tạo RDS Security Group<br>* Tạo DB Subnet Group<br>+ Tạo EC2 instance<br>+ Tạo RDS database instance<br>+ Triển khai ứng dụng<br>+ Backup và restore<br>+ Dọn dẹp tài nguyên | 08/10/2026 | 08/10/2026 | [Lab 11 Intro](https://000005.awsfcaj.com/vi/1-introduce/)<br>[Create RDS](https://000005.awsfcaj.com/vi/4-create-rds/)<br>[Backup](https://000005.awsfcaj.com/vi/6-backup/) |
| **6** | **- Thực hành Lab 12: Triển khai ứng dụng FCJ Management với Auto Scaling Group**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>* Thiết lập hạ tầng mạng<br>* Khởi tạo EC2 Instance<br>* Khởi tạo Database Instance với Amazon RDS<br>* Cài đặt dữ liệu cho Database<br>* Triển khai máy chủ web<br>* Chuẩn bị các metric cho Predictive scaling<br>+ Tạo Launch Template<br>+ Thiết lập Load Balancer<br>* Tạo Target Group<br>* Tạo Load Balancer<br>+ Kiểm tra kết quả<br>+ Tạo Auto Scaling Group<br>+ Kiểm thử các giải pháp<br>* Kiểm thử giải pháp manual scaling<br>* Kiểm thử giải pháp scheduled scaling<br>* Kiểm thử giải pháp dynamic scaling<br>* Đọc metrics của giải pháp predictive scaling<br>+ Dọn dẹp tài nguyên | 09/10/2026 | 09/10/2026 | [Lab 12 Intro](https://000006.awsfcaj.com/vi/1-introduction/)<br>[Launch Template](https://000006.awsfcaj.com/vi/3-create-launch-template/)<br>[ASG](https://000006.awsfcaj.com/vi/6-create-auto-scaling-group/)<br>[Test Solutions](https://000006.awsfcaj.com/vi/7-test-solutions/) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 5:

1. Hoàn thành Lab 10: Xây dựng thành công Website tĩnh trên S3, bảo mật bucket và tăng tốc độ truy cập toàn cầu bằng Amazon CloudFront.
2. Hoàn thành Lab 11: Triển khai thành công Database Instance trên RDS, kết nối ứng dụng và thực hiện quy trình Backup/Restore cơ sở dữ liệu.
3. Hoàn thành Lab 12: Xây dựng hệ thống High Availability với Auto Scaling Group và Elastic Load Balancer; thực hành thành thạo các chiến lược scaling (Manual, Scheduled, Dynamic, Predictive).
4. Củng cố kiến thức lý thuyết về các loại hình cơ sở dữ liệu trên AWS (SQL vs NoSQL, OLTP vs OLAP).

