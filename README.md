# Dự án Phát Hiện Đối Tượng bằng OpenCV 🇻🇳

## 📖 Giới thiệu

Dự án này sử dụng thư viện **OpenCV** để phát hiện và định vị các đối tượng (templates) trong một hình ảnh lớn bằng hai phương pháp chính:

1. **SIFT + Homography**: Phát hiện đặc trưng và xử lý biến dạng phức tạp.
2. **Template Matching**: So sánh trực tiếp với khả năng thay đổi tỷ lệ.

Mục tiêu là tìm kiếm và đánh dấu vị trí của các đối tượng trong ảnh bằng cách vẽ hình chữ nhật bao quanh.

---

## 🚀 Cài đặt

### Yêu cầu

- **Python 3.x** 🐍
- Các thư viện:
  - `opencv-python` (cv2)
  - `matplotlib`
  - `numpy`
  - `imutils`

### Hướng dẫn cài đặt

1. Cài đặt Python nếu chưa có: [Tải Python](https://www.python.org/downloads/).
2. Cài đặt các thư viện bằng pip:
   ```bash
   pip install opencv-python matplotlib numpy imutils
   ```

---

## 📂 Cấu trúc thư mục

```
project/
│
├── finding/               # Thư mục chứa tất cả các ảnh
│   └── data               # Chứa các ảnh templates
│   └── cut_2.png          # Ảnh lớn để tìm kiếm đối tượng
├── report                 # Báo cáo dự án
└── find_object.ipynb      # File code dự án
```

---

## Kết quả:

- **Phương pháp SIFT**: Hiển thị hình chữ nhật xanh lá cây 🌿 bao quanh khu vực khớp.
- **Phương pháp Template Matching**: Hiển thị hình chữ nhật xanh da trời bao quanh khu vực khớp.

---

## 📈 Các phương pháp

### 1. SIFT + Homography 🔍

- Phát hiện đặc trưng bằng thuật toán SIFT.
- Tính ma trận Homography để xử lý xoay, thay đổi tỷ lệ, và biến dạng phối cảnh.
- **Ưu điểm**: Linh hoạt với các biến dạng phức tạp.
- **Nhược điểm**: Yêu cầu đủ đặc trưng để khớp.

### 2. Template Matching 📏

- So sánh trực tiếp ảnh mẫu với ảnh lớn ở nhiều tỷ lệ khác nhau.
- **Ưu điểm**: Đơn giản, nhanh chóng.
- **Nhược điểm**: Không xử lý tốt xoay hoặc biến dạng.

---

## 🎨 Kết quả minh họa

- **SIFT**: Hình chữ nhật xanh lá cây 🌿
- **Template Matching**: Hình chữ nhật đỏ ❤️

---

## 📜 Giấy phép

Dự án được phát hành dưới giấy phép **MIT**. Xem chi tiết tại [LICENSE](LICENSE).

---

## 🤝 Đóng góp

Mọi ý kiến đóng góp đều được hoan nghênh! Hãy tạo **Issue** hoặc **Pull Request** trên repository này. ⭐

---

**Cảm ơn bạn đã quan tâm đến dự án!** 😊
