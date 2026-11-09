# Xử lý sự cố

[English](../troubleshooting.md) | **Tiếng Việt**

Để gửi một báo lỗi có ích, mở Táp Lô › Cài đặt (bánh răng) › **Xuất nhật ký** ngay sau khi lỗi xảy ra và
gửi file đó. File có nhật ký gần đây của Táp Lô, model điện thoại và phiên bản Android, Android Auto,
Shizuku. Báo lỗi tại [Issues](../../../../issues), viết tiếng Việt hay tiếng Anh đều được.

## Thiết lập

**"Khởi động Shizuku" không được đánh dấu sau khi khởi động lại máy.** Shizuku dừng mỗi lần điện thoại
khởi động lại. Bật Gỡ lỗi không dây, nối Wi-Fi, mở Shizuku và chạm Khởi động.

**Gỡ lỗi không dây tự tắt.** Nó cần Wi-Fi và tự tắt khi mất Wi-Fi hoặc đổi mạng. Bật lại (và cho phép
mạng đó) trước khi khởi động Shizuku.

**"Cho phép Táp Lô" báo bị từ chối.** Trước đó bạn đã chọn Từ chối. Mở Shizuku › Ứng dụng được ủy quyền
và bật Táp Lô.

**Cài hoặc cập nhật thì hiện "Nên quét ứng dụng".** Google Play Protect hỏi về app nó chưa thấy, và mỗi
bản mới của Táp Lô hay Kênh Xe đều mới với nó. Chạm **Quét ứng dụng**, hoặc **Chi tiết khác** › **Cài
đặt mà không quét**. Chỉ tải Táp Lô từ trang phát hành của nó.

**Thiếu một app trong danh sách.** Danh sách chỉ có app có biểu tượng ở màn hình chính. App bạn đã vô
hiệu hoá không hiện.

## Android Auto

**Táp Lô không có trong danh sách app trên xe.** Bật chế độ nhà phát triển và **Nguồn không xác định**
của Android Auto ([hướng dẫn cài đặt](install.md), bước 7), rồi ngắt và kết nối lại xe.

**Android Auto bị tắt sau khi đổi Cài đặt › Màn hình xe.** Thanh dưới của Android Auto có thể giữ biểu
tượng cũ của Táp Lô vài phút, và chạm vào biểu tượng đó làm Android Auto tắt. Hãy mở Táp Lô từ danh sách
app của Android Auto; nếu Android Auto đã tắt, kết nối lại điện thoại.

**Màn hình xe hiện hình cũ sau khi cập nhật hoặc cài lại Táp Lô.** Táp Lô xin xe vùng vẽ mới sau khoảng
3 giây (có thể thấy "Đang kết nối lại…" một lát). Nếu vẫn đứng hình, mở danh sách app trên xe và chọn
Táp Lô lần nữa.

**Nút của Táp Lô trên màn hình xe ở đâu?** Sau nút tròn Táp Lô trên đường chia giữa hai ô: chạm để mở
Bố cục, Quay lại, Ứng dụng và Thông tin, chạm lần nữa để đóng; menu cũng tự đóng sau 10 giây. Khi chỉ có
một ô, nút nằm ở mép màn hình. Android Auto cũng hiện một nút Táp Lô ở góc trên (tự ẩn sau vài giây; chạm
màn hình để hiện lại), mở cùng menu đó.

