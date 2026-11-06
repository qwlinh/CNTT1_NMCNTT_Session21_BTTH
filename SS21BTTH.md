# (Bài tập tổng hợp) Hành Trình Xử Lý 1 Lỗi Cài Đặt Thật

## Vấn đề:

- Bạn vừa cài **Node.js** trên laptop **Windows 11** mới để chuẩn bị làm bài tập lập trình web. 

- Mở Terminal trong **VS Code**, bạn gõ `npm -v` để kiểm tra thì máy báo lỗi.

- Bạn quyết định tự xử lý theo đúng quy trình 4 bước trước khi nhờ trợ giảng

## Yêu cầu:

### **Phần 1 –** Googling đúng cách

1. Giải thích vì sao câu hỏi "văn nói" ở mục 3b khiến Google trả về kết quả kém chất lượng.

2. Bóc tách lỗi ở mục 3a theo **3 thành phần cốt lõi**:

3. Viết **3 câu truy vấn Google** tối ưu, mỗi câu dùng 1 toán tử khác nhau:
   
   - 1 câu giới hạn trong StackOverflow (`site:`)
   
   - 1 câu dùng ngoặc kép cho lỗi nguyên văn (`" "`)
   
   - 1 câu loại trừ các bài viết cũ không liên quan (`-`)

### **Phần 2 –** Thẩm định StackOverflow

1. So sánh Câu trả lời A và B ở mục 3c theo **3 tiêu chí thẩm định uy tín**:

2. Kết luận bạn áp dụng câu trả lời nào và giải thích vì sao **Câu trả lời B** là một **"bẫy" nguy hiểm** nếu áp dụng nhầm.

3. Theo **Quy trình 30 Giây Đọc lướt**, liệt kê đúng thứ tự các bước khi mở 1 trang StackOverflow mới (thay vì đọc dịch toàn bộ phần mô tả câu hỏi).

### **Phần 3 –** Hỏi AI đúng cách và nhận diện rủi ro

1. Lỗi vẫn còn sau khi làm theo Câu trả lời A (mục 3d). Viết 1 Prompt hoàn chỉnh theo **Công thức Prompt 3 Thành phần** (Ngữ cảnh – Lỗi Nguyên văn – Yêu cầu), có nêu rõ bạn **đã thử thêm PATH nhưng vẫn lỗi**.

2. Đọc câu trả lời của AI ở mục 3e. Áp dụng **3 Nguyên tắc An toàn Vàng** để chỉ ra: đây có phải câu trả lời an toàn để làm theo không? Vì sao?

3. Nếu là bạn, bạn sẽ **phản hồi/hỏi lại AI** như thế nào trước khi quyết định có chạy lệnh đó hay không?

**Phần 4** – Viết Bug Report chuẩn để nhờ hỗ trợ
Sau khi thử cả 3 bước trên vẫn chưa hết lỗi, bạn quyết định nhắn tin nhờ trợ giảng của lớp hỗ trợ.

1. Viết 1 tin nhắn kiểu "Tin nhắn Kém" (mù mờ, thiếu ngữ cảnh) như ví dụ đã học.

2. Viết lại thành 1 tin nhắn chuẩn, đầy đủ 4 mảnh ghép của Bug Reporting Framework:

3. Nêu đúng **phím tắt chụp màn hình trên Windows** đã học và **1 lưu ý bảo mật** khi đính kèm ảnh chụp.

## Cách làm:

**Phần 1**:

1. Câu hỏi văn nói quá dài, mang tính trò chuyện và không có từ khóa kỹ thuật cụ thể. Vì vậy, Google khó xác định chính xác vấn đề cần tìm kiếm và có thể trả về nhiều kết quả không liên quan.

2. 

