## Xử lý dữ liệu

### Làm sạch:
- `Loan_Amount_Requested`: đổi kiểu dữ liệu từ object sang float sau khi loại bỏ dấu ','.
- `Home_Owner`: Chuyển 'None' và giá trị nan thành giá trị ước lượng.
- `Length_Employed`: Thay giá trị nan bằng ước lượng và chuẩn hóa format.
- `Annual_Income` và `Months_Since_Deliquency`: Điền giá trị nan bằng giá trị ước lượng sử dụng IterativeImputer.
- Xử lý outlier: Loại bỏ outlier sử dụng phương pháp z-score.
- Loại bỏ cột ID.

### Xây dựng mô hình:
- Chia data thành tập train và tập test theo tỉ lệ 8:2 và áp dụng oversampling bằng SMOTE.
- Áp dụng các mô hình Decision tree, Xgboost, Catboost và tinh chỉnh các tham số để tối ưu hiệu suất.
- Xây dựng mô hình deeplearning MLP và điều chỉnh tham số để đạt kết quả phân loại tốt.

## Kết luận:
- Cân đối giữa các độ đo để xử lý imbalace trong label.
- Tập train và tập test có độ chính xác tương tự.
- Các model không có hiện tượng overfitting.
