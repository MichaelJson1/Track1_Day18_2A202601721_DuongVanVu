# Prototype Feedback Note — mỗi thành viên hoàn thành một bản

> Mỗi thành viên tự chạy một buổi test micro-prototype với một tester, rồi điền một bản riêng bên dưới. Không gộp chung một bản cho cả nhóm.

---

## Chuẩn bị test

### 1. Chốt context và task

**Relevant context** — một câu hỏi, tối đa 2 phút trong lúc test:

> "Gần đây bạn có từng phải quay lại dùng nội dung của một bài hay khoá bạn đã học trước đó không?"

Nếu tester chưa từng có context liên quan, vẫn có thể dùng họ để tìm interaction breakdown nhưng không đưa ra value claim mạnh.

**Outcome task** — nói kết quả cần đạt, không nói nút cần bấm:

> "Trong tình huống này, hãy dùng từng phương án để lấy lại đúng phần nội dung bạn cần, đủ để tiếp tục làm việc đang dở."

**Observation focus** (tối đa năm thứ):

1. First action
2. Hesitation (chỗ dừng/do dự/hiểu sai)
3. Evidence read/ignored
4. Correction/recovery (cách tester tự sửa hoặc lấy lại control)
5. Option được chọn và trade-off

### 2. Luật facilitation

1. Tester tự điều khiển prototype.
2. Dùng cùng một task cho A/B/C.
3. Không narrate hoặc giải thích icon.
4. Không lấp im lặng.
5. Không hỏi "Bạn có thích không?".
6. Khi tester hỏi cách hoạt động, hỏi lại: "Theo bạn, nó nên hoạt động như thế nào?"

**Ba câu cứu hộ:**

- "Bạn cứ nói to suy nghĩ của mình nhé."
- "Bạn sẽ làm gì tiếp theo?"
- "Theo bạn, nó nên hoạt động như thế nào?"

---

## Bản của Cao Nhật Minh

**Tester/context:** Đặng Đức Hoà — MSV 2A202601351. Context cụ thể (câu trả lời cho câu hỏi "relevant context" mở đầu) không được ghi lại chi tiết trong feedback nhận được — chỉ có phản ứng của tester với từng option sau khi thử.

| Observation                               | Note      |
| ----------------------------------------- | --------- |
| First action                              | **A:** kéo thả chỉ 2 note, tỏ ra "lười" thao tác tiếp. **B:** lướt và đọc chăm chú. **C:** tỏ ra rất muốn đọc. |
| Chỗ dừng, do dự hoặc hiểu sai        | **A:** lóng ngóng vì phải thao tác nhiều. **B:** chưa hiểu vì sao còn 3/6 notes. |
| Evidence được đọc hay bỏ qua        | Không ghi lại chi tiết — chỉ biết ở B tester "đọc chăm chú" (có khả năng có đọc phần trích dẫn nguồn), còn đọc kỹ tới đâu, có mở tooltip flag ở C hay không thì chưa rõ. |
| Cách tester sửa hoặc lấy lại control | Không ghi lại. |
| Option được chọn                      | **B + C** (tester chủ động nói muốn kết hợp cả hai, không chọn một option đơn lẻ) |
| Lý do và trade-off                      | Option A: thấy bất tiện khi có nhiều note — dễ bị trùng nhau hoặc kiến thức bao hàm nhau mà chính tester không nhận ra (A không có bước nào giúp phát hiện trùng lặp/chồng lấn). Option B: thích việc AI gom nhóm, thấy nó giảm được note trùng nhau. Option C: thích output cuối cùng của C nhất, nhưng muốn có **một bản kết hợp cả B và C** — dùng cơ chế của B để xem từng ghi chú và gom nhóm trước, rồi để C tổng hợp phần đã gom đó thành một bản nháp chứa hướng đi, cách học tiếp theo. |
| Evidence chống lại kỳ vọng của nhóm | Ở Option B: bảng trade-off ban đầu không hề dự đoán việc tester sẽ hiểu lầm "3/6 notes" là thiếu mục — đây là một gap về Evidence/Uncertainty mà Chặng 3 đã lường trước cho Option C nhưng nhóm chưa nghĩ tới cho Option B (B cũng cần nói rõ "6 mục gốc đã gộp thành 3 nhóm", không chỉ hiển thị số 3 trơ). Ở Option A: bảng trade-off ban đầu chỉ dự đoán A "tốn công, dễ bỏ dở" (và first action — chỉ kéo 2/6 note rồi dừng — khớp đúng dự đoán này); nhưng rủi ro "note trùng/chồng lấn mà không biết" do thiếu bước đối chiếu là một rủi ro khác, nhóm chưa tính tới khi đó. |

