# 01 — Individual Problem Scan

## Thông tin cá nhân

- Họ và tên: [Điền Họ và Tên của bạn]
- Mã học viên: [Điền Mã học viên]
- Vai trò / bối cảnh: Sinh viên năm cuối ngành Công nghệ thông tin / Kỹ thuật Dữ liệu & AI, Thực tập sinh Kỹ thuật Dữ liệu/NLP.
- Công việc hằng tuần:
  - Khảo sát tài liệu nghiên cứu, đọc các bài báo (paper) chuyên ngành AI/ML để tìm baseline và phương pháp cải tiến mô hình.
  - Xử lý, làm sạch và gán nhãn sơ bộ các tập dữ liệu thô (văn bản tin tức, chuỗi thời gian tài chính).
  - Viết code pipeline huấn luyện mô hình, tinh chỉnh siêu tham số và theo dõi các chỉ số đánh giá (loss, accuracy, F1, AUC).
  - Thảo luận tiến độ, giải quyết lỗi kỹ thuật và cập nhật task hàng tuần trên kênh Discord/Slack của nhóm.

---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | **Tốn thời gian** | Đọc và trích xuất thủ công các thông số mô hình, metric đánh giá (F1, AUC, accuracy) từ paper học thuật 10–15 trang vào bảng benchmark. | Sinh viên làm đồ án, nghiên cứu sinh | Bấm giờ mất 90–120 phút/paper; mỗi tuần đọc 2–3 paper; dễ sót baseline cũ hoặc nhầm số liệu giữa các ablation studies. |
| 2 | **Lặp lại** | Viết nhật ký thí nghiệm (experiment log summary) tổng hợp từ các lần train model (loss, epoch, siêu tham số, ghi chú thay đổi) vào báo cáo tuần. | Sinh viên, kỹ sư ML | Diễn ra đều đặn 1 lần/tuần, mất 45–60 phút/lần copy-paste từ wandb/terminal log sang file Docs/Markdown. |
| 3 | **Pain từ người khác** | Thành viên trong nhóm dự án không đồng bộ môi trường (CUDA version, thư viện Python), liên tục hỏi lại cách cấu hình để chạy thử code. | Thành viên phụ trách kỹ thuật (lead dev) và người mới vào nhóm | Trung bình 3–4 lần/tuần, mỗi lần mất 20–30 phút gọi video hoặc chat để gỡ lỗi "chạy được trên máy tôi nhưng crash trên máy bạn". |
| 4 | **AI có thể tốt hơn** | Tìm kiếm lại các quyết định kỹ thuật, link tài liệu hoặc code mẫu đã thống nhất từ các tuần trước trong kênh Discord/Slack bị trôi tin nhắn. | Tất cả thành viên nhóm dự án (3–5 người) | Mất 15–25 phút/lần tìm kiếm; trung bình có 2 câu hỏi/tuần: "Tuần trước thống nhất dùng module nào/link repo ở đâu ấy nhỉ?". |
| 5 | **Lặp lại** | Gán nhãn sơ bộ (data annotation/labeling) sắc thái hoặc phân loại chủ đề cho tập dữ liệu văn bản thô phục vụ bài toán NLP. | Người xử lý dữ liệu (data annotator / sinh viên) | Thực hiện 1–2 lần/tháng, mỗi batch 300–500 mẫu, mất 3–4 tiếng bấm tay liên tục, dễ giảm độ tập trung và mất nhất quán ở các mẫu cuối. |
| 6 | **Tốn thời gian** | Chuyển đổi công thức toán phức tạp và cấu trúc bảng từ PDF bài báo sang cú pháp LaTeX/Markdown để đưa vào báo cáo đồ án. | Sinh viên viết đồ án / báo cáo khoa học | Mất 30–40 phút cho mỗi trang lý thuyết; thường xuyên gõ sai ký hiệu Hy Lạp, thiếu ngoặc hoặc lệch chỉ số trên/dưới. |
| 7 | **Pain từ người khác** | Bạn cùng nhóm nộp Pull Request hoặc gửi file code nhưng không có chú thích (docstrings, kiểu dữ liệu, giải thích luồng), người review phải đọc lại từ đầu. | Người review code / trưởng nhóm kỹ thuật | Tần suất 2–3 PR/tuần; thời gian review kéo dài từ 15 phút lên 45 phút/PR vì phải liên tục nhắn tin hỏi lại ý đồ xử lý. |
| 8 | **Lặp lại** | Soạn tóm tắt nội dung cuộc họp nhóm (meeting notes) và danh sách việc cần làm (action items) sau mỗi buổi thảo luận sprint cuối tuần. | Nhóm trưởng / người chủ trì họp | Mất 25–35 phút sau mỗi cuộc họp 1 tiếng để nghe lại ghi chú và sắp xếp task vào Trello/Notion. |
| 9 | **AI có thể tốt hơn** | Lọc và phân loại các thông báo lỗi runtime/biên dịch phức tạp (traceback dài nhiều tầng) để xác định đúng dòng code gốc gây lỗi thay vì đọc từng dòng log thư viện. | Lập trình viên mới / sinh viên debug | Gặp 5–7 lần/tuần, tốn 15–30 phút/lỗi chỉ để dò qua hàng chục dòng exception của framework trung gian. |
| 10 | **Tốn thời gian** | Viết bộ dữ liệu kiểm thử biên (edge cases / unit tests) cho các hàm tiền xử lý dữ liệu trước khi ghép vào pipeline chính. | Người viết code pipeline | Mất 45–60 phút/module; thường bị bỏ qua vì tốn công, dẫn tới phát sinh bug ngầm khi chạy trên tập dữ liệu thực tế. |

