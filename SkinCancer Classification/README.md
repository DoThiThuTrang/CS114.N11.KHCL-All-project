# Project: Skin Cancer Classification
## Dataset 
Dữ liệu nhóm sử dụng được lưu trữ tại đây: https://drive.google.com/drive/folders/1JUOEy-ICHthIpnFU00tqWipl-kTBbWa5?usp=sharing
## Xử lý dữ liệu
Với dữ liệu có được, nhóm xử lý thông qua 2 cách:
- Xử lý bằng cách resize ảnh với kích thước tối thiểu (450 x 600) và chuyển ảnh xám. Sau đó sử dụng PCA để giảm số lượng chiều. Chúng 
- Xử lý bằng cách trích xuất đặc trưng (Feature Engineering) resize ảnh, blue channel, dilation và sử dụng CLAHE. Sau đó sử dụng histogram để trích xuất đặc trưng của ảnh.
## Model 
- Với cách xử lý đầu tiên, nhóm em sử dụng model Logistic Regression, KNN và SVM để dự đoán. Đây là các model hoạt động tốt trên pixel.
- Với cách xử lý thứ hai, nhóm sử dụng model Gaussian Naive Bayes và SVM. 
Kế quả cho ra như sau: 
## Kết quả 
<b> Đánh giá mô hình LR, KNN và SVM với cách xử lý đầu tiên </b> 

| Model | Accuracy | Precision | Recall | F1 score | Cross-Validation score |
| --- | --- | --- | --- | --- | --- |
| LR | 0.655172 | 0.671111 | 0.665198 | 0.668142 | 0.664065
| KNN | 0.673563 | 0.688889 | 0.682819 | 0.685841 | 0.694535 
| SVM	| 0.657471 | 0.687500	| 0.629956 | 0.657471 | 0.659134

<b> Đánh giá mô hình LR, KNN và SVM với cách xử lý đầu tiên </b>

| Model | Accuracy | Precision | Recall | F1 score | Cross-Validation score |
| --- | --- | --- | --- | --- | --- |
| Gaussian naive bayes | 0.668966	| 0.706522	| 0.590909	| 0.643564	| 0.703446
| SVM	0.655172	| 0.650862	| 0.686364	| 0.668142	| 0.636585
