# DỰ ÁN: TỪ DỮ LIỆU ĐẾN PHÂN TÍCH VỚI PYTHON
- **Họ và tên:** Tri Văn Dũng
- **MSSV:** 2400005830
- **Lớp:** 24DTH2B

## Trả lời câu hỏi thu hoạch
Câu 1: Vì sao chuỗi tiếng Việt có dấu tốn nhiều byte hơn chuỗi tiếng Anh có cùng số ký tự?
Đáp án:Tiếng Anh không dấu sử dụng các ký tự thuộc bảng mã ASCII cơ bản, mỗi ký tự chỉ tốn 1 byte lưu trữ. Tiếng Việt có dấu chứa các ký tự đặc biệt(như à, á, ệ, ư, đ...) không có trong bảng mã ASCII. Chuẩn mã hóa UTF-8 phải sử dụng từ 2 đến 3 bytes để biểu diễn 1 ký tự tiếng Việt có dấu. Do đó, cùng số lượng ký tự nhưng chuỗi tiếng Việt luôn tốn nhiều dung lượng byte hơn.   
Câu 2: So sánh file CSV và JSON. Khi dữ liệu phân cấp lồng nhau (nested), ta nên dùng định dạng nào?
Đáp án:So sánh:
CSV: Lưu dữ liệu dạng bảng 2 chiều(dòng và cột), đơn giản, dung lượng nhẹ nhưng chỉ phù hợp với dữ liệu phẳng. 
JSON: Lưu dữ liệu dạng đối tượng (cặp key-value hoặc danh sách lồng nhau), cấu trúc linh hoạt nhưng dung lượng lớn hơn CSV.   
Lựa chọn: Khi dữ liệu phân cấp lồng nhau (nested), ta nên dùng định dạng JSON vì CSV không thể biểu diễn trực quan các cấu trúc lồng nhau phức tạp mà không làm rối dữ liệu.   
Câu 3: Hiện tượng gì xảy ra khi mở một file ảnh bằng Notepad? Giải thích nguyên nhân.
Đáp án:Hiện tượng: Màn hình Notepad hiển thị vô số các ký tự lạ, ngoằng ngoèo, lỗi font(thường gọi là "rác dữ liệu").
Nguyên nhân: File ảnh là file nhị phân (Binary file) lưu trữ dữ liệu dạng các byte màu sắc. Trong khi đó, Notepad là trình đọc file văn bản (Text file), nó sẽ cố gắng ép các byte dữ liệu nhị phân của ảnh chuyển thành các ký tự văn bản tương ứng trong bảng mã, dẫn đến việc hiển thị các ký tự không thể đọc được.   
Câu 4: Vì sao trong Khoa học Dữ liệu phải tách data/raw/ với data/processed/ và phải có file .gitignore?
Đáp án:Tách data/raw/ và data/processed/: Để đảm bảo tính nguyên bản và tái lập (Reproducibility). Thư mục data/raw/ chứa dữ liệu thô ban đầu(tuyệt đối không sửa đổi để làm mốc khôi phục), còn data/processed/ chứa dữ liệu đã qua làm sạch/tiền xử lý để đưa vào mô hình phân tích.Có file .gitignore: Giúp loại bỏ các file rác, file hệ thống, file môi trường nặng (venv) và đặc biệt là dữ liệu rác/dữ liệu bảo mật không bị đưa lên GitHub, tránh làm lộ thông tin và giữ cho kho chứa nhẹ nhàng.   
Câu 5: Nêu nhận xét ngắn về điểm GPA (trung bình, cao nhất, thấp nhất) rút ra từ biểu đồ phân tích ở Buổi 2.
Đáp án mẫu:Điểm GPA cao nhất: $3.8$ (sinh viên Trần Thị B).   
Điểm GPA thấp nhất: $3.1$ (sinh viên Lê Văn C).   
Điểm GPA trung bình: $\approx 3.43$.   
Nhận xét: Mức điểm GPA của sinh viên nằm trong khoảng từ $3.1$ đến $3.8$, đa số đạt mức khá - giỏi và không có sinh viên nào rơi vào nhóm điểm yếu/trung bình.   