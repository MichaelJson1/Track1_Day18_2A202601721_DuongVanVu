# Track1 — Day 17 — Finding and Validating Pain Points

**Case đã chọn:** Case B — AI Notes: Personal Learning Notes

> Trong khi học, học viên có thể highlight một đoạn nội dung, đánh dấu  **“Chưa hiểu”** , hoặc viết một câu hỏi hay ghi chú ngắn.
>
> Khi bài học kết thúc, AI Notes kết hợp những dấu vết này với nội dung bài để tạo một bản ghi chú có cấu trúc. Học viên có thể chỉnh sửa và xác nhận trước khi lưu.

| Thành phần | Solution đã mô tả                                                                |
| ------------ | ------------------------------------------------------------------------------------ |
| Trigger      | Học viên hoàn thành bài học                                                    |
| Input        | Nội dung bài, highlights, điểm “Chưa hiểu”, câu hỏi và ghi chú cá nhân |
| AI action    | Chọn lọc, nhóm và tổ chức thông tin                                           |
| Output       | Bản ghi chú cá nhân có cấu trúc                                               |
| User control | Học viên chỉnh sửa và xác nhận trước khi lưu                               |

**Người phù hợp để phỏng vấn:** trong bảy ngày gần đây đã ghi chú, highlight hoặc lưu lại nội dung để xem sau.

---

**Thành viên:**

| MSV         | Họ tên          |
| ----------- | ----------------- |
| 2A202601721 | Cao Nhật Minh    |
| 2A202601663 | Dương Văn Vũ  |
| 2A202601507 | Phạm Khánh Linh |

---

## 1. Hypothesis Problem của nhóm

**Capability trung tính (đã gỡ khỏi hình thức triển khai):**

> Khả năng giúp người học gom lại những dấu vết rời rạc phát sinh trong lúc học (điểm quan trọng, điểm chưa hiểu, câu hỏi/ghi chú) thành một bản tổng hợp có cấu trúc mà không cần tự làm thủ công, đồng thời vẫn giữ cho người học quyền kiểm soát nội dung cuối cùng trước khi lưu lại.

**Actor được chọn để điều tra trước:** Học viên — **lúc cần dùng lại nội dung đã học** (không phải lúc đang học), vì đây là actor có khả năng cao nhất đang trải nghiệm pain rõ ràng, cụ thể và có thể hỏi được bằng một sự kiện gần đây.

**Situation & Job:**

> Khi có việc buộc phải dùng lại nội dung của một bài đã học cách đó vài ngày (làm bài tập, chuẩn bị kiểm tra, hoặc áp dụng vào việc thật), học viên đang cố lấy lại đúng phần mình cần, đủ nhanh để làm tiếp việc đang dở, bằng cách mở lại bài học và tua tìm, lục lại những gì mình đã lưu, hoặc hỏi người khác.

**JTBD Hypothesis:**

> Khi tôi cần dùng lại nội dung của một bài đã học nhưng không còn nhớ rõ, tôi muốn lấy lại đúng phần mình cần đủ nhanh để không phải dừng việc đang làm, để có thể hoàn thành việc đó đúng hạn mà không phải học lại bài từ đầu.

**Pain Hypothesis đã chọn để điều tra trước — A (vấn đề nằm ở việc TÌM lại):**

> Khi cần dùng lại nội dung của một bài đã học cách đó vài ngày, học viên gặp khó khăn trong việc lấy lại đúng phần mình cần vì nội dung nằm rải ở nhiều nơi (bài học gốc, chỗ họ tự ghi lại, trí nhớ) và không có điểm vào rõ ràng để biết cần mở chỗ nào trước; dẫn đến họ phải tua và đọc lại nhiều hơn dự tính, hoặc bỏ cuộc giữa chừng và làm tiếp việc đang dở với hiểu biết mơ hồ.

Hai cách giải thích cạnh tranh cho cùng một hành vi quan sát được (để tránh chọn A chỉ vì nó khớp sẵn với solution directive):

- **Pain Hypothesis B** — vấn đề nằm ở việc **HIỂU** lại, không phải tìm: thứ tìm lại được không giúp học viên hiểu ra, vì chỗ đó vốn đã không hiểu ngay từ lúc học.
- **Cách giải thích C** — không có pain đáng giải: học viên tìm lại nhanh, không thấy phiền, không có hậu quả đáng kể.

**Problem Hypothesis mang sang Chặng 2:**

> Khi có việc buộc phải dùng lại nội dung của một bài đã học cách đó vài ngày, học viên có thể gặp khó khăn trong việc lấy lại đúng phần mình cần vì nội dung nằm rải ở nhiều nơi và không có điểm vào rõ ràng; điều này có thể khiến họ phải tua và đọc lại nhiều hơn dự tính, hoặc bỏ cuộc giữa chừng và làm tiếp việc đang dở với hiểu biết mơ hồ.

---

## 2. Ba Practice Notes (một note / thành viên)

| Thành viên      | Practice Note | Nội dung |
| ----------------- | ------------- | --------- |
| Cao Nhật Minh    |               |           |
| Dương Văn Vũ  |               |           |
| Phạm Khánh Linh |               |           |

---

## 3. Solution Parking Lot (tối thiểu 5 hướng)

| # | Hướng giải quyết | Có dùng AI? | Ghi chú |
| - | -------------------- | ------------- | -------- |
| 1 |                      |               |          |
| 2 |                      |               |          |
| 3 |                      |               |          |
| 4 |                      |               |          |
| 5 |                      |               |          |

---

## 4. Conversation Guide — phiên bản cuối

**Big 3 (điều cần học, có 1 câu hỏi "đáng sợ"):**

| # | Điều cần học                                                         | Đáng sợ? |
| - | ------------------------------------------------------------------------ | ----------- |
| 1 | Situation có thật và có lặp không                                  |             |
| 2 | Họ thực sự đã làm gì để lấy lại nội dung                     |             |
| 3 | Tốn công tới đâu, hậu quả là gì, barrier nằm ở TÌM hay HIỂU | ✅          |

**Tiêu chí tuyển người:** đã ghi chú/highlight/lưu nội dung trong 7 ngày gần đây, **và** đã từng có lần phải quay lại dùng nội dung một bài/khoá đã học trước đó (recruitment check 2 vế).

**Story opener:** "Kể mình nghe về lần gần nhất bạn phải quay lại dùng nội dung của một bài hay khoá bạn đã học trước đó — hôm đó là chuyện gì, và bạn cần dùng nó để làm gì?"

**4 câu bị gắn cờ sau buổi luyện thật và cách sửa:**

- Bỏ qua recruitment check → bắt buộc hỏi trước khi vào phỏng vấn.
- Câu dẫn dắt "cách này hiệu quả đúng không?" → bỏ hẳn.
- Câu liệt kê sẵn vấn đề gợi ý → đổi thành hỏi mở theo Big 3.
- Trả lời chung chung không được Anchor lại → luôn hỏi "lần gần nhất là khi nào?".