**AI đã dùng ở Phase 1 (nếu có):**
- **Prompt đã hỏi:** "Tôi là sinh viên ngành CNTT làm nghiên cứu AI/ML và làm đồ án nhóm. Hãy gợi ý các bottleneck tốn thời gian hằng tuần theo 4 lăng kính: Lặp lại, Tốn thời gian, AI có thể tốt hơn, Pain từ người khác. Chỉ nêu workflow cụ thể, không đề xuất sản phẩm AI chung chung."
- **Ý dùng được:** Gợi ý về việc tra cứu trace log dài nhiều tầng và việc chuyển đổi công thức toán/bảng biểu từ PDF sang LaTeX.
- **Ý bỏ vì không phải pain thật:** Gợi ý "AI tự động viết code đồ án từ đầu đến cuối" (bỏ vì quá viển vông, không có workflow kiểm soát cụ thể và vi phạm tính liêm chính học thuật).

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| **1** | **Trích xuất thông số & metric từ paper học thuật vào bảng benchmark** | Actor rất cụ thể; workflow tuyến tính dễ định lượng; bottleneck rõ ràng ở bước đọc trích xuất bảng; đo lường được bằng thời gian và độ chính xác của con số so với bản gốc. | Khả năng đọc hiểu bảng biểu phức tạp hoặc biểu đồ hình ảnh (nếu model PDF parser trích xuất kém). |
| **2** | **Tìm kiếm và tổng hợp quyết định kỹ thuật trôi trong Discord/Slack nhóm** | Tác động trực tiếp đến toàn bộ thành viên nhóm; lặp lại hàng tuần; giảm thiểu thời gian gián đoạn công việc của nhau. | Vấn đề phân quyền truy cập tin nhắn (data privacy/API) và scope tích hợp có thể bị phình to trong buổi lab. |
| **3** | **Gán nhãn sơ bộ sắc thái/chủ đề tập dữ liệu văn bản thô** | Tác vụ thủ công lặp lại nặng; tốn nhiều thời gian của người làm dữ liệu; bài toán NLP phân loại nhãn nháp có tính khả thi kỹ thuật cao. | Tiêu chuẩn chất lượng nhãn (annotation guidelines) dễ bị mơ hồ ở các trường hợp câu mang sắc thái mỉa mai hoặc trung tính. |

---

### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Trích xuất thông số & metric từ paper học thuật vào bảng benchmark

