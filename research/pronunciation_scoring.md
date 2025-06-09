# 🌵 The problem of Pronunciation Scoring (PS)

> 🎯 Mục tiêu cụ thể: Xây dựng hệ thống chấm điểm hoặc phát hiện lỗi phát âm tiếng Anh dành cho người học. <br>
> 📌 Hướng tiếp cận đề xuất: <br>
> - Phát hiện lỗi phát âm (mispronunciation detection)
> - Chấm điểm phát âm (pronunciation scoring)
> - Phản hồi sửa lỗi (diagnosis & feedback)

## 📋 Content

- [Timeline](#-timeline)
- [Datasets](#️-datasets)
- [Benchmarks for Pronunciation Scoring Datasets](#️-benchmarks-for-pronunciation-scoring-datasets)

## ⏳ Timeline

| Phase | Deadline | Task | Description | Resource |
| :---: | :------: | :--- | :---------- | :------: |
| 01: Nghiên cứu tổng quan & Chuẩn bị dữ liệu | 02/06 - 02/07, 2025 | Week01: Tổng quan về bài toán Pronunciation Scoring | - Phân tích 3 chức năng, mục tiêu chính của bài toán (detect, score, feedback). <br> - Nghiên cứu một số paper quan trọng liên quan đến PS (GOP, DNN-GOP, Wav2Vec-Scoring). <br> - Nghiên cứu một số kiến trúc PS tổng thể (gồm phần thu âm, xử lý âm thanh, phân tích, chấm điểm và phản hồi cho người học). | |
| | | Week02: Thu thập và tìm hiểu một số bộ dữ liệu công khai | - Lựa chọn, tìm các bộ dữ liệu người Việt nói Tiếng Anh hoặc người không phải bản địa nói tiếng Anh. <br> - Chuẩn hóa âm thanh sao cho có định dạng đảm bảo tính phù hợp và chât lượng. <br> - Tạo transcript đi kèm, chuyển sang dạng phát âm từng âm tiết. <br> - Căn khớp âm thanh với văn bản, sử dụng một số công cụ căn khớp để xác định chính xác vị trí từng âm thanh trong câu nói (Montreal Forced Aligner hoặc Gentle). | |
| | | Week03: Chạy mô hình đánh giá cơ bản và phân tích lỗi | - Dùng một số mô hình đơn giản có sẵn như GOP để chấm điểm từng âm người học phát ra, từ đó biết âm nào phát đúng, âm nào sai. <br> - Dựa vào kết quả mô hình, đánh giá thủ công, xác định một số lỗi phổ biến mà người Việt thường mắc phải khi nói tiếng Anh. <br> - Lựa chọn hoặc tự tạo một bộ dữ liệu thủ công, tự gán nhãn đúng sai nhằm so sánh kết quả mà mô hình đưa ra. | |
| | | Week04: Phân tích đặc trưng & Thử nghiệm mô hình chấm điểm | - Lấy đặc điểm của âm thanh để phân tích mở rộng, sử dụng môt số công cụ như librosa hoặc openSMILE để trích xuất một số đặc điểm quan trọng (độ cao giọng, độ vang, hình dạng âm thanh,v.v.). <br> - Sử dụng một số thuật toán dễ huấn luyện để ước lượng điểm phát âm của người học dựa trên các đặc trưng đã trích xuất. <br> - Thử nghiệm và phản hồi cơ bản như âm nào người học đã nói sai, cách phát âm đúng là gì.v.v. | |
| 02: Thử nghiệm mô hình & Tối ưu hóa | 02/07 - 02/08, 2025 | Week01: Huấn luyện mô hình phát hiện lỗi phát âm (Mispronunciation Detection) | - Sử dụng một số mô hình âm thanh truyền thống hoăc hiện đại để tinh chỉnh trên dữ liệu phát âm sai (HuBERT, Wav2Vec2). <br> - So sánh kết quả của mô hình này với phương pháp truyền thống GOP ở phare 01 xem cái náo phát hiện lỗi tốt hơn. <br> - Kiểm thử bằng tay để kiểm tra mô hình bằng cách tự tạo bộ dữ liệu gán nhãn thủ công. | |
| | | Week02: Huấn luyện mô hình chấm điểm phát âm (Pronunciation Scoring) | - Sử dụng mô hình học máy hoặc học sâu để lấy đặc trưng âm thanh, sau đó đưa vào một số mô hình đơn giản nhắm tính ra điểm tổng thể cho mỗi câu nói. <br> - So sánh điểm máy chấm với điểm dữ liệu chấm thực tế để đo độ tương đồng (correlation). | |
| | | Week03: Tạo phản hồi sửa lỗi cho người học | - Khi mô hình phát hiện ra lỗi phát âm, hệ thống cần xác định lỗi nào, gợi ý sửa lỗi đó. <br> - Tạo mẫu gợi ý phát âm chuẩn theo text hoặc audio,v.v. | | 
| | | Week04: Đánh giá lại mô hình | - Đánh giá tổng thể hiệu suất các mô hình bằng các chỉ số phổ biến khác như precision, recall. <br> - Với mô hình chấm điểm. sử dụng độ đo sai số trung bình MSE để đánh giá. | |
| 03: Triển khai và kiểm thử thực tế | 02/08 - 02/09, 2025 | Week01: Tích hợp hoàn chỉnh các mô hình | - Ghép các thành phần chính: phát hiện lỗi, chấm điểm, phàn hồi sửa lỗi vào cùng một hệ thống. <br> - Thiết kết luồng xử lý từ nhận âm thanh đầu vao cho đến khi đưa ra kết quả cuối cùng cho người dùng. | |
| | | Week02 & Week03: Kiểm thử với các phàn hồi thực tế | - Thu thập phản hồi để đánh giá và cải thiện, tinh chỉnh thêm mô hình hoặc hệ thống. <br> - Tổng hợp các góp ý để lên kế hoạch nâng cấp hoặc chỉnh sửa. | |
| | | Week04: Tổng kết và báo cáo kết quả | - Đánh giá tổng quan về hiệu quả của hệ thống và những hạn chế còn tồn tại. <br> - Viết báo cáo kỹ thuật tổng hợp kết quả nghiên cứu và triển khai hệ thống thực tế. <br> - Đề xuất hướng cải thiện tiếp theo. | |

## 🛢️ Datasets 

| No. | Name | Details | Link |
| :-: | :--: | :------ | :--: |
| 01  | `Speechocean762` | - Tập dữ liệu giọng nói phục vụ cho bài toán đánh giá phát âm. <br> - Gồm 5000 câu tiếng Anh được phát âm bởi 250 người không phải bản địa, trong đó một nửa là trẻ em. Nhãn được các chuyên gia ngôn ngữ đánh giá ở ba cấp độ: cấp câu (sentence-level), cấp từ (word-level), cấp âm vị (phoneme-level).| [speechocean762](https://huggingface.co/datasets/mispeech/speechocean762) |
| 02  | `L2-ARCTIC`| - Bộ dữ liệu gồm 26.867 câu thoại của 24 người không phải bản địa, có cân bằng giới tính. <br> - Tổng 27 giờ âm thanh và có gán nhãn lỗi phát âm (thay âm, thiếu âm, thêm âm) | [l2-arctic](https://psi.engr.tamu.edu/l2-arctic-corpus/) |
| 03 | `LibriSpeech` | - Bộ dữ liệu lớn gần 1000 giờ gồm các đoạn ghi âm sách nói tiếng Anh. <br> - Được chia thành hai type chính (clean và other), trong đó clean được cho là dễ dàng nhận dạng hơn còn other có tiềng ồn và khó nhận biết hơn. | [librispeech](https://www.openslr.org/12/) |

## ⚔️ Benchmarks for Pronunciation Scoring Datasets

| No. | Dataset | Task | Model | PCC | Notes | Resources |
| :-: | :-----: | :--: | :---- | :-: | :---- |:-------: |
| 01 | `Speechocean762` | Phone-level | HierCB+ConPCO | 0.70 | Sử dụng contrastive learning & orginal regression để cải thiện độ chính xác | [Paper](https://paperswithcode.com/paper/conpco-preserving-phoneme-characteristics-for) |
| 02 |  |  | GOPT-PAII  | 0.68 | Sử dụng mô hình transformer cho phân tích về nhiều khía cạnh tiếng nói | [Paper](https://arxiv.org/pdf/2205.03432v1) |
| 03 |  |  | SpeechBlender + LSTM | 0.63 | Tạo dữ liệu lỗi giả lập + LSTM để chấm điểm | [Paper](https://arxiv.org/pdf/2211.00923v3) |
| 04 |  |  | HiPAMA-LibriSpeech | 0.62 | Áp dụng attention để đánh giá phát âm theo cấu trúc phân cấp | [Paper](https://arxiv.org/pdf/2211.08102v2) |
| 05 |  |  | GOP | 0.45 | Phương pháp truyền thống | [Paper]() | 
| 01 | `Speechocean762` |  Word-level | 3MH | 0.69 | | [Paper](https://arxiv.org/pdf/2305.18146v4) |
| 02 | | | GOPT-PAII | 0.60 | | [Paper](https://arxiv.org/pdf/2205.03432v1) |
| 03 | | | HiPAMA-Librispeech | 0.59 | | [Paper](https://arxiv.org/pdf/2211.08102v2) |
| 01 | `Speechocean762` | Utterance-level | 3MH | 0.81 | | [Paper](https://arxiv.org/pdf/2305.18146v4) |
| 02 | | | HierCB+ConPCO | 0.80 | | [Paper](https://paperswithcode.com/paper/conpco-preserving-phoneme-characteristics-for) |
| 03 | | | GOPT-Librispeech | 0.74 | | [Paper]() |
| 04 | | | GOPT-PAII | 0.73 | | [Paper](https://arxiv.org/pdf/2205.03432v1) |
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         