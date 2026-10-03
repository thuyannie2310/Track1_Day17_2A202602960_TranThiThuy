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

> Trạng thái nghiên cứu: Đây là buổi luyện problem interview. Kết quả dưới đây là hypothesis và practice evidence, chưa phải validation.

## 2. Problem Hypothesis Brief

### 2.1. Solution directive

Thêm nút “Tôi vẫn chưa hiểu” vào bài học. Khi học viên chủ động yêu cầu trợ giúp, AI Tutor sử dụng nội dung bài hiện tại, các câu trả lời gần đây và lịch sử học tập để đặt một số câu hỏi chẩn đoán, lựa chọn kiến thức nền cần ôn, giải thích ngắn và đưa học viên trở lại bài đang học.

### 2.2. Capability trung tính

Giúp học viên xác định điểm kiến thức đang gây vướng mắc và nhận được hướng dẫn phù hợp với ngữ cảnh ngay trong lúc học, để họ có thể tiếp tục mà không phải tự tìm kiếm qua nhiều nguồn.

### 2.3. Chuỗi thay đổi kỳ vọng

```text
Hỗ trợ đúng thời điểm và đúng ngữ cảnh
→ học viên xác định rõ điểm đang thiếu kiến thức
→ nhận được phần giải thích hoặc kiến thức nền phù hợp
→ giảm thời gian tìm kiếm bên ngoài
→ quay lại bài học sớm hơn và duy trì mạch học
```

Phần giải thích là **output** của giải pháp. Việc học viên hiểu hơn, tiếp tục học và giảm gián đoạn là **outcome** mà giải pháp chỉ có thể tác động, không thể bảo đảm.

### 2.4. Actor được xem xét

| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Lợi ích kỳ vọng |
|---|---|---|---|
| Học viên | Học hoặc ôn lại nội dung trực tuyến | Không hiểu một phần bài, phải tìm nguồn ngoài, bị ngắt mạch | Nhận hỗ trợ đúng lúc và tiếp tục học |
| Giảng viên | Giảng dạy và giải đáp thắc mắc | Không thể hỗ trợ đồng thời hoặc ngoài giờ | Giảm câu hỏi lặp lại, biết điểm học viên thường mắc |
| Lab Coach/TA | Hỗ trợ học viên trong giờ lab | Bận hỗ trợ nhiều người, phản hồi có độ trễ | Tập trung vào trường hợp cần hỗ trợ sâu hơn |

**Actor điều tra trước:** Học viên.

**Lý do:** Học viên là người trực tiếp trải nghiệm điểm kẹt, thực hiện workaround và chịu chi phí thời gian. Case A cũng quy định người phù hợp là học viên từng không hiểu một phần bài học trong bảy ngày gần đây.

### 2.5. Situation & Job

Khi đang học hoặc ôn lại một bài trực tuyến và gặp một khái niệm, logic hoặc mối liên hệ chưa hiểu, học viên đang cố làm rõ nội dung để tiếp tục học. Hiện tại họ thường đọc lại slide, tìm kiếm bên ngoài, hỏi AI, hỏi bạn học hoặc chờ giảng viên/Lab Coach phản hồi.

**JTBD Hypothesis**

> Khi gặp một phần chưa hiểu trong lúc học trực tuyến, tôi muốn xác định đúng điểm mình đang thiếu và nhận được lời giải thích phù hợp với ngữ cảnh, để có thể tiếp tục học mà không bị gián đoạn lâu.

### 2.6. Hai Pain Hypothesis cạnh tranh

**Pain Hypothesis A — Thiếu hỗ trợ tức thời**

> Khi gặp nội dung chưa hiểu trong lúc học trực tuyến, học viên khó nhận được hỗ trợ tức thời và đúng ngữ cảnh, nên phải chuyển sang tìm kiếm bên ngoài trong khoảng 5–10 phút, làm gián đoạn mạch học.

**Pain Hypothesis B — Nội dung học chưa đủ khả năng tự giải thích**

