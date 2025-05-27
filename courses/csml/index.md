<nav class="nav-container">
  <a href="../../" class="nav-item">🏠 Home</a>
  <a href="../../research/" class="nav-item">📝 Research Notes</a>
  <a href="../../courses/" class="nav-item">🎓 Course Notes</a>
  <a href=" " class="nav-item">📚 Knowledge Base</a>
</nav>

<style>
  .nav-container {
    display: flex;
    justify-content: center;
    gap: 20px; /* khoảng cách giữa các mục */
    padding: 12px 0;
    background-color: #fff;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }

  .nav-item {
    padding: 8px 16px;
    border: 2px solid transparent;
    border-radius: 8px;
    color: #555;
    text-decoration: none;
    font-weight: 600;
    transition: all 0.3s ease;
    display: flex;
    align-items: center;
    gap: 6px;
    background-color: #f5f5f5;
  }

  .nav-item:hover {
    background-color: #007BFF;
    color: white;
    border-color: #0056b3;
  }

  .nav-item:focus {
    outline: none;
    box-shadow: 0 0 0 3px rgba(0,123,255,0.5);
  }
</style>

<div style="
    background-image: url('../../assets/images/courses.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    min-height: 60vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: white;
    text-align: center;
    padding: 40px 20px;
    margin-bottom: 30px;
">
</div>

# 🌲 Applied Machine Learning Course - Khóa học Ứng dụng Học máy
> Học sâu - Làm thật - Ứng dụng thực tiễn

[![Static Badge](https://img.shields.io/badge/CS229-Machine_Learning-purple?style=flat&logo=coursera&logoColor=white)](https://) [![Static Badge](https://img.shields.io/badge/Geekfor-Geeks-Silver?style=flat&logo=geeksforgeeks&logoColor=red)](https://) [![Static Badge](https://img.shields.io/badge/Google-Colab-red?style=flat&logo=googlecolab&logoColor=orange)](https://) [![Static Badge](https://img.shields.io/badge/Tensorflow-docs-tavily?logo=tensorflow&logoColor=orange)]([https://](https://www.tensorflow.org/))

## 🔍 Thông tin khóa học

Khóa học [Applied Machine Learning](https://) cung cấp nền tảng vững chắc về Machine Learning (Học máy), một lĩnh vực cốt lõi trong trí tuệ nhân tạo. Bạn đọc sẽ được tiếp cận các thuật toán quan trọng trong Supervised Learning (học có giám sát) và Unsupervised Learning (học không giám sát), cùng với các kỹ thuật phổ biến như tiền xử lý dữ liệu, lựa chọn đặc trưng và đánh giá mô hình. Ngoài ra, khóa học hướng dân chi tiết quy trình xây dựng hệ thống học máy từ đầu tới cuối, giúp người đọc có cái nhìn toàn diện và khả năng áp dụng vào thực tế.

## 🎯 Bạn sẽ học được gì ?

- Hiểu rõ khái niệm cốt lõi và cơ chế hoạt động của các thuật toán học máy nền tảng.

- Xây dựng các mô hình học máy hoàn chỉnh bằng cách sử dụng các thư viện phổ biến như Tensorflow, scikit-learn và Keras. Bao gồm các thuật toán như hồi quy (Linear Regression, Lasso Regression) và phân loại (Support Vector Machine, Naive Bayes, Decision Tree).

- Thành thạo các kỹ thuật tinh chỉnh, đánh giá và tối ưu hóa mo hình để nâng cao hiệu suất và độ chính xác.

## 🛠️ Yêu cầu tiên quyết

- Có nền tảng vững chắc về đại số tuyến tính, xác suất thống kê và vi phân cơ bản, nhằm hiểu rõ các khái niệm toán học đứng sau các thuật toán học máy.

- Thành thạo lập trình Python và quen thuộc với việc viết, chạy và gỡ lỗi mã cho các bài toán học máy.

- Đã có kinh nghiệm thực hành với các thư viện học máy phổ biến như Tensorflow, scikit-learn và Keras để triển khai và thử nghiệm các thuật toán khác nhau.

## ⏰ Lịch trình bài giảng

| STT | Chủ đề | Mô tả | Trạng thái | Tài liệu |
| :-: | :----- | :---- | :--------: | :------: |
| 1 | Tổng quan về Machine Learning | - Khái niệm về Machine Learning <br> - Ứng dụng thực tiễn và Phân loại hệ thống học máy <br> - Vòng đời của một mô hình học máy <br> - Kỹ thuật phân chia tập dữ liệu trong quá trình huấn luyện | N/A | N/A | 
| 2 | Linear Regression (hồi quy tuyến tính) | - Hàm mất mát bình phương sai số (MSE) <br> - Phương trình chuẩn (Normal Equation) <br> - Gradient Descent và một số biến thể <br> - Hồi quy đa thức và Regularization (điều chuẩn) | N/A | N/A |
| 3 | Phân loại (Classification) | - Tổng quan phân loại trong học máy <br> - Hồi quy Logistic <br> - Đo lường hiệu suất: Accuracy, Precision, Recall, F1-Score và Trade-off <br> - Phân loại đa lớp, đa nhãn và đa đầu ra | N/A | N/A |
| 4 | Naive Bayes Classifier | - Định lý Bayes và xác suất hậu nghiệm <br> - Gỉa định độc lập điều kiện trong Naive Bayes <br> - Các biến thể: Gaussian, Multinomial, Bernoulli | N/A | N/A |
| 5 | Support Vector Machine | - Phân loại tuyến tính với SVM <br> - Soft Margin và điều chỉnh độ mềm biên <br> - Phân loại phi tuyến với Kernel trick: đa thức, Gaussian RBF <br> - Hồi quy SVM (SVM Regression) <br> - Phức tạp tính toán và các lớp bài toán<br> | N/A | N/A |
| 6 | Decision Trees | - Huấn luyện và trực quan hóa cây quyết định <br> - Dự đoán và ước lượng xác suất <br> - Thuật toán CART và tiêu chí phân chia (Gini, Entropy) <br> - Regularization, hồi quy cây và độ nhạy mô hình | N/A | N/A |
| 7 | Ensemble Learning và Random Forests | - Voting Classifiers và học tổ hợp cơ bản <br> - Kỹ thuật Bagging, Pasting và đánh giá Out-of-Bag <br> - Random Forests, Extra-Trees và đo lường độ quan trọng đặc trưng <br> - Boosting: AdaBoost, Gradient Boosting, Histogram-Based GB, và Stacking | N/A | N/A |
| 8 | Dimensionality Reduction Techniques | - Khó khăn của mô hình với dữ liệu đa chiều <br> - Các phương pháp chiếu, học đa tạp <br> - Ứng dụng thư viện Học máy để giải thích và lựa chọn số chiều <br> - PCA nén, PCA ngẫu nhiên, PCA tăng dần <br> - Chiếu ngẫu nhiên, LLE và một số kỹ thuật giảm chiều khác | N/A | N/A |
| 9 | Unsupervised Learning Techniques | - Clustering Algorithms: k-means và DBSCAN <br> - k-means và giới hạn của k-means <br> - Ứng dụng clustering cho phân đoạn ảnh và học bán giám sát <br> - DBSCAN và các thuật toán clustering khác <br> - Gaussian Mixtures và ứng dụng phát hiện dị thường <br> - Chọn số cụm, Bayesian Gaussian Mixture Models <br> - Các thuật toán khác cho phát hiện dị thường và mới lạ | N/A | N/A |
| 10 | Hyperparameter Tuning & Model Optimization | - Grid search, Random Search, Bayesian optimization <br> - Learning rate scheduler, early stoping, v.v. | N/A | N/A |

## 💪 Lời cảm ơn

Tôi xin gửi lời cảm ơn chân thành đến hai tác giả đã truyền cảm hứng mạnh mẽ cho tôi trong quá trình xây dựng các ghi chú bài giảng này:

- [Andrew Ng](https://) - người sáng lập khóa học [CS229 Machine Learning](https://), một trong những khóa học kinh điển giúp tôi xây dựng nền tảng vững chắc về học máy.

- [Aurélien Géron](https://) - tác giả của cuốn [Hands-On Machine Learning with Scikit-learn, Keras, and Tensorflow](https://), một nguồn tài liệu thực hành quý giá đã đồng hành cùng tôi trên hành trình khám phá thế giới AI.

Những công trình và chia sẻ của họ không chỉ giúp tôi tiếp cận kiến thức một cách bài bản mà còn thôi thúc tôi chia sẻ lại cho cộng đồng.