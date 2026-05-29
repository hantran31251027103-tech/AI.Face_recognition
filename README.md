# AI.Face_recognition
Dự án này sử dụng mạng nơ-ron tích chập (CNN) được xây dựng từ đầu (scratch) để nhận diện khuôn mặt thông qua hình ảnh. Mô hình được tối ưu hóa để phát hiện và phân biệt các đặc trưng quan trọng trên khuôn mặt như mắt, mũi, miệng và cấu trúc khuôn mặt nhằm tăng độ chính xác trong quá trình nhận diện.

## Tải Xuống Mô Hình Pre-trained

Do giới hạn dung lượng file trên GitHub, file trọng số mô hình `.h5` được lưu trữ tại Google Drive. Bạn có thể tải về để sử dụng ngay mà không cần huấn luyện lại:

👉 https://drive.google.com/file/d/1KUKO3fGTSNk6hRNZrve5xvq0UOOl4Uqs/view?usp=drive_link

## 📂 Cấu Trúc Thư Mục Dự Án

* face_recognition.ipynb: File Google Colab chứa toàn bộ mã nguồn từ xử lý dữ liệu đến huấn luyện mô hình.
* test: Thư mục chứa các hình ảnh khuôn mặt thực tế dùng để kiểm thử (Test).
* README.md: Hướng dẫn và thông tin dự án.

## 🛠️ Cách Chạy Mô Hình

Bạn có thể nạp lại mô hình trong môi trường Python/Colab bằng lệnh sau:

```python 
from tensorflow.keras.models import load_model

# Load model từ file đã tải về
model = load_model('face_recognition.h5')

# Dự đoán ảnh mới
# predictions = model.predict(img_prepared)

print("✅ Mô hình nhận diện khuôn mặt đã sẵn sàng!")
```
