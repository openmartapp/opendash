# Lệnh giọng nói

[English](../voice-commands.md) | **Tiếng Việt**

Chạm 🎤 trên màn hình xe rồi nói điều bạn muốn: "dừng lại", một bài hát cần phát, một nơi cần tới. Bộ
nhận dạng giọng nói của điện thoại (thường là của Google, cần có mạng) nghe câu nói, qua micro của xe
từ Android 13, hoặc micro của điện thoại với bản cũ hơn. Video tạm dừng trong lúc nghe. Màn hình xe hiện
câu đã nghe và việc Táp Lô làm, rồi quay về video.

Táp Lô không dùng Trợ lý Google của Android Auto cho việc này: Trợ lý chỉ chuyển yêu cầu tới app media
hoặc app dẫn đường mà nó tự chọn. Nếu dùng Trợ lý, hãy gọi tên Kênh Xe: "phát nhạc jazz trên Kênh Xe";
Kênh Xe chuyển câu tìm sang Táp Lô, và Táp Lô phát video đầu tiên tìm được.

## Cài đặt

Táp Lô › Cài đặt › **Lệnh giọng nói**:

- Công tắc bật hoặc tắt nút 🎤 trên màn hình xe.
- **Ngôn ngữ nhận dạng**: tiếng Việt (mặc định), tiếng Anh, hoặc **Khác** với mã ngôn ngữ BCP 47 như
  `fr-FR`. Mỗi ngôn ngữ có bộ lệnh riêng.
- **Sửa bộ lệnh**: các luật ở dưới, cho ngôn ngữ đang nhận dạng.
- **App chỉ đường**: **Tự động**, hoặc một app dẫn đường trên máy. Tự động chọn app đang dẫn đường,
  nếu không có thì app dùng lần trước, nếu không thì Google Maps. Táp Lô biết WazeMod đang dẫn đường khi
  WazeMod đã được kết nối làm nguồn tốc độ; với các app khác, hãy **Cho phép đọc thông báo dẫn đường**:
  Táp Lô chỉ xem các thông báo đang chạy, và với thông báo dẫn đường thì chỉ đọc đó là app nào và hướng
  rẽ kế tiếp (hiện trên xe, không lưu lại).
- **Cho phép dùng micro**, nếu lần đầu bạn chưa cho phép.
- **Cho hiển thị trên ứng dụng khác**: từ Android 14, app chạy nền không được mở app khác, mà Táp Lô chạy
  nền khi màn hình xe đang hiện nó. Có quyền này, Táp Lô hiện một cửa sổ trong suốt 1 điểm ảnh trong chốc
  lát để mở chỉ đường.

Chỉ đường mở trong app dẫn đường trên điện thoại, app đó đọc hướng dẫn qua loa xe. Màn hình xe vẫn hiện
Táp Lô (Android Auto chỉ hiện một app dẫn đường mỗi lúc), với hướng rẽ kế tiếp trên video. Với Cài đặt ›
**Màn hình xe** › **Chạy cùng Google Maps**, chỉ đường mở thẳng trong Google Maps trên màn xe (không cần
quyền hiển thị trên ứng dụng khác), nhạc vẫn phát.

**Khi app khác đang hiện trên màn xe** (Google Maps): nút giọng nói bạn đã chọn cho Táp Lô vẫn dùng được.
Táp Lô nghe mà không hiện lại trên màn xe: một thông báo ở trên cùng màn xe báo đang nghe, rồi báo đã nghe
gì và đã làm gì. Chỉ đường mở như trên. Lệnh nhạc thì đổi bài, nhưng video vẫn dừng dưới app kia trừ khi
bật Cài đặt › **Phát tiếp khi app khác che**. Trợ lý của
Android Auto cũng vậy: nói "chỉ đường đến …" khi Táp Lô đang trên màn hình xe thì chỉ đường cũng mở trong
app đó, kể cả ở bản miễn phí.

Khi điện thoại đang khoá:

