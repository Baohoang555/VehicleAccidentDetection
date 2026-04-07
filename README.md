# 🚗 Road Accident Detection System from CCTV Footages

Hệ thống phát hiện tai nạn giao thông tự động dựa trên thị giác máy tính (Computer Vision) và học sâu (Deep Learning), sử dụng dữ liệu từ camera giám sát (CCTV).

## 📌 Tổng quan dự án
Dự án tập trung vào việc giám sát luồng giao thông theo thời gian thực, nhận diện các loại phương tiện và tự động đưa ra cảnh báo khi phát hiện các hành vi bất thường dẫn đến tai nạn (va chạm, phanh gấp, lệch quỹ đạo).

## 🛠 Công nghệ sử dụng
* **Ngôn ngữ:** Python
* **Object Detection:** YOLOv8 (Ultralytics)
* **Deep Learning:** TensorFlow/Keras & PyTorch
* **Computer Vision:** OpenCV (Phân tích Optical Flow & Quỹ đạo)
* **Data Analysis:** Pandas, NumPy, Scikit-learn
* **Visualization:** Matplotlib, Seaborn

## 🚀 Các tính năng chính
1. **Theo dõi phương tiện (Vehicle Tracking):** Sử dụng `AdvancedVehicleTracker` để định danh và lưu trữ lịch sử di chuyển của từng xe qua các khung hình.
2. **Đánh giá rủi ro đa tầng (Multi-factor Risk Assessment):**
    * **Tốc độ:** Phát hiện giảm tốc đột ngột (Sudden deceleration).
    * **Hướng di chuyển:** Phát hiện các góc bẻ lái bất thường hoặc mất kiểm soát.
    * **Khoảng cách:** Cảnh báo khi các phương tiện quá gần nhau (Proximity Monitoring).
3. **Mô hình AI chuyên biệt:** Kết hợp YOLOv8 để trích xuất đặc trưng và một mạng Neural Network để phân loại trạng thái tai nạn.
4. **Dashboard báo cáo:** Trực quan hóa độ chính xác, tỷ lệ lỗi (False Positive/Negative) và tốc độ xử lý (FPS).

## 📂 Cấu trúc Dataset
Dữ liệu được sử dụng từ bộ dataset [Road Accidents from CCTV Footages](https://www.kaggle.com/datasets/suryaprabhakaran2005/road-accidents-from-cctv-footages-dataset) với hơn 27,000 hình ảnh:
* `Accident/`: Hình ảnh hiện trường va chạm thực tế.
* `NonAccident/`: Hình ảnh giao thông bình thường.
* `SeverityScore/`: Nhãn đánh giá mức độ nghiêm trọng từ 1 đến 3.

## 📊 Hiệu suất hệ thống
Dựa trên kết quả thực nghiệm:
* **Độ chính xác nhận diện phương tiện:** 89.0%
* **Độ chính xác phát hiện tai nạn (Precision):** 82.0%
* **Tốc độ xử lý trung bình:** 45.6 FPS (Đáp ứng yêu cầu Real-time).
* **Điểm hệ thống tổng thể:** 84.9%

## ⚙️ Hướng dẫn cài đặt

### 1. Clone project
```bash
git clone [https://github.com/hoangbao/accident-detection-system.git](https://github.com/hoangbao/accident-detection-system.git)
cd accident-detection-system

### 2. Cài đặt thư viện
pip install ultralytics tensorflow opencv-python pandas seaborn scikit-learn python-dotenv
## 3. Cấu hình môi trường
KAGGLE_USERNAME=your_username
KAGGLE_API_KEY=your_api_key
## 4. Sử dụngPythonfrom main import process_accident_video
# Phân tích video và xuất kết quả
'''
💡Tác giả: Hoàng Bảo 

