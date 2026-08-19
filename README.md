# Track1 — Day 18 — Cao Nhật Minh

## 1. Thông tin cá nhân và nhóm

- **MSV:** 2A202601721
- **Họ tên:** Cao Nhật Minh
- **Tên nhóm:** Hoo Lee Sheet
- **Ba thành viên:**

  | MSV         | Họ tên          |
  | ----------- | ----------------- |
  | 2A202601721 | Cao Nhật Minh    |
  | 2A202601663 | Dương Văn Vũ  |
  | 2A202601507 | Phạm Khánh Linh |

- **Case:** Case B — AI Notes: Personal Learning Notes

  > Trong khi học, học viên có thể highlight một đoạn nội dung, đánh dấu "Chưa hiểu", hoặc viết một câu hỏi hay ghi chú ngắn. Khi bài học kết thúc, AI Notes kết hợp những dấu vết này với nội dung bài để tạo một bản ghi chú có cấu trúc. Học viên có thể chỉnh sửa và xác nhận trước khi lưu.

## 2. Hypothesis Problem (bản nhóm dùng trong Day 18)

Bản đã chốt sau Evidence huddle ở group-feedback-synthesis.md, dùng làm điểm xuất phát cho Chặng 3–4:

> Khi có việc buộc phải dùng lại nội dung của một bài đã học cách đó vài ngày, học viên có thể gặp khó khăn trong việc lấy lại đúng phần mình cần vì nội dung nằm rải ở nhiều nơi và không có điểm vào rõ ràng; điều này có thể khiến họ phải tua và đọc lại nhiều hơn dự tính, hoặc bỏ cuộc giữa chừng và làm tiếp việc đang dở với hiểu biết mơ hồ.

Evidence ban đầu ủng hộ: cả ba practice notes đều cho thấy không ai có một điểm vào duy nhất để lấy lại nội dung cũ, mỗi người tự chắp vá quy trình riêng. Điều chưa chứng minh được ở Day 17: hậu quả thật (có trễ việc đang làm không) và barrier nằm ở TÌM hay HIỂU — chi tiết xem `day_17_artifacts.md` và `group-feedback-synthesis.md`.

## 3. Three Solution Options

Ba option cùng giải một Hypothesis Problem, khác nhau ở mức AI tham gia (xem đầy đủ ở `three-option-design-sheet.md`):