```text
Problem 1 câu:
Mỗi tuần sinh viên nghiên cứu mất khoảng 120 phút đọc lướt và nhặt thủ công các thông số, baseline và metric từ các paper dài 10-15 trang để đưa vào bảng so sánh (benchmark), bước này chậm và rất dễ nhầm lẫn số liệu.

Actor:
Sinh viên làm đồ án tốt nghiệp / Nghiên cứu sinh ngành AI-Data cần xây dựng bảng tổng quan nghiên cứu (literature review & baseline comparison).

Thời điểm / bối cảnh:
Giai đoạn khảo sát tài liệu và định kỳ hàng tuần khi cập nhật kết quả so sánh thử nghiệm của đề tài.

Current workflow 3-7 bước:
1. Tải file PDF bài báo từ arXiv/Google Scholar về máy.
2. Đọc lướt Abstract, Introduction và Conclusion để xác định bài toán.
3. Cuộn đến phần "Experiments" và "Results", dò tìm các bảng số liệu so sánh.
4. Đối chiếu tên mô hình, dataset thử nghiệm, giá trị metric (F1, AUC, BLEU, latency).
5. Copy/gõ tay từng số liệu vào file Excel/Google Sheets tổng hợp của đề tài.

Bottleneck:
Bước 3 & 4 (Đọc sâu và nhặt dữ liệu bảng biểu): Mất 40-50 phút/paper vì bảng có nhiều biến thể (ablation), nhiều dataset khác nhau và font chữ nhỏ, rất dễ nhặt nhầm cột.

Impact:
Tốn khoảng 4-6 tiếng/tuần cho 1 cá nhân; làm chậm tiến độ thử nghiệm; nếu nhập nhầm số liệu của baseline sẽ dẫn đến đánh giá sai kết quả đồ án.

Success metric:
Giảm tổng thời gian trích xuất 1 paper từ 120 phút xuống dưới 35 phút; độ chính xác của các con số trích xuất so với bản gốc đạt tối thiểu 95% sau khi người rà soát lại.

Non-AI alternative:
Sử dụng công cụ chuyển PDF sang Excel thông thường kết hợp phím tắt Ctrl+F từ khóa "Table", "Results". Hạn chế: Không phân tích được ngữ cảnh dòng chú thích bảng và không gom đúng cấu trúc mong muốn.

AI hypothesis:
AI parse cấu trúc tài liệu, xác định phần kết quả thực nghiệm và trích xuất bảng số liệu thành định dạng Markdown/JSON chuẩn hoá. Con người chỉ đóng vai trò kiểm tra chéo với PDF gốc và bấm duyệt.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết

```

**Draft workflow Card #1:**

```text
CURRENT STATE — 120 phút

[1 Tải PDF: 5']
→ [2 Đọc lướt bối cảnh: 20']
→ [3 Dò tìm bảng Experiments/Results: 25']
→ [4 Nhặt số liệu & đối chiếu ngữ cảnh bảng: 45']  <-- bottleneck
→ [5 Nhập tay vào bảng Benchmark: 25']

FUTURE STATE — 30 phút

[1 Tải PDF & tải lên tool: 3']
→ [2 Script trích xuất text & table (Rule/Parser): 2']
→ [3 AI tóm tắt bối cảnh & cấu trúc bảng kết quả thành JSON/Markdown: 5']
→ [4 Người đối chiếu số liệu trích xuất với PDF gốc (Review & Edit): 18']  <-- human boundary
→ [5 Đồng bộ vào Google Sheets đồ án: 2']

Fallback: nếu AI trích xuất sai cấu trúc hoặc bịa số liệu -> Người dùng bấm "Hủy draft", quay lại xem text thô đã parse để nhặt thủ công.

```

<!--File đính kèm (nếu vẽ riêng): `01-individual-problem-scan-workflow-card-1.png`-->

---

#### Problem Card #2 — Tra cứu và tổng hợp quyết định kỹ thuật trong Discord nhóm

