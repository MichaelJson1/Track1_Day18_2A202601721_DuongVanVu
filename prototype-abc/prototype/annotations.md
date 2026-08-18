# Prototype annotations (facilitator only — không cho tester xem)

Case: AI Notes — Personal Learning Notes. Common context, content fixture và task giống nhau ở cả ba option (`index.html`). Chỉ critical interaction khác nhau: `option-a.html`, `option-b.html`, `option-c.html`, mỗi cái dẫn tới màn kết quả riêng (`result-a/b/c.html`) và có đường quay lại `index.html`.

---

OPTION A
We expect the tester to: tự chọn từng mục (highlight / chưa hiểu / câu hỏi) rồi đặt vào đúng ô trong mẫu ("Ý chính", "Cần xem lại", "Câu hỏi mở") mà không cần được giải thích quy trình 2 bước (chọn → chạm ô).
Watch for: tester có bỏ cuộc giữa chừng vì thấy tốn công tự viết/sắp xếp không; có hiểu ngay là AI không tham gia gì ở bước này không, hay họ chờ AI gợi ý.
Do not explain: không nói trước quy trình "chạm để chọn, chạm ô để đặt" — để xem tester có tự khám phá được thao tác không.

---

OPTION B
We expect the tester to: đọc từng gợi ý AI kèm nguồn trích dẫn, rồi chủ động Nhận / Sửa / Bỏ từng gợi ý thay vì nhận tất cả theo quán tính; có thể dùng "+ Thêm mục tự viết" nếu thấy AI bỏ sót.
Watch for: tester có đọc nguồn trích dẫn dưới mỗi gợi ý trước khi quyết định không, hay bấm Nhận ngay không đọc; có nhận ra nhãn "GỢI Ý AI" nghĩa là nội dung chưa được xác nhận không.
Do not explain: không nói trước ý nghĩa của nhãn "Gợi ý AI" hay quy trình Nhận/Sửa/Bỏ — để xem tester tự suy ra được vai trò của mình so với AI.

---

OPTION C
We expect the tester to: đọc lại toàn bộ bản nháp AI đã tạo sẵn trước khi lưu (không bấm Xác nhận ngay); chú ý và hiểu được phần tô vàng là AI không chắc; dùng "Sửa nội dung" hoặc "Tạo lại bản nháp" nếu thấy sai.
Watch for: tester có đọc kỹ bản nháp hay chỉ lướt qua rồi bấm Xác nhận & Lưu ngay; có hiểu vì sao một đoạn được tô vàng khi họ hover vào không; có thử "Tạo lại" khi thấy bản nháp không ổn, hay chỉ sửa tay.
Do not explain: không nói trước ý nghĩa của phần tô vàng hay sự khác biệt giữa "Sửa nội dung" và "Tạo lại bản nháp" — đây chính là chỗ rủi ro cao nhất nên cần xem tester tự hiểu được mà không cần facilitator narrate.

---

## Definition of testable — self-check

- Tester tự mở `index.html` và thao tác được cả ba option mà không cần hỏi. ✓ (điều hướng bằng link/nút rõ ràng, không cần biết code)
- Cả ba bắt đầu từ cùng context/task. ✓ (cùng fixture 6 mục trong `index.html`, cùng câu mô tả task)
- Không cần facilitator narrate để hiểu option. → cần verify khi test thật; annotation trên dùng để facilitator tự chấm, không hiện cho tester.
- Nội dung đủ thật để ra quyết định. ✓ (canned content bám sát nội dung khoá học, không phải lorem ipsum)
- Mỗi option thể hiện điểm user lấy lại control. ✓ (A: chọn/bỏ chip; B: Nhận/Sửa/Bỏ từng gợi ý; C: Sửa nội dung / Tạo lại / Xác nhận)
- Có đường reset về common context. ✓ (nút "Quay lại context ban đầu" ở mọi màn kết quả + link breadcrumb ở mọi trang)