| Option | Mô tả ngắn |
| --- | --- |
| **A — Tự tạo bằng mẫu** | Học viên tự kéo/thả highlight, điểm "Chưa hiểu", câu hỏi vào đúng mục trong một mẫu ghi chú có sẵn. AI không tham gia xử lý nội dung (Don't Act). |
| **B — AI gợi ý, học viên chọn** | AI đọc highlight/điểm "Chưa hiểu"/câu hỏi, gợi ý nhóm nội dung theo chủ đề kèm nguồn trích dẫn. Học viên Nhận/Sửa/Bỏ từng gợi ý trước khi lưu (Ask). |
| **C — AI tạo sẵn, học viên duyệt** | AI tự động tổng hợp toàn bộ thành một bản ghi chú hoàn chỉnh ngay sau khi kết thúc bài, tự flag những đoạn không chắc chắn. Học viên xem lại, sửa hoặc yêu cầu tạo lại trước khi xác nhận (Act có điều kiện). |

**Prototype:** ba micro-prototype tương tác được (HTML/CSS/JS, không cần server) nằm trong `prototype-abc.zip` — giải nén rồi mở `prototype/index.html`. Hướng dẫn mở và ghi chú facilitator (không cho tester xem) ở `prototype-link.md` và `prototype/annotations.md`.

## 4. Đóng góp của tôi trong nhóm

- Dựng **common context và content fixture** dùng chung cho cả ba option trong prototype (cùng một bộ 6 mục: highlight, điểm "Chưa hiểu", câu hỏi) để đảm bảo A/B/C chỉ khác nhau ở critical interaction, đúng yêu cầu "giữ nguyên 70%" của Chặng 4.
- Điền **Human–AI Decision Table** (Chặng 3) cho cả ba option — năm quyết định: User/AI làm gì, AI Act/Ask/Don't Act, Expectation, Evidence and Uncertainty, Control and Recovery. File: `three-option-design-sheet.md`.
- **Build cả ba micro-prototype** (Option A/B/C) bằng HTML/CSS/JS: kéo-thả thật cho A, luồng gợi ý Nhận/Sửa/Bỏ kèm Hoàn tác cho B, luồng AI tự soạn kèm flag chỗ không chắc và trạng thái "đang soạn" cho C. Thiết kế lại giao diện từ mobile sang web layout, và chỉnh trang chọn option để chỉ hiện nhãn A/B/C (không mô tả cơ chế) nhằm tránh dẫn dắt lựa chọn của tester.
- **Facilitate buổi test** micro-prototype với tester Đặng Đức Hoà (MSV 2A202601351) theo đúng luật facilitation đã đặt ra (không narrate, không hỏi "có thích không", dùng ba câu cứu hộ khi cần).
- **Tổng hợp feedback** của buổi test theo đúng format bốn lớp OBSERVED / INTERPRETED / DECIDED — NEXT CHANGE / STILL UNPROVEN. File: `prototype-feedback-note.md`.

## 5. Prototype Feedback

Tóm tắt từ buổi facilitate với Đặng Đức Hoà (MSV 2A202601351) — chi tiết đầy đủ ở `prototype-feedback-note.md`:

**Observation chính:**

- First action: A — kéo thả chỉ 2 note rồi tỏ ra "lười" thao tác tiếp; B — lướt và đọc chăm chú; C — tỏ ra rất muốn đọc.
- Hesitation: A — lóng ngóng vì phải thao tác nhiều; B — chưa hiểu vì sao vẫn còn "3/6 notes" (tưởng thiếu mục, thực ra là đã gộp nhóm).
- Option được chọn: **B + C** — tester chủ động muốn kết hợp cả hai, không chọn một option đơn lẻ.

**Bốn lớp synthesis:**

- **OBSERVED:** A bất tiện vì note dễ trùng/chồng lấn mà không biết; B được thích vì AI gom nhóm giảm trùng lặp; C được thích vì có output đọc ngay được, nhưng tester đề xuất muốn có bản kết hợp cả B lẫn C.
- **INTERPRETED:** nhu cầu lõi là phát hiện/gộp trùng lặp giữa các note — A không đáp ứng được vì không có bước đối chiếu; B đáp ứng đúng nhu cầu đó nhưng dừng ở gợi ý rời rạc; C cho ra bản đọc ngay nhưng ẩn hết quá trình gom nhóm nên tester không yên tâm.
- **DECIDED — NEXT CHANGE:** kết hợp luồng B (AI gom nhóm, hiển thị nguồn, Nhận/Sửa/Bỏ) làm bước giữa, rồi thêm bước cuối kiểu C tổng hợp đúng phần đã duyệt thành bản nháp có hướng đi/cách học. Riêng B cần sửa cách hiển thị số nhóm ("6 mục gốc → 3 nhóm") để tránh hiểu lầm.
- **STILL UNPROVEN:** chưa quan sát được evidence đọc/bỏ qua và cách tester dùng đường phục hồi (Hoàn tác ở B, Sửa/Tạo lại ở C); mức độ nghiêm trọng của pain ở A chưa rõ; đề xuất ghép B+C mới đến từ một người, cần test thêm 2–3 tester nữa trước khi coi là hướng chốt.

## 6. AI Support Log

Tóm tắt — bản đầy đủ ở `ai-support-log.md`:

- **AI đã giúp:** dựng Human–AI Decision Table, build cả ba micro-prototype (kèm test tự động Playwright sau mỗi lần sửa), tổng hợp feedback thật vào đúng format bốn lớp.
- **AI sai/hời hợt:** tự ý làm giao diện phone-frame dù chưa được yêu cầu; lẫn phần diễn giải của mình vào ô quan sát (OBSERVED) thay vì giữ thuần dữ liệu; ba thẻ chọn option ban đầu lộ mô tả cơ chế có thể gây thiên kiến cho tester; quên đồng bộ phần STILL UNPROVEN sau khi bảng quan sát có thêm dữ liệu mới.
- **Tôi tự sửa/quyết định lại:** yêu cầu đổi sang layout web, yêu cầu bỏ mô tả ở trang chọn option để tránh bias, yêu cầu viết lại các ô quan sát cho thuần dữ liệu, và tự quyết định ghi "Option được chọn" là **B + C** thay vì rút gọn về một option để không làm sai lệch ý tester.
