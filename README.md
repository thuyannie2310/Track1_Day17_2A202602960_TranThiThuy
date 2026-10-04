# Track 1 — Day 17: Finding and Validating Pain Points

## 1. Thông tin cá nhân và nhóm

- **Mã học viên:** 2A202602960
- **Họ và tên:** Trần Thị Thuý
- **Tên nhóm:** Track 1
- **Thành viên:**
  - Trần Thị Thuý — 2A202602960
  - Lê Thị Duyên — 2A202602411
  - Nguyễn Thùy Linh — 2A202602497
- **Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher
- **Ngày thu thập evidence:** 03/10/2026

> **Trạng thái nghiên cứu:** Đây là evidence từ một buổi practice interview dài 03:59. Kết quả giúp điều chỉnh hypothesis nhưng chưa đủ để coi là validation.

## 2. Problem Hypothesis Brief

### 2.1. Solution directive

Thêm nút “Tôi vẫn chưa hiểu” vào bài học. Khi học viên chủ động yêu cầu trợ giúp, AI Tutor sử dụng nội dung bài hiện tại và câu trả lời của học viên để đặt câu hỏi chẩn đoán, xác định kiến thức nền cần ôn, giải thích ngắn và đưa học viên trở lại bài đang học.

### 2.2. Capability trung tính

Giúp học viên xác định điểm kiến thức đang gây vướng mắc và nhận hướng dẫn phù hợp với ngữ cảnh ngay trong lúc học, để họ có thể tiếp tục mà không phải tự chuyển nội dung qua nhiều công cụ.

### 2.3. Chuỗi thay đổi kỳ vọng

```text
Hỗ trợ đúng thời điểm và đúng ngữ cảnh
→ xác định điểm kiến thức còn thiếu
→ nhận giải thích hoặc kiến thức nền phù hợp
→ giảm thời gian tìm kiếm và chuyển đổi công cụ
→ quay lại bài học sớm hơn
```

Phần giải thích là **output**. Việc hiểu hơn, quay lại bài học và giảm gián đoạn là **outcome** mà giải pháp chỉ có thể tác động, không thể bảo đảm.

### 2.4. Actor được xem xét

| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Lợi ích kỳ vọng |
|---|---|---|---|
| Học viên | Học hoặc ôn nội dung trực tuyến | Không hiểu một phần bài, phải chụp/chuyển nội dung sang AI hoặc tìm hiểu sau | Nhận hỗ trợ đúng ngữ cảnh và tiếp tục học |
| Giảng viên | Giảng dạy và giải đáp thắc mắc | Không thể hỗ trợ mọi học viên cùng lúc hoặc ngoài giờ | Biết điểm học viên thường mắc và giảm câu hỏi lặp lại |
| Lab Coach/TA | Hỗ trợ học viên trong giờ lab | Phản hồi có thể chậm khi nhiều người cùng cần hỗ trợ | Tập trung vào trường hợp cần hỗ trợ sâu hơn |

**Actor điều tra trước:** Học viên.

**Lý do:** Học viên trực tiếp gặp điểm kẹt, thực hiện workaround và chịu chi phí thời gian. Case A cũng yêu cầu người phù hợp là học viên từng không hiểu một phần bài học trực tuyến trong bảy ngày gần đây.

### 2.5. Situation & Job

P01 học khóa học trên V-Learn và có lúc không hiểu một phần slide. Người tham gia muốn hiểu nội dung để tiếp tục học. Cách xử lý hiện tại là chụp phần slide chưa hiểu, gửi cho AI, nói rõ mình chưa hiểu và đôi khi yêu cầu AI đưa ra lộ trình “cần hiểu gì trước”. Khi vấn đề khó, P01 ghi chú lại nội dung cần tìm hiểu, tiếp tục nghe giảng rồi quay lại sau.

**JTBD Hypothesis**

> Khi gặp một phần chưa hiểu trong bài học trực tuyến, tôi muốn xác định mình đang thiếu kiến thức gì và nhận hướng dẫn bám sát phần slide đó, để có thể tiếp tục học mà không bị gián đoạn lâu.

### 2.6. Hai Pain Hypothesis cạnh tranh

**Pain Hypothesis A — Khó chẩn đoán điểm thiếu kiến thức**

> Khi chưa hiểu một phần slide và không biết bắt đầu từ đâu, học viên phải tự mô tả vấn đề cho AI hoặc yêu cầu một lộ trình kiến thức. Vấn đề đơn giản có thể mất 5–10 phút; vấn đề phức tạp có thể mất vài giờ và phải xem lại sau.

