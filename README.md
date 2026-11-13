# Vòng chung kết – Thử thách lật 8 ô

Website tĩnh, chạy trực tiếp trên GitHub Pages.

## Đăng lên GitHub Pages
1. Tạo repository mới trên GitHub (ví dụ `lat-8-o`).
2. Upload **toàn bộ nội dung** thư mục này (gồm `index.html`, thư mục `assets`, `.nojekyll`) lên nhánh `main`.
3. Vào **Settings → Pages**, mục *Build and deployment* chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)` rồi Save.
4. Sau 1–2 phút, trang chạy tại `https://<tên-github>.github.io/<tên-repo>/`.

## Thay hình ảnh / logo
Thay file cùng tên trong thư mục `assets/` (giữ đúng tên):
- `anh-01.jpg` … `anh-08.jpg`: hình của ô 01–08 (nên là JPG, rộng tối đa 1920px).
- `logo-1.png`, `logo-2.png`, `logo-3.png`: cụm logo theo thứ tự trái → phải.

## Admin
- Bấm biểu tượng ⚙ mờ ở góc dưới bên phải màn hình.
- Mật khẩu mặc định: `betma2026` (nên đổi: tạo mã SHA-256 của mật khẩu mới rồi thay giá trị `PW_HASH` trong `index.html`).
- Chức năng: xem số ô đã mở/chưa mở và **RESET GAME**.

## Lưu ý quan trọng
- Trạng thái các ô lưu trong **trình duyệt của máy đang chiếu** (localStorage): refresh không mất, các tab cùng trình duyệt tự đồng bộ. **Không đồng bộ giữa các thiết bị khác nhau** – hãy dùng một máy duy nhất để điều khiển và trình chiếu.
- Mật khẩu Admin kiểm tra ngay trên trình duyệt nên chỉ ngăn thao tác nhầm, không phải bảo mật cao. Cần đồng bộ nhiều thiết bị thật sự thì phải dùng thêm backend (Supabase/Firebase).
