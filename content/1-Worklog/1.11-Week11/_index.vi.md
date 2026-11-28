---
title: "Worklog Tuần 11"
date: 2026-11-23
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### MỤC TIÊU TRONG WEEK 11:
- Hoàn thành phần Cost Estimation & Optimization cho CPAWS sau khi nhóm release production ngày 23/11, trong giai đoạn hoàn thiện hồ sơ và video demo.
- Xây dựng dự toán bằng AWS Pricing Calculator dựa trên tài nguyên đã triển khai, historical usage và kịch bản tải theo tháng; đề xuất tối ưu chi phí và hướng dẫn clean-up.
- Hoàn thiện báo cáo COST song ngữ và chuẩn bị tài liệu bàn giao cho nhóm.
- Thực hành quản trị chi phí tài nguyên với IAM (Lab 30) và giám sát bằng CloudWatch (Lab 33).

**Bối cảnh dự án:** Nhóm CPAWS đã release production v1.0.1 ngày 23/11; công việc hoàn thiện hồ sơ nộp và video demo của nhóm diễn ra trong giai đoạn 23–25/11. Sau mốc này, phần việc project cá nhân của em tập trung vào AWS Pricing Calculator và báo cáo COST, không phụ trách deploy, quay demo hoặc kiểm thử lại mô hình. Phạm vi dự toán là môi trường `cpaws-dev-*` hiện có.

