# AI Support Log — mỗi thành viên viết ngắn

**AI đã giúp tôi ở đâu?**

Dựng toàn bộ Human–AI Decision Table (Chặng 3) cho case AI Notes dựa trên ba option đã chốt ở group-feedback-synthesis.md — điền đủ năm dòng (Role and Agency, Act/Ask/Don't Act, Expectation, Evidence and Uncertainty, Control and Recovery) cho cả A/B/C. Build ba micro-prototype hoàn chỉnh bằng HTML/CSS/JS (không cần Figma): Option A có kéo-thả thật, Option B có luồng AI gợi ý/Nhận-Sửa-Bỏ kèm Hoàn tác, Option C có trạng thái "AI đang soạn" và đoạn flag chỗ AI không chắc. AI tự chạy test tự động (Playwright) qua cả ba luồng sau mỗi lần sửa để bắt lỗi JS trước khi tôi mở thử. Sau đó AI tổng hợp giúp feedback thật từ buổi test với Đặng Đức Hoà vào đúng format bốn lớp OBSERVED/INTERPRETED/DECIDED/STILL UNPROVEN trong prototype-feedback-note.md.

**AI sai, hời hợt hoặc làm các options giống nhau ở đâu?**

Lần đầu dựng prototype, AI tự ý làm giao diện dạng khung điện thoại (phone-frame) dù tôi chưa yêu cầu — phải nói lại mới đổi sang layout web đúng ý. Khi điền cột "First action" và "Chỗ dừng/hiểu sai" vào bảng quan sát, AI tự chèn thêm phần diễn giải của mình vào ngay trong ô quan sát (ví dụ giải thích lý do vì sao tester hiểu lầm "3/6 notes"), làm lẫn OBSERVED với INTERPRETED — đúng lỗi mà quy trình "tách bốn lớp" của bài học muốn tránh. Ba thẻ chọn option ban đầu cũng có mô tả cơ chế chi tiết ngay trên trang chọn, có thể khiến tester bị dẫn dắt trước khi thử — AI không tự nhận ra vấn đề này cho tới khi tôi nói thẳng ra. Sau khi tôi thêm dữ liệu hành vi thật vào bảng, AI cũng quên cập nhật đồng bộ phần STILL UNPROVEN, khiến nó vẫn nói "chưa có first action" dù bảng đã có — một chỗ thiếu nhất quán AI tự phát hiện nhưng ban đầu bỏ sót.

**Tôi đã tự sửa hoặc quyết định lại điều gì?**

Yêu cầu đổi hẳn giao diện phone-frame sang web layout (top nav full-width, nhiều cột) cho đúng ngữ cảnh dùng trên máy tính. Yêu cầu bỏ tiêu đề và mô tả cơ chế ở trang chọn option, chỉ giữ nhãn A/B/C để không dẫn dắt lựa chọn của tester — đây là quyết định thiết kế nghiên cứu của tôi, không phải AI tự đề xuất. Yêu cầu viết lại các ô quan sát cho thuần dữ liệu, bỏ phần diễn giải AI tự chèn vào. Sau khi đọc lại feedback thật, tôi tự quyết định ghi "Option được chọn" là **B + C** thay vì chỉ chốt một option — vì tester nói rõ muốn kết hợp cả hai, và tôi không muốn đơn giản hoá feedback thật thành một lựa chọn gọn hơn cho dễ báo cáo.
