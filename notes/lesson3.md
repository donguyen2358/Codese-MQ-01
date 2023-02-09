# Lesson 3
## Message Queue là gì?
- Message queue là một kiến trúc cung cấp giao tiếp không đồng bộ. Ý nghĩa của queue ở đây chính là 1 hàng đợi chứa message chờ để được xử lý tuần tự theo cơ chế vào trước thì ra trước (FIFO - First In First Out)
- Một message là các dữ liệu cần vận chuyển giữa người gửi và người nhận.

## Khi nào thì sử dụng MQ?
- Sử dụng trong hệ thống dùng kiến trúc microservice, mà các service ở đó liên hệ với nhau 1 cách bất đồng bộ.
- Đảm bảo duration/recovery. Do message đã được luu trong queue, nên khi comsumer xử lý message bị crash hoặc lỗi, ta có thể lấy message từ trong queue để xử lý lại.
- Phân tách hệ thống
- Hỗ trợ rate limit, batching.
- Dễ scaling
