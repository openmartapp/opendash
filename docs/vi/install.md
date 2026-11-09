# Cài đặt Táp Lô (OpenDash)

[English](../install.md) | **Tiếng Việt**

Làm một lần, ở nhà hoặc khi xe đang đỗ, với điện thoại đang nối Wi-Fi. Mất khoảng 10 phút. App Táp Lô
cũng dẫn bạn qua đúng các bước này và tự đánh dấu từng bước khi thấy đã xong.

## 1. Cài Táp Lô

Tải `opendash-<phiên bản>.apk` từ [trang Releases](../../../../releases/latest) rồi mở file. Khi được
hỏi, cho phép trình duyệt hoặc trình quản lý file cài app.

Google Play Protect có thể hiện **Nên quét ứng dụng** ("Play Protect chưa từng thấy ứng dụng này"), cả
khi Táp Lô tự cập nhật: nó chưa thấy file mới này. Chạm **Quét ứng dụng** để Google kiểm tra trước, hoặc
**Chi tiết khác** › **Cài đặt mà không quét**.

Cài thêm `dashplayer-<phiên bản>.apk` từ cùng bản phát hành nếu bạn muốn thẻ media của xe, nút media
trên vô lăng và ô tìm kiếm của Android Auto điều khiển trình phát của Táp Lô. App này không có màn
hình riêng; Android Auto liệt kê nó trong các app media với tên **Kênh Xe**.

Trên điện thoại cài tiếng Việt, hai app có tên **Táp Lô** (OpenDash) và **Kênh Xe** (Dash Player):
những từ mà nhận dạng giọng nói tiếng Việt của Google nghe tốt.

Bước 2 tới 6 chỉ cần cho chế độ **Màn hình ảo** (app đã cài trong các ô). Với chế độ **Trực tiếp**
(YouTube, mặc định) và **Built-in**, chuyển thẳng tới bước 7.

## 2. Cài Shizuku

Shizuku cho Táp Lô quyền tạo màn hình ảo mà không cần root. Cài từ
[Google Play](https://play.google.com/store/apps/details?id=moe.shizuku.privileged.api) hoặc
[GitHub](https://github.com/RikkaApps/Shizuku/releases) (nút **Tải Shizuku** trong Táp Lô mở trang tải).

## 3. Bật Tùy chọn nhà phát triển

Cài đặt › Giới thiệu về điện thoại › chạm **Số hiệu bản tạo** (Build number) 7 lần (nhập mã PIN nếu được hỏi).

| Điện thoại | "Số hiệu bản tạo" nằm ở |
| --- | --- |
| Pixel, đa số máy | Cài đặt › Giới thiệu về điện thoại |
| Samsung | Cài đặt › Thông tin điện thoại › Thông tin phần mềm |
| Xiaomi, Redmi, POCO | Cài đặt › Giới thiệu điện thoại › chạm **Phiên bản MIUI** / **Phiên bản HĐH** |

## 4. Bật Gỡ lỗi không dây

Cài đặt › Hệ thống › Tùy chọn nhà phát triển › **Gỡ lỗi không dây** › bật, và cho phép trên mạng Wi-Fi
của bạn. Điện thoại phải nối Wi-Fi (mạng nào cũng được, không cần internet).

## 5. Khởi động Shizuku

Mở Shizuku › **Khởi động qua Gỡ lỗi không dây** (Start via Wireless debugging) › **Ghép nối** (Pairing), rồi làm theo hướng dẫn: Shizuku nhờ
bạn mở "Ghép nối thiết bị bằng mã ghép nối" trong Gỡ lỗi không dây và gõ mã vào thông báo của
Shizuku. Chỉ cần ghép nối một lần; sau đó chạm **Khởi động** (Start).

Shizuku dừng mỗi khi điện thoại khởi động lại. Sau mỗi lần khởi động lại, mở Shizuku và chạm **Khởi
động** (lúc đó Gỡ lỗi không dây phải bật và điện thoại phải nối Wi-Fi). Nếu máy đã root, Shizuku có thể
tự khởi động.

## 6. Cho phép Táp Lô

Trong Táp Lô, chạm **Cấp quyền** và chọn **Luôn cho phép** (Allow all the time). Thẻ thiết lập sẽ hiện "Đã kết nối service".

## 7. Hiện Táp Lô trong Android Auto

Android Auto chỉ hiện app ngoài Play Store khi bật chế độ nhà phát triển:

1. Mở cài đặt Android Auto (nút **Mở cài đặt Android Auto** trong Táp Lô).
2. Kéo xuống dưới, chạm **Phiên bản** 10 lần; đồng ý bật cài đặt nhà phát triển.
3. ⋮ (góc trên bên phải) › **Cài đặt nhà phát triển** › bật **Nguồn không xác định** (bản Android Auto mới ghi **Không rõ nguồn gốc**).

Nếu Android Auto đang bị tắt trên điện thoại, nút đó mở trang của nó trên cửa hàng: bật lại ở đó.
Cập nhật Android Auto nếu phiên bản cũ hơn 17.

## 8. Chọn nội dung và kết nối xe

Trong Táp Lô, chọn chế độ hiển thị ở Cài đặt. Ở chế độ Màn hình ảo hoặc Built-in, chọn bố cục và app
hoặc nội dung cho từng ô. Rồi kết nối xe (cáp hoặc không dây), mở danh sách app trên màn hình xe và
chọn **Táp Lô**. Bước thiết lập cuối tự đánh dấu khi Táp Lô mở lần đầu trên xe.

Khi có nhiều ô, trên màn hình xe: chạm một ô để chọn nó (viền xanh), rồi dùng nút tròn Táp Lô để mở
**Bố cục**, **Quay lại** và **Ứng dụng**.

## Lệnh giọng nói

Lần đầu bạn chạm 🎤 trên màn hình xe, điện thoại hỏi quyền dùng micro (hoặc cho phép trước trong Táp
Lô › Cài đặt › Lệnh giọng nói). Xem [`voice-commands.md`](voice-commands.md).

## Cài đặt pin

Một số điện thoại đóng app chạy nền rất mạnh tay. Nếu app trong các ô dừng hoặc khởi động lại khi tắt
màn hình, cho Táp Lô chạy nền: Cài đặt › Ứng dụng › Táp Lô › Pin › **Không hạn chế** (Xiaomi: bật
thêm **Tự khởi động**).

## Thử khi không có xe

Desktop Head Unit (DHU) của Google hiện Android Auto trên máy tính. Xem phần "Trying it without a car"
trong [hướng dẫn tiếng Anh](../install.md#trying-it-without-a-car).