**Pain Hypothesis B — Khó chuyển đúng ngữ cảnh từ V-Learn sang công cụ hỗ trợ**

> Việc chọn hoặc đánh dấu chính xác phần chưa hiểu trên V-Learn còn khó; AI đôi lúc không đọc được slide. Vì vậy người học phải chụp màn hình, dùng công cụ vẽ hoặc thử lại, làm tăng ma sát trước khi nhận được trợ giúp.

**Giả thuyết được điều tra tiếp:** Chưa loại trừ giả thuyết nào. Interview cho thấy cả khó khăn chẩn đoán lẫn ma sát chuyển ngữ cảnh. Cần phỏng vấn thêm và đo xem yếu tố nào gây chi phí lớn hơn.

### 2.7. Evidence Map

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
|---|---|---|
| Situation có thật | Người học kể được lần gần đây và phần nội dung cụ thể bị kẹt | Chỉ nói chung chung, không nhớ sự kiện |
| Workaround tồn tại | Chụp slide, hỏi AI, tìm nguồn ngoài, ghi chú để xem lại | Xử lý ngay trong bài mà không cần hành động thêm |
| Pain có ý nghĩa | Mất thời gian, phải hoãn việc tìm hiểu, ảnh hưởng mạch học | Chỉ là bất tiện nhỏ và được giải quyết ngay |
| Chẩn đoán là nút thắt | Không biết bắt đầu từ đâu, cần câu hỏi/lộ trình để lộ lỗ hổng kiến thức | Đã biết rõ câu hỏi và chỉ cần câu trả lời |
| Chuyển ngữ cảnh là nút thắt | Khó chọn/highlight, phải chụp màn hình, AI không đọc được slide | Công cụ luôn nhận đúng nội dung và ngữ cảnh |
| Pattern có lặp | Nhiều học viên có cùng trình tự và hậu quả | Chỉ là lỗi hiếm hoặc phụ thuộc một slide |

### 2.8. Evidence hiện có từ practice interview P01

- P01 đáp ứng recruitment check: trong bảy ngày gần đây đã gặp nội dung không hiểu khi học trực tuyến.
- Workaround được kể: chụp phần slide chưa hiểu, gửi cho AI và yêu cầu giải thích hoặc đưa ra lộ trình kiến thức.
- Vấn đề đơn giản mất khoảng **5–10 phút**; vấn đề phức tạp có thể mất **vài giờ** và phải xem lại ở nhà.
- Khi việc tìm hiểu kéo dài, P01 vẫn nghe giảng, ghi chú phần cần tìm hiểu rồi quay lại sau. Đây là **trì hoãn xử lý**, không đủ bằng chứng để kết luận bỏ học.
- Với khái niệm khó, tìm kiếm bên ngoài không nhất thiết giải quyết được ngay; khái niệm đơn giản có thể được làm rõ nhanh hơn.
- P01 đề xuất một cơ chế để nhập phần chưa hiểu, sau đó AI hỏi ngược, đánh giá câu trả lời đúng/đúng một phần và tiếp tục follow-up.
- Ma sát trên V-Learn: khó bôi đen/highlight đủ và chính xác; công cụ vẽ có thể không chuẩn; AI đôi lúc không đọc được slide.
- Interview không đo được số lần lặp lại và không xác định được một “nguyên nhân gốc” duy nhất.

### 2.9. Điều kiện để giả thuyết đứng vững hoặc bị sửa

Giả thuyết đứng vững hơn nếu nhiều học viên kể được cùng pattern: gặp điểm kẹt, không biết bắt đầu từ đâu hoặc không truyền được đúng ngữ cảnh, phải chuyển công cụ/ghi chú để xử lý sau và phát sinh thời gian đáng kể.

Giả thuyết cần sửa nếu phần lớn học viên giải quyết được ngay bằng công cụ hiện có, nếu lỗi đọc/highlight slide chỉ là sự cố hiếm, hoặc nếu vấn đề chủ yếu đến từ cấu trúc/chất lượng tài liệu.

### 2.10. Solution Parking Lot

| Hướng giải quyết có thể có | Loại | Nguồn |
|---|---|---|
| AI đặt câu hỏi ngắn để chẩn đoán điểm thiếu kiến thức rồi follow-up theo câu trả lời | AI | Người tham gia đề xuất |
| Trợ lý đọc trực tiếp phần slide được chọn và giải thích theo ngữ cảnh | AI | Suy ra từ workaround và lỗi đọc slide |
| Cải thiện thao tác chọn/highlight chính xác trên slide | Không bắt buộc AI | Người tham gia nêu pain |
| Bản đồ kiến thức tiên quyết giúp quay lại đúng khái niệm nền | AI hoặc rule-based | Suy ra từ nhu cầu “cần hiểu gì trước” |
| Hàng đợi để Lab Coach/TA phản hồi trường hợp khó | Không bắt buộc AI | Giải pháp thay thế cần kiểm tra |

