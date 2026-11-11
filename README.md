# Nhật ký thói quen

App theo dõi thói quen hằng ngày. Chỉ gồm vài file tĩnh, không cần server hay cơ sở dữ liệu.

- Đánh dấu thói quen theo tuần, xem chuỗi ngày liên tiếp, tỉ lệ 30 ngày và lịch 18 tuần
- Cài được lên màn hình chính điện thoại (PWA), chạy cả khi không có mạng
- Dữ liệu lưu trên trình duyệt của từng máy, có nút xuất/nhập file sao lưu

## Đưa lên GitHub Pages

1. Tạo repository mới trên GitHub, ví dụ `habit-tracker` (chọn Public).
2. Tải tất cả file trong thư mục này lên repo (Add file → Upload files), rồi Commit.
3. Vào **Settings → Pages**. Ở mục *Source* chọn **Deploy from a branch**, chọn nhánh `main`, thư mục `/ (root)`, rồi Save.
4. Đợi khoảng 1–2 phút, app sẽ có ở `https://<tên-tài-khoản>.github.io/habit-tracker/`.

## Cài lên điện thoại

- **iPhone (Safari):** mở link → nút Chia sẻ → *Thêm vào MH chính*.
- **Android (Chrome):** mở link → menu ⋮ → *Cài đặt ứng dụng* (hoặc *Thêm vào màn hình chính*).

## Lưu ý về dữ liệu

Dữ liệu nằm trong trình duyệt của từng thiết bị, không tự đồng bộ giữa điện thoại và máy tính.
Muốn chuyển máy: bấm **Xuất file sao lưu** ở máy cũ, rồi **Nhập từ file** ở máy mới.
Xoá dữ liệu duyệt web hoặc gỡ app sẽ làm mất dữ liệu, nên hãy sao lưu định kỳ.

## Cập nhật app

Khi sửa file, đổi `CACHE = 'thoi-quen-v1'` trong `sw.js` thành `v2`, `v3`… để điện thoại tải bản mới.
