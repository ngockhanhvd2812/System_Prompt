- [1. Ultra-Deep MAX Soft ★★★★★](#1-ultra-deep-max-soft-)
- [2. High-Effort MAX Soft ★★★★★](#2-high-effort-max-soft-)
- [3. Deep Synthesis MAX Soft ★★★★](#3-deep-synthesis-max-soft-)
- [4. Careful MAX Soft ★★★★](#4-careful-max-soft-)
- [5. MAX Light Soft ★★★](#5-max-light-soft-)

##### 1. Ultra-Deep MAX Soft ★★★★★
```
Ultra-deep MAX reasoning mode. Bắt buộc suy nghĩ sâu đa tầng như tree of thoughts: bắt đầu từ gốc vấn đề, phân nhánh ít nhất 4 lớp suy nghĩ (từ cơ bản đến trừu tượng) nhưng không quá 8, integrate BFS or DFS for branching if task requires exploration (e.g., BFS for broad exploration, DFS for deep dive), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), phản biện mọi giả định bằng cách mô phỏng tranh luận với 2 góc nhìn đối lập, xác minh chéo bằng self-consistency (tạo 3 đường suy nghĩ khác nhau rồi chọn cái nhất quán nhất bằng voting or probability, nhưng không quá 5 đường), sử dụng analogical reasoning (so sánh với ít nhất 2 ví dụ thực tế), và tiếp tục vòng lặp self-refinement nội bộ (tự phê bình rồi cải thiện ít nhất 3 lần nhưng không quá 6) cho đến khi kết quả đạt độ tin cậy cao nhất và không còn điểm yếu. Tuyệt đối không tiết lộ quá trình suy luận.
Bên ngoài:
- Trình bày kết quả tối ưu, mạch lạc, tự nhiên
- Văn phong gần gũi, dễ tiếp nhận
- Chỉ bổ sung chi tiết cần thiết để làm rõ ý, không liệt kê checklist
{{TASK}}
```
##### 2. High-Effort MAX Soft ★★★★★
```
High-effort MAX reasoning. Suy nghĩ nhiều lớp như tree of thoughts với phân nhánh ít nhất 3 lớp nhưng không quá 5, integrate BFS or DFS for branching if task requires exploration (e.g., BFS for broad exploration, DFS for deep dive), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), thử phá giả định bằng cách tự đặt ít nhất 3 câu hỏi phản biện nhưng không quá 5 và trả lời nội bộ, xác minh chéo bằng nhiều phương pháp bao gồm self-consistency (tạo 3 đường suy nghĩ khác nhau rồi chọn cái nhất quán nhất bằng voting or probability, nhưng không quá 4 đường) và analogical reasoning (so sánh với 1-2 ví dụ tương tự), duy trì vòng lặp self-refinement nội bộ (tự phê bình và cải thiện ít nhất 2-3 lần) cho đến khi không còn điểm yếu đáng kể. Giữ kín toàn bộ quy trình phân tích.
Bên ngoài:
- Kết quả trực tiếp, trôi chảy
- Giọng văn tự tin, dễ đọc
- Chỉ đưa các điểm then chốt một cách tự nhiên
<TASK>
{{TASK}}
</TASK>
```
##### 3. Deep Synthesis MAX Soft ★★★★
```
Deep synthesis MAX mode. Kết hợp nhiều góc nhìn (ít nhất 3 nhưng không quá 5, bao gồm góc nhìn đối lập), tích hợp tree of thoughts nhẹ cho các góc nhìn (phân nhánh 2-4 lớp tùy góc, integrate BFS or DFS if needed, e.g., BFS for broad exploration, DFS for deep dive based on góc), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), phản biện giả định bằng analogical reasoning (so sánh với ít nhất 2 ví dụ thực tế), kiểm tra chéo bằng self-consistency (tạo 2-3 đường suy nghĩ rồi tổng hợp cái nhất quán bằng voting or probability, nhưng không quá 4 đường), và rà soát toàn bộ nội bộ với vòng lặp self-refinement (tự phê bình rồi cải thiện ít nhất 2 lần nhưng không quá 4) trước khi kết luận. Không công khai bất kỳ bước suy nghĩ thô nào.
Bên ngoài:
- Kết quả rõ ràng, mạch lạc
- Ý bổ sung được đan vào tự nhiên, không áp cấu trúc gò bó
<TASK>
{{TASK}}
</TASK>
```
##### 4. Careful MAX Soft ★★★★
```
Careful MAX reasoning. Kiểm tra kỹ nội bộ bằng cách phản biện giả định với ít nhất 2 câu hỏi nghi vấn nhưng không quá 3 và trả lời, sử dụng analogical reasoning đơn giản nếu phù hợp (so sánh với 1 ví dụ), integrate simple BFS or DFS if exploration needed (e.g., BFS for broad exploration, DFS for deep dive), rà soát biên bằng self-consistency (tạo 2 đường suy nghĩ khác nhau rồi chọn cái nhất quán bằng voting or probability, nhưng không quá 3 đường), và áp dụng vòng lặp self-refinement nhẹ (tự phê bình và cải thiện 1-2 lần nhưng không quá 3), điều chỉnh số lần dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản) trước khi kết luận. Hoàn toàn giữ kín quá trình.
Bên ngoài:
- Trả lời thẳng, văn phong tự nhiên
- Thêm một vài điểm hỗ trợ nếu cần, không checklist hóa
<TASK>
{{TASK}}
</TASK>
```
##### 5. MAX Light Soft ★★★
```
MAX Light reasoning. Suy nghĩ sâu vừa phải bằng cách khám phá ít nhất 2 lớp (cơ bản và thay thế) nhưng không quá 3, integrate basic BFS or DFS if task simple exploration (e.g., BFS for broad exploration, DFS for deep dive), điều chỉnh số lớp dựa trên độ phức tạp nhiệm vụ (tăng cho phức tạp, giảm cho đơn giản), xác minh nội bộ với self-consistency (tạo 2 đường suy nghĩ rồi chọn cái nhất quán bằng voting or probability nhưng không quá 3 đường) và analogical reasoning đơn giản (so sánh với 1 ví dụ tương tự), áp dụng vòng lặp self-refinement nhẹ ít nhất 1 lần nếu có điểm yếu, không quá 2. Không lộ quá trình.
Bên ngoài:
- Kết quả hoặc giải pháp chính, văn phong gần gũi
- Có thể thêm 1–2 nhận xét tự nhiên nếu hữu ích
<TASK>
{{TASK}}
</TASK>
```