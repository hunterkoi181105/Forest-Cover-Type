# Forest-Cover-Type
# BÀI TẬP PHÂN LOẠI CÁC LOẠI THẢM THỰC VẬT DỰA TRÊN TẬP DỮ LIỆU FOREST COVER BẰNG CÁC THUẬT TOÁN PHÂN LOẠI CỔ ĐIỂN
## Giới thiệu bài toán

Xây dựng 4 mô hình phân loại dựa trên các chiến lược phân loại khác nhau nhằm phân loại các loại thảm thực vật trong tập dữ liệu **Forest Cover Type**.

**Forest Cover Type** là một tập dữ liệu lớn với mục tiêu phân loại các loại thảm thực vật trong khu rừng.

### Đặc điểm của tập dữ liệu Forest Cover Type

- **Quy mô**: 581,012 mẫu với 54 tính năng.  
- **Số lớp**: 7 loại thảm thực vật khác nhau.  
- **Nguồn gốc**: Tập dữ liệu được thu thập từ **Cục Quản lý Rừng Mỹ (U.S. Forest Service)**.  
- **Dữ liệu**: Bao gồm các tính năng về địa hình, độ cao, khoảng cách đến các khu vực thủy văn, hệ thống giao thông và các đặc điểm khác.  
- **Sự phân bố không đồng đều**: Các lớp có số lượng mẫu khác nhau.  

#### Thông số kỹ thuật

- **Tổng số mẫu**: 581,012 mẫu  
- **Số lớp**: 7 lớp thảm thực vật (từ Type 1 đến Type 7)  
- **Số tính năng**: 54 tính năng (bao gồm các đặc điểm như *Elevation*, *Slope*, *Soil Types*, *Distance Features*)  
- **Format dữ liệu**: Dữ liệu số  
- **Training set**: Chia theo tỷ lệ, với một phần dùng để huấn luyện và một phần cho kiểm tra  
- **Kích thước**: Đa dạng, thường được resize về 224×224  
- **Trang chủ dataset**: [Forest Cover Type - UCI](https://archive.ics.uci.edu/ml/datasets/forest+cover+type)

## Thách thức của tập dữ liệu Forest Cover Type

- **Đặc điểm lớp không đồng đều**: Lớp thảm thực vật có sự phân bố không đồng đều trong dữ liệu, có thể dẫn đến sự thiên lệch trong mô hình.  
- **Đa dạng tính năng**: Các tính năng có thể không có mối liên hệ rõ ràng với nhau, điều này đòi hỏi mô hình cần phải học được những đặc điểm phức tạp.  
- **Tính không gian**: Dữ liệu đặc trưng cho môi trường tự nhiên, không phải lúc nào cũng dễ nhận diện hoặc chia nhỏ.  
- **Đặc điểm dữ liệu không phải hình ảnh**: Mặc dù dữ liệu không phải hình ảnh nhưng cũng có thể có sự tương tác phức tạp giữa các tính năng.  

## Mục tiêu của bài toán

- **Xây dựng pipeline hoàn chỉnh**: từ việc tải dữ liệu, xử lý, phân tích (EDA), huấn luyện đến đánh giá mô hình.  
- **So sánh nhiều mô hình phân loại**: Từ các mô hình đơn giản như *Decision Tree*, *Random Forest* đến các mô hình phức tạp hơn như *SVM*, *MLP Classifier*.  
- **Phân tích chi tiết**: Tạo ra các chỉ số đánh giá mô hình như *Accuracy*, *Precision*, *Recall*, *F1-Score* và phân tích kết quả qua *confusion matrix*, phân phối dữ liệu, và độ chính xác trên các lớp khác nhau.  
- **Áp dụng chiến lược tuning mô hình**: *Tuning* siêu tham số để tối ưu hóa kết quả.  

### Các mô hình sẽ được triển khai

- Decision Tree  
- Random Forest  
- SVM  
- MLP Classifier
- Gradient Boosting Classifier

Tất cả 5 mô hình sẽ được triển khai và đánh giá với các phương pháp huấn luyện khác nhau, so sánh kết quả và phân tích hiệu quả của từng mô hình.  
**Mục tiêu là tìm ra mô hình phù hợp nhất** cho bài toán phân loại thảm thực vật này dựa trên tập dữ liệu **Forest Cover Type**.
