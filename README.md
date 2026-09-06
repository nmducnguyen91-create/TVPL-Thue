# TVPL Thuế — Thư viện Pháp luật Thuế 2025–2026

Trang tra cứu & học tập tĩnh: Luật Quản lý thuế 108/2025/QH15 cùng toàn bộ nghị
định, thông tư và văn bản hợp nhất hướng dẫn (hiệu lực 01/7/2026).
11 văn bản · 509 điều toàn văn · chuyên đề Hóa đơn điện tử (điểm mới, hỏi–đáp).

## Cấu trúc

```
index.html        ← trang chính
support.js        ← runtime (bắt buộc, cùng thư mục index.html)
vendor/           ← React, ReactDOM, Babel (nhúng sẵn — KHÔNG phụ thuộc CDN ngoài)
data/index.js     ← danh mục 11 văn bản
data/hddt.js      ← chuyên đề hóa đơn điện tử
data/docs/*.js    ← toàn văn từng văn bản (nạp khi mở)
```

Các thư viện React/Babel đã được đặt trong `vendor/` và trang tự nạp từ đó, nên
**không cần Internet tới CDN ngoài** — chạy ổn định kể cả khi mạng chặn unpkg.

## GitHub Pages

Settings → Pages → *Deploy from a branch* → branch `main`, thư mục `/ (root)` → Save.
Địa chỉ: `https://<tài-khoản>.github.io/<tên-repo>/`

## Ghi chú

- Phải chạy qua http/https (GitHub Pages là đủ); mở bằng `file://` có thể không chạy.
- Tab **Nguồn văn bản**: thêm/sửa danh mục, lưu trong localStorage của máy; có
  **Xuất/Nhập .json** để đồng bộ giữa các máy. Không đổi bản gốc.
