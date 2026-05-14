---
artifact: 03-takenotes — Quan sát cá nhân sau phần chia sẻ nhóm khác
bai-tap: 3 — Quan sát + rút ra bài học (cá nhân)
phase: Sau phần shareout của các nhóm
time: 15 phút (xem deck slide 4 để biết khung giờ chính xác)
input: Phần thuyết trình của ít nhất 2 nhóm khác trên lớp
nop-cuoi: Có — file cuối Lab 3 (cá nhân)
---

# 03 — Take notes: quan sát + bài học cá nhân

Đây là phần cá nhân. Sau khi nhóm bạn trình bày Lab 2 và nghe ít nhất 2 nhóm khác chia sẻ Analysis Report của họ, bạn ghi lại quan sát + bài học của riêng mình vào file này.

Mục tiêu: rèn kỹ năng nghe, đối chiếu, và rút ra bài học từ phân tích của người khác — không chỉ từ phân tích của chính nhóm mình.

Quy tắc khi viết:

- Trích dẫn cụ thể tên sản phẩm + nhóm đã quan sát (không nói chung chung).
- Bằng chứng yếu / lập luận lỏng cần chỉ rõ chỗ nào trong slide deck của nhóm khác.
- Câu hỏi đặt cho nhóm khác phải gắn với bằng chứng cụ thể từ phần trình bày của họ.

---

## Thông tin

- **Mã học viên**: 2A202600486
- **Họ tên**: Nguyen Tien Huy Hoang
- **Ngày**: 2026-05-14
- **Nhóm Lab 2 của tôi**: Perplexity vs ChatGPT Search trong ngành Tìm kiếm

---

## Phần 1 — Nhóm đã quan sát (≥ 2 nhóm khác)

| # | Tên nhóm / mã 2 học viên | Ngành | 2 sản phẩm họ test |
|---|---|---|---|
| 1 | Nhóm GitHub Copilot | B — Lập trình | GitHub Copilot vs Cursor |
| 2 | Nhóm Notion AI | C — Viết lách | Notion AI vs Gamma.app |
| 3 | (tuỳ chọn) Nhóm Midjourney | D — Thiết kế | Midjourney vs Adobe Firefly |

---

## Phần 2 — Điều thấy hay từ nhóm khác

Góc nhìn / framework / case study mà nhóm khác đưa ra mà nhóm mình chưa nghĩ tới.

**Quan sát 1** (từ nhóm: GitHub Copilot):

- Cụ thể họ đưa ra: Nhóm dùng framework "Tab Completion Rate" — đo tỷ lệ lần Cursor đề xuất code và developer bấm Tab chấp nhận (acceptance rate). GitHub Copilot ~27%, Cursor ~35% trong bài test của họ. Đây là metric tôi chưa dùng khi phân tích Perplexity vs ChatGPT Search.
- Vì sao tôi thấy hay: Acceptance rate là behavioral proxy mạnh hơn "tôi thấy hay" — nó đo trust bằng hành động thực tế (Tab key) chứ không phải cảm nhận chủ quan. Khi nhóm tôi nói Perplexity "tạo trust mạnh hơn", tôi chỉ dùng trust signals định tính. Nếu có metric tương tự (ví dụ: tỷ lệ lần user click citation để verify), lập luận sẽ chặt hơn nhiều.

**Quan sát 2** (từ nhóm: Notion AI):

- Cụ thể họ đưa ra: Nhóm phân tích **switching cost** bằng cách đo thời gian "onboarding" — mất bao lâu để user mới tạo được 1 bài trình bày có chất lượng trên Gamma (3 phút) vs Notion AI (8 phút, vì phải biết block system trước). Đây là cách quantify friction cụ thể hơn cách tôi đã làm (chỉ đếm số click).
- Vì sao tôi thấy hay: Đo thời gian thực tế (minutes to first value) là metric onboarding chuẩn trong product management. Nhóm tôi đã đo "số bước" (2 bước vs 4 bước) nhưng không đo thời gian thực — đây là gap rõ ràng cần bổ sung vào phân tích S2 nếu làm lại.

---

## Phần 3 — Điểm yếu / chỗ chưa thuyết phục

Bằng chứng yếu, lập luận lỏng, framework dùng sai. Chỉ rõ chỗ nào trong slide deck của nhóm khác.

**Điểm yếu 1** (từ nhóm: GitHub Copilot):

- Cụ thể: Slide S5.4 (Moat Analysis) của nhóm ghi Cursor có "Network Effect: Mạnh" vì "nhiều developer dùng thì Cursor cải thiện nhanh hơn". Lập luận này lẫn lộn Data Flywheel với Network Effect.
- Bằng chứng gì còn thiếu: Network Effect thực sự đòi hỏi giá trị của Cursor cho user A phải tăng khi user B join — điều này chỉ đúng nếu Cursor có social/sharing feature (code review, shared snippets). Nhóm chưa chứng minh được cơ chế này tồn tại trong Cursor.
- Tôi sẽ đề xuất họ làm thêm gì: Phân tách rõ "Data Flywheel" (nhiều user → model tốt hơn → cải thiện output) vs "Network Effect" (nhiều user → giá trị tăng cho từng user do interaction). Cursor hiện tại có Data Flywheel, chưa chắc có Network Effect.

**Điểm yếu 2** (từ nhóm: Notion AI):

