# Thư viện Pháp luật Thuế 2025–2026

Trang tra cứu & học tập tĩnh (HTML thuần, không cần server, không cần Firebase).

## Cách up lên GitHub Pages

1. Tạo repo mới, giải nén và đẩy **toàn bộ** các file sau lên nhánh `main`:

```
index.html          ← trang chính (bản copy để chạy trên web)
support.js          ← runtime, bắt buộc
data/index.js       ← danh mục 11 văn bản (nhẹ, nạp ngay)
data/docs/*.js      ← toàn văn từng văn bản (nạp khi mở)
data/hddt.js        ← chuyên đề hóa đơn điện tử (điểm mới, hỏi–đáp)
```

2. Vào **Settings → Pages**, chọn `Deploy from a branch` → branch `main`, folder `/ (root)` → Save.
3. Vài phút sau truy cập `https://<tên-tài-khoản>.github.io/<tên-repo>/`.

## Lưu ý

- Phải chạy qua http/https (GitHub Pages là đủ). Mở trực tiếp bằng `file://` sẽ không nạp được dữ liệu.
- Không cần Firebase: toàn văn nằm trong `data/`, phần "Nguồn văn bản" người dùng sửa được và lưu trong localStorage của chính máy họ. Chỉ cần Firebase nếu muốn nhiều người sửa và thấy chung một bản cập nhật.
- Chia sẻ bản cập nhật giữa các máy: tab **Nguồn văn bản → Xuất cập nhật (.json)**, máy khác dùng **Nhập từ .json**.
- File `Thư viện Pháp luật Thuế.dc.html` là bản gốc để tiếp tục sửa thiết kế; `index.html` là bản copy dùng cho hosting. Sửa bản gốc thì copy lại thành `index.html`.