**Tách bốn lớp:**

- **OBSERVED** — Tester đã làm hoặc nói gì?

  Tester nói rõ theo từng option: (A) "bất tiện khi nhiều note, có thể note bị trùng nhau hoặc kiến thức bao hàm nhau mà không biết"; (B) thích việc AI gom nhóm, giảm note trùng nhau; (C) thích output của C, và chủ động đề xuất muốn có một bản tổng hợp cả B và C — dùng B để xem từng ghi chú/gom nhóm, rồi C tổng hợp thành bản nháp có hướng đi, cách học.
- **INTERPRETED** — Nhóm nghĩ điều đó có thể có nghĩa gì?

  Giá trị thật tester tìm kiếm không nằm gọn trong một option đơn lẻ: (1) nhu cầu lõi là *phát hiện và gộp trùng lặp/chồng lấn giữa các note*, thứ chỉ Option A không đáp ứng được vì A không có bước đối chiếu nào; (2) Option B giải quyết đúng nhu cầu đó (gom nhóm) nhưng dừng ở dạng gợi ý rời rạc, chưa ra một bản đọc được ngay; (3) Option C cho ra bản đọc được ngay (đúng "desired outcome" ban đầu của nhóm) nhưng tester không chắc bản đó có đối chiếu/gom trùng kỹ như B hay không vì quá trình bị ẩn hoàn toàn. Nói cách khác, tester muốn *nhìn thấy bước gom nhóm* (sự minh bạch của B) *trước khi* nhận bản tổng hợp cuối (sự tiện lợi của C) — khớp với đúng mối lo "Evidence and Uncertainty" mà nhóm đã đặt ra cho Option C ở Chặng 3.
- **DECIDED — NEXT CHANGE** — Nhóm sẽ sửa, kết hợp hoặc test gì tiếp?

  Kết hợp hai option nhưng giữ một cơ chế chính rõ ràng: dùng luồng của B (AI gom nhóm, hiển thị nguồn trích dẫn, user Nhận/Sửa/Bỏ từng nhóm) làm bước giữa, sau đó thêm một bước cuối kiểu C — AI tổng hợp đúng những nhóm user đã duyệt ở bước B thành một bản nháp có cấu trúc (hướng đi, cách học tiếp theo), user chỉ xác nhận/sửa bản nháp đó ở bước cuối. Cần test lại thiết kế ghép này với ít nhất một tester nữa trước khi coi là hướng chốt.
- **STILL UNPROVEN** — Điều gì chưa thể kết luận từ một người?

  Đã có first action và hesitation cho A/B (xem bảng), nhưng evidence được đọc/bỏ qua và cách tester tự sửa hoặc lấy lại control thì chưa ghi nhận được ở option nào — nên chưa biết tester có thật sự dùng các đường phục hồi đã thiết kế (Hoàn tác ở B, Sửa nội dung/Tạo lại bản nháp ở C) hay tester không cần tới chúng. Cũng chưa quan sát được first action/hesitation của C ngoài "rất muốn đọc" — chưa rõ tester có đọc kỹ phần flag (tô vàng) trước khi muốn lưu hay bỏ qua luôn vì đã "muốn đọc". Mức độ nghiêm trọng của pain "note trùng/chồng lấn" ở Option A cũng chưa rõ (tốn công đáng kể hay chỉ khó chịu nhẹ). Quan trọng nhất: đề xuất "muốn cả B lẫn C" mới đến từ một người — chưa biết người khác có thấy bước gom nhóm hiển thị (của B) là cần thiết trước khi nhận bản tổng hợp, hay phần lớn user sẽ thấy bước đó là thừa và chỉ muốn thẳng ra kết quả như C. Cần test thiết kế ghép B+C với ít nhất 2-3 tester nữa trước khi coi đây là hướng chốt.

---

**Next Change có thể là:**

- Giữ một option và sửa interaction.
- Kết hợp hai options nhưng giữ một cơ chế chính rõ ràng.
- Bỏ một option vì tester không hiểu hoặc nó không tạo khác biệt.
- Sửa cả ba rồi test người tiếp theo.
