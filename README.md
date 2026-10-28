# MineBT · BTLauncher

Kho phát hành chính thức của BTLauncher: bộ cài và các manifest cập nhật đã ký.

[Tải các bản phát hành](https://github.com/vanden16072004-wq/BTLauncher-Releases/releases)

## Windows

Tải tệp `BTLauncher-<phiên bản>-x64.exe` ở mục Releases, mở bộ cài và chọn thư mục cài đặt. Không cần cài Node.js hay công cụ lập trình. Launcher sẽ chuẩn bị các thành phần Minecraft phù hợp khi người chơi chọn cài profile.

Profile MineBT sử dụng Minecraft 1.12.2, Forge, OptiFine theo điều kiện của nhà phát triển và AegisAC. Có thể lưu nhiều username offline và mở nhiều phiên game tùy tài nguyên máy. Tài khoản offline chỉ vào được các server cho phép offline; server yêu cầu tài khoản Minecraft bản quyền vẫn cần xác thực hợp lệ.

Chứng thư ký Windows hiện là chứng thư MineBT tự cấp, chưa được CA công khai bảo chứng. Kiểm tra đúng kho phát hành và đối chiếu `SHA256SUMS.txt` trước khi chạy bộ cài.

## Cập nhật

Nguồn stable: [stable.json](https://raw.githubusercontent.com/vanden16072004-wq/BTLauncher-Releases/main/stable.json).

Manifest chứa payload và chữ ký Ed25519. Launcher xác minh bằng khóa công khai đã pin, kiểm tra thời hạn và sequence, rồi kiểm tra dung lượng và SHA-256 của tệp tải về. Nội dung có chữ ký sai hoặc rollback bị từ chối. Một URL tải được không thay thế bước xác minh chữ ký.

Bản 1.0.1 cũ chưa có URL online trong bộ cài. Cần cài một lần bản mới có nguồn này hoặc tự nhập URL đã xác minh trong phần cấu hình launcher. Sau đó launcher có thể kiểm tra cập nhật khi mở và trong lúc đang chạy.

## Android và iOS

Đang chuẩn bị ứng dụng native riêng cho Android và iOS. Chỉ tải APK/IPA khi bản phát hành ghi rõ nền tảng và điều kiện cài đặt. IPA chưa ký Apple không cài trực tiếp được lên iPhone. Chính sách bắt buộc cập nhật đồng bộ chỉ bật khi đủ bộ cài hợp lệ của cả ba nền tảng.

## MineBT Network

Địa chỉ server công khai chưa được thiết lập. Khi có địa chỉ chính thức, launcher nhận thay đổi qua manifest đã ký. Không có IP nhà hoặc thông tin đăng nhập máy chủ trong kho này.

Các tệp JAR phát hành là thành phần biên dịch dùng cho profile MineBT. Repository này không chứa source AegisAC, private key hay tài khoản của người chơi. Không có hệ thống chống gian lận nào bảo đảm ngăn được mọi loại hack; việc xử lý dựa trên chính sách xác minh và kiểm tra ở server.
