Bước 1: Load Dataset

Bước 2: Feature extraction

- Không có đủ kiến thức để ứng dụng feature vô trong mô hình phân loại.
- Giả thiết của chúng em:
+ Data Segmentation: Cắt đoạn dữ liệu thành từng đoạn nhỏ ngẫu nhiên theo chiều ngang và theo nhóm để code có thể chạy được.
+ So sánh độ biến thiên của các dữ liệu: Acc, Mag, Gyro. Để đưa ra đánh giá sơ bộ cho việc phân loại.
+ Vẽ đồ thị FFT (với timeseries là chiều ngang của dataframe).
+ So sánh độ biến thiên: Vẽ boxplot để đưa ra góc nhìn sơ bộ về thống kê mô tả của từng label.
+ Đánh giá label: Dựa trên boxplot, chúng em sẽ đánh giá các label thành các hành động tương ứng theo bảng sau.

![Uploading image.png…]()


Bước 3: Sử dụng model Classification để phân loại.
Sử dụng model CatBoost để phân loại label và tự động gắn nhãn hành động với label tương ứng.

Bước 4: show kết quả.