Các hướng trên chưa được chứng minh. Đề xuất tính năng của P01 là **solution evidence**, không tự động chứng minh problem hypothesis.

## 3. Conversation Guide — phiên bản sau practice

### 3.1. Ba điều quan trọng nhất cần học

| Điều cần học | Evidence cần tìm | Điều khiến nhóm xem lại giả thuyết |
|---|---|---|
| Điểm kẹt xảy ra trong tình huống nào? | Lần gần nhất, mục tiêu, phần slide/khái niệm cụ thể | Không nhớ sự kiện hoặc chỉ nói chung |
| Người học thực sự xử lý thế nào? | Trình tự hành động, công cụ, thời gian, kết quả | Cách hiện tại xử lý nhanh, không gây bất tiện |
| Nút thắt nằm ở chẩn đoán hay truyền ngữ cảnh? | Không biết hỏi gì; hoặc biết rõ nhưng công cụ không nhận đúng nội dung | Cả hai đều không tạo chi phí đáng kể |

### 3.2. Tiêu chí tuyển người

Người đã có ít nhất một lần không hiểu một phần bài học trực tuyến trong bảy ngày gần đây và phải tìm cách xử lý.

**Recruitment check**

> Trong bảy ngày vừa rồi, bạn có lần nào đang học trực tuyến nhưng gặp một phần không hiểu và phải làm thêm một việc để xử lý không?

### 3.3. Lời mở đầu

> Bọn mình đang tìm hiểu cách học viên xử lý khi gặp nội dung khó hiểu trong quá trình học. Không có câu trả lời đúng hoặc sai; bọn mình muốn nghe trải nghiệm thực tế, không đánh giá năng lực học. Cuộc trao đổi khoảng 10–15 phút. Chỉ ghi âm khi bạn đồng ý và bản ghi chỉ được chia sẻ với người chấm theo phạm vi đã thống nhất.

### 3.4. Story opener

> Bạn kể lại lần gần nhất bạn đang học trực tuyến và gặp một phần không hiểu được không? Phần đó là gì và lúc ấy bạn đang cố hoàn thành việc gì?

### 3.5. Big 3 Questions

1. Ngay khi nhận ra mình chưa hiểu, bạn đã làm gì? Hãy kể từng bước.
2. Mỗi bước mất bao lâu và kết quả ra sao? Cuối cùng bạn quay lại bài học lúc nào?
3. Phần khó nhất trong quá trình đó là xác định mình cần hỏi gì, đưa đúng nội dung cho công cụ, hay điều gì khác?

### 3.6. Probe bank

- Bạn có thể chỉ rõ đoạn slide/khái niệm gây vướng không?
- Sau đó chuyện gì xảy ra?
- Vì sao bạn chọn cách đó?
- Bạn đã dùng nguồn hoặc công cụ nào?
- Công cụ có hiểu đúng phần nội dung bạn đưa vào không?
- Bạn có phải viết lại bối cảnh hoặc thử lại không?
- Bạn mất khoảng bao lâu trước khi tiếp tục bài?
- Nếu chưa giải quyết ngay, bạn đã làm gì với phần đó?
- Lần gần nhất trước đó xảy ra khi nào?
- Có trường hợp nào cách hiện tại giải quyết vấn đề ngay và không làm bạn gián đoạn không?

### 3.7. Tự rà soát

- Không gợi sẵn “AI Tutor”, nút “Tôi vẫn chưa hiểu” hoặc nguyên nhân thiếu hỗ trợ.
- Không hỏi dồn nhiều giả định trong một câu.
- Neo câu hỏi vào một sự kiện đã xảy ra.
- Tách hành vi/lời nói của người tham gia khỏi diễn giải của nhóm.
- Chỉ hỏi ý tưởng giải pháp ở cuối và ghi rõ đó là solution evidence.
- Luôn hỏi một câu có thể làm giả thuyết yếu đi.

### 3.8. Điều chỉnh sau buổi luyện