```text
Problem 1 câu:
Thành viên nhóm dự án mất 15-25 phút mỗi khi cần tìm lại các link tài liệu, mã nguồn hoặc quyết định kiến trúc đã thống nhất trong các thread chat Discord bị trôi.

Actor:
Thành viên nhóm làm bài tập lớn / đồ án công nghệ (nhóm 3-5 người).

Thời điểm / bối cảnh:
Trong quá trình code hàng ngày hoặc trước buổi họp review tiến độ hàng tuần.

Current workflow 3-7 bước:
1. Nhớ lại mốc thời gian hoặc từ khóa liên quan đến quyết định/tài liệu.
2. Dùng thanh Search của Discord với các bộ lọc from:, has: link, in:.
3. Đọc lướt qua hàng chục tin nhắn trong kết quả tìm kiếm.
4. Mở từng thread để đọc toàn bộ ngữ cảnh chốt phương án.
5. Tổng hợp lại câu trả lời và áp dụng vào công việc.

Bottleneck:
Bước 3 & 4 (Đọc ngữ cảnh thread): Các thảo luận thường bị ngắt quãng bởi các tin nhắn tán gẫu hoặc chia làm nhiều thread nhỏ, mất rất nhiều thời gian đọc gom lại.

Impact:
Mất 40-60 phút/tuần/người; gây ức chế, thường dẫn đến việc phải tag người khác hỏi lại làm gián đoạn luồng làm việc của đồng đội.

Success metric:
Giảm thời gian tìm đúng thông tin quyết định từ 20 phút xuống dưới 3 phút; giảm số lần phải nhắn hỏi lại trên kênh chung xuống 0 lần/tuần đối với các thông tin đã thảo luận.

Non-AI alternative:
Tạo channel Discord riêng #decisions-and-links và bắt buộc mọi người sau khi thống nhất phải pin tin nhắn hoặc tự copy vào 1 trang Notion chung.

AI hypothesis:
Một bot tóm tắt định kỳ tự động phát hiện tin nhắn có chứa link/quyết định quan trọng để đưa vào danh mục tra cứu nhanh, hoặc hỗ trợ query ngữ nghĩa từ khóa tìm kiếm.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết

```

**Draft workflow Card #2:**

```text
CURRENT STATE — 20 phút

[1 Nhớ từ khóa: 2']
→ [2 Discord Search: 3']
→ [3 Lướt đọc từng tin nhắn kết quả: 7']
→ [4 Đọc ngữ cảnh thread để xác nhận quyết định chốt: 8']  <-- bottleneck

FUTURE STATE — 4 phút

[1 Gõ câu hỏi tìm kiếm ngữ nghĩa: 1']
→ [2 AI quét ngữ cảnh các thread liên quan & trích xuất câu chốt + link: 1']
→ [3 Người bấm vào link dẫn chứng để kiểm chứng tính xác thực: 2']  <-- human boundary

Fallback: nếu AI không tìm thấy hoặc trích xuất mơ hồ -> Mở trực tiếp link gốc tin nhắn Discord mà AI gợi ý để đọc lại đoạn chat.

```

<!--File đính kèm: `01-individual-problem-scan-workflow-card-2.png`-->

---

#### Problem Card #3 — Gán nhãn sơ bộ sắc thái dữ liệu văn bản tin tức

```text
Problem 1 câu:
Người làm dữ liệu mất từ 3-4 tiếng bấm chuột thủ công để gán nhãn sơ bộ sắc thái (tích cực/tiêu cực/trung tính) cho hàng trăm dòng tin tức tài chính/công nghệ, gây mệt mỏi và sai lệch độ nhất quán.

Actor:
Sinh viên/nghiên cứu sinh chuẩn bị dữ liệu thử nghiệm cho bài toán phân loại văn bản (NLP Classification).

Thời điểm / bối cảnh:
Mỗi khi thu thập được tập dữ liệu mới từ báo chí hoặc mạng xã hội phục vụ bài toán.

Current workflow 3-7 bước:
1. Mở file CSV/Sheets chứa 500 bài báo/đoạn tin tức thô.
2. Đọc từng câu tiêu đề và đoạn tóm tắt.
3. Suy luận sắc thái dựa trên bộ quy tắc gán nhãn (guideline).
4. Nhập giá trị nhãn (0: Tiêu cực, 1: Trung tính, 2: Tích cực) vào cột nhãn.
5. Lặp lại cho đến hết tập dữ liệu và rà soát các mẫu còn nghi ngờ.

Bottleneck:
Bước 2 & 3: Đọc và suy luận lặp lại liên tục hàng trăm lần khiến tốc độ chậm dần và độ tập trung giảm mạnh sau 1 tiếng làm việc.

Impact:
Tốn 3-4 tiếng/batch; hiệu suất làm việc giảm; nhãn ở cuối tệp dữ liệu thường bị nhiễu do người gán nhãn mệt mỏi.

Success metric:
Giảm thời gian xử lý 500 mẫu từ 210 phút xuống dưới 60 phút; độ đồng thuận (inter-annotator agreement) giữa nhãn AI gợi ý và nhãn người chốt đạt trên 85%.

Non-AI alternative:
Dùng bảng tra cứu từ điển từ ngữ cảm xúc (Sentiment Lexicon: tích cực/tiêu cực). Hạn chế: Bỏ sót ngữ cảnh, không xử lý được sắc thái mỉa mai hoặc phủ định kép.

AI hypothesis:
LLM phân tích ngữ cảnh của câu và tự động điền nhãn nháp kèm mức độ tự tin (confidence score). Người chỉ cần tập trung rà soát các mẫu có confidence score thấp (< 0.8).

Quick gut:
[ ] No AI / process fix
[x] Rule
[ ] Workflow
[ ] Agent
[ ] Chưa biết

```

