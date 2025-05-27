<nav class="nav-container">
  <a href="../" class="nav-item">🏠 Home</a>
  <a href="../research/" class="nav-item">📝 Research Notes</a>
  <a href="../courses/" class="nav-item">🎓 Course Notes</a>
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
    background-image: url('../assets/images/research.jpg');
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

# 🔬 Research Notes - Nhật ký Nghiên cứu

> Tổng hợp từ các dự án thực tế và hành trình học tập cá nhân

[![Static Badge](https://img.shields.io/badge/Python-docs-yellow?style=flat&logo=python&logoColor=white)](https://python.org) [![Static Badge](https://img.shields.io/badge/Pytorch-docs-pink?style=flat&logo=pytorch&logoColor=brown)](https://pytorch.org/) [![Static Badge](https://img.shields.io/badge/mlflow-docs-orange?style=flat&logo=mlflow&logoColor=white)](https://mlflow.org/)

## 📌 Chủ đề nghiên cứu

| STT | Chủ đề | Mô tả |
| :----: | :---- | :----- |
| 1 | Phát hiện sớm và phân loại ung thư cổ tử cung (Cervical Cancer Cytology) | Ứng dụng các kỹ thuật Deep Learning/Machine Learning cho bộ dữ liệu ung thư cổ tử cung, nhằm hỗ trợ phát hiện sớm và phân loại các tế bào ác tính |
| 2 | Tư vấn, giải đáp câu hỏi y tế liên quan đến hình ảnh tế bào ung thư cổ tử cung | Nghiên cứu mô hình kết hợp thị giác và ngôn ngữ, nhằm sinh ngôn ngữ, tóm tắt, truy vấn tri thức và giải đáp các câu hỏi xoay quanh hình ảnh tế bào ung thư cổ tử cung.
| 3 | Công cụ hỗ trợ gán nhãn tự động cho các loại định dạng ảnh, video cho bài toán phân loại, phát hiện đối tượng | Khảo sát, nghiên cứu và triển khai nhanh một số công cụ hỗ trợ gán nhãn dữ liệu hình ảnh y tế |

## 📂 Nhiệm vụ chi tiết

| STT | Tên | Trạng thái | Mô tả | Tài liệu |
| :--: | :--- | :--: | :--- | :---: |
| 1 | Nghiên cứu kỹ thuật Ensemble Learning cho phân loại ung thư cổ tử cung tế bào học | ✅ | - Nghiên cứu kỹ thuật Ensemble Learning và các phương pháp của chúng. <br> - Thực nghiệm kỹ thuật Ensemble Learning cho bộ dữ liệu thực tế. <br> - Triển khai đánh giá và cài đặt huấn luyện nhằm so sánh hiệu suất giữa mô hình đơn lẻ và mô hình kết hợp. | [[Paper]](https://arxiv.org/pdf/2308.02781) <br> [[Slides]](https://) <br> [[Code]](https://) |
| 2 | Nghiên cứu nền tảng & định hướng về Self-Supervised Learning (Học tự giám sát) | ✅ | - Nghiên cứu tổng quan về Self-Supervised Learning (SSL) <br> - Tìm hiểu về một số mô hình SSL phổ biến: BYOL, MoCo, SimCLR <br> - Phân tích, đi sâu vào kiến trúc của mô hình SimCLR (backbone, loss function, augmentation & projection head, v.v.) | [[Paper:01]](https://arxiv.org/pdf/2002.05709) <br> [[Paper:02]](https://) <br> [[Slides]](https://) <br> [[Code]](https://) |
| 3 | Cài đặt & triển khai mô hình SimCLR | ✅ | - Cài đặt kiến trúc SimCLR, đánh giá tính phù hợp và huấn luyện cho bài toán phân loại tế bào học <br> - Lên phương án thực nghiệm nhanh, đánh giá kết quả sơ bộ và lên kế hoạch điều chỉnh <br> Tối ưu hóa và mở rộng tinh chỉnh, gia tăng hiệu suất cho mô hình | [[Notes]](https://) <br> [[Code]](https://) | 

## 🛢️ Bộ dữ liệu

Bộ dữ liệu về ung thư cổ tử cung được thu thập và gán nhãn thủ công bởi các bác sĩ chuyên khoa tại [Bệnh viện A, Thái Nguyên](https://). Dữ liệu hiện đã được công khai phục vụ cho mục đích tham khảo và nghiên cứu.

- Link: [Atlat datasets](https://label.ai4med.vn/auth/login)
- Account: ```BOCSDL@ai4med.com```
- Password: ```BenhvienAThaiNguyen```

