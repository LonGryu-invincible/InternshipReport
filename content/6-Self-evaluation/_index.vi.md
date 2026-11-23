---
title: "Tự đánh giá"
date: 2026-10-28
weight: 6
chapter: false
pre: " <b> 6. </b> "
---

Trong chương trình **First Cloud AI Journey (FCAJ)**, em tham gia dự án **CPAWS — hệ thống dự báo hàng hóa trên AWS** với vai trò chính là **Modeling & Evaluation**. Công việc của em không chỉ là kiểm tra kết quả cuối cùng mà còn trải dài từ góp ý cách đặt bài toán, nghiên cứu mô hình đến xây dựng quy trình đánh giá và kiểm chứng bằng chứng thực nghiệm.

Ngay từ giai đoạn xác định yêu cầu, em đã **đề xuất dự báo lợi suất log (log return) thay vì trực tiếp dự báo mức giá tuyệt đối**. Em cũng tham gia rà soát cách biểu diễn đầu ra cho 1–7 phiên giao dịch, các phân vị của phân phối dự báo và xác suất tăng giá, bảo đảm chúng có ý nghĩa nhất quán khi được hiển thị và đánh giá. Đây là đóng góp về định nghĩa bài toán thuộc phạm vi chuyên môn của em, không có nghĩa em phụ trách định hướng hay triển khai toàn bộ dự án.

Trong quá trình thực hiện, em tập trung vào thử nghiệm và phân tích mô hình, triển khai/kiểm thử các chỉ số đánh giá, xây dựng và rà soát **Rolling Accuracy**, review tài liệu kỹ thuật và thực hiện **official test2020**. Em chủ động đóng góp ý kiến trong những nội dung Modeling & Evaluation, đồng thời cố gắng hoàn thành tốt các nhiệm vụ trưởng nhóm phân công.

### Bảng tự đánh giá

| STT | Tiêu chí | Mô tả | Tốt | Khá | Trung bình |
|---|---|---|:---:|:---:|:---:|
| 1 | **Kiến thức và kỹ năng chuyên môn** | Hiểu biết về ngành, vận dụng kiến thức, sử dụng công cụ và chất lượng công việc | ✅ | ☐ | ☐ |
| 2 | **Khả năng học hỏi** | Tiếp thu kiến thức mới và chủ động nghiên cứu | ✅ | ☐ | ☐ |
| 3 | **Chủ động** | Tự tìm hiểu, đề xuất ý kiến và chủ động thực hiện công việc | ✅ | ☐ | ☐ |
| 4 | **Tinh thần trách nhiệm** | Hoàn thành nhiệm vụ và chú trọng chất lượng kết quả | ✅ | ☐ | ☐ |
| 5 | **Kỷ luật** | Tuân thủ giờ giấc, nội quy và quy trình làm việc | ☐ | ✅ | ☐ |
| 6 | **Tính cầu tiến** | Tiếp nhận góp ý và cải thiện bản thân | ☐ | ✅ | ☐ |
| 7 | **Giao tiếp** | Trao đổi, trình bày ý tưởng và báo cáo công việc | ☐ | ✅ | ☐ |
| 8 | **Hợp tác nhóm** | Phối hợp, trao đổi và hỗ trợ các thành viên | ✅ | ☐ | ☐ |
| 9 | **Ứng xử chuyên nghiệp** | Tôn trọng đồng nghiệp và có tác phong phù hợp | ☐ | ✅ | ☐ |
| 10 | **Tư duy giải quyết vấn đề** | Nhận diện vấn đề, phân tích và đề xuất phương án | ☐ | ✅ | ☐ |
| 11 | **Đóng góp vào dự án/tổ chức** | Đóng góp chuyên môn, chất lượng và hiệu quả công việc | ✅ | ☐ | ☐ |
| 12 | **Tổng thể** | Đánh giá chung toàn bộ quá trình thực tập | ☐ | ✅ | ☐ |

### Điểm mạnh

**1. Phân tích bài toán và xác định đầu ra dự báo**

Em quan tâm đến việc xác định đúng biến mục tiêu và cách đo lường kết quả trước khi lựa chọn mô hình. Trong CPAWS, bên cạnh đề xuất sử dụng log return, em còn góp ý về horizon theo phiên giao dịch, các mức phân vị dự báo, `prob_up` và điều kiện hợp lệ của giá ở điểm đầu/cuối kỳ. Em cũng tham gia review hợp đồng API để cách tính của mô hình, nội dung lưu trữ và dữ liệu hiển thị không mâu thuẫn với nhau.

Qua công việc này, em nhận thấy một quyết định về đầu ra dự báo có thể ảnh hưởng trực tiếp đến thiết kế mô hình, quy trình kiểm tra dữ liệu và cách người dùng hiểu kết quả.

**2. Nghiên cứu, thử nghiệm và so sánh các phương pháp dự báo**

Em tham gia thực hiện, phân tích và rà soát các thử nghiệm trên tập **validation 2019**. Công việc của em liên quan đến **DLinear**, **CEEMDAN–DLinear (K3)** và các hướng điều chỉnh theo độ biến động như **K3b/S1a**. Em tập trung đối chiếu hiệu quả của các phương pháp này với `baseline-q252`, xem xét kết quả theo từng tài sản và kỳ dự báo, thay vì chỉ chọn mô hình có vẻ phức tạp hơn.

