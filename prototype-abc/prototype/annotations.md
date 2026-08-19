# Prototype annotations (facilitator only — không cho tester xem)

Case: AI Notes — Personal Learning Notes. Common context, content fixture và task giống nhau ở cả ba option (`index.html`). Chỉ critical interaction khác nhau: `option-a.html`, `option-b.html`, `option-c.html`, mỗi cái dẫn tới màn kết quả riêng (`result-a/b/c.html`) và có đường quay lại `index.html`.

---

OPTION A
We expect the tester to: kéo một mục vào ô mẫu, hoặc dùng cách chạm-để-chọn-rồi-chạm-ô nếu không nghĩ tới kéo thả — cả hai đường đều dẫn tới cùng kết quả, không cần giải thích trước.
Watch for: tester có tự thử kéo thả trước không (đúng với mental model "kéo/thả" của Option A) hay đi thẳng vào cách chạm; có bỏ cuộc giữa chừng vì thấy tốn công tự viết/sắp xếp không; có hiểu ngay AI không tham gia gì ở bước này không, hay họ chờ AI gợi ý.
Do not explain: không nói trước là có thể kéo thả HAY có thể chạm để chọn — để xem tester tự khám phá được ít nhất một trong hai cách.

---

OPTION B
We expect the tester to: đọc từng gợi ý AI kèm nguồn trích dẫn, rồi chủ động Nhận / Sửa / Bỏ từng gợi ý — có thể dùng "Nhận tất cả gợi ý" nếu muốn nhanh, nhưng vẫn cần nhận ra mình có thể sửa/bỏ lại từng cái sau đó; item đã Bỏ có thể Hoàn tác ngay, không cần nhớ đã bỏ cái gì.
Watch for: tester có đọc nguồn trích dẫn trước khi quyết định không, hay bấm "Nhận tất cả" ngay không đọc; nếu bấm Bỏ nhầm, tester có tự tìm ra nút Hoàn tác không hay nghĩ là mất luôn.
Do not explain: không nói trước ý nghĩa của nhãn "Gợi ý AI", nút "Nhận tất cả", hay việc mục đã Bỏ vẫn Hoàn tác được — để xem tester tự suy ra được vai trò của mình so với AI và độ an toàn của các thao tác.

---

OPTION C
We expect the tester to: đợi AI "soạn" xong (có trạng thái đang tạo, không phải xuất hiện tức thì), đọc lại toàn bộ bản nháp trước khi lưu; chú ý và hiểu được phần tô vàng là AI không chắc; dùng "Sửa nội dung" hoặc "Tạo lại bản nháp" nếu thấy sai — và hiểu Tạo lại nghĩa là bản cũ mất, không phải giữ cả hai.
Watch for: tester có đọc kỹ bản nháp hay chỉ lướt qua rồi bấm Xác nhận & Lưu ngay; có hiểu vì sao một đoạn được tô vàng khi hover vào không; có thử "Tạo lại" khi thấy bản nháp không ổn, hay chỉ sửa tay; nếu tester bấm Xác nhận ngay khi đang gõ sửa dở (không bấm Lưu chỉnh sửa trước), hệ thống tự lưu đúng phần họ vừa gõ — quan sát xem tester có nhận ra điều đó hay tưởng mình mất nội dung.
Do not explain: không nói trước ý nghĩa của phần tô vàng, sự khác biệt giữa "Sửa nội dung" và "Tạo lại bản nháp", hay việc Tạo lại sẽ mất bản cũ — đây chính là chỗ rủi ro cao nhất nên cần xem tester tự hiểu được mà không cần facilitator narrate.

---

## Definition of testable — self-check

- Tester tự mở `index.html` và thao tác được cả ba option mà không cần hỏi. ✓ (điều hướng bằng link/nút rõ ràng, không cần biết code)
- Cả ba bắt đầu từ cùng context/task. ✓ (cùng fixture 6 mục trong `index.html`, cùng câu mô tả task)
- Không cần facilitator narrate để hiểu option. → cần verify khi test thật; annotation trên dùng để facilitator tự chấm, không hiện cho tester.
- Nội dung đủ thật để ra quyết định. ✓ (canned content bám sát nội dung khoá học, không phải lorem ipsum)
- Mỗi option thể hiện điểm user lấy lại control. ✓ (A: chọn/bỏ chip; B: Nhận/Sửa/Bỏ từng gợi ý; C: Sửa nội dung / Tạo lại / Xác nhận)
- Có đường reset về common context. ✓ (nút "Quay lại context ban đầu" ở mọi màn kết quả + link breadcrumb ở mọi trang)
