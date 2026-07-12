<div align="center">

# 🚀 ColabDrive Downloader & Merger

**Công cụ đa năng tải video từ mọi nguồn (Drive, YouTube, OK.ru, VK, Facebook, TikTok, Torrent/Magnet, m3u8, mpd) trực tiếp vào Google Drive và hỗ trợ ghép nối video/phân mảnh tốc độ cao bằng Google Colab.**

![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?logo=googlecolab&logoColor=white)
![yt-dlp](https://img.shields.io/badge/yt--dlp-FF0000?logo=youtube&logoColor=white)
![ffmpeg](https://img.shields.io/badge/FFmpeg-007800?logo=ffmpeg&logoColor=white)

🌐 **[Mở trong Colab](https://colab.research.google.com/github/huyvu2512/ColabDrive_Downloader/blob/main/ColabDrive_Downloader.ipynb)** · 📦 **[GitHub](https://github.com/huyvu2512/ColabDrive_Downloader)**

</div>

---

## ✨ Tính năng nổi bật

| Tính năng | Mô tả |
|---|---|
| 🌍 **Tải video đa nguồn** | Hỗ trợ YouTube, Facebook, TikTok, OK.ru, VK, **Link Torrent/Magnet**, direct link `.mp4`, luồng trực tiếp `.m3u8` và `.mpd`. |
| 🚀 **Tốc độ cực nhanh** | Tải và đồng bộ trực tiếp lên Google Drive qua băng thông siêu tốc của máy chủ Google (Lên tới 50-100MB/s). |
| 💾 **Đồng bộ Google Drive** | Lưu trữ trực tiếp vào Drive cá nhân để tránh mất dữ liệu khi ngắt kết nối Colab. |
| 🧩 **Tải & Ghép phân mảnh (.m4s, .ts...)** | Tải song song đa luồng các phân mảnh video từ link trần, tự động gộp nhị phân và remux bằng FFmpeg để sửa lỗi timeline giúp tua mượt mà. |
| 📺 **Quay ngược thời gian Live IPTV (Catchup)** | Tự động tính toán múi giờ và chèn tham số quay ngược thời gian (như `startTime`/`stopTime` của Seenow/VTV Prime) để tải lại các chương trình đã phát sóng trước đó. |
| 🎬 **Ghép nhiều video sẵn có** | Hỗ trợ ghép hàng loạt video trong thư mục hoặc theo danh sách chỉ định với 2 chế độ: **Ghép siêu tốc (copy stream)** hoặc **Ghép chất lượng (re-encode sang 1080p)**. |
| 🎨 **Giao diện thân thiện** | Giao diện Form gọn gàng, Việt hóa 100%, ẩn code phức tạp. |

---

## 🖥️ Hướng dẫn sử dụng nhanh

> **Chạy ngay trên trình duyệt:** [👉 BẤM VÀO ĐÂY ĐỂ MỞ TRÊN GOOGLE COLAB](https://colab.research.google.com/github/huyvu2512/ColabDrive_Downloader/blob/main/ColabDrive_Downloader.ipynb)

### Các bước thực hiện:
1. **Mở Colab:** Bấm vào link trên hoặc tải tệp `.ipynb` lên sổ tay Google Colab của bạn.
2. **Cài đặt thư viện:** Chạy **Bước 1** để chuẩn bị môi trường (`yt-dlp`, `ffmpeg`, `aria2`).
3. **Kết nối Google Drive:** Chạy **Bước 2** để liên kết tài khoản Drive lưu trữ.
4. **Tải và xử lý:**
   - **Tải link đơn lẻ:** Dán link (YouTube, Facebook, Torrent, hoặc link xem lại `.mpd`/`.m3u8` đã bắt được) vào ô cấu hình ở **Bước 3**.
   - **Tải danh sách link phân mảnh (.m4s, .ts):** Dán danh sách link và tệp khởi tạo (init) vào **Bước 4**.
   - **Tải chương trình xem lại từ kênh Live:** Nhập link Live gốc và chọn mốc giờ phát sóng (giờ Việt Nam) ở **Bước 5**.
   - **Ghép nối video:** Thiết lập thư mục hoặc danh sách file cần ghép ở **Bước 6**.

---

## 🏗️ Cấu trúc thư mục

```
ColabDrive_Downloader/
├── ColabDrive_Downloader.ipynb  # Sổ tay Jupyter chính chạy trên Google Colab
├── README.md                    # Tài liệu hướng dẫn sử dụng (File bạn đang xem)
├── LICENSE                      # Giấy phép phần mềm (MIT)
└── .gitignore                   # Cấu hình bỏ qua các tệp không cần thiết
```

---

## 📄 Giấy phép

Dự án được phân phối theo giấy phép **MIT**. Xem chi tiết tại [LICENSE](LICENSE).
