<nav class="nav-container">
  <a href="../" class="nav-item">🏠 Home</a>
  <a href="../research/" class="nav-item">📝 Research Notes</a>
  <a href="../courses/" class="nav-item">🎓 Course Notes</a>
  <a href="../notes/" class="nav-item">📚 Knowledge Base</a>
</nav>

<style>
.nav-container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 12px; 
  padding: 8px 0;
  background-color: #fff;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.nav-item {
  padding: 6px 12px; 
  border: 2px solid transparent;
  border-radius: 8px;
  color: #555;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
  display: flex;
  align-items: center;
  gap: 4px; 
  background-color: #f5f5f5;
  white-space: nowrap;
  font-size: 14px; 
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

@media (max-width: 480px) {
  .nav-item {
    padding: 5px 8px;
    font-size: 13px;
  }
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

# 🔬 Research Notes

> 🌹 "Dream big. Start small. Act now"
>
> 🌻 "The expert in anything was once a beginner"

[![Python](https://img.shields.io/badge/python-org-blue?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
[![PyTorch](https://img.shields.io/badge/pytorch-framework-yellow?style=for-the-badge&logo=pytorch&logoColor=brown)](https://pytorch.org)
[![MLFlow](https://img.shields.io/badge/MLflow-tracking-blue?style=for-the-badge&logo=mlflow&logoColor=blue)](https://mlflow.org)
[![NumPy](https://img.shields.io/badge/NumPy-library-purple?style=for-the-badge&logo=numpy&logoColor=blue)](https://numpy.org)
[![HuggingFace](https://img.shields.io/badge/hugging_face-framework-pink?style=for-the-badge&logo=huggingface&logoColor=yellow)](https://huggingface.co)
[![Pandas](https://img.shields.io/badge/pandas-framework-brown?style=for-the-badge&logo=pandas&logoColor=purple)](https://pandas.pydata.org)
[![Google Colab](https://img.shields.io/badge/google-colab-green?style=for-the-badge&logo=googlecolab&logoColor=orange)](https://colab.research.google.com)

## 💡 Tổng quan

Trong quá trình nghiên cứu tại [Viện Khoa học và Công nghệ Ứng dụng (IAST)](https://iast.ictu.edu.vn), tôi đã có cơ hội tham gia vào nhiều dự án liên quan đến ứng dụng trí tuệ nhân tạo (AI) trong lĩnh vực chăm sóc sức khỏe và giáo dục. Trong các dự án này, tôi trực tiếp đảm nhiệm một số nhiệm vụ nghiên cứu và triển khai các giải pháp kỹ thuật.

Mỗi dự án được chia thành nhiều chủ đề nhỏ nhằm mở rộng hướng tiếp cận và khai thác đa chiều bài toán thực tiễn. Toàn bộ các chủ đề cũng như báo cáo chi tiết về từng nhiệm vụ tôi đã thực hiện đều được hệ thống hóa và trình bày tại mục [Research Notes](../research/).

## 🏷️ Chủ đề nghiên cứu

| STT | Dự án | Chủ đề | Liên kết |
| :----: | :---- | :--- | :---: |
| 1 | `🏥 Ứng dụng AI hỗ trợ bác sĩ trong phân loại ung thư cổ tử cung tế bào học` | Xây dựng và phát triển mô hình AI nhằm phân loại và hỗ trợ bác sĩ gán nhãn tự động | [[Link]]() |
|   |                              | Sử dụng Vision Language Model (VLM) để triển khai ứng dụng VQA (hỏi & đáp) để tư vấn, giải đáp về ảnh tế bào học |  |
| 2 | `🏫 Ứng dụng công nghệ AI hỗ trợ giáo dục phổ thông (Ứng dụng hỗ trợ học và dạy tiếng Anh)` | Nghiên cứu bài toán Pronunciation Scoring - Chấm điểm phát âm tiếng Anh | [[Link]]() |

## 📋 Kế hoạch & Nhiệm vụ

> `🏥 Ứng dụng AI hỗ trợ bác sĩ trong phân loại ung thư cổ tử cung tế bào học`

| No. | Dealine | Task | Status | Desciption | Resources |
| :-: | :--: | :--- | :-: | :-- | :-: |
| 1 | 08/2024 - 11/2024 | Nghiên cứu kỹ thuật Ensemble Learning cho bộ dữ liệu ung thư cổ tử cung tế bào học | ✅ | - Nghiên cứu kỹ thuật Ensemble Learning và các phương pháp liên quan. <br> - Thực nghiệm kỹ thuật Ensemble Learning cho bộ dữ liệu thực tế. <br> - Triển khai đánh giá và cài đặt huấn luyện nhằm so sánh hiệu suất giữa mô hình đơn lẻ và mô hình kết hợp. | [[Paper]]() [[Code]]() |
| 2 | 02/2025 - 05/2025 | Nghiên cứu nền tảng & định hướng về Self-Supervised Learning (Học tự giám sát) | ✅ | - Nghiên cứu tổng quan về Self-Supervised Learning (SSL). <br> - Tìm hiểu về một số mô hình SSL phổ biến: BYOL, MoCo, SimCLR. <br> - Phân tích, đi sâu vào kiến trúc của mô hình SimCLR (backbone, loss function, augmentation & projection head, v.v.). | [[Paper]]() [[Notes]]() |
| 3 | 02/2025 - 05/2025 | Cài đặt & triển khai mô hình SimCLR | ✅ | - Cài đặt kiến trúc SimCLR, đánh giá tính phù hợp và huấn luyện cho bài toán phân loại tế bào học. <br> - Lên phương án thực nghiệm nhanh, đánh giá kết quả sơ bộ và lên kế hoạch điều chỉnh. <br> - Tối ưu hóa và mở rộng tinh chỉnh, gia tăng hiệu suất cho mô hình. | [[Notes]]() [[Code]]() |

> `🏫 Ứng dụng công nghệ AI hỗ trợ giáo dục phổ thông (Ứng dụng hỗ trợ học và dạy tiếng Anh)`

| No. | Dealine | Task | Status | Desciption | Resources |
| :-: | :--: | :--- | :-: | :-- | :-: |