# Đồ án IE105 - Tìm hiểu cách tấn công trình tổng hợp mô hình học liên kết
# 📌 Giới thiệu

Dự án này tập trung vào việc nghiên cứu và triển khai phương pháp Tấn công Suy luận Thành viên (Membership Inference Attack - MIA) trong môi trường Học Liên kết (Federated Learning - FL), cụ thể là phương pháp FedMIA. Phương pháp này khai thác nguyên lý "All for One", sử dụng thông tin từ tất cả các khách hàng (client) để tăng hiệu quả tấn công.

# 🗂️ Cấu trúc Dự án

├── experiments/                  # Thư mục chứa các tập lệnh thực nghiệm và kết quả

├── models/                       # Thư mục chứa định nghĩa các mô hình học máy

├── utils/                        # Thư mục chứa các hàm tiện ích hỗ trợ

├── dataset.py                    # Tập lệnh xử lý và tải dữ liệu

├── _federated_learning.py        # Tập lệnh triển khai học liên kết

├── _fed_membership_attack.py     # Tập lệnh triển khai tấn công FedMIA

├── 1_run_federated_learning.sh   # Tập lệnh shell chạy học liên kết

├── 2_run_fed_membership_attack.sh# Tập lệnh shell chạy tấn công FedMIA

├── requirements.txt              # Danh sách các thư viện phụ thuộc

└── README.md                     # Tập tin hướng dẫn (tập tin này)

# ⚙️ Cài đặt

## 1. Tạo môi trường ảo (Tuỳ chọn)

python3 -m venv venv
source venv/bin/activate

## 2. Cài đặt Thư viện Phụ thuộc

pip install -r requirements.txt

Lưu ý: Dự án yêu cầu Python 3.8 hoặc cao hơn.

# 🚀 Hướng dẫn Sử dụng

## 1. Huấn luyện Mô hình Học Liên kết

Chạy lệnh sau để bắt đầu quá trình huấn luyện mô hình FL:

bash 1_run_federated_learning.sh

## 2. Thực hiện Tấn công FedMIA

Sau khi huấn luyện xong mô hình FL, chạy lệnh sau để thực hiện tấn công suy luận thành viên:

bash 2_run_fed_membership_attack.sh

# 🧪 Kết quả

Kết quả của quá trình huấn luyện và tấn công sẽ được lưu trong thư mục experiments/. Bạn có thể tìm thấy các biểu đồ, số liệu và mô hình đã được huấn luyện tại đây.

# 📚 Tài liệu Tham khảo

FedMIA: An Effective Membership Inference Attack Exploiting the "All for One" Principle in Federated Learning.

Mã nguồn tham khảo từ [Liar-Mask/FedMIA](https://github.com/Liar-Mask/FedMIA).