### CÁC ĐẦU VIỆC CỦA WEEK 11:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
|:---:|---|:---:|:---:|---|
| **2** | **- Mốc chung của nhóm: Release production, hoàn thiện hồ sơ nộp và quay video demo**<br>+ Nhóm release production v1.0.1 ngày 23/11 và hoàn thiện hồ sơ, minh chứng video demo trong giai đoạn 23–25/11; phần việc project cá nhân tiếp theo tập trung vào dự toán chi phí.<br>**- Thực hành Lab 30: Quản trị Chi phí và Sử dụng tài nguyên với IAM trên AWS**<br>+ Chuẩn bị<br>* Tạo IAM Group<br>* Tạo IAM user<br>+ Giới hạn theo Region<br>* Tạo policy giới hạn<br>* Gán policy vào group<br>* Kiểm tra hiệu quả policy<br>+ Giới hạn theo EC2 family<br>* Tạo policy giới hạn<br>* Gán policy vào group<br>* Kiểm tra hiệu quả policy<br>+ Giới hạn theo instance size<br>* Cập nhật policy giới hạn<br>* Kiểm tra hiệu quả policy<br>+ Giới hạn theo EBS volume<br>* Tạo policy giới hạn<br>* Gán policy vào group<br>* Kiểm tra hiệu quả policy<br>+ Dọn dẹp tài nguyên | 23/11/2026 | 23/11/2026 | [Lab 30 Intro](https://000064.awsfcaj.com/vi/1-preparation/)<br>[Limit Region](https://000064.awsfcaj.com/vi/2-limit-region/)<br>[Limit Family](https://000064.awsfcaj.com/vi/3-limit-family/)<br>[Limit Size](https://000064.awsfcaj.com/vi/4-limit-size/) |
| **3** | **- CPAWS: phân tích chi phí sau triển khai bằng AWS Pricing Calculator**<br>+ Đối chiếu kiến trúc đã triển khai và cấu hình tài nguyên AWS tại Singapore (`ap-southeast-1`); giới hạn dự toán trong môi trường `cpaws-dev-*` hiện có, dùng làm baseline production lưu lượng thấp.<br>+ Sử dụng CSV Cost Explorer, CloudWatch metrics/logs và cấu hình tài nguyên để phân biệt usage quan sát được với giả định workload; dự toán 5 MAU, 2.700 API requests và 300 lượt chat/tháng.<br>+ Hoàn thành AWS Console Calculator (34 usage lines, 1,49 USD/tháng) và export CSV ngày 24/11; sử dụng Public Calculator cho Bedrock (3,77 USD/tháng) và EventBridge Scheduler (0,00 USD/tháng).<br>+ Bổ sung SSM Standard và KMS vào phạm vi dự toán, không thay đổi tài nguyên AWS. | 24/11/2026 | 24/11/2026 | [AWS Pricing Calculator](https://calculator.aws/)<br>[AWS Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)<br>[Amazon CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html)<br>[Bedrock estimate](https://calculator.aws/#/estimate?id=f81e944af4c143c007493dbfad5bfa39c934efbe)<br>[Scheduler estimate](https://calculator.aws/#/estimate?id=1530e02ff22ccf47d5f43f5a203d3d3bc392f421) |
| **4** | **- CPAWS: kiểm chứng dự toán và hoàn thiện báo cáo COST song ngữ**<br>+ Kiểm tra CSV đã export: 34 usage ID khác nhau; đối chiếu dự toán Console và Public Calculator cho 13 nhóm dịch vụ.<br>+ Ghi nhận tổng chi phí hiển thị 5,26 USD/tháng và 63,12 USD/năm, phân biệt số gốc chưa làm tròn với số hiển thị; xác định Bedrock và CloudWatch là hai nguồn chi phí chính.<br>+ Hoàn thành `CPAWS_Cost_Estimation_and_Optimization.md` bằng tiếng Việt và tiếng Anh, gồm giả định workload, phân tích độ nhạy, tài liệu tham khảo, đề xuất tối ưu (giảm token/context, Lambda right-sizing, lifecycle và retention) và hướng dẫn clean-up theo CDK.<br>+ Hoàn thiện nội dung bàn giao cho Khải, tổng hợp minh chứng và giới hạn dự toán. Các biện pháp tối ưu và clean-up được tài liệu hóa, không thực thi trên hệ thống đang vận hành. | 25/11/2026 | 25/11/2026 | [AWS Pricing Calculator](https://calculator.aws/)<br>[AWS Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)<br>[Amazon CloudWatch](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/WhatIsCloudWatch.html)<br>[Bedrock estimate](https://calculator.aws/#/estimate?id=f81e944af4c143c007493dbfad5bfa39c934efbe)<br>[Scheduler estimate](https://calculator.aws/#/estimate?id=1530e02ff22ccf47d5f43f5a203d3d3bc392f421) |
| **5** | **- Thực hành Lab 33: Amazon CloudWatch Workshop**<br>+ Giới thiệu<br>+ Các bước chuẩn bị<br>+ CloudWatch Metrics<br>* Viewing Metrics<br>* Search expressions<br>* Math expressions<br>* Dynamic Labels<br>+ CloudWatch Logs<br>* CloudWatch Logs Insights<br>* CloudWatch Metric Filter | 26/11/2026 | 26/11/2026 | [Lab 33 Intro](https://000036.awsfcaj.com/vi/1-introduce/)<br>[Metrics](https://000036.awsfcaj.com/vi/3-cloudwatchmetric/)<br>[Logs](https://000036.awsfcaj.com/vi/4-cloudwatchlogs/) |
| **6** | **- Tiếp tục Lab 33: Amazon CloudWatch Workshop**<br>+ CloudWatch Alarms<br>+ CloudWatch Dashboards<br>+ Dọn dẹp tài nguyên | 27/11/2026 | 27/11/2026 | [Lab 33 Intro](https://000036.awsfcaj.com/vi/1-introduce/)<br>[Alarms](https://000036.awsfcaj.com/vi/5-cloudwatchalarm/)<br>[Lab 33 Guide](https://000036.awsfcaj.com/vi/) |
| **7** | **- Nộp Workshop và báo cáo thực tập cá nhân**<br>+ Chốt Worklog song ngữ đến thời điểm nộp; kết thúc giai đoạn thực hiện Workshop. | 28/11/2026 | 28/11/2026 | [Quy định Workshop FCAJ](https://hcm-rules.awsfcaj.com/project) |

### THÀNH TỰU ĐẠT ĐƯỢC TRONG WEEK 11:

1. Hoàn thành dự toán chi phí sau triển khai CPAWS cho 13 nhóm dịch vụ, kiểm chứng 34 usage lines riêng biệt trên Console Calculator và xây dựng baseline theo tháng với lưu lượng thấp.
2. Đối chiếu tổng chi phí hiển thị 5,26 USD/tháng (63,12 USD/năm) với số gốc chưa làm tròn; xác định Bedrock và CloudWatch là hai nguồn chi phí chính. Đây là dự toán, không phải hóa đơn AWS thực tế.
3. Hoàn thành báo cáo Markdown Cost Estimation & Optimization song ngữ, gồm minh chứng, giả định workload, đề xuất tối ưu và hướng dẫn clean-up; hoàn thiện nội dung bàn giao cho nhóm.
4. Thực hành quản trị tài nguyên bằng IAM (Lab 30) và giám sát bằng CloudWatch (Lab 33).
5. Hoàn thành và nộp Workshop ngày 28/11/2026; thời gian thực tập chính thức vẫn kéo dài đến 14/12/2026.
