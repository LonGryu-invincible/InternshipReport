---
title: "Sự Kiện 3"
date: 2026-11-14
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Event 3 — Cloud Mastery 1: Amazon Bedrock AgentCore

## 1. Tổng quan sự kiện

- **Ngày:** 14/11/2026
- **Địa điểm:** Tầng 26, Bitexco Financial Tower, Quận 1, TP.HCM
- **Hình thức:** Buổi chia sẻ kỹ thuật
- **Vai trò:** Người tham dự
- **Chủ đề:** Amazon Bedrock AgentCore

Cloud Mastery 1 là buổi chia sẻ kiến thức về việc xây dựng và vận hành ứng dụng AI Agent trên nền tảng AWS. Chủ đề chính của chương trình là Amazon Bedrock AgentCore, tập hợp những dịch vụ hỗ trợ triển khai và vận hành ứng dụng Agentic AI.

Em quan tâm đến sự kiện này vì trước đây việc học AI của em chủ yếu tập trung vào mô hình và thuật toán. AgentCore đề cập đến một hướng khác: làm thế nào để AI Agent có thể sử dụng công cụ, quản lý ngữ cảnh và vận hành trong một hệ thống thực tế.

## 2. Nội dung nổi bật

### 2.1. AI trong ứng dụng doanh nghiệp

Phần mở đầu đề cập đến vai trò của AI trong sản phẩm doanh nghiệp. Một điểm em chú ý là AI không nhất thiết phải là toàn bộ sản phẩm. Trong nhiều trường hợp, mô hình chỉ đảm nhiệm một phần công việc, còn các thành phần khác xử lý dữ liệu, quản lý người dùng và kết nối các chức năng.

Trước đây, khi thử nghiệm mô hình, em thường quan tâm đến đầu vào và đầu ra. Qua chủ đề này, em hiểu thêm rằng triển khai AI trong một sản phẩm thực tế còn phải giải quyết nhiều vấn đề nằm ngoài bản thân mô hình.

### 2.2. Các thành phần của Amazon Bedrock AgentCore

Từ nội dung sự kiện và tài liệu AWS, em tìm hiểu những thành phần chính của AgentCore:

**AgentCore Runtime** cung cấp môi trường được quản lý để triển khai và thực thi AI Agent, giảm bớt công việc tự xây dựng và duy trì máy chủ.

**AgentCore Gateway** giúp Agent kết nối với công cụ và dịch vụ bên ngoài, chẳng hạn API hoặc AWS Lambda. Đây là khả năng quan trọng vì Agent đôi khi cần truy xuất dữ liệu hoặc thực hiện nhiệm vụ thông qua công cụ, thay vì chỉ tạo câu trả lời.

**AgentCore Memory** hỗ trợ quản lý thông tin và ngữ cảnh trong quá trình tương tác. Em thấy thành phần này hữu ích đối với ứng dụng cần duy trì thông tin qua nhiều bước, thay vì xử lý từng yêu cầu độc lập.

**AgentCore Identity** hỗ trợ xác thực và quản lý danh tính khi Agent tương tác với hệ thống khác. Qua đó, em hiểu thêm tầm quan trọng của việc cấp quyền phù hợp, đặc biệt khi Agent sử dụng công cụ thay mặt người dùng.

**AgentCore Observability** hỗ trợ theo dõi hoạt động của Agent để kiểm tra, phân tích và xử lý lỗi. Thành phần này khiến em chú ý vì một hệ thống AI không chỉ cần tạo ra kết quả mà còn cần có cách theo dõi quá trình tạo ra kết quả đó.

### 2.3. Những khả năng bổ sung

Ngoài các thành phần trên, tài liệu AWS còn giới thiệu:

- **Code Interpreter:** Hỗ trợ thực thi mã để xử lý những nhiệm vụ phù hợp.
- **Browser:** Cho phép Agent tương tác với ứng dụng web thông qua môi trường trình duyệt được quản lý.

Những công cụ này giúp mở rộng khả năng của AI Agent so với chatbot chỉ thực hiện hỏi đáp thông thường.

## 3. Trải nghiệm cá nhân

Điều em quan tâm tại Cloud Mastery 1 là cách các thành phần của AgentCore có thể phối hợp để tạo thành một hệ thống hoàn chỉnh.

Trước đây, khi học Machine Learning, em dành nhiều thời gian cho việc xử lý dữ liệu, lựa chọn mô hình và đánh giá kết quả. Vì vậy, các chủ đề về môi trường thực thi, quản lý quyền truy cập và giám sát Agent mang đến cho em góc nhìn mới.

Sau buổi chia sẻ, em tiếp tục tìm hiểu tài liệu chính thức của AWS để hiểu rõ hơn vai trò từng thành phần. Em cũng nhận thấy một ứng dụng Agentic AI không nhất thiết phải dùng tất cả dịch vụ ngay từ đầu; việc lựa chọn thành phần nên dựa trên mục tiêu và phạm vi dự án.

## 4. Bài học rút ra và định hướng

Bài học quan trọng nhất đối với em là **xây dựng AI Agent không chỉ là lựa chọn một foundation model phù hợp**. Một hệ thống thực tế còn cần môi trường thực thi, khả năng sử dụng công cụ, quản lý ngữ cảnh, kiểm soát quyền truy cập và giám sát hoạt động.

Trong thời gian tới, em muốn thử phát triển một dự án AI Agent sử dụng các thành phần của Amazon Bedrock AgentCore. Mục tiêu là lần lượt tìm hiểu Runtime, Gateway, Memory, Identity và Observability, sau đó thử kết hợp chúng trong một ứng dụng có thể xử lý nhiều bước và tương tác với các dịch vụ bên ngoài.

Đây là định hướng học tập và thực hành trong tương lai, chưa phải một hệ thống em đã triển khai.

## 5. Minh chứng tham gia

![Ảnh tại sự kiện Cloud Mastery 1 về Amazon Bedrock AgentCore](/images/4-Event/anh_event_3.jpg)



## 6. Tài liệu tham khảo

- [Amazon Bedrock AgentCore — AWS](https://aws.amazon.com/bedrock/agentcore/)
- [Amazon Bedrock AgentCore Developer Guide](https://docs.aws.amazon.com/bedrock-agentcore/latest/devguide/what-is-bedrock-agentcore.html)
