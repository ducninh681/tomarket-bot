
# Tool Auto Tomarket NodeJS

**Tool phát triển và chia sẻ miễn phí bởi NinhND**

## 🛠️ Hướng dẫn cài đặt
> Yêu cầu đã cài đặt NodeJS

- Bước 1: Tải về phiên bản mới nhất của tool [tại đây ⬇️](https://github.com/zuydd/tomarket/archive/refs/heads/main.zip)
- Bước 2: Giải nén tool
- Bước 3: Tại thư mục tool vừa giải nén, chạy lệnh `npm install` để cài đặt các thư viện bổ trợ


## 💾 Cách thêm dữ liệu tài khoản
> Tool hỗ trợ cả `user` và `query_id` (khuyến khích dùng user)

> Tất cả dữ liệu mà bạn cần nhập đều nằm ở các file trong thư mục 📁 `src / data`

- [users.txt](src/data/users.txt) : chứa danh sách `user` hoặc `query_id` của các tài khoản, mỗi dòng ứng với một tài khoản
- [proxy.txt](src/data/proxy.txt) : chứa danh sách proxy, proxy ở mỗi dòng sẽ ứng với tài khoản ở dòng đó trong file users.txt phía trên, để trống nếu không dùng proxy
- [token.json](src/data/token.json) : chứa danh sách token được tạo ra từ `user` hoặc `query_id`. Có thể copy token từ các tool khác qua file này (miễn cùng format) để chạy.

> Định dạng proxy: http://user:pass@ip:port

> Lưu ý: `user` và `query_id` chỉ có thời gian sống (có thể get token) trong tầm 1-2 ngày, `token` có thời gian sống 30 ngày. Vậy nên nếu nhận được thông báo đăng nhập thất bại, hãy lấy mới lại `user` hoặc `query_id`


## 🕹️ Các tính năng có trong tool
- tự động làm nhiệm vụ
- tự động làm daily combo
- tự động claim
- tự động chơi game
- tự động daily check-in
- nhận diện proxy tự động, ae ai chạy proxy thì thêm vào file proxy.txt ở dòng ứng với dòng chứa acc muốn chạy proxy đó, acc nào không muốn chạy proxy thì để trống hoặc gõ skip vào
- đa luồng chạy bao nhiêu acc cũng được, không bị block lẫn nhau

