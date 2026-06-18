# 🛒 PHÂN TÍCH DỮ LIỆU GIAO DỊCH TRÊN NỀN TẢNG INSTACART NHẰM TĂNG SỐ LƯỢNG SẢN PHẨM BÁN RA TRÊN MỖI ĐƠN HÀNG

![Instacart Data Analysis](https://img.shields.io/badge/Data_Analysis-Instacart-2ea44f?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-Dashboard-e97627?style=for-the-badge&logo=tableau&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

---

## 🎯 Mục tiêu dự án (Project Goal)
Phân tích hành vi mua sắm của khách hàng trên nền tảng Instacart nhằm:
- **Tăng số lượng sản phẩm trên mỗi đơn hàng** nhờ các chiến lược tối ưu.
- **Xác định các nhóm khách hàng** có hành vi tương đồng (Customer Segmentation).
- **Khám phá các sản phẩm thường được mua cùng nhau** thông qua Luật kết hợp (Association Rules).
- **Xây dựng hệ thống gợi ý sản phẩm** phục vụ chiến lược Cross-Selling và Upselling.
- **Hỗ trợ ra quyết định** dựa trên dữ liệu trong lĩnh vực bán lẻ và thương mại điện tử.

---

## 📊 Demo & Visualization

Dự án cung cấp cái nhìn chi tiết và trực quan về dữ liệu giao dịch cũng như việc triển khai thực tế thông qua Dashboard và Video Demo.

### 📈 Dashboard Tableau
Dự án cung cấp dashboard trực quan hóa dữ liệu giao dịch Instacart, hỗ trợ phân tích hành vi khách hàng, hiệu suất sản phẩm, phân khúc khách hàng và hệ thống gợi ý sản phẩm.

👉 **[Xem Tableau Dashboard tại đây](https://public.tableau.com/views/LeDienTuan_NguyenHoangDuy_BuiQuangHuy_DinhHoaiNam/Overview?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)**

### 🎥 Video Demo
Video trình bày toàn bộ quy trình thực hiện dự án: từ tổng quan dashboard phân tích, quá trình chạy mô hình phân cụm khách hàng đến cách thức hoạt động của hệ thống đề xuất sản phẩm trên nền tảng web.

👉 **[Xem Youtube Demo Video tại đây](https://youtu.be/ZpBSvvhYwZo)**

---

## 🏆 Kế hoạch & Kết quả đạt được (Project Deliverables)

- 🔍 **Exploratory Data Analysis (EDA):** Khám phá và xử lý dữ liệu từ tập dữ liệu Instacart.
- 📉 **Interactive Tableau Dashboard:** Xây dựng hệ thống báo cáo và Dashboard tương tác.
- 👥 **Customer Segmentation:** Phân cụm khách hàng sử dụng thuật toán **K-Means Clustering**.
- 🛒 **Association Rule Mining:** Khai phá luật kết hợp (Market Basket Analysis) với Apriori/FP-Growth.
- 💡 **Product Recommendation System:** Ứng dụng web hiển thị các đề xuất sản phẩm phù hợp.
- 📊 **Business Insights & Strategic Recommendations:** Đề xuất các báo cáo chiến lược kinh doanh.
- 📑 **Final Project Report:** Báo cáo tổng kết dự án.
- 💻 **Source Code & Demo Application:** Mã nguồn hoàn chỉnh kèm ứng dụng mô phỏng.

---

## ⚙️ Mô tả hệ thống và Cấu trúc dự án

Hệ thống được chia làm hai phần chính:
1. **Luật kết hợp (Association Rules):** Phân cụm khách hàng để giảm chi phí tính toán, sau đó tiến hành phân tích tập dữ liệu khách hàng & đơn hàng để khai phá các luật kết hợp nhằm tìm ra liên hệ giữa các sản phẩm.
2. **Recomendation Base:** Hệ thống web gợi ý ứng dụng các luật kết hợp đã được trích xuất để đưa ra các đề xuất sản phẩm phù hợp (Hỗ trợ Cross-Selling).

### 📂 Cấu trúc dự án (Project Structure)
```text
📦 Capstone 1
├── 📂 Luật kết hợp/           # Tiền xử lý, phân cụm và khai phá luật
│   ├── 📂 Data/               # Chứa dữ liệu đầu vào (orders, products, aisles...)
│   ├── 📂 Output/             # Chứa kết quả luật sinh ra dưới dạng CSV
│   ├── 📓 EDA.ipynb           # Notebook phân tích dữ liệu khám phá (EDA)
│   ├── 📓 Tien_Xu_Ly.ipynb    # Notebook làm sạch và xử lý dữ liệu
│   ├── 📓 Kmeans.ipynb        # Phân cụm khách hàng bằng K-Means
│   ├── 📓 AssociationRules.ipynb # Chạy thuật toán Apriori/FP-Growth khai phá luật
│   └── 📄 requirements.txt    # Các thư viện Python cần thiết
│
└── 📂 Recomendation base/     # Ứng dụng web hệ thống gợi ý
    ├── 📂 Rule/               # Chứa các file kết quả luật từ thư mục Output
    ├── 🐍 app.py              # File chạy ứng dụng web giao diện
    ├── 🐍 recommender.py      # Logic chính xử lý hệ thống gợi ý
    └── 📄 requirements.txt    # Các thư viện phụ thuộc cho Streamlit app
```

---

## 🚀 Hướng dẫn Cài đặt & Sử dụng (Installation & Usage)

### 1. Cài đặt môi trường
Mở terminal/cmd tại đường dẫn thư mục gốc. Dự án yêu cầu Python.

```bash
# Tạo và kích hoạt môi trường ảo
python -m venv .env

# Đối với MacOS/Linux
source .env/bin/activate       
# Đối với Windows
.\.env\Scripts\activate        
```

Sau đó, cài đặt các thư viện cần thiết cho từng phần:
```bash
# Cài đặt thư viện cho phần Luật kết hợp
pip install -r "Luật kết hợp/requirements.txt"

# Cài đặt thư viện cho phần Ứng dụng Gợi ý
pip install -r "Recomendation base/requirements.txt"
```

### 2. Hướng dẫn sử dụng
- **Phân tích & Khai phá dữ liệu:** Truy cập vào thư mục `Luật kết hợp/` và mở các file Jupyter Notebook (bắt đầu từ `Tien_Xu_Ly.ipynb`, `EDA.ipynb`...) để xem quy trình phân tích và khai phá tập luật.
- **Chạy ứng dụng Web Gợi ý (Demo):** Truy cập vào thư mục `Recomendation base/` và khởi chạy Streamlit:
  ```bash
  cd "Recomendation base"
  streamlit run app.py 
  ```

---

## 💾 Nguồn dữ liệu (Dataset)
**Instacart Online Grocery Shopping Dataset**  
Dữ liệu được lấy từ cuộc thi trên Kaggle: **[Instacart Market Basket Analysis](https://www.kaggle.com/c/instacart-market-basket-analysis)**.  
Dữ liệu được làm sạch và cung cấp các tập giao dịch trong quá khứ lưu trữ hành vi mua sắm hàng tạp hóa trực tuyến của khách hàng trên nền tảng Instacart.

---

## 👥 Nhóm thực hiện & Giảng viên hướng dẫn

### 👨‍🏫 Giảng viên hướng dẫn
- **TS. Lê Diên Tuấn**

### 🧑‍💻 Thành viên nhóm (Team Members)
- **Đinh Hoài Nam** (Email: hnamsflex@gmail.com)
- **Bùi Quang Huy**
- **Nguyễn Hoàng Duy**

---

## 📜 Giấy phép & Liên hệ (License/Contact)
Dự án được triển khai cho môn **Đề án thực hành 1**. Phân phối chủ yếu cho mục đích học tập và nghiên cứu.
