
# Heart Disease Data Analysis

Dự án phân tích dữ liệu bệnh tim sử dụng Python, bao gồm làm sạch dữ liệu, xử lý giá trị thiếu (MICE), phân tích khám phá dữ liệu (EDA), feature engineering và xây dựng mô hình Machine Learning.

## 📋 Mục lục

- [Giới thiệu](#giới-thiệu)
- [Tính năng](#tính-năng)
- [Cài đặt](#cài-đặt)
- [Cách sử dụng](#cách-sử-dụng)
- [Cấu trúc dự án](#cấu-trúc-dự-án)
- [Kết quả](#kết-quả)

## 🎯 Giới thiệu

Dự án này thực hiện phân tích toàn diện trên bộ dữ liệu `heart_disease.csv` nhằm:
- Khám phá và hiểu các yếu tố liên quan đến bệnh tim
- Xây dựng mô hình dự đoán nguy cơ mắc bệnh tim
- Trực quan hóa dữ liệu để rút ra insights

## ✨ Tính năng

- **Data Cleaning**: Loại bỏ dữ liệu trùng lặp
- **Missing Value Imputation**: Xử lý giá trị thiếu bằng phương pháp MICE (Multiple Imputation by Chained Equations)
- **Outlier Detection**: Phát hiện outliers sử dụng phương pháp IQR
- **EDA**: Phân tích khám phá dữ liệu với các biểu đồ:
  - Pie Chart: Phân bố bệnh tim
  - Histogram: Phân bố BMI
  - Bar Chart: Tình trạng hút thuốc
  - Box Plot: BMI theo tình trạng bệnh tim
  - Scatter Plot: BMI vs Physical Health
  - Correlation Matrix
- **Feature Engineering**: One-Hot Encoding và Standard Scaling
- **Machine Learning**: Random Forest Classifier

## 🛠️ Cài đặt

### Yêu cầu hệ thống

- Python 3.8+
- Jupyter Notebook hoặc VS Code với extension Jupyter

### Cài đặt thư viện

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

Hoặc cài đặt từ requirements file:

```bash
pip install -r requirements.txt
```

### Tạo file requirements.txt (nếu chưa có)

```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=1.0.0
```

## 🚀 Cách sử dụng

1. **Clone repository**
   ```bash
   git clone <repository-url>
   cd Project
   ```

2. **Chuẩn bị dữ liệu**
   - Đảm bảo file `heart_disease.csv` nằm trong thư mục dự án

3. **Chạy notebook**
   - Mở file `analysis.ipynb` bằng Jupyter Notebook hoặc VS Code
   - Chạy các cells theo thứ tự từ trên xuống dưới

## 📁 Cấu trúc dự án

```
Project/
├── README.md              # File hướng dẫn
├── analysis.ipynb         # Notebook phân tích chính
├── heart_disease.csv      # Dữ liệu đầu vào
├── requirements.txt       # Danh sách thư viện
└── output/                # Thư mục chứa kết quả xuất ra
```

## 📊 Kết quả

Sau khi chạy notebook, bạn sẽ có:

1. **Báo cáo thống kê**: Thông tin về dữ liệu, missing values, outliers
2. **Biểu đồ trực quan**: Các chart được hiển thị trong notebook
3. **Mô hình ML**: Random Forest model với đánh giá performance
4. **Feature Importance**: Xếp hạng các đặc trưng quan trọng

## 📝 Ghi chú

- Nếu không có missing values trong dữ liệu, chương trình sẽ tự động tạo 1% missing data để demo phương pháp MICE


