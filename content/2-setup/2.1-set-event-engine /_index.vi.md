---
title : "Thiết lập Non-event engine - Bước 1"
date :  "`r Sys.Date()`" 
weight : 2 
chapter : false
pre : " <b> 2.1. </b> "
---
{{% notice note %}}
Các hướng dẫn này chỉ cần được tuân theo nếu bạn đang chạy workshop trong tài khoản non-Event Engine.
{{% /notice %}}

### Thiết lập Non Event Engine 
Nếu bạn đang chạy điều này trong tài khoản AWS của mình, **non-production**, bạn sẽ cần triển khai các CloudFormation templates được cung cấp trong hai phần tiếp theo. Trước tiên, bạn sẽ triển khai các mẫu CloudFormation cần thiết, trong khi chúng đang hoàn thành bạn sẽ xem qua tổng quan về workshop.

{{% notice note %}}
Chúng tôi thực sự khuyên bạn nên chạy workshop này trong tài khoản non-production AWS bằng cách sử dụng khu vực us-east-1
{{% /notice %}}

### Bối cảnh
Trong workshop này, bạn sẽ điều tra hai sự kiện bảo mật khác nhau bằng cách phân tích các AWS CloudTrail logs, cập nhật tài liệu hướng dẫn ứng phó với sự cố, sau đó thực hiện các bước để kiểm soát sự kiện. Ở phần này, bạn sẽ đi qua cấu hình ban đầu của CloudTrail Lake, tải lên một số runbooks mẫu dưới dạng Jupyter notebook và hiểu về những thông tin có sẵn.

### Gợi ý
Trong khi bạn thực hiện workshop, sẽ có sẵn các gợi ý nếu bạn gặp khó khăn, chúng sẽ được hiển thị dưới dạng các phần thu gọn như sau

Nhấn để xem gợi ý!
Các gợi ý này sẽ cung cấp các đoạn mã để giúp bạn trong suốt workshop này!

### Câu hỏi
Trong toàn bộ hướng dẫn của workshop, bạn sẽ thấy các câu hỏi như sau:

**When was the town of Boston incorporated?**

Ghi chú lại câu trả lời cho những câu hỏi này vì chúng sẽ hữu ích cho workshop.

Hãy tiếp tục với việc thiết lập environment của chúng ta.