- Màn hình chỉ tắt, khoá vuốt, hoặc Smart Lock đang tin cậy máy: chỉ đường bắt đầu ngay.
- Khoá bằng mã PIN, hình vẽ hoặc mật khẩu: Android không cho app dẫn đường chạy khi máy còn khoá. Xe báo
  điều đó trong vài giây, và chỉ đường bắt đầu ngay khi bạn mở khoá (trong vòng 5 phút). Hoặc mở Google
  Maps (hay Waze) trên xe rồi ra lệnh ở đó: app đó dẫn đường được khi máy vẫn khoá.
- Mẹo: bật Smart Lock (Cài đặt › Màn hình khoá › Smart Lock › Thiết bị tin cậy) với Bluetooth của xe, máy
  sẽ không khoá khi đang nối với xe, nên chỉ đường bắt đầu ngay.
- Với Cài đặt › **Màn hình xe** › **Chạy cùng Google Maps** thì không cần những điều trên: chỉ đường đi
  thẳng tới Google Maps trên màn xe, và Maps dẫn đường được khi máy vẫn khoá.

## Bộ lệnh

Lệnh là văn bản thường, mỗi dòng một lệnh:

```
hành_động: câu | câu | …
```

- `{text}` trong câu nhận phần được nói ở chỗ đó: tên bài hát, địa điểm. `youtube` và `navigate` cần
  `{text}` trong mọi câu; các hành động khác không được có.
- Câu không có `{text}` phải khớp cả câu nói.
- Khi nhiều câu cùng khớp, câu không có `{text}` thắng, rồi tới câu có nhiều chữ riêng nhất.
- Câu nói không khớp lệnh nào sẽ được tìm nguyên câu trên YouTube.
- Không phân biệt hoa thường, dấu câu, hay cách gõ dấu tiếng Việt.
- Dòng bắt đầu bằng `#` là ghi chú. Dòng Táp Lô không hiểu được liệt kê dưới ô soạn thảo và bị bỏ qua;
  các dòng khác vẫn chạy.

Các hành động (giữ nguyên tên tiếng Anh):

| Hành động | Làm gì |
| --- | --- |
| `youtube {text}` | Tìm trên YouTube và phát video đầu tiên |
| `navigate {text}` | Chỉ đường tới nơi đó, trong app chỉ đường |
| `play`, `pause` | Phát hoặc tạm dừng video |
| `next`, `previous` | Video tiếp theo hoặc video trước |
| `forward`, `rewind` | Tua tới hoặc lùi trong video |

Ví dụ, một phần bộ lệnh tiếng Việt có sẵn:

```
# Giữ những chữ giúp tìm kiếm: "mở nhạc sến" sẽ tìm "nhạc sến".
pause: dừng | dừng lại | tạm dừng | tắt nhạc
play: tiếp tục | phát tiếp | phát
next: bài tiếp | bài tiếp theo | qua bài | bỏ qua
previous: bài trước | video trước | quay lại bài trước
forward: tua tới | tua nhanh
rewind: tua lại | lùi lại
navigate: chỉ đường đến {text} | đường đi tới {text} | dẫn đường tới {text} | đưa tôi về {text}
youtube: mở {text} | phát {text} | nghe {text} | {text} trên youtube
```

Dưới ô soạn thảo, **Thử một câu** cho biết một câu sẽ làm gì với bộ lệnh đang có trong ô, dù đã lưu hay
chưa. **Lưu** giữ bộ lệnh cho lần nói sau; **Khôi phục mặc định** quay về bộ lệnh có sẵn của Táp Lô.

## Góp bộ lệnh cho một ngôn ngữ

Bộ lệnh có sẵn của Táp Lô là các file trong `app/src/main/assets/voice/`, đặt tên theo ngôn ngữ
(`vi.txt` dùng cho `vi-VN` và mọi biến thể tiếng Việt). Hiện có tiếng Việt (`vi.txt`) và tiếng Anh
(`en.txt`). Với ngôn ngữ khác, bộ lệnh ban đầu trống và mọi câu nói được tìm trên YouTube cho tới khi
bạn thêm lệnh. Muốn chia sẻ bộ lệnh cho ngôn ngữ của bạn, thêm một file vào đó qua pull request.
