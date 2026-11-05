# WazeMod: tốc độ và giới hạn tốc độ từ Waze

[English](../wazemod.md) | **Tiếng Việt**

WazeMod là bản Waze đã sửa do một nhà phát triển trong cộng đồng làm, không phải của Táp Lô hay
Waze. WazeMod chia sẻ tốc độ và giới hạn tốc độ của con đường cho app khác qua API dữ liệu. Táp Lô
hiện các số này trên video ở chế độ Trực tiếp và trên thẻ nhạc của xe, như các nguồn tốc độ khác.

Táp Lô không lưu trữ hay bảo đảm cho WazeMod. Chỉ tải WazeMod từ trang chính thức
[wazemod.io.vn](https://wazemod.io.vn/), và hỏi cộng đồng của WazeMod khi gặp vấn đề với nó (link ở
cuối bài).

## 1. Chọn bản cài

Trên [wazemod.io.vn](https://wazemod.io.vn/), bấm **Download** (hoặc **Tải APK Waze Mod** trên
menu), rồi chọn:

- **Phiên bản.** Lấy bản mới nhất được ghi là ổn định hoặc mới nhất, không lấy bản Beta: bản Beta có
  thể chưa có API dữ liệu, khi đó Táp Lô không đọc được.
- **Phiên bản Android** của máy (Táp Lô cần Android 11 trở lên).
- **"Có Android Auto"** nếu muốn dùng cả Waze trên màn hình xe; **"Đã gỡ AA"** thì không có.
- **Kiểu cài:**
  - **DUAL** cài bên cạnh Waze của Google; cả hai cùng ở trên máy, dữ liệu riêng.
  - **Cài đè** thay Waze của Google: gỡ Waze của Google trước.

Táp Lô tìm được WazeMod với cả hai kiểu cài.

## 2. Cài đặt

1. Cho phép trình duyệt (hoặc trình quản lý tệp) cài app: lần đầu mở file APK, Android sẽ hỏi; chọn
   **Cài đặt** › **Cho phép từ nguồn này**.
2. Với **Cài đè**, gỡ Waze của Google trước (địa điểm đã lưu vẫn còn trong tài khoản Waze).
3. Mở file APK vừa tải và bấm **Cài đặt**.
4. Mở WazeMod một lần, đăng nhập hoặc bỏ qua, và cho phép quyền vị trí.

Trang **Hướng dẫn cài đặt APK** trên website của WazeMod có hình minh hoạ từng bước.

## 3. Kết nối với Táp Lô

1. Trong Táp Lô: Cài đặt › **Nguồn tốc độ**. Dòng WazeMod có nút **Kết nối WazeMod**.
2. Bấm nút đó: WazeMod hỏi có cho Táp Lô đọc dữ liệu không (tốc độ, giới hạn, hướng rẽ, cảnh báo,
   thời gian đến, tên đường; không gồm vị trí GPS). Bấm **Cho phép**.
3. Kéo **WazeMod** lên trên nếu muốn dùng nó trước GPS điện thoại và OpenStreetMap.

Có thể thu hồi quyền trong WazeMod: Cài đặt › Ứng dụng đã kết nối. Khi đó Táp Lô dùng nguồn tiếp
theo trong danh sách.

## Khi không chạy

- **"Chưa cài"** dưới dòng WazeMod: bản đang cài không có API dữ liệu (thường là bản Beta). Cài bản
  ổn định mới nhất.
- **Không có tốc độ khi chạy xe:** WazeMod chỉ cho tốc độ khi đang mở và đã bắt được GPS; mở WazeMod
  trước khi đi. Kiểm tra WazeMod đang bật trong **Nguồn tốc độ**.
- **WazeMod chưa cho phép:** bấm lại **Kết nối WazeMod** và chọn **Cho phép**.

Về chính WazeMod (lỗi cài đặt, bản đồ, cảnh báo): hỏi trong
[nhóm Facebook](https://www.facebook.com/groups/wazevn) hoặc nhóm hỗ trợ có link trên
[wazemod.io.vn](https://wazemod.io.vn/).