Một bài học quan trọng là mô hình mới không mặc nhiên tốt hơn baseline. Khi bằng chứng thực nghiệm chưa đủ thuyết phục, em cùng nhóm duy trì `baseline-q252` làm champion và xem **S1a** là challenger chạy **shadow** để tiếp tục theo dõi, không tự động thay thế mô hình hiện hành.

**3. Thiết kế và kiểm thử phương pháp đánh giá**

Đây là phần công việc em dành nhiều thời gian. Em tham gia xây dựng và kiểm thử bộ chỉ số đánh giá, trong đó **pinball skill** so với baseline phân vị 252 phiên là chỉ số chính; các chỉ số phụ giúp quan sát thêm sai số lợi suất, độ phủ và độ rộng khoảng dự báo, cũng như chất lượng xác suất tăng giá.

Em làm việc với các quy tắc đánh giá như chia dữ liệu theo thời gian, kiểm tra `valid mask`, đồng nhất các mẫu so sánh và tránh sử dụng thông tin tương lai. Em cũng tham gia rà soát schema phân biệt **validation, test và rolling_8w**, giúp kết quả có thể truy vết và diễn giải đúng mục đích.

**4. Xây dựng và rà soát Rolling Accuracy**

Trong phần **Rolling Accuracy**, em tham gia xây dựng đặc tả và xử lý logic đánh giá: cửa sổ 56 ngày, ghép bản dự báo đã phát hành với giá thực tế theo `base_date`/`target_date`, điều kiện **eligibility**, tính hợp lệ của nguồn dữ liệu (**provenance**) và các trường hợp thiếu dữ liệu hoặc lỗi upstream.

Em cũng tham gia review hợp đồng dữ liệu phục vụ API `/accuracy/{asset}`, kiểm tra sự nhất quán giữa trạng thái job, kết quả được lưu và thông tin hiển thị. Công việc này giúp em hiểu rằng một tác vụ chạy thành công không đồng nghĩa hệ thống đã có đủ dữ liệu hợp lệ để công bố độ chính xác.

**5. Kiểm chứng thực nghiệm và bảo đảm tính tái lập**

Em tham gia review kế hoạch và runner **test2020**, bao gồm cách chọn mẫu hợp lệ, kiểm định thống kê, khoảng tin cậy bootstrap và điều chỉnh nhiều phép kiểm định. Ngày **16/11/2026**, em trực tiếp thực hiện **một lượt official test2020** theo cấu hình và dữ liệu đã chốt, sau đó kiểm tra các artifact và đối chiếu **7/7 checksum SHA-256**.

Khi tổng hợp kết quả cho báo cáo, em chú trọng phân biệt những kết quả có ý nghĩa thống kê với các trường hợp chưa đủ bằng chứng, đồng thời trình bày giới hạn của dữ liệu và phương pháp. Việc đánh giá này chỉ phục vụ kiểm chứng/báo cáo, không được sử dụng để tối ưu lại mô hình hoặc tự động thay champion.

**6. Trách nhiệm, tự học và phối hợp nhóm**

Em khá hướng ngoại, thoải mái trao đổi và thường chủ động nêu quan điểm khi thảo luận những vấn đề thuộc Modeling & Evaluation. Bên cạnh công việc nghiên cứu, em cũng review Pull Request, góp ý **Proposal, ADR, API contract** và hỗ trợ đối chiếu tài liệu báo cáo với kết quả kỹ thuật.

Em cố gắng hoàn thành tốt công việc do trưởng nhóm phân công và chủ động đọc tài liệu khi gặp vấn đề mới. Quá trình cộng tác với các thành viên phụ trách dữ liệu, API và hạ tầng giúp em rèn luyện khả năng nhìn nhận ảnh hưởng của một quyết định kỹ thuật đến những thành phần khác trong hệ thống.

### Điểm cần cải thiện

**1. Diễn đạt vấn đề kỹ thuật phức tạp**

Mặc dù chủ động giao tiếp, đôi khi em trình bày quá nhiều điều kiện và chi tiết trong một lần trao đổi, khiến ý chính chưa thật sự rõ ràng. Em cần cải thiện khả năng tóm tắt vấn đề, giải thích bằng ví dụ dễ hiểu và sắp xếp nội dung theo thứ tự **vấn đề – bằng chứng – phương án – kết luận**.

**2. Quản lý thời gian khi có nhiều nhiệm vụ**

Có những giai đoạn em phải cân đối giữa nghiên cứu mô hình, review kỹ thuật, bài thực hành AWS, việc học tại trường và báo cáo. Em nhận thấy cần ưu tiên công việc tốt hơn, chia nhiệm vụ thành các mốc nhỏ và chủ động dự phòng thời gian cho vấn đề phát sinh.

### Suy ngẫm

Em tự đánh giá **tổng thể ở mức Khá**. Em hài lòng vì đã đóng góp vào nhiều giai đoạn của CPAWS, từ định nghĩa đầu ra dự báo, nghiên cứu và so sánh mô hình đến thiết kế quy trình đánh giá, Rolling Accuracy và kiểm chứng official test2020. Đồng thời, em hiểu rằng các kết quả có giá trị phải đi kèm dữ liệu hợp lệ, quy trình tái lập được và những kết luận không vượt quá bằng chứng.

FCAJ cũng giúp em nhận ra tầm quan trọng của trách nhiệm cá nhân và phối hợp nhóm trong một hệ thống AI có nhiều thành phần. Em muốn tiếp tục cải thiện cách trình bày vấn đề và quản lý thời gian để chuẩn bị cho định hướng nghiên cứu **AI và Robotic AI** trong tương lai.