> Khi gặp slide dài, cô đọng hoặc nhiều thuật ngữ, học viên khó xác định và hiểu phần kiến thức cần thiết vì tài liệu thiếu cấu trúc, lời giảng hoặc ví dụ, dẫn đến phải tự tổng hợp lại nội dung.

**Giả thuyết được điều tra trước:** Pain Hypothesis A.

**Lý do:** Evidence từ P01 cho thấy tình huống đã lặp lại ba lần gần đây. Mỗi lần tìm kiếm bên ngoài mất khoảng 5–10 phút và làm gián đoạn việc học. P01 xác định nguyên nhân chính là thiếu hỗ trợ tức thời. Tuy nhiên, Pain Hypothesis B vẫn được giữ làm cách giải thích cạnh tranh.

### 2.7. Evidence Map

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
|---|---|---|
| Situation có thật | Người học kể được một sự kiện gần đây và điểm bị kẹt cụ thể | Chỉ nói chung chung hoặc không nhớ sự kiện |
| Pain có ý nghĩa | Mất thời gian, gián đoạn, ảnh hưởng bài tập hoặc phần học sau | Chỉ là bất tiện nhỏ và xử lý ngay bằng cách hiện có |
| Workaround tồn tại | Đọc lại, tìm Google, hỏi AI/người khác hoặc chờ hỗ trợ | Không cần thực hiện thêm hành động nào |
| Consequence tồn tại | Mất 5–10 phút, đứt mạch học, bỏ qua hoặc phải quay lại | Không phát sinh thời gian hoặc ảnh hưởng đáng kể |
| Pattern có lặp | Xảy ra nhiều lần trong thời gian gần đây | Sự cố hiếm và không lặp lại |

### 2.8. Evidence hiện có từ practice interview

- P01 đáp ứng tiêu chí tuyển người và đã gặp tình huống trong bảy ngày gần đây.
- Tình huống tương tự xảy ra **3 lần**.
- Mỗi lần tìm kiếm bên ngoài mất khoảng **5–10 phút**.
- P01 không bỏ dở bài nhưng bị gián đoạn tạm thời.
- Tìm kiếm bên ngoài có thể trả về kết quả rộng và thiếu ngữ cảnh.
- Có trường hợp xử lý nhanh khi P01 kích đúp vào nội dung và nhận được giải thích kèm ví dụ dễ hiểu.
- Evidence này làm giả thuyết cụ thể hơn: pain quan sát được là **gián đoạn và tốn thời gian**, chưa phải bỏ học.

### 2.9. Điều kiện để giả thuyết đứng vững hoặc bị sửa

Giả thuyết đứng vững hơn nếu nhiều học viên kể được sự kiện gần đây có cùng pattern: gặp điểm kẹt, không có hỗ trợ đúng lúc, phải chuyển sang nguồn ngoài, phát sinh thời gian và đứt mạch học.

Giả thuyết cần sửa hoặc bác bỏ nếu phần lớn học viên xử lý được ngay bằng công cụ hiện có, không thấy gián đoạn đáng kể, hoặc nguyên nhân chính là chất lượng/cấu trúc tài liệu chứ không phải thiếu hỗ trợ tức thời.

### 2.10. Solution Parking Lot

| Hướng giải quyết có thể có | Loại |
|---|---|
| AI đặt câu hỏi ngắn để chẩn đoán điểm thiếu kiến thức rồi gợi ý phần ôn phù hợp | AI |
| Trợ lý giải thích theo ngữ cảnh, kèm nguồn từ slide/bài học | AI |
| Bản đồ kiến thức tiên quyết giúp học viên quay lại đúng khái niệm nền | AI hoặc rule-based |
| Hộp hỏi ẩn danh và hàng đợi để Lab Coach/TA phản hồi | Không bắt buộc AI |
| Thiết kế lại slide với mục lục, glossary và ví dụ đã được giảng viên kiểm duyệt | Không sử dụng AI |