**Draft workflow Card #3:**

```text
CURRENT STATE — 210 phút

[1 Mở file CSV: 5']
→ [2 Đọc từng câu: 100']  <-- bottleneck
→ [3 Suy luận sắc thái: 75']  <-- bottleneck
→ [4 Nhập nhãn thủ công: 30']

FUTURE STATE — 55 phút

[1 Import dữ liệu thô vào script/tool: 2']
→ [2 AI gán nhãn sơ bộ + trả về confidence score (0-1): 3']
→ [3 Lọc các mẫu điểm tự tin thấp (< 0.8) để người trực tiếp kiểm tra & sửa: 45']  <-- human boundary
→ [4 Xuất file CSV nhãn hoàn chỉnh: 5']

Fallback: nếu AI gán nhãn lệch hoàn toàn do ngữ cảnh mới -> Đặt lại prompt phân loại hoặc quay về cách lọc theo từ khóa quy tắc (Lexicon rule) kết hợp gán tay.

```

<!--File đính kèm: `01-individual-problem-scan-workflow-card-3.png`-->

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #1 — Trích xuất thông số & metric từ paper học thuật vào bảng benchmark.

```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Đây là quy trình cực kỳ quen thuộc với mọi sinh viên và nhóm làm kỹ thuật/nghiên cứu: từ khâu đọc PDF, dò bảng đến tổng hợp baseline. Vấn đề có số đo rõ ràng (giảm từ 120 phút xuống dưới 35 phút/paper, đo được độ chính xác của con số trích xuất so với PDF gốc). Giải pháp dừng ở mức Workflow có con người kiểm tra (human boundary), không sa đà vào việc ảo tưởng làm một Agent tự động hoàn toàn.

```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Các bảng số liệu trong paper thường có format rất đa dạng (bảng ngang, bảng lồng nhau, bảng có footnote giải thích ký hiệu đặc biệt), liệu parser và AI có lấy đúng số mà không bị lệch cột hay không?
2. Nếu một công cụ non-AI kết hợp phím tắt tìm kiếm và template bảng chuẩn hóa đã có thể giúp tiết kiệm thời gian, liệu việc can thiệp AI vào bước này có thật sự cần thiết và an toàn về mặt độ chính xác học thuật?

```

**AI phản biện Card (nếu có):**

* **Điểm yếu AI chỉ ra:** Trích xuất số liệu nghiên cứu yêu cầu độ chính xác 100%, AI dễ gặp ảo giác (hallucination) biến số 0.842 thành 0.824 mà mắt thường khó nhận ra; đồng thời chưa làm rõ ranh giới con người sẽ kiểm tra bằng cách nào nếu bảng quá dài.
* **Tôi sửa gì:** Bổ sung bước rà soát đối chiếu trực tiếp (Human boundary) chiếm tới 18/30 phút trong Future Workflow, và đặt Success Metric là con số sau khi đã qua bước người kiểm tra chéo với văn bản gốc.

### Self-check nộp phần 01

* [x] Có 5+ problems + top 3 Cards đủ field
* [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
* [x] Đã chọn 1 card pitch + câu hỏi challenge

```

```
