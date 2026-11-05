# OpenDash (Táp Lô)

[English](README.md) | **Tiếng Việt** · Website: [opendash.openmart.app](https://opendash.openmart.app/vi)

**Đưa app và nội dung trên điện thoại lên màn hình xe, đặt cạnh nhau, qua Android Auto.**

OpenDash là app Android của OpenMart, tải miễn phí, có bản trả phí (mã bản quyền). Trên điện thoại cài tiếng Việt, app có tên **Táp
Lô**, còn app đi kèm Dash Player có tên **Kênh Xe**. Táp Lô chạy các app bạn chọn trong màn hình ảo
(qua [Shizuku](https://shizuku.rikka.app/), không cần root) hoặc hiện nội dung riêng của nó
(YouTube, thư viện media, website), ghép chúng thành một khung hình và hiện lên màn hình xe; chạm
trên màn hình xe sẽ tới đúng app.

Kho này chứa các bản phát hành và hướng dẫn sử dụng của Táp Lô. Táp Lô không phải mã nguồn mở.

> [!WARNING]
> **Lái xe an toàn.** Táp Lô hiện những app không được thiết kế để dùng khi lái xe. Hãy thiết lập
> khi xe đang đỗ, giữ mắt trên đường và tuân thủ luật giao thông nơi bạn lái. Bạn chịu trách nhiệm
> về cách mình sử dụng app.

## Tính năng

Ba chế độ hiển thị, mỗi chế độ giữ cấu hình riêng:

| Chế độ | Hiện gì | Cần gì |
| --- | --- | --- |
| **Trực tiếp** (mặc định) | YouTube hoặc thư viện media, vẽ thẳng lên màn hình xe cho hình mượt nhất, kèm tốc độ, giới hạn tốc độ và hướng rẽ kế tiếp | Không cần gì thêm |
| **Built-in** | Tối đa 4 ô với nội dung riêng của Táp Lô: website, trình phát media, trang làm cho Táp Lô | Không cần gì thêm: app ngân hàng (vốn không chạy khi bật gỡ lỗi) vẫn dùng được |
| **Màn hình ảo** | Tối đa 4 app đã cài trên máy, mỗi app vừa với ô của nó | Shizuku, khởi động bằng Gỡ lỗi không dây hoặc root |

- **Bố cục:** toàn màn hình, chia đôi ngang, chia đôi dọc, 1 lớn + 2 nhỏ, hoặc 2 × 2; đổi cỡ hoặc
  ẩn ô ngay trên điện thoại hoặc trên xe.
- **Chạm trên màn hình xe:** chạm, kéo, vuốt và chụm hai ngón tới đúng app dưới ngón tay. Nút Táp Lô
  nổi trên màn hình xe mở Bố cục, Quay lại, Ứng dụng và Thông tin, không cần đụng tới điện thoại.
- **Vẫn chạy** khi bạn đổi bố cục, khoá điện thoại hay kết nối không dây chập chờn một lúc.
  Khi Android Auto kết thúc, các app đóng lại và Táp Lô dừng; lần lái xe sau chúng mở lại.
- **Kênh Xe** (Dash Player), app nhỏ đi kèm, cho thẻ media của xe, nút media trên vô lăng và ô tìm
  kiếm của Android Auto điều khiển trình phát.
- **Lệnh giọng nói** bằng nút 🎤 trên màn hình xe: phát, tạm dừng, chuyển bài, tìm YouTube, hoặc chỉ
  đường trong app dẫn đường của bạn. Bộ lệnh là văn bản bạn sửa được ngay trong app, cho mọi ngôn
  ngữ; có sẵn tiếng Việt và tiếng Anh.
- **Tốc độ và giới hạn tốc độ** từ GPS điện thoại, OpenStreetMap hoặc WazeMod.
- **Trình hướng dẫn thiết lập** tự kiểm tra từng bước. Giao diện tiếng Việt và tiếng Anh.

**Trạng thái:** đang phát triển (0.x). Chạy được trên Desktop Head Unit của Google và các điện thoại
đã thử. Rất mong nhận báo cáo từ xe và đầu Android Auto thật.

## Yêu cầu

- Android 11 trở lên.
- Android Auto, bật chế độ nhà phát triển và **Nguồn không xác định** (Táp Lô không có trên Play Store).
- Xe hoặc đầu màn hình có Android Auto (có dây hoặc không dây), hoặc Desktop Head Unit của Google để thử.
- Chỉ chế độ Màn hình ảo: [Shizuku](https://shizuku.rikka.app/) 11 trở lên.

## Cài đặt

1. Tải `opendash-<phiên bản>.apk`, và `dashplayer-<phiên bản>.apk` nếu muốn dùng nút media của xe,
   từ [bản phát hành mới nhất](../../releases/latest). Chỉ tải Táp Lô ở đây: bản được bán hay chia sẻ
   ở nơi khác có thể đã bị sửa.
2. Cài cả hai, rồi mở Táp Lô: trình hướng dẫn sẽ dẫn bạn qua các bước còn lại.

Hướng dẫn từng bước, kèm chế độ nào cần bước nào: [`docs/vi/install.md`](docs/vi/install.md).

## Tài liệu tiếng Việt

| Nội dung | Đọc |
| --- | --- |
| Cài đặt và thiết lập | [`docs/vi/install.md`](docs/vi/install.md) |
| Sử dụng: chế độ, màn hình xe, nút, cài đặt | [`docs/vi/user-guide.md`](docs/vi/user-guide.md) |
| Lệnh giọng nói và bộ lệnh | [`docs/vi/voice-commands.md`](docs/vi/voice-commands.md) |
| Tốc độ và giới hạn tốc độ từ WazeMod | [`docs/vi/wazemod.md`](docs/vi/wazemod.md) |
| Xử lý sự cố | [`docs/vi/troubleshooting.md`](docs/vi/troubleshooting.md) |

## Quyền riêng tư

Táp Lô không có tài khoản, quảng cáo, phân tích hay báo cáo lỗi tự động. App không gửi gì về bạn
cho nhà phát triển. Táp Lô dùng các quyền như sau:

- **Vị trí:** chỉ khi xe đang hiện tốc độ, để đo tốc độ bằng GPS điện thoại. Vị trí ở lại trên máy,
  trừ việc nguồn giới hạn tốc độ OpenStreetMap hỏi máy chủ [Overpass](https://overpass-api.de/)
  công cộng về các con đường trong khu vực bạn đang ở (từng ô bản đồ rộng khoảng 2 km quanh xe), rồi
  lưu trên máy 30 ngày.
- **Micro:** chỉ khi màn hình lệnh giọng nói đang nghe. Âm thanh tới bộ nhận dạng giọng nói của điện
  thoại (thường là của Google, theo điều khoản của Google), không tới nhà phát triển Táp Lô.
- **Thông báo** (không bắt buộc): để biết app dẫn đường nào đang chạy và hiện hướng rẽ kế tiếp trên
  xe. Táp Lô chỉ xem các thông báo đang chạy, và với thông báo dẫn đường thì chỉ đọc đó là app nào và
  hướng rẽ kế tiếp, không lưu lại.
- **Mạng:** các website và stream bạn mở, YouTube cho trình phát và tìm kiếm, và máy chủ Overpass ở trên.
- **Hiển thị trên ứng dụng khác** (không bắt buộc): chỉ để mở chỉ đường khi bạn yêu cầu trên xe,
  bằng một cửa sổ trong suốt 1 điểm ảnh trong chốc lát.
- **Nhật ký:** nằm trên máy. Cài đặt › Xuất nhật ký tạo một file để bạn tự chọn gửi đi; file có
  nhật ký của Táp Lô, model điện thoại và phiên bản Android, Android Auto, Shizuku.

## Cộng đồng

Tin tức, bản mới và hỏi đáp: [website](https://opendash.openmart.app/vi) và [trang Facebook Táp Lô - OpenDash](https://www.facebook.com/taplo.opendash).
Báo lỗi thì gửi ở [GitHub issues](../../issues) để không bị sót.

## Điều khoản sử dụng

Copyright © 2026 OpenMart. Bảo lưu mọi quyền. Táp Lô được tải miễn phí; bản trả phí cần mã bản quyền
của OpenMart. Không được bán app hay mã bản quyền, sửa, đóng gói lại, vượt qua phần kiểm tra bản quyền
hay dịch ngược app: xem [`LICENSE`](LICENSE) (tiếng Anh). Các phần mềm bên thứ ba mà app
dùng và giấy phép của chúng có trong app, ở Cài đặt › Giấy phép phần mềm bên thứ ba. Giới hạn tốc độ ©
những người đóng góp [OpenStreetMap](https://www.openstreetmap.org/copyright) (ODbL).

OpenDash không liên quan tới, cũng không được Google hay YouTube bảo trợ. Android Auto và YouTube là
thương hiệu của Google LLC.