Không hướng nào trong Parking Lot được coi là giải pháp đã được chứng minh.

## 3. Conversation Guide — phiên bản cuối

### 3.1. Ba điều quan trọng nhất cần học

| Điều cần học | Evidence cần tìm | Điều khiến nhóm xem lại giả thuyết |
|---|---|---|
| Điểm kẹt có xảy ra trong một tình huống thật không? | Một câu chuyện gần đây, mục tiêu và điểm bắt đầu vướng cụ thể | Không nhớ sự kiện hoặc chỉ trả lời chung chung |
| Người học thực sự xử lý thế nào? | Trình tự hành động, nguồn đã dùng, thời gian và kết quả | Cách hiện tại xử lý nhanh và không gây bất tiện |
| Pain có đủ ý nghĩa và lặp lại không? | Tần suất, chi phí thời gian và hậu quả quan sát được | Hiếm xảy ra hoặc bỏ qua mà không có hậu quả |

### 3.2. Tiêu chí tuyển người

Người đã có ít nhất một lần không hiểu một phần bài học trực tuyến trong bảy ngày gần đây và đã phải tìm cách xử lý.

**Recruitment check**

> Trong bảy ngày vừa rồi, bạn có lần nào đang học trực tuyến nhưng gặp một phần không hiểu và phải tìm cách xử lý không?

### 3.3. Lời mở đầu

> Bọn mình đang tìm hiểu cách học viên xử lý khi gặp nội dung khó hiểu trong quá trình học. Không có câu trả lời đúng hoặc sai; bọn mình muốn nghe về trải nghiệm thực tế, không phải đánh giá năng lực học của bạn. Nếu thực hiện phỏng vấn bằng lời nói, cuộc trao đổi kéo dài khoảng 15 phút và chỉ được ghi âm sau khi bạn đồng ý. Bản ghi chỉ phục vụ bài học và không được chia sẻ công khai.

### 3.4. Story opener

> Bạn kể cho mình nghe về lần gần nhất bạn đang học nhưng gặp một phần không hiểu được không?

### 3.5. Big 3 Questions

1. **Lúc đó bạn đang cố hoàn thành việc gì, và đến điểm nào bạn nhận ra mình chưa hiểu?**
2. **Ngay sau khi nhận ra mình chưa hiểu, bạn đã làm gì? Hãy kể lần lượt các bước.**
3. **Việc đó ảnh hưởng như thế nào đến quá trình học của bạn?**

### 3.6. Probe bank

- Chuyện gì xảy ra tiếp theo?
- Trong chính lần gần nhất đó, bạn đã làm gì?
- Vì sao bạn chọn cách đó?
- Bạn đã thử nguồn, công cụ hoặc nhờ người nào?
- Bạn mất khoảng bao lâu?
- Cách đó có giúp bạn tiếp tục bài học không?
- Lần gần nhất trước đó xảy ra khi nào?
- Có lần nào bạn chưa hiểu nhưng bỏ qua và sau đó không gặp ảnh hưởng đáng kể không?
- Có trường hợp nào cách hiện tại đã giải quyết vấn đề rất nhanh không?

### 3.7. Tự rà soát

- Không nhắc đến “AI Tutor” hoặc nút “Tôi vẫn chưa hiểu”.
- Không hỏi “Bạn có dùng/thích/muốn tính năng này không?”.
- Mỗi câu hỏi neo vào một sự kiện đã xảy ra.
- Tách hành vi và lời nói của user khỏi diễn giải của nhóm.
- Luôn hỏi một câu có thể làm giả thuyết yếu đi.

### 3.8. Điều chỉnh sau buổi luyện

Guide ban đầu tập trung vào việc người học có bị kẹt hay không. Sau practice interview, guide được sửa để:

- Hỏi thời gian xử lý cụ thể thay vì chỉ hỏi “có mất thời gian không?”.
- Tìm cả workaround hiệu quả, không chỉ thu thập trường hợp thất bại.
- Phân biệt “bỏ dở bài” với “gián đoạn tạm thời”.
- Bổ sung câu hỏi đáng sợ về trường hợp không hiểu nhưng bỏ qua mà không có hậu quả.
- Không mặc định nguyên nhân là slide hoặc thiếu AI; yêu cầu người tham gia mô tả hành vi trước.

## 4. Practice Reflection

### 4.1. Câu hỏi nào đã giúp người tham gia kể tình huống cụ thể?

“Bạn kể cho mình nghe về lần gần nhất bạn đang học nhưng gặp một phần không hiểu được không?” giúp neo câu trả lời vào một sự kiện đã xảy ra. Câu hỏi tiếp theo “Bạn đã làm gì ngay sau đó?” giúp lấy được workaround thay vì ý kiến chung về sản phẩm.

### 4.2. Chỗ nào cần làm tốt hơn ở lần phỏng vấn thật?

Hình thức viết bất đồng bộ hạn chế khả năng hỏi tiếp ngay khi xuất hiện chi tiết đáng chú ý. Lần sau cần thực hiện phỏng vấn đồng bộ, xin phép ghi âm và đào sâu trình tự hành động, thời gian, nguồn đã sử dụng và kết quả của từng bước. Interviewer cũng cần tránh suy diễn “gián đoạn” thành “bỏ dở” khi người tham gia không nói như vậy.

### 4.3. Nhóm đã sửa Conversation Guide ở đâu và vì sao?

Nhóm bổ sung câu hỏi về thời gian cụ thể, tần suất, workaround đã giải quyết nhanh và trường hợp pain không gây hậu quả. Những thay đổi này giúp guide thu được cả evidence ủng hộ lẫn evidence làm giả thuyết yếu đi, đồng thời tách rõ pain “mất 5–10 phút và bị ngắt mạch” khỏi kết luận mạnh hơn nhưng chưa có dữ liệu như “bỏ học”.

## 5. AI Support Log

### AI đã hỗ trợ gì?

- Rà soát yêu cầu của lab và cấu trúc repo.
- Chuyển dữ liệu đã được người thực hiện xác nhận thành Problem Hypothesis Brief, Evidence Map, Conversation Guide và Interview Record.
- Kiểm tra các câu hỏi có làm lộ solution hoặc hỏi dự đoán tương lai hay không.
- Tách fact, diễn giải và khoảng trống evidence.
- Chuẩn hóa cách trình bày Markdown.

### Điểm AI có thể sai hoặc hời hợt

- AI ban đầu không biết ngày thu thập, tần suất, thời gian xử lý và hậu quả cụ thể.
- AI có nguy cơ suy diễn rằng người học bỏ dở bài, trong khi fact được xác nhận là chỉ gián đoạn tạm thời.
- AI không thể tự xác minh consent, danh tính người tham gia hoặc sự tồn tại của bản ghi.
- AI không được dùng để tạo quote, hành vi hoặc interview data mới.

### Cách người thực hiện đã kiểm tra và sửa

- Xác nhận ngày thu thập là 03/10/2026.
- Xác nhận tình huống xảy ra trong bảy ngày gần đây và lặp lại ba lần.
- Bổ sung chi phí thời gian 5–10 phút cho mỗi lần tìm kiếm bên ngoài.
- Sửa hậu quả từ “có thể bỏ dở” thành “không bỏ dở nhưng bị gián đoạn tạm thời”.
- Bổ sung workaround hiệu quả: kích đúp vào nội dung để nhận giải thích kèm ví dụ.
- Xác nhận nguyên nhân chính theo P01 là thiếu hỗ trợ tức thời.

## Nguồn tham khảo

- VLearn — Day 17: Finding and Validating Pain Points.
- [Day 17 — Reverse the Pain Point](https://track1-product.vercel.app/days/17), dùng để tham khảo các cụm pain và solution options. Evidence P01 trong bài này được ghi theo xác nhận của người thực hiện.