- Bổ sung probe yêu cầu chỉ rõ phần slide hoặc khái niệm cụ thể.
- Tách thời gian cho vấn đề đơn giản và phức tạp; không biến 5–10 phút thành con số áp dụng cho mọi trường hợp.
- Hỏi rõ người học trì hoãn xử lý hay bỏ dở bài.
- Phân biệt hai nút thắt: chẩn đoán kiến thức thiếu và truyền đúng ngữ cảnh slide.
- Chuyển câu hỏi về tính năng xuống cuối để tránh dẫn dắt.
- Bổ sung câu hỏi phản chứng về trường hợp công cụ hiện tại đã xử lý nhanh.

## 4. Practice Reflection

### 4.1. Câu hỏi nào giúp người tham gia kể tình huống thực tế?

Recruitment check về “bảy ngày vừa rồi” xác nhận tình huống gần đây. Câu hỏi “lần gần nhất… bạn đã giải quyết như thế nào?” giúp lấy được chuỗi hành vi: chụp slide, gửi cho AI và xin lộ trình khi không biết bắt đầu từ đâu. Câu hỏi về thời gian cũng làm lộ hai mức độ: 5–10 phút với nội dung đơn giản và vài giờ với nội dung phức tạp.

### 4.2. Chỗ nào cần làm tốt hơn ở lần phỏng vấn tiếp theo?

Interviewer chuyển sang giải pháp quá sớm và có câu dẫn dắt như hỏi liệu khó khăn có phải do “thiếu cái đấy” hay không. Một số câu hỏi chứa nhiều ý và không đào sâu đúng một sự kiện cụ thể. Interview chưa hỏi rõ phần slide/khái niệm nào gây vướng, số lần lặp lại, kết quả cuối cùng của lần gần nhất, hoặc trường hợp đối chứng khi công cụ hiện tại hoạt động tốt. Lần sau cần hỏi từng bước, im lặng để người tham gia kể, và tách problem evidence khỏi góp ý tính năng.

### 4.3. Nhóm đã sửa Conversation Guide ở đâu và vì sao?

Guide được bổ sung câu hỏi về nội dung cụ thể, trình tự hành động, thời gian của từng bước, thời điểm quay lại bài và nút thắt chẩn đoán so với truyền ngữ cảnh. Câu hỏi giải pháp được chuyển xuống cuối. Các thay đổi này nhằm thu được evidence có thể kiểm chứng và tránh suy diễn từ mong muốn tính năng thành xác nhận nguyên nhân.

## 5. AI Support Log

### AI đã hỗ trợ gì?

- Chuẩn hóa transcript đã được người thực hiện cung cấp, giữ timestamp và đánh dấu `[không rõ]`.
- Đối chiếu transcript với bản bài nộp cũ để tìm chi tiết không có nguồn.
- Chuyển evidence có thật thành Interview Record, Evidence Map và hypothesis cần kiểm tra tiếp.
- Rà soát Conversation Guide để giảm câu hỏi dẫn dắt và phân biệt problem evidence với solution evidence.
- Chuẩn hóa cách trình bày Markdown.

### Điểm AI có thể sai hoặc hời hợt

- AI có thể nghe/diễn giải sai các đoạn âm thanh không rõ; các đoạn này được giữ nhãn `[không rõ]` thay vì đoán.
- AI không được phép biến đề xuất tính năng thành bằng chứng xác nhận nguyên nhân gốc.
- AI không thể tự xác minh danh tính, consent hoặc quyền chia sẻ bản ghi.
- Một cuộc phỏng vấn ngắn chưa đủ để kết luận pattern trên nhiều học viên.

### Cách người thực hiện đã kiểm tra và sửa

- Cung cấp transcript có timestamp và file ghi âm gốc dài 03:59.
- Loại bỏ các chi tiết không có trong bản ghi: “3 lần”, “phỏng vấn viết”, “kích đúp”, quote về Google và kết luận nguyên nhân duy nhất là thiếu hỗ trợ tức thời.
- Giữ đúng phạm vi evidence: 5–10 phút cho trường hợp dễ; vài giờ với trường hợp phức tạp; có thể ghi chú và tìm hiểu sau.
- Không đưa file ghi âm lên repo công khai. Recording link riêng tư và consent vẫn phải được người thực hiện hoàn tất trước khi nộp nếu rubric yêu cầu.

## Nguồn tham khảo

- VLearn — Day 17: Finding and Validating Pain Points.
- [Day 17 — Reverse the Pain Point](https://track1-product.vercel.app/days/17), dùng để tham khảo cấu trúc hypothesis và solution options.
- `interview/notes.md` — Interview Record P01 dựa trên bản ghi.
- `interview/transcript.md` — Transcript có timestamp; đoạn không rõ được đánh dấu rõ ràng.
