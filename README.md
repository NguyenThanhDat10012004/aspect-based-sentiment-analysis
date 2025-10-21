# aspect-based-sentiment-analysis
## comment: 
### nội dung buổi học này giải quyết 2 bài toán ATE detect được các term đang nói tới, ABSA detect được các text được nói tới và nhãn của của mỗi câu positive, negative, neurtral. Mô hình sử dụng ở đây là lstm, conv1d kết hợp với fc, distil-bert, trong đó distil-bert lúc nào cũng cho kết quả cao nhất. 
### một chú ý nhỏ ở bài toán này là để nhãn của <pad> thành -100 để nó đạt chỉ số ignore_index trong crossentropy giúp tiết kiệm thời gian tính toán. 
### còn lại bài toán chỉ đơn giản là có câu , có nhãn và cho mô hình học, cách huấn luyện ở đây là lấy hết tất cả checkpoint dựa theo best_lost_metric để lấy ra checkpoint tốt nhất. 
