---
title: "Worklog Tuần 2"
date: 2026-09-21
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### MỤC TIÊU TRONG WEEK 2:
- Nắm vững kỹ năng xử lý sự cố (troubleshooting) VPN và mở rộng kết nối Site-to-Site với Transit Gateway.
- Hiểu và triển khai mô hình Hybrid DNS sử dụng Route 53 Resolver để phân giải tên miền giữa On-premise và AWS.
- Làm chủ các mô hình kết nối đa VPC (VPC Peering và Transit Gateway).
- Hệ thống hóa kiến thức chuyên sâu về dịch vụ Compute (EC2, AMI, EBS, Auto-scaling).
- Hệ thống hóa kiến thức Compute và tham gia trao đổi ý tưởng CPAWS ban đầu trong tuần.
### CÁC ĐẦU VIỆC CỦA WEEK 2:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Tiếp tục thực hành Lab 5:**<br>+ Thiết lập AWS Site-to-Site VPN:<br>5.2 Cấu hình kết nối VPN:<br>5.2.7 Hướng dẫn Troubleshooting VPN<br>5.2.8 Hướng dẫn Troubleshooting VPN Chính thức từ AWS<br>5.3 Cấu hình VPN bằng strongSwan với Transit Gateway:<br>5.3.1 Tạo Customer Gateway<br>5.3.2 Tạo Transit Gateway<br>5.3.3 Tạo kết nối VPN<br>5.3.4 Tạo Transit Gateway Attachment<br>5.3.5 Cấu hình Route Tables<br>5.3.6 Cấu hình Customer Gateway<br>+ Dọn dẹp Tài nguyên<br>+ Infrastructure as Code Templates | 21/09/2026 | 21/09/2026 | [Lab 5 VPN](https://000003.awsfcaj.com/vi/5-vpnsitetosite/) |
| **3** | - Làm việc trực tuyến tại nhà. | 22/09/2026 | 22/09/2026 | — |
| **4** | **- Thực hành Lab 6: Thiết lập Hybrid DNS với Route 53 Resolver**<br>+ Các bước chuẩn bị:<br>* Tạo Key Pair<br>* Khởi tạo CloudFormation Template<br>* Cấu hình Security Group<br>+ Kết nối đến RDGW<br>+ Triển khai Microsoft AD<br>+ Thiết lập DNS:<br>* Tạo Route 53 Outbound Endpoint<br>* Tạo Route 53 Resolver Rules<br>* Tạo Route 53 Inbound Endpoints<br>* Thử nghiệm kết quả<br>+ Dọn dẹp tài nguyên | 23/09/2026 | 23/09/2026 | [Lab 6 Prereq](https://000010.awsfcaj.com/vi/2-prerequiste/)<br>[Connect RDGW](https://000010.awsfcaj.com/vi/3-connecttordgw/)<br>[Setup AD](https://000010.awsfcaj.com/vi/4-setupad/)<br>[Hybrid DNS](https://000010.awsfcaj.com/vi/5-setuphyriddns/) |
| **5** | **- Thực hành Lab 7: Thiết lập VPC Peering**<br>+ Các bước chuẩn bị:<br>* Khởi tạo CloudFormation Template<br>* Tạo Security Group<br>* Tạo EC2 instance<br>+ Cập nhật Network ACL<br>+ Tạo kết nối Peering<br>+ Kích hoạt Cross-Peer DNS<br>+ Dọn dẹp tài nguyên<br>**- Thực hành Lab 8: Tổng quan về AWS Transit Gateway**<br>+ Các bước chuẩn bị:<br>* Tạo Key Pair<br>* Khởi tạo CloudFormation Template<br>+ Tạo Transit Gateway<br>+ Tạo Transit Gateway Attachments<br>+ Tạo Transit Gateway Route Tables<br>+ Thêm Transit Gateway Routes vào VPC Route Tables<br>+ Dọn dẹp tài nguyên | 24/09/2026 | 24/09/2026 | [Lab 7 Guide](https://000019.awsfcaj.com/vi/)<br>[Lab 8 Guide](https://000020.awsfcaj.com/vi/) |
| **6** | **- Họp team project: lên ý tưởng, phân tích, nghiên cứu để chọn lọc idea phù hợp**<br>+ Tham gia phân tích các đề tài dự kiến, so sánh tính khả thi về dữ liệu và phạm vi thực hiện trên AWS<br>+ Cùng nhóm thảo luận hướng dự báo vàng, bạc và dầu; ghi nhận các vấn đề cần nghiên cứu về nguồn giá, cách kiểm chứng mô hình và chi phí triển khai<br>**- Học Module 03: Compute VM on AWS:**<br>+ 03-01: Compute VM on AWS<br>+ 03-01-01: Instance type<br>+ 03-01-02: AMI / Backup / Key Pair<br>+ 03-01-03: Elastic block store<br>+ 03-01-04: Instance store<br>+ 03-01-05:  User data<br>+ 03-01-06: Meta data<br>+ 03-01-07: EC2 auto scaling<br>+ 03-02: EFS/FSx - Lightsail - MGN | 25/09/2026 | 25/09/2026 | [World Bank Commodity Markets](https://www.worldbank.org/en/research/commodity-markets)<br>[03-01](https://www.youtube.com/watch?v=-t5h4N6vfBs)<br>[03-01-01](https://www.youtube.com/watch?v=e7XeKdOVq40)<br>[03-01-02](https://www.youtube.com/watch?v=yAR6QRT3N1k)<br>[03-01-03](https://www.youtube.com/watch?v=hKr_TfGP7NY)<br>[03-01-04](https://www.youtube.com/watch?v=6IHNDJ85aoQ)<br>[03-01-05](https://www.youtube.com/watch?v=_v_43Wi7zjo)<br>[03-01-06](https://www.youtube.com/watch?v=Ew3QRaKJQSA)<br>[03-01-07](https://www.youtube.com/watch?v=bbLcPitXJSY)<br>[03-02](https://youtu.be/hFVYG8WqfU0?si=pwMJL01CuoVoxMQS) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 2:

1. Hoàn thành Lab 5 nâng cao: Biết cách Troubleshooting VPN và cấu hình VPN kết hợp với Transit Gateway (StrongSwan).
2. Triển khai thành công kiến trúc Hybrid DNS (Lab 6), cấu hình Inbound/Outbound Endpoints để phân giải tên miền 2 chiều (AWS <-> On-prem).
3. Xây dựng và kết nối thành công các mạng VPC thông qua VPC Peering (Lab 7) và AWS Transit Gateway (Lab 8).
4. Nắm vững lý thuyết Module 03 về Compute: Hiểu sâu về các loại EC2, các loại ổ cứng EBS, và cơ chế Auto-scaling để tối ưu hóa hiệu suất và chi phí.
5. Tham gia thành lập nhóm CPAWS, tìm hiểu các ý tưởng ban đầu và các yêu cầu dữ liệu/đánh giá cho hướng dự báo vàng, bạc, dầu thô.