| Thành phần | Nội dung |
|---|---|
| Tên phần mềm / Hệ điều hành | Node.js / Windows 11 |
| Mã lỗi nguyên văn | `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| Thao tác đang làm | Nhập lệnh `npm -v` trong Terminal của VS Code để kiểm tra phiên bản npm. |

3. Viết 3 câu truy vấn Google

1. Dùng site::

site:stackoverflow.com npm not recognized Windows 11

2. Dùng ngoặc kép " ":

"npm is not recognized as an internal or external command"

3. Dùng dấu -:

npm not recognized Windows 11 -Windows XP

**Phân 2**:

1. So sánh hai câu trả lời trên StackOverflow

| Tiêu chí | Câu trả lời A | Câu trả lời B |
|---|---|---|
| Vote và tích xanh | +186 vote, có tích xanh | +2 vote, không có tích xanh |
| Thời gian đăng bài | 2 năm trước | 9 năm trước |
| Tags | node.js, windows, npm | node.js, windows-xp |

2. 

- Em chọn câu trả lời A

- Câu trả lời B là bẫy nguy hiểm vì hướng dẫn cài lại driver mạng trên Windows XP, không liên quan đến lỗi npm trên Windows 11. Nếu làm theo sẽ mất thời gian và có thể gây ra lỗi khác.

Câu 3. Quy trình 30 giây đọc lướt

1. Xem số lượt bình chọn (Vote).

2. Kiểm tra câu trả lời có tích xanh hay không.

3. Xem thời gian đăng bài.

4. Kiểm tra các thẻ Tags.

5. Đọc nội dung câu trả lời và bình luận để đánh giá mức độ phù hợp.

**Phần 3**: Hỏi AI đúng cách và nhận diện rủi ro

1. Viết Prompt 3 Thành phần

a: Ngữ cảnh:

Em vừa cài Node.js trên laptop Windows 11 và sử dụng Terminal trong VS Code để kiểm tra phiên bản npm. Em đã thêm đường dẫn cài đặt Node.js vào biến môi trường PATH và mở Terminal mới nhưng lỗi vẫn xuất hiện.

b: Lỗi nguyên văn:

'npm' is not recognized as an internal or external command,
operable program or batch file.

c: Yêu cầu:

Hãy giải thích nguyên nhân và hướng dẫn cách kiểm tra, khắc phục lỗi từng bước bằng tiếng Việt đơn giản. Không đưa ra các lệnh có nguy cơ xóa dữ liệu hoặc làm hỏng Windows.

Câu 2. Đánh giá câu trả lời của AI
Theo em, đây là câu trả lời không an toàn và tuyệt đối không được thực hiện.

1. Lệnh được đề xuất có thể xóa các tệp quan trọng trong thư mục C:\Windows\System32.

2. AI đưa ra hướng dẫn nguy hiểm mà không có bằng chứng lỗi PATH liên quan đến thư mục này.

3. Không được chạy lệnh khi chưa hiểu rõ tác dụng và chưa kiểm tra độ an toàn.

3. Phản hồi và hỏi lại AI

Em sẽ hỏi lại AI:

"Tại sao lỗi npm không được nhận diện lại cần xóa các tệp trong System32? Lệnh này có thể gây hỏng Windows không? Hãy đưa ra cách kiểm tra biến PATH và khắc phục an toàn mà không xóa dữ liệu hệ thống."

**Phần 4**: Viết Bug Report chuẩn
1. Tin nhắn kém

"Thầy ơi máy em bị lỗi npm rồi, thầy xem giúp em với ạ."

2. Tin nhắn chuẩn theo 4 mảnh ghép

### Câu 2. Viết tin nhắn chuẩn theo Bug Reporting Framework 4 bước

| Mảnh ghép | Nội dung |
|---|---|
| Context | Em sử dụng laptop Windows 11, vừa cài Node.js và mở Terminal trong VS Code. |
| Expected | Khi nhập `npm -v`, máy sẽ hiển thị phiên bản npm. |
| Actual | Máy báo lỗi: `'npm' is not recognized as an internal or external command, operable program or batch file.` |
| Log & Screenshot | Em đã thêm đường dẫn Node.js vào PATH và mở Terminal mới nhưng lỗi vẫn còn. |

**Tin nhắn gửi trợ giảng:**

Thầy ơi, em vừa cài Node.js trên laptop Windows 11. Khi nhập lệnh `npm -v` trong Terminal của VS Code, máy báo lỗi không nhận diện được lệnh npm. Em đã thử thêm đường dẫn Node.js vào PATH và mở Terminal mới nhưng vẫn chưa khắc phục được. Em gửi kèm ảnh lỗi, mong thầy hướng dẫn giúp em. Em cảm ơn thầy ạ!

3. Phím tắt chụp màn hình và lưu ý bảo mật
-
- Phím tắt: Windows + Shift + S để chụp một vùng màn hình.
- Lưu ý bảo mật: Trước khi gửi ảnh, cần che hoặc xóa mật khẩu, API Key và các thông tin cá nhân nếu có.