- Cụ thể: Slide S5.7 (Spark → Loop → System) nhóm xếp Gamma.app ở giai đoạn "System" vì "được nhiều người dùng". Tuy nhiên Gamma chỉ có 10 triệu users (theo số liệu họ nêu) — so với định nghĩa "System" thường gắn với dominant market position và moat dày, 10M users trong category presentation tool là Loop chứ không phải System.
- Bằng chứng gì còn thiếu: Để gọi là System cần chứng minh: (1) market share dominant trong niche, hoặc (2) switching cost/moat đủ dày để block competitor mới. Nhóm chưa cung cấp so sánh market share Gamma vs Canva AI vs Beautiful.ai.
- Tôi sẽ đề xuất họ làm thêm gì: Dùng mốc so sánh cụ thể: Canva (125M users) là System, Gamma (10M) là Loop đang tăng trưởng. Verdict "System" cần được defend bằng moat analysis ở S5.4.

---

## Phần 4 — Câu hỏi đặt cho nhóm khác

Câu hỏi gắn với bằng chứng cụ thể, không hỏi chung chung.

- Cho nhóm GitHub Copilot: Slide S2 của nhóm so sánh Cursor và GitHub Copilot trên cùng bài test coding. Khi Cursor có acceptance rate 35% và Copilot 27%, liệu nhóm có kiểm soát được biến "độ khó task" không? Task càng phức tạp thì acceptance rate thường thấp hơn — nếu nhóm test task đơn giản hơn trên Cursor và task khó hơn trên Copilot, con số 35% vs 27% có thể bị skewed.
- Cho nhóm Notion AI: Slide S5.8 của nhóm liên hệ Notion AI với case disruption của Figma bị Adobe mua lại. Nhóm nói Gamma có rủi ro tương tự — bị Canva "buy or copy". Nhưng trong case Chegg (Lab 1 của tôi), disruption đến từ nền tảng AI tổng quát (ChatGPT), không phải từ M&A. Nhóm có thể phân tích thêm: kịch bản nào có xác suất cao hơn với Gamma — bị Canva copy, hay bị ChatGPT thêm "presentation mode" trực tiếp?
- (Tuỳ chọn) Cho nhóm Midjourney: Slide S3 về trust signals — nhóm ghi Adobe Firefly có "Disclaimer khi không chắc: Có" vì có watermark "AI-generated". Nhưng watermark là compliance feature (EU AI Act) chứ không phải trust signal theo nghĩa "AI tự nhận ra giới hạn của mình". Nhóm có thể phân tách 2 loại trust signal này để tránh nhầm lẫn khi đánh giá Product vs Regulatory compliance.

---

## Phần 5 — Điều tôi rút ra cho bản thân

Bài học cụ thể tôi sẽ áp dụng vào lần phân tích sản phẩm AI tiếp theo. Không viết câu chung chung như "tôi học được nhiều" — cụ thể về phương pháp, bằng chứng, hoặc framework.

**Bài học 1**:

- Tôi sẽ làm khác lần sau: Thêm 1 behavioral metric đo trust bằng hành động (không chỉ cảm nhận). Ví dụ: với Perplexity vs ChatGPT Search, đo "% lần user click citation để verify" hoặc "thời gian từ lúc có output đến khi user tin và copy".
- Lý do: Nhóm GitHub Copilot cho thấy acceptance rate là metric mạnh hơn nhiều so với "tôi cảm thấy trust hơn". Trong bài phân tích của tôi, trust analysis (S3) chủ yếu là định tính — nếu có thêm 1 số đo hành vi, verdict ở S5.1 sẽ có nền tảng thuyết phục hơn nhiều.

**Bài học 2**:

- Tôi sẽ làm khác lần sau: Phân tách rõ Data Flywheel vs Network Effect vs Switching Cost khi phân tích moat (S5.4). Ba khái niệm này khác nhau về cơ chế và thường bị dùng lẫn nhau.
- Lý do: Nhóm GitHub Copilot nhầm Data Flywheel với Network Effect ở slide moat analysis. Sau khi nghe giải thích, tôi nhận ra bài phân tích của nhóm tôi cũng có nguy cơ tương tự — tôi ghi ChatGPT có "Network Effect: Mạnh" vì "200M users feed RLHF" nhưng chưa chứng minh được cơ chế người dùng A và người dùng B tạo ra giá trị lẫn nhau (chứ không chỉ feed data cho OpenAI). Lần sau cần define rõ cơ chế trước khi label "Network Effect".

**Bài học 3** (tuỳ chọn):

- Khi dùng Spark → Loop → System framework, phải có anchor point so sánh market size — không thể gọi 1 sản phẩm là "System" chỉ dựa vào số lượng user tuyệt đối mà không so với dominant player trong niche. Gamma có 10M users là ấn tượng, nhưng Canva có 125M users trong cùng category — trong bối cảnh đó, Gamma đang ở Loop stage tăng trưởng, chưa phải System.

---

## Checklist trước khi nộp

- [x] Phần 1 ghi rõ ≥ 2 nhóm đã quan sát (mã 2 học viên + ngành + sản phẩm).
- [x] Phần 2 có ≥ 2 quan sát hay, gắn với nhóm cụ thể.
- [x] Phần 3 có ≥ 2 điểm yếu / câu hỏi chưa được trả lời.
- [x] Phần 4 có ≥ 2 câu hỏi cụ thể cho nhóm khác.
- [x] Phần 5 có ≥ 2 bài học rút ra, kèm lý do và cách áp dụng lần sau.
