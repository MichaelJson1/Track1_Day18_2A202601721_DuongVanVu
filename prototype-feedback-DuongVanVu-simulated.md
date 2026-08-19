# Prototype Feedback — Cá nhân: Dương Văn Vũ 


## Tester/context

- **Tester:**  Nguyễn Quốc Thịnh - 01675
- **Relevant Context:** Trong lớp khi nghe giảng, bạn có thường highlight nội dung quan trọng hoặc nội dung bạn chưa hiểu không? Sau buổi học thì bạn làm gì với highlight đấy?
- **Outcome task:** Dùng từng phương án để tạo một bản ghi chú có cấu trúc từ nội dung đã lưu, đủ để tiếp tục ôn tập mà không cần mở lại toàn bộ bài học.

## Observation

| Observation | Note |
| --- | --- |
| First action | **A:** chọn các chip highlight trước, sau đó đưa vào từng mục của mẫu. **B:** đọc tiêu đề và nguồn của gợi ý đầu tiên trước khi quyết định; không dùng “Nhận tất cả”. **C:** chờ trạng thái AI tạo nháp kết thúc, rồi đọc phần tô vàng trước. |
| Chỗ dừng, do dự hoặc hiểu sai | **A:** phải tự quyết định highlight nào thuộc “Ý chính” hay “Chưa hiểu”, nên chậm hơn. **B:** lúc đầu chưa rõ “Nhận tất cả” có làm mất quyền sửa sau đó không; copy cạnh nút giúp giảm do dự. **C:** hiểu phần tô vàng là chỗ cần kiểm tra, nhưng cần hover mới thấy lý do nên có thể bị bỏ lỡ nếu tester không di chuột. |
| Evidence được đọc hay bỏ qua | **A:** không có AI evidence. **B:** đọc nguồn trích dẫn của gợi ý đầu tiên và mục có nhãn “AI chưa chắc”; các mục còn lại có xu hướng quyết định nhanh hơn. **C:** đọc warning và lý do của đoạn tô vàng; các đoạn không tô vàng ít được đối chiếu với dữ liệu gốc. |
| Cách tester sửa hoặc lấy lại control | **A:** bỏ một chip đã chọn và chọn lại mục khác trước khi lưu. **B:** chọn “Bỏ” một gợi ý rồi dùng “Hoàn tác”, sau đó “Sửa” nội dung một gợi ý trước khi xác nhận lưu. **C:** chọn “Sửa nội dung” để chỉnh đoạn uncertainty; không dùng “Tạo lại” vì cảnh báo bản cũ sẽ mất khiến thao tác này có rủi ro. |
| Option được chọn | **Option B.** |
| Lý do và trade-off | B tạo cân bằng tốt nhất: AI giảm công phân nhóm nhưng người học vẫn kiểm chứng bằng nguồn, nhận/bỏ/sửa từng phần. A kiểm soát cao nhưng tốn công; C nhanh nhất nhưng dễ khiến người học chỉ duyệt nhanh bản nháp. |
| Evidence chống lại kỳ vọng của nhóm | Kỳ vọng C sẽ giúp nhanh nhất đúng về số thao tác, nhưng warning “AI chưa chắc” và quyết định sửa/tạo lại khiến tester vẫn phải đọc kỹ; lợi ích tốc độ có thể không lớn nếu người học cần độ chính xác cao. |

## Tách bốn lớp

### OBSERVED

- Có thể mở `index.html`, đi qua A/B/C và quay về common context mà không cần giải thích cách điều hướng.
- Ở Option B, tester dùng cả Bỏ, Hoàn tác và Sửa trước khi lưu.
- Ở Option C, tester nhận ra highlight vàng là tín hiệu uncertainty, nhưng chỉ đọc lý do sau khi thử hover.

### INTERPRETED

- Option B thể hiện agency rõ nhất vì control xuất hiện ngay tại từng suggestion và có recovery tức thì.
- Cần làm lý do uncertainty ở Option C dễ thấy hơn; chỉ dựa vào hover có thể không đủ trong test không được facilitator hướng dẫn.
- “Tạo lại bản nháp” là control hữu ích nhưng cần tín hiệu rõ hơn về phần nào sẽ thay đổi, vì người dùng có thể ngại mất bản đang xem.

### DECIDED — NEXT CHANGE

- Giữ cả ba option cho test thật để so sánh trade-off.
- Với C, hiển thị lý do uncertainty ngay dưới đoạn tô vàng hoặc thêm nút “Xem lý do”, thay vì chỉ hover.
- Trước nút “Tạo lại”, nêu ngắn bản cũ sẽ bị thay thế và cho phép quay lại chỉnh tay nếu không muốn tạo lại.

### STILL UNPROVEN

- Người học thật có thấy việc tổng hợp này đủ giá trị để dùng sau mỗi bài học không.
- Tester có thực sự đọc evidence ở B/C trong bối cảnh có áp lực thời gian không.
- Người dùng có chọn B thay vì C khi dùng dữ liệu học của chính họ, không phải fixture của prototype.