**Phím mũi tên hoặc nút media trên vô lăng không có tác dụng.** Android Auto giữ phím mũi tên và núm xoay
cho riêng nó, và gửi nút media cho app media. Thay vào đó hãy dùng: nút thêm của Táp Lô trên màn hình xe,
vuốt và chụm trên màn hình cảm ứng của xe, phím trên điện thoại hoặc remote Bluetooth (Cài đặt › **Thiết
lập nút**), và với nút media thì cài [Kênh Xe](user-guide.md#kênh-xe-nút-media-của-xe).

**Quay lại hoặc Ứng dụng tác động nhầm ô.** Chúng tác động lên ô đang chọn (viền xanh): ô bạn chạm gần
nhất trên màn hình xe.

**Cuộn trong một ô lại làm ô khác chạy.** Chạm ô đó trước rồi mới cuộn hoặc vuốt. Android Auto cho app
biết vị trí khi chạm, nhưng khi kéo chỉ cho biết kéo bao xa, nên Táp Lô gửi thao tác kéo tới ô đang chọn.

## Chế độ Trực tiếp và YouTube

**"Đang tải YouTube…" mãi, hoặc "Không tải được YouTube".** Chạm **Thử lại**, hoặc **Tải lại** trong các
nút của Táp Lô (chạm vào video). Khi chưa có video nào để phát tiếp, trình phát tự tìm một video để
bắt đầu, việc này cũng cần mạng. Kiểm tra mạng. Nếu máy cài cả bản release lẫn bản debug của Táp Lô,
Android Auto có thể mở nhầm bản: chỉ giữ một bản.

**Một video không phát trong Trình phát IFrame.** Chủ kênh không cho nhúng video đó vào trang khác. Chọn
**Trang YouTube** ở Cài đặt › **Trình phát YouTube**.

**Mất tiếng khi bản đồ chiếm màn hình xe.** Đó là mặc định. Bật Cài đặt › **Phát tiếp khi app khác che**
để giữ âm thanh.

**Không thấy tốc độ hoặc giới hạn trên video.** Cài đặt › **Nguồn tốc độ**: bật một nguồn và cho phép
những gì nó hỏi (vị trí cho GPS và OpenStreetMap, sự đồng ý trong WazeMod cho WazeMod). OpenStreetMap chỉ
biết giới hạn của những đường đã được ghi trên bản đồ, và lần đầu đi qua một con đường cần có mạng.

**Điện thoại nóng, hoặc video trên xe bị giật.** Nếu màn hình điện thoại chạy 90 hoặc 120 Hz, Táp Lô
và WebView giữ nhịp đó suốt lúc xe hiện video, kể cả khi màn hình điện thoại tắt. Hãy để điện thoại ở
60 Hz: trên Samsung, Cài đặt › Màn hình › **Chuyển động mượt** › **Tiêu chuẩn**; trên Pixel, tắt Cài
đặt › Màn hình › **Màn hình mượt**; máy khác thì tìm **Tần số quét** trong mục Màn hình. Trên máy thử,
cách này giảm số khung hình video bị bỏ và giảm tải cho điện thoại. Sạc, Android Auto không dây và
nắng chiếu cũng làm máy nóng thêm: dùng cáp và đặt máy ở giá đỡ thoáng, có bóng râm sẽ đỡ hơn.

## Kênh Xe và nút media của xe

**Kênh Xe không có trong các app media của Android Auto.** Cài `dashplayer-<phiên bản>.apk` từ cùng bản
phát hành với Táp Lô: Kênh Xe chỉ làm việc với Táp Lô được ký cùng khoá. Có thể cần kết nối lại xe, và
phải bật Nguồn không xác định ([hướng dẫn cài đặt](install.md), bước 7).

**Thẻ media hiện "Mở Táp Lô trên xe".** Kênh Xe chỉ chuyển lệnh: mở Táp Lô trên màn hình xe một lần, sau
đó thẻ media và nút vô lăng điều khiển được.

**Nút vô lăng không có tác dụng (hay gặp trên vivo, iQOO, Xiaomi, OPPO).** Android Auto gửi phím cho app
media của nó là Kênh Xe, và Kênh Xe phải đang chạy. Táp Lô giữ cho Kênh Xe chạy, nhưng một số điện thoại chỉ
cho Android Auto khởi động nó. Hãy đặt Kênh Xe làm app media của Android Auto: mở **Kênh Xe** một lần từ danh
sách app của Android Auto trên xe; từ đó mỗi lần nối xe Android Auto tự khởi động nó. Nếu bạn nghe nhạc bằng
app khác, mở lại Kênh Xe sau đó.

**"Phát … trên Kênh Xe" lại phát thứ khác.** Đọc đúng tên app như điện thoại hiện (**Kênh Xe** trên máy
cài tiếng Việt). Trợ lý chọn app theo tên đó; nút 🎤 của Táp Lô thì không cần gọi tên.

## Lệnh giọng nói

**"Hãy cho Táp Lô dùng micro".** Cho phép trên điện thoại khi được hỏi, hoặc ở Cài đặt › Lệnh giọng nói ›
**Cho phép dùng micro**.

**"Cho Speech Recognition and Synthesis from Google dùng micro" (hoặc tên một app khác), dù Táp Lô đã có
quyền micro.** Lệnh giọng nói do bộ nhận dạng giọng nói của điện thoại nghe, và Android chỉ đưa âm thanh
cho nó khi nó cũng được dùng micro, kể cả khi nghe bằng micro của xe. Trên một số điện thoại, app này
mặc định chưa có quyền đó. Cài đặt › Lệnh giọng nói › **Mở cài đặt của app đó**, rồi Quyền › Micro ›
Cho phép.

**"Nhận dạng giọng nói cần có mạng" hoặc "Điện thoại này không có nhận dạng giọng nói".** Táp Lô dùng
bộ nhận dạng giọng nói của điện thoại, thường là của Google: cần có mạng và phải hỗ trợ ngôn ngữ đang
chọn. Thử nhận dạng giọng nói ở app khác, như nút micro trên bàn phím.

**Nghe sai, hoặc làm sai lệnh.** Kiểm tra Cài đặt › Lệnh giọng nói › **Ngôn ngữ nhận dạng**. Trong **Sửa
bộ lệnh**, gõ câu mà nó đã nghe vào **Thử một câu** để xem luật nào khớp, rồi thêm những chữ bạn hay nói
([`voice-commands.md`](voice-commands.md)).

**Chỉ đường mở nhầm app.** Cài đặt › Lệnh giọng nói › **App chỉ đường**: chọn một app, hoặc cho phép đọc
thông báo dẫn đường để chế độ Tự động biết app nào đang dẫn đường.

## App trong các ô

**Ô màu đen với dòng "App này chặn chiếu màn hình".** App đó (thường là app ngân hàng, thanh toán, hoặc
tab ẩn danh của trình duyệt) cấm chụp màn hình, nên hệ thống hiện nó màu đen trong mọi màn hình ảo. Chọn
app khác cho ô đó.

**Một app cứ khởi động lại.** Táp Lô khởi động lại app bị dừng, tối đa 5 lần liên tiếp, rồi báo lỗi cho
ô đó. App có thể không hỗ trợ chạy trên màn hình thứ hai; thử nó một mình ở bố cục Toàn màn hình.

**App có viền đen hai bên hoặc không lấp đầy ô.** App chỉ hỗ trợ màn hình dọc (như trình phát YouTube
Shorts) được hiện đứng, có viền.

**Chữ quá nhỏ hoặc quá lớn.** Táp Lô chọn mật độ theo cỡ màn hình xe và cỡ ô. Đổi cho mọi ô ở Cài đặt ›
**Cỡ chữ và biểu tượng**.

**Các ô hiện "Tạm dừng khi điện thoại khoá".** Một số máy tắt hoặc làm đen màn hình ảo của Táp Lô khi
khoá máy (thấy trên Android 17 và một số máy Samsung chạy Android 16). App chạy tiếp khi mở khoá. Bật Cài
đặt › **Giữ app chạy khi tắt màn hình**: khi xe đang hiện Táp Lô, nút nguồn (hoặc hết thời gian chờ) sẽ
làm tối màn hình điện thoại thay vì tắt hẳn, nên app vẫn chạy. Bấm nút nguồn để dùng lại điện thoại; màn
hình khoá hiện như thường. Khi ngắt kết nối xe, điện thoại trở lại bình thường.

**Màn hình điện thoại cứ sáng khi một ô đang phát video.** Website đang phát video xin Android giữ màn
hình sáng, và Android áp dụng cho màn hình điện thoại. Táp Lô gỡ việc đó, trừ khi bật Cài đặt › **Cho
video giữ màn hình điện thoại sáng**.

**App dừng hoặc khởi động lại khi tắt màn hình.** Cho Táp Lô chạy nền: Cài đặt › Ứng dụng › Táp Lô › Pin
› Không hạn chế (Xiaomi: bật thêm Tự khởi động).

## App trên điện thoại

**Khung xem trước hiện "Đang hiển thị trên màn hình xe".** Khi xe đang hiện Táp Lô, khung xem trước trên
điện thoại tạm dừng; hãy dùng màn hình xe.
