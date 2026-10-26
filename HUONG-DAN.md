# Sổ chi tiêu cho iPhone

Bản này chạy hoàn toàn trong iPhone: dữ liệu lưu ngay trong điện thoại, dùng được cả khi không có mạng,
không cần máy tính hay máy chủ. Máy chủ web chỉ dùng để "giao" app cho điện thoại một lần, không bao giờ nhận dữ liệu của bạn.

## Bước 1. Đưa app lên một địa chỉ https (làm một lần)

iPhone chỉ cho cài app web khi nó nằm ở địa chỉ https, nên cần đăng thư mục này lên một nơi miễn phí.
Chọn một trong hai cách (giao diện các trang này có thể thay đổi đôi chút theo thời gian):

**Cách A: Netlify (đơn giản nhất)**
1. Giải nén file zip. Vào https://app.netlify.com/drop và đăng ký tài khoản miễn phí nếu được hỏi.
2. Kéo cả thư mục `so-chi-tieu-iphone` thả vào trang. Netlify trả về một địa chỉ dạng `https://tên-ngẫu-nhiên.netlify.app`.
3. Đăng nhập tài khoản để giữ lại trang (trang thả khi chưa có tài khoản có thể bị xóa sau một thời gian ngắn).
4. Có thể đổi tên địa chỉ ở Site configuration > Change site name.

**Cách B: GitHub Pages**
1. Tạo tài khoản và một repository mới ở https://github.com (để chế độ Public).
2. Bấm Add file > Upload files, tải lên TOÀN BỘ file trong thư mục này (không phải cả thư mục bọc ngoài), rồi Commit.
3. Vào Settings > Pages, ở Branch chọn `main` và thư mục `/ (root)`, bấm Save.
4. Sau 1 đến 2 phút, địa chỉ là `https://tên-bạn.github.io/tên-repository/`.

Địa chỉ này công khai, nhưng chỉ chứa mã của app, không chứa dữ liệu của bạn.
Ai biết địa chỉ cũng mở được app, nhưng họ chỉ thấy một sổ trống trong máy của họ.

## Bước 2. Cài lên màn hình chính iPhone

1. Mở **Safari** (không dùng Chrome) và vào địa chỉ ở bước 1.
2. Bấm nút Chia sẻ (ô vuông có mũi tên lên), kéo xuống chọn **Thêm vào Màn hình chính**, rồi bấm **Thêm**.
3. Từ giờ mở app bằng biểu tượng quyển sổ trên màn hình chính, nó chạy toàn màn hình như app thật.

Quan trọng: dữ liệu trong Safari và dữ liệu trong app đã cài là hai nơi riêng.
Hãy nhập và dùng dữ liệu trong app đã cài, đừng nhập thử ở Safari trước rồi mong nó tự chuyển sang.

## Bước 3. Chuyển dữ liệu đang có trên máy tính sang (nếu cần)

1. Trên máy tính (bản cũ đã cập nhật): vào mục Danh mục, bấm **Xuất dữ liệu để chuyển sang iPhone (.json)**.
2. Gửi file `.json` đó sang iPhone bằng AirDrop, iCloud Drive, Zalo, email, v.v. và lưu vào ứng dụng Tệp.
3. Trong app trên iPhone: mục Danh mục > **Khôi phục từ file**, chọn file vừa gửi. Lưu ý thao tác này thay thế toàn bộ dữ liệu đang có trong điện thoại.

## Sao lưu (rất nên làm)

Dữ liệu nằm trong bộ nhớ của app trên điện thoại. Gỡ app, xóa dữ liệu trang web của Safari hoặc đổi máy sẽ làm mất dữ liệu.
Hãy vào Danh mục > **Sao lưu dữ liệu** để lưu một file `.json` vào ứng dụng Tệp hoặc iCloud, ví dụ mỗi tuần một lần.
Khôi phục bằng nút **Khôi phục từ file** ngay bên cạnh.

## Xuất Excel

Mục Thống kê > **Xuất Excel**: iPhone mở bảng Chia sẻ, bạn chọn **Lưu vào Tệp** hoặc mở thẳng bằng Excel/Numbers.

## Cập nhật app về sau

Đăng lại các file mới lên cùng địa chỉ (Netlify: Deploys > kéo thả lại; GitHub: tải file mới lên đè).
App tự lấy bản mới khi mở lại lúc có mạng. Dữ liệu của bạn không bị ảnh hưởng.

## Yêu cầu

iPhone dùng iOS 16.2 trở lên là tốt nhất (iPhone 13 cập nhật được). Bản cũ hơn vẫn chạy nhưng một số màu nền có thể hiển thị đơn giản hơn.
