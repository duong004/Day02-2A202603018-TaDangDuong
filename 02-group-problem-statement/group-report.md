# 02 — Group Problem Statement (Bản nộp nhóm)

> Làm chung 1 bản, mỗi thành viên copy vào repo cá nhân. Đi theo Phase 3 → 6 trong `01-worksheet.md`. Nhóm chỉ chọn **candidate problem** ở Phase 3, viết Problem Statement sau khi validate + vẽ workflow.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm (VD: facilitator, workflow, research, writer) |
|-----|-----------|-------------|---------------------------------------------------------------|
| 1   | Trần Ngọc Khánh | 2A202602923 | Đưa candidate fanpage, workflow, writer |
| 2   | Phùng Đức Đăng | 2A202602956 | Đưa candidate backend/CI-CD, technical challenge |
| 3   | Đào Duy Hiếu | 2A202602651 | Đưa candidate CV/tài liệu, research |
| 4   | Đặng Thái Anh | 2A202602740 | Đưa candidate dữ liệu/kênh thông tin, score |
| 5   | Tạ Đăng Dương | 2A202603018 | Đưa candidate research/NLP, validation |
| 6   | Nguyễn Hữu Thành | 2A202602807 | Đưa candidate quản lý task/họp/gia sư, facilitator |

**Candidate problem nhóm chọn (1 câu):**
Chuẩn hóa commit message và tối ưu quy trình merge code nhiều lập trình viên khi push lên các nhánh feature và production trong dự án phát triển phần mềm.

---

## Phase 3 — Group Convergence: từ 9-12 candidates về 1

### 3.1. Trình bày top 3 mỗi người (mỗi candidate 1-2 phút)

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---|---|---|---|---|---|
| 1 | Trần Ngọc Khánh | Trả lời các câu hỏi lặp lại về giá, màu, size, phí ship và tồn kho trong tin nhắn fanpage | Người trực page và khách mua hàng | Mở file kiểm tra kho/giá và gõ lại câu trả lời cho từng khách (1-3 phút/khách, 30 khách/ngày) | Vấn đề rõ, dễ hiểu nhưng các chatbot Rule hiện có đã xử lý tương đối tốt |
| 2 | Trần Ngọc Khánh | Phân loại và sắp xếp thứ tự ưu tiên tin nhắn khách hàng trong giờ cao điểm | Quản lý fanpage và khách cần hỗ trợ gấp | Đọc lịch sử từng chat để xếp thứ tự xử lý (30-60 giây/chat, 45 chat/ngày) | Thao tác nhẹ, chưa tạo tác động đủ lớn |
| 3 | Phùng Đức Đăng | Chuẩn hóa commit message và tối ưu quy trình merge code khi nhiều dev push lên các nhánh feature/production | Software Engineer và Tech Lead | Nhánh và commit lộn xộn, phải rà soát và chạy interactive rebase tay ngốn 15-20 phút/PR | Vấn đề kỹ thuật sát sườn, nhóm lập trình đều gặp, quy trình và ranh giới rõ ràng |
| 4 | Phùng Đức Đăng | Tự động phân tích và tóm tắt nguyên nhân fail của pipeline CI/CD, trích xuất dòng lỗi test/build | Dev phụ trách deploy và QA | Đọc log build hàng nghìn dòng để tìm nguyên nhân gốc (15-30 phút/lần lỗi) | Vấn đề hay nhưng phụ thuộc log format của từng framework, khó test đồng bộ |
| 5 | Phùng Đức Đăng | Viết mock data, assertion boilerplate và test case integration cho REST API backend | Backend Developer và Reviewer | Viết boilerplate lặp lại, tốn thời gian chuẩn bị dữ liệu biên (30-45 phút/endpoint) | Có thể giải quyết tốt bằng prompt template IDE đơn giản |
| 6 | Đào Duy Hiếu | Chỉnh sửa CV và Cover letter theo từng mô tả công việc (JD) khác nhau khi ứng tuyển | Sinh viên mới ra trường và Fresher | Tìm cách đảo chữ, lồng ghép từ khóa kỹ năng mà vẫn trung thực (15-20 phút/lần nộp) | Mang tính cá nhân cao, khó đo lường quy chuẩn chính xác trong nhóm |
| 7 | Đào Duy Hiếu | Tìm kiếm bài đăng tuyển dụng phù hợp với số năm kinh nghiệm thực tế | Sinh viên và người tìm việc | Mở từng link JD dài để tìm dòng yêu cầu kinh nghiệm, 80% bị loại (35-40 phút/ngày) | Dữ liệu web tuyển dụng đổi liên tục, scraping kém ổn định |
| 8 | Đặng Thái Anh | Tải datasheet vận hành, làm sạch và chuẩn hóa số liệu trước khi cập nhật Power BI | Nhân viên kỹ thuật và người làm báo cáo | Ghép file, chuẩn hóa tên cột, timestamp và đơn vị bằng tay (45-60 phút/tuần) | Nghiêng nhiều về data pipeline truyền thống, ít đất cho AI xử lý ngôn ngữ |
| 9 | Đặng Thái Anh | Gom và lọc thông báo, yêu cầu công việc bị phân tán giữa Email, Zalo, Facebook | Project Manager và kỹ sư | Tự đọc lọc tin trùng và ghi nhận task thủ công (20-30 phút/ngày) | Phụ thuộc quyền truy cập API bảo mật của nhiều nền tảng |
| 10 | Tạ Đăng Dương | Đọc và trích xuất thông số mô hình, metric đánh giá (F1, AUC) từ paper học thuật vào bảng benchmark | Nghiên cứu sinh, sinh viên làm đồ án AI | Đọc lướt văn bản, dò bảng kết quả và copy số liệu thủ công (40-50 phút/paper) | Hay nhưng hẹp, chỉ phù hợp nhóm nhỏ nghiên cứu học thuật |
| 11 | Tạ Đăng Dương | Tìm lại các quyết định kiến trúc kỹ thuật bị trôi trong các luồng tin nhắn chat Discord | Thành viên nhóm làm đồ án công nghệ | Cuộn tìm lịch sử chat để xác định quyết định cuối cùng (15-20 phút/lần tìm) | Giải quyết bằng quy ước ghi chép Notion/Wiki hiệu quả hơn |
| 12 | Nguyễn Hữu Thành | Lọc thông tin và chuyển nội dung cuộc họp online thành biên bản có cấu trúc và task deadline | Thành viên dự án và người chủ trì | Nghe lại bản ghi hoặc đọc transcript để ghi nhận việc cần làm (20-30 phút/cuộc họp) | Đã có nhiều công cụ transcription AI thương mại phổ biến trên thị trường |

### 3.2. Gom trùng / cluster (gom 9-12 ý thành 3-4 cụm)

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A | #3, #4, #5 | Quy trình phát triển phần mềm nhiều người: lãng phí thời gian vào soát lỗi, tích hợp mã nguồn, log và kiểm thử | Cả 6 thành viên đều có kỹ năng kỹ thuật, dễ thử nghiệm trực tiếp ngay trong lab |
| B | #6, #8, #10 | Xử lý tài liệu và số liệu bán cấu trúc, tốn thời gian đọc dò và trích xuất | Tính cá nhân hóa cao hoặc bài toán hẹp trong nghiên cứu |
| C | #1, #2, #9 | Giao tiếp đa kênh và chăm sóc khách hàng: phân loại tin nhắn, trích xuất ý định và sinh câu phản hồi | Nhiều giải pháp Rule-based và SaaS hiện hành đã phủ rộng |
| D | #7, #11, #12 | Quản lý công việc và cộng tác nhóm: theo dõi tiến độ, họp hành và tìm kiếm thông tin nội bộ | Hành vi người dùng phân tán, phụ thuộc thói quen cá nhân |

### 3.3. Shortlist (giữ 2-3 bài trả lời được 7 câu hỏi worksheet)

| Candidate | Vì sao vào shortlist (2-3 ý) | Rủi ro / điều chưa rõ |
|---|---|---|
| 1. Chuẩn hóa commit message và tối ưu quy trình merge code (#3) | Actor và workflow chuẩn hóa cực kỳ rõ ràng; cả nhóm đều trực tiếp trải nghiệm nỗi đau merge conflict và commit rác; phân định ranh giới Rule/AI/Human tuyệt đối minh bạch | Cần xác lập giới hạn không cho AI can thiệp vào code nghiệp vụ lõi khi xử lý xung đột |
| 2. Tự động phân tích CI/CD pipeline fail log (#4) | Tiết kiệm trực tiếp thời gian đọc log dài của lập trình viên; có thể đo lường bằng thời gian phát hiện root cause | Định dạng log giữa các framework (Node, Java, Python, Docker) rất khác nhau, khó tổng quát trong phạm vi lab |
| 3. Trả lời câu hỏi FAQ lặp lại trên fanpage (#1) | Dữ liệu dễ thu thập, nhu cầu kinh doanh thực tế rõ ràng, dễ demo kịch bản hỏi đáp | Các công cụ Rule chatbot hiện tại đã giải quyết 70-80% nhu cầu mà không bắt buộc cần AI |

### 3.4. Score để đồng thuận (chấm 1-5, ép nói rõ vì sao cho 5 / cho 3)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| 1. Chuẩn hóa commit và merge code | 5 | 5 | 5 | 5 | 5 | 5 | 5 | 35 |
| 2. Phân tích CI/CD fail log | 4 | 4 | 4 | 4 | 3 | 4 | 4 | 27 |
| 3. Trả lời FAQ fanpage | 4 | 4 | 4 | 3 | 4 | 3 | 4 | 26 |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Chuẩn hóa commit message và tối ưu quy trình merge code nhiều lập trình viên khi push lên các nhánh feature và production trong dự án phát triển phần mềm.
```

**Vì sao chọn (4-5 câu):**

```text
Đây là bài toán có mức độ đồng thuận tuyệt đối (35/35 điểm) vì tất cả thành viên trong nhóm đều là sinh viên kỹ thuật phần mềm và đã từng trực tiếp chịu tổn thất từ việc merge code xung đột hoặc lịch sử commit lộn xộn. Workflow từ lúc gõ lệnh git đến khi merge vào production có ranh giới kỹ thuật vô cùng rành mạch giữa công cụ Git, hệ thống CI/CD và người reviewer. Dữ liệu đầu vào (git diff, git log, branch name) là dữ liệu kỹ thuật chuẩn hóa, hoàn toàn không phụ thuộc vào cảm xúc chủ quan. Tác động của bài toán đo đếm được chính xác bằng phút xử lý PR và tỷ lệ tuân thủ tiêu chuẩn kỹ thuật. Đặc biệt, việc tự chủ xây dựng agent/workflow nội bộ mang lại lợi thế chiến lược cốt tử về mặt bảo mật mã nguồn (Source Code Privacy): kiểm soát 100% luồng dữ liệu diff, không rò rỉ bí mật kinh doanh hay mã nguồn doanh nghiệp ra bên ngoài, đồng thời hoàn toàn không bị phụ thuộc vào các nhà cung cấp AI độc quyền (Zero Vendor Lock-in) nhờ khả năng linh hoạt chuyển đổi giữa API đám mây và các mô hình LLM mã nguồn mở tự host tại chỗ (Self-hosted Local LLMs).
```

**Vì sao KHÔNG chọn các candidate còn lại (mỗi bài 2-3 câu):**

```text
- Candidate Phân tích log CI/CD (#4): Mặc dù có giá trị thực tế cao nhưng định dạng log giữa các framework (Node.js, Java, Python, Docker) rất đa dạng và cồng kềnh, việc giả lập môi trường pipeline lỗi đa dạng trong thời lượng lab ngắn là khó khả thi.
- Candidate Trả lời FAQ fanpage (#1): Phần lớn các trường hợp hỏi giá, size, tồn kho hoàn toàn giải quyết được bằng Rule-based chatbot đơn giản với chi phí rẻ hơn; việc đưa AI vào tiềm ẩn rủi ro trả lời sai giá hoặc sai chính sách bán hàng.
```

**Disagreement (nếu có — ai lo gì, chốt ra sao):**

```text
Một thành viên ban đầu lo ngại rằng nếu để AI can thiệp vào quy trình Git thì liệu AI có tự ý làm mất code của thành viên khác khi giải quyết merge conflict hay không. Nhóm đã thảo luận và thống nhất chốt chặn ranh giới an toàn: AI tuyệt đối không được tự ý sửa code logic khi có conflict, mà chỉ đọc diff giải thích nguyên nhân gây xung đột; lập trình viên con người bắt buộc phải tự tay sửa code trong IDE.
```

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation (ít nhất 1 cách: interview 2-3 người hoặc survey 5-10 người)

| Nguồn | Số người / mẫu | Tín hiệu xác nhận (kèm quote nguyên văn) | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Interview | 3 lập trình viên backend và Tech Lead | "Nhiều bạn commit ghi đúng một chữ 'fix' hoặc 'done', lúc production gặp lỗi muốn dùng git bisect tìm lại dòng gây bug thì hoàn toàn bất lực" (Tech Lead) | "Nếu bắt cài quá nhiều tool hook local thì máy yếu sẽ bị chậm khi gõ lệnh commit" | Thiết kế hook nhẹ, phần AI phân tích ngữ nghĩa đẩy về PR template và CI pipeline thay vì ép chạy nặng ở local |
| Survey / poll | 8 sinh viên CNTT đang làm đồ án nhóm | 7/8 người thừa nhận từng bị xung đột mã nguồn sát giờ nộp bài; 6/8 người không nắm rõ quy tắc Conventional Commits | 2 người cho rằng chỉ cần bấm squash merge trên GitHub là đủ sạch commit | Làm rõ rằng squash merge chỉ gộp commit trên nhánh chính, không giải quyết được việc mô tả PR sơ sài và xung đột giữa các nhánh con |
| Log / ticket / review (nếu có) | Phân tích 30 Pull Requests gần nhất | Hơn 65% số commit message vi phạm chuẩn (thiếu scope, thông điệp vô nghĩa); trung bình mất 22 phút từ khi mở PR đến khi được merge do phải sửa lại lịch sử | Các PR nhỏ dưới 10 dòng diff thì thời gian review nhanh, ít bị phàn nàn | Đặt ngưỡng: các commit nhỏ vẫn phải tuân thủ chuẩn tự động, tránh kiểm tra thủ công gây phiền toái |

**Insight sau validation (1-2 câu — pain thật nằm ở đâu):**

```text
Nỗi đau thật không nằm ở việc gõ lệnh Git, mà nằm ở sự thiếu kỷ luật thống nhất: lập trình viên ngại suy nghĩ để viết commit chuẩn và mô tả PR đầy đủ, dẫn đến gánh nặng dồn lên vai Tech Lead phải rà soát, dọn dẹp thủ công và gánh rủi ro khi merge code lỗi lên production.
```

Bằng chứng đính kèm (nếu có): `02-group-problem-statement-survey.png`, `...-interview-notes.md`

### 4.2. Research giải pháp đã có (ít nhất 2-3 tools/patterns + 1-2 link kiểm được)

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Commitizen + Commitlint | https://www.conventionalcommits.org | Chuẩn hóa cú pháp commit message tại local qua CLI tương tác | Kiểm soát chặt bằng regex rule, không cho commit sai định dạng | Ép người dùng chọn từng bước thủ công qua prompt CLI, tốn thao tác và không tự hiểu ngữ cảnh code diff | Dùng Rule để chặn cú pháp cuối cùng, nhưng dùng AI để sinh gợi ý ban đầu |
| GitHub Copilot for PRs / Copilot Workspace | https://github.com/features/copilot | Tự động tóm tắt thay đổi mã nguồn và sinh mô tả Pull Request | Đọc diff đa file tốt, sinh tóm tắt súc tích, gắn checklist tự động | Chi phí bản quyền cao, nhà cung cấp độc quyền (Vendor Lock-in), nguy cơ rò rỉ mã nguồn nội bộ ra máy chủ bên thứ ba | Cần xây dựng agent/workflow nội bộ tự chủ, hỗ trợ mô hình on-premise để bảo vệ bí mật mã nguồn |
| Semantic Release | https://github.com/semantic-release/semantic-release | Tự động phân tích commit history để tăng version và sinh Changelog | Hoàn toàn tự động hóa quy trình phát hành dựa trên chuẩn Conventional Commits | Phụ thuộc 100% vào việc commit đầu vào phải chuẩn; nếu commit rác thì toàn bộ versioning bị sai | Chứng minh giá trị cốt lõi: nếu chuẩn hóa được commit từ đầu thì khâu release được tự động hóa 100% |

**Research takeaway (2-3 câu — nên build gì / không build gì):**

```text
Nên tận dụng Rule có sẵn (Commitlint, GitHub Branch Protection, Semantic Release) để làm khung kiểm soát cứng và dùng AI ở hai điểm đắt giá nhất: đọc git diff để draft commit/PR summary chuẩn, và giải thích nguyên nhân merge conflict. Về mặt kiến trúc, nhóm quyết định tự xây dựng workflow/agent tích hợp thay vì mua dịch vụ SaaS đóng kín của bên thứ ba để đảm bảo an toàn bí mật mã nguồn (IP protection) không bị truyền ra ngoài phục vụ huấn luyện mô hình, đồng thời tránh bẫy khóa chặt nhà cung cấp (Zero Vendor Lock-in), cho phép tự do chuyển đổi giữa API thương mại và các mô hình LLM mã nguồn mở tự host tại chỗ (Local LLMs). Tuyệt đối không tự xây lại bộ linter hay để AI tự tiện merge code mà không có người phê duyệt.
```

> Lưu ý: không dùng số liệu AI đưa nếu không verify được link chính thức. Ghi rõ giả định chưa chắc.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

Dán workflow hoặc link file: `02-group-problem-statement-workflow.png/pdf/md`

```text
[1. Code và Stage: 2' - Dev] → [2. Commit vội 'fix/wip': 1' - Dev] → [3. Mở PR: 3' - Dev] → [4. Rebase/Sửa commit tay: 15-20' - Dev (BOTTLENECK)] → [5. Merge code: 5' - Lead] → [6. Soạn Changelog tay: 10' - Lead]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú (handoff? bottleneck?) |
|---|---|---|---|---|---|
| 1 | Developer | Feature/bugfix code hoàn thành trên local | File được đưa vào Git staging index | 1-2 phút; 4-6 lần/ngày | Dev tự thực hiện cục bộ |
| 2 | Developer | Staged changes | Commit message lộn xộn ("wip", "fix bug", "done") | 1 phút; 4-6 lần/ngày | Vi phạm chuẩn Conventional Commits |
| 3 | Developer | Nhánh tính năng chứa commit rời rạc | Pull Request trên GitHub/GitLab | 2-3 phút; 2-3 PR/ngày | Handoff chuyển sang cho Tech Lead review |
| 4 | Developer | Yêu cầu chuẩn hóa và dọn commit từ Tech Lead | Lịch sử Git được squash/reword thủ công | 15-20 phút/PR; 2-3 PR/ngày | BOTTLENECK CHÍNH: Dev phải nhớ lại code, chạy interactive rebase tay, dễ mất commit hoặc gây xung đột thứ cấp |
| 5 | Tech Lead | PR đã dọn sạch commit | Mã nguồn được merge vào nhánh develop/staging | 3-5 phút (nếu êm); 15-30 phút (nếu xung đột) | Handoff sang nhánh chung của dự án |
| 6 | Release Lead | Danh sách commit đã merge | Bản ghi chép Changelog và Release Notes viết tay | 10-15 phút/lần release | Phải đọc lại từng PR để tóm tắt thủ công |

**Bottleneck chính (2-3 câu):**

```text
Điểm nghẽn nghiêm trọng nhất nằm ở Bước 4 (Soát và rebase commit thủ công). Do lập trình viên có thói quen commit vội trong quá trình viết code, khi mở PR, Tech Lead buộc phải yêu cầu dọn dẹp lịch sử để đảm bảo khả năng truy vết lỗi sau này. Việc chạy git rebase -i thủ công ngốn từ 15 đến 20 phút mỗi PR, dễ gây ức chế tâm lý và tiềm ẩn rủi ro thao tác nhầm làm mất mã nguồn.
```

### 5.2. Future workflow bản nhóm

Phải nhìn ra 5 thứ: bước nào máy (Rule), bước nào AI, bước nào người, boundary ở đâu, fallback khi AI sai.

```text
[1. Prompt Task: 30s - người] → [2. AI Auto Branch, Code, Add, Commit, Push: 1-2' - AI] → [3. Auto PR & Sanity Check: 30s - người (boundary)] → [4. CI Gates Lint/Test/Build: 2' - máy] → [5. AI Conflict Explanation / Dev Fix: 10' - AI+người] → [6. Lead Review & Approve: 2' - người (boundary)] → [7. Merge Enforcement: 1s - máy] → [8. Protected Release: 1' - người]

Fallback: Nếu AI gặp sự cố (mất mạng, timeout, sinh code/commit sai), dev tự checkout nhánh, tự code, tự gõ commit bằng tay theo chuẩn thủ công (Commitlint ở Bước 4 vẫn gác cổng). PR description dev tự soạn tay. Toàn bộ quy trình phát triển phần mềm vẫn hoạt động bình thường, không bị gián đoạn.
```

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Tổng thời gian | 25-35 phút / PR | Dưới 15 phút / PR (giảm trên 50%) | Log timestamp từ lúc mở PR đến khi hoàn tất merge trên GitHub/GitLab |
| Số bước | 6 bước phân tán | 8 bước chuẩn hóa có kiểm soát | Đếm số bước vận hành trong quy trình |
| Số bước thủ công | 5 / 6 bước thủ công | 2 bước kiểm soát của con người (Dev xem lướt 30s và Lead duyệt 2 phút) | Đếm các bước đòi hỏi con người thao tác trực tiếp |
| Bottleneck chính | Mất 15-20 phút chạy interactive rebase dọn commit tay | Triệt tiêu hoàn toàn: Commit đã chuẩn hóa ngay từ lúc đẩy lên | Đo thời gian lập trình viên phải sửa lại commit trên nhánh |
| Risk mới | Nguy cơ mất code do rebase nhầm | Lập trình viên ỷ lại vào AI, bấm duyệt commit mà không đọc kỹ | Đo bằng tỷ lệ phát hiện lỗi qua CI và phản ánh từ Tech Lead |

### 5.3. Problem Statement v0 (mỗi field 2-3 câu)

| Field | Nội dung |
|---|---|
| **Actor** | Software Engineer (người viết mã nguồn, tạo commit, mở PR) và Tech Lead / Release Engineer (người review, duyệt merge, quản lý nhánh và triển khai phiên bản) trong các dự án phần mềm có nhiều lập trình viên cùng làm việc. |
| **Workflow** | Quy trình tích hợp Git: Tạo nhánh tính năng -> Viết code -> Tạo commit -> Mở Pull Request -> Kiểm tra tính hợp lệ CI -> Reviewer phê duyệt -> Merge vào nhánh chính -> Triển khai lên Production qua release PR. |
| **Bottleneck** | Do chưa có quy trình thống nhất về cách đặt tên branch, viết commit và điều kiện merge: Tech Lead phải rà soát và yêu cầu sửa commit thủ công ngốn 15-20 phút/PR; merge conflict bị phát hiện muộn sát giờ tích hợp; PR thiếu mô tả phạm vi ảnh hưởng và checklist kiểm thử. |
| **Impact** | Quá trình tích hợp code mất nhiều thời gian (lãng phí 1.5-2 giờ/ngày của cả nhóm); lịch sử Git bị phân mảnh gây khó khăn khi dùng git bisect truy vết bug trên production; có nguy cơ đưa mã nguồn chưa vượt qua test/build lên môi trường vận hành thật. |
| **Success Metric** | - Baseline hiện trạng: Thời gian trung bình từ lúc mở PR đến khi merge là 25-35 phút; Tỷ lệ commit đúng chuẩn Conventional Commits dưới 40%; Tỷ lệ tự động hóa Changelog bằng 0%.<br>- Target kỳ vọng: Thời gian xử lý PR giảm ít nhất 30% (xuống dưới 15 phút); Tỷ lệ branch và commit đúng quy chuẩn đạt 100%; Số lần Leader phải yêu cầu sửa commit giảm ít nhất 80%; Tỷ lệ PR vượt qua test và build trước khi merge đạt 100%; Số lần push trực tiếp vào production bằng 0.<br>- Cách đo: Đo timestamp tích hợp trên GitHub; chạy script kiểm tra regex lịch sử commit; kiểm tra trạng thái branch protection rule. |
| **Boundary** | - In-Scope (AI được phép làm): Tự checkout nhánh feature, sinh code, tự git add, tự soạn commit message theo Conventional Commits, tự git push lên nhánh feature riêng, tự mở PR kèm summary, đọc giải thích nguyên nhân gây merge conflict.<br>- Out-of-Scope (AI tuyệt đối CẤM làm): Không được tự sửa code logic khi có xung đột (dev phải sửa tay trong IDE); không được tự phê duyệt PR; không được tự ý merge; không được tự ý push vào các nhánh được bảo vệ (develop, main, production). |

**Câu hỏi AI phản biện v0 (nếu có):**
- Field nào mơ hồ: Phần Success Metric lúc đầu chỉ ghi "nhanh hơn và chuẩn hơn" thiếu số liệu gốc; phần Boundary chưa phân định rõ quyền của AI trên nhánh feature riêng so với các nhánh chính được bảo vệ.
- Tôi sửa gì: Bổ sung bộ số liệu đo lường trong 2 tuần / 20 PRs với tỷ lệ phần trăm cụ thể; thiết lập ranh giới quyền hạn: AI được tự động hóa trên nhánh feature con nhưng bị chặn tuyệt đối trước các nhánh protected.

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp (suy nghĩ nhanh, không thay quyết định cuối)

- Độ mơ hồ: [x] Thấp (có đúng/sai rõ) / [ ] Cao (nhiều cách trả lời vẫn OK) — Vì sao: Cú pháp branch và commit có chuẩn mực quốc tế chính xác (Conventional Commits), điều kiện CI test/build pass hay fail có kết quả nhị phân rõ ràng, không có sự mập mờ cảm tính.
- Độ phức tạp: [ ] Thấp (1-2 bước) / [x] Cao (3+ bước/nguồn, phụ thuộc nhau) — Vì sao: Luồng xử lý kéo dài từ máy local của dev qua hệ thống quản trị mã nguồn (GitHub/GitLab), qua hạ tầng CI/CD pipeline, quy trình review nhiều người và cổng triển khai production.

**Bài toán nhóm nằm ở ô nào:**

```text
Độ phức tạp cao / Độ mơ hồ thấp
```

**Vì sao (2-3 câu):**

```text
Với bài toán có tính đúng sai rõ ràng nhưng quy trình đa bước phức tạp, việc áp dụng Rule cứng cho toàn bộ là không đủ (vì Rule không hiểu ngữ nghĩa của code diff để viết commit hay giải thích conflict), nhưng nếu thả nổi cho một Autonomous Agent tự quyết định hết thì rủi ro phá hủy hệ thống là quá lớn. Mô hình tối ưu bắt buộc phải là Workflow có kiểm soát (Governed Workflow), trong đó kết hợp Rule làm khung chốt chặn, AI làm nhiệm vụ xử lý ngôn ngữ/tổng hợp và Con người giữ vai trò phê duyệt then chốt.
```

### 6.1. So sánh Rule / Workflow / Agent (so trên cùng 1 bài)

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? (Dùng cho bước nào?) |
|---|---|---|---|---|
| **Rule** | Dùng Git hooks, Commitlint regex, Branch Protection Rules trên GitHub, script CI kiểm tra cú pháp và chạy test/build tự động | Đủ khi chỉ cần kiểm tra tính hợp lệ về mặt hình thức (đúng format chữ cái, pass unit test, đủ số lượt approve) | Không hiểu ngữ nghĩa code diff; không tự sinh được nội dung commit có ý nghĩa; gây phiền toái nếu dev phải tự nhớ và gõ cú pháp dài dòng | Chọn dùng làm khung nền: Dùng cho Bước 4 (CI Lint/Test/Build Gate), Bước 7 (Merge Condition) và Bước 8 (Protected Production) |
| **Workflow** | Quy trình kết hợp nhiều bước tuần tự: Hook gọi AI đọc diff để sinh gợi ý, dev bấm xác nhận, CI chạy tự động, Leader review và hệ thống merge | Đủ khi quy trình có các bước cố định, cần AI xử lý ngôn ngữ ở vài chốt chặn nhưng vẫn cần con người kiểm soát kết quả | Phụ thuộc vào tính ổn định của API AI; cần xây dựng giao diện tích hợp mượt mà giữa CLI và web | Chọn dùng làm kiến trúc tổng thể của toàn bộ hệ thống |
| **Agent** | AI Coding Agent (tương tự Claude Code, Cursor, Copilot Workspace) tự động checkout branch, viết code, tự git add, commit, push và mở PR | Cần thiết khi muốn giải phóng hoàn toàn lập trình viên khỏi các thao tác gõ lệnh Git cơ bản ở local | Nguy cơ sinh ảo giác (hallucination), code lỗi logic hoặc vi phạm bảo mật nếu không có người kiểm tra | Chọn dùng cục bộ trong phạm vi hẹp: Dùng cho Bước 2 (tự động hóa code, add, commit, push trên nhánh feature cá nhân) |

**5 câu hỏi chốt (trả lời câu đầy đủ):**
1. Rule có giải được 70-80% case không?
-> Có, Rule giải quyết triệt để khâu kiểm tra cú pháp, chạy test và chặn merge trái phép. Tuy nhiên Rule không thể tự hiểu diff để viết commit hay giải thích conflict.
2. Các bước có đi thẳng một đường không hay phải rẽ nhánh?
-> Có rẽ nhánh: khi CI fail hoặc có merge conflict, luồng xử lý phải rẽ sang nhánh Exception/Retry để dev sửa tay rồi mới quay lại luồng chính.
3. Có thật sự cần Agent tự lập kế hoạch + gọi tool không?
-> Ở cấp độ toàn dự án thì không cần và không được phép; nhưng ở cấp độ tác vụ cục bộ của lập trình viên, AI Agent gọi tool Git để checkout branch, add, commit và push giúp tiết kiệm thời gian đáng kể.
4. Nếu AI sai, ai phát hiện đầu tiên và sửa trong bao lâu?
-> CI pipeline và Linter sẽ phát hiện lỗi cú pháp trong 1-2 phút; Reviewer con người sẽ phát hiện lỗi logic trong 2-3 phút khi đọc code review. Lập trình viên sửa lại trong 5-10 phút.
5. Có hạ được từ Agent → Workflow → Rule không?
-> Hoàn toàn hạ được. Nếu tắt toàn bộ phần AI, hệ thống tự động fallback về quy trình Rule-based truyền thống (dev tự gõ commit tay, Commitlint vẫn gác cổng kiểm tra).

**Mức chọn:**

```text
Workflow có kiểm soát (kết hợp Rule chốt chặn an toàn và AI Agent hỗ trợ tác vụ cục bộ)
```

**Vì sao chọn (3-4 câu):**

```text
Mô hình này dung hòa hoàn hảo giữa tốc độ và tính an toàn. Nó tận dụng được sức mạnh tự động hóa của AI Agent giúp lập trình viên không phải gõ các lệnh Git lặp lại, đồng thời sử dụng các Rule cứng và sự phê duyệt của con người để triệt tiêu 100% rủi ro đưa code lỗi lên môi trường production. Quan trọng hơn, giải pháp này đặt quyền kiểm soát bảo mật mã nguồn (Source Code Privacy) vào tay đội ngũ kỹ thuật: mã nguồn không bị gửi cho bên thứ ba tùy tiện, và hệ thống được thiết kế theo kiến trúc mở (Agnostic Architecture) cho phép chạy với bất kỳ model nào (OpenAI, Anthropic hoặc Local LLM nội bộ), triệt tiêu hoàn toàn sự lệ thuộc độc quyền vào một nhà cung cấp (Zero Vendor Lock-in).
```

**Vì sao không chọn mức đơn giản hơn (2-3 câu):**

```text
Nếu chỉ dùng thuần Rule (như Commitizen hay hook thông thường), lập trình viên vẫn phải tự mình căng thẳng đọc diff, tự nghĩ cách diễn đạt và gõ từng từ commit message; Leader vẫn phải tốn công đọc lướt PR thiếu mô tả và tự mình giải thích xung đột code cho cấp dưới. Ngược lại, nếu mua các giải pháp SaaS đóng gói sẵn của bên thứ ba, nhóm sẽ phải trả phí bản quyền đắt đỏ hàng tháng theo đầu người, đồng thời đối mặt với rủi ro rò rỉ mã nguồn và bị trói buộc hoàn toàn vào chính sách giá cũng như hạ tầng của nhà cung cấp đó.
```

### 6.2. Problem Statement v1 (v0 sửa chặt hơn + 3 field cuối)

| Field | Nội dung |
|---|---|
| **Actor** | Software Engineer (người viết mã nguồn, tạo commit, mở PR) và Tech Lead / Release Engineer (người review, duyệt merge, quản lý nhánh và triển khai phiên bản) trong các dự án phần mềm có nhiều lập trình viên cùng làm việc. |
| **Workflow** | Quy trình tích hợp Git: Tạo nhánh tính năng -> Viết code -> Tạo commit -> Mở Pull Request -> Kiểm tra tính hợp lệ CI -> Reviewer phê duyệt -> Merge vào nhánh chính -> Triển khai lên Production qua release PR. |
| **Bottleneck** | Do chưa có quy trình thống nhất về cách đặt tên branch, viết commit và điều kiện merge: Tech Lead phải rà soát và yêu cầu sửa commit thủ công ngốn 15-20 phút/PR; merge conflict bị phát hiện muộn sát giờ tích hợp; PR thiếu mô tả phạm vi ảnh hưởng và checklist kiểm thử. |
| **Impact** | Quá trình tích hợp code mất nhiều thời gian (lãng phí 1.5-2 giờ/ngày của cả nhóm); lịch sử Git bị phân mảnh gây khó khăn khi dùng git bisect truy vết bug trên production; có nguy cơ đưa mã nguồn chưa vượt qua test/build lên môi trường vận hành thật. |
| **Success Metric** | Thử nghiệm trong 2 tuần hoặc tối thiểu 20 Pull Requests: Thời gian từ mở PR đến khi merge giảm ít nhất 30%; Tỷ lệ branch và commit đúng quy chuẩn đạt 100%; Số lần Leader phải yêu cầu sửa commit giảm ít nhất 80%; Tỷ lệ PR vượt qua test/build trước khi merge đạt 100%; Số lần push trực tiếp vào production bằng 0; Tỷ lệ commit do AI gợi ý được dev chấp nhận đạt trên 85%. |
| **Boundary** (làm / không làm) | - Được làm: AI tự tạo branch feature, tự code, tự git add, tự tạo commit Conventional Commits, tự push lên nhánh feature riêng, tự mở PR kèm summary, giải thích nguyên nhân merge conflict.<br>- Tuyệt đối CẤM làm: AI không được tự sửa code logic khi có conflict; không được tự approve PR; không được tự merge; không được tự push vào các protected branches (develop, main, production). |
| **AI intervention point** (can thiệp sau bước nào, trước bước nào) | Can thiệp ở 3 điểm chính: Can thiệp ngay sau khi dev giao task (để tạo branch, sinh code, add, commit và push); can thiệp khi mở PR (tự sinh bản tóm tắt mô tả thay đổi); can thiệp khi có xung đột code (phân tích và giải thích nguyên nhân xung đột cho dev). |
| **Mức chọn** (Rule / Workflow / Agent + 1 câu vì sao) | Workflow kết hợp: Dùng AI Agent cục bộ trên nhánh feature riêng để tăng tốc độ tác nghiệp, nhưng toàn bộ khung tích hợp và bảo vệ nhánh chính được điều khiển bằng Workflow nghiêm ngặt với các Rule kiểm soát và chốt chặn phê duyệt của con người. |
| **Rủi ro & người thật kiểm tra** (rủi ro lớn nhất + ai kiểm tra bằng cách nào) | Rủi ro lớn nhất là AI sinh code có lỗi logic ngầm hoặc dev ỷ lại vào commit message do AI gợi ý mà không đọc kỹ. Chốt chặn kiểm tra: CI tự động chạy 100% bộ test và linter; Reviewer con người bắt buộc phải đọc diff và ký duyệt Approved trước khi mở khóa nút merge. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú (câu đầy đủ) |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Đối tượng là Developer và Tech Lead; quy trình 8 bước từ task đến release được định nghĩa chi tiết đến từng phút. |
| Baseline + metric đo được chưa? | Yes | Có đầy đủ bộ 6 chỉ số đo lường với baseline hiện trạng và mục tiêu định lượng trong 2 tuần / 20 PRs. |
| Data/input đủ dùng chưa? | Yes | Dữ liệu đầu vào là mã nguồn, git diff, commit log và issue tracker có cấu trúc chuẩn mực cao. |
| AI sai, hậu quả chấp nhận được không? | Yes | Hoàn toàn kiểm soát được vì code do AI sinh ra nằm độc lập trên nhánh feature riêng, được CI test và Reviewer thẩm định trước khi merge. |
| Có người review/owner không? | Yes | Bắt buộc Tech Lead hoặc Peer Reviewer con người phải phê duyệt thì hệ thống mới cho phép merge. |
| Có cách non-AI đơn giản hơn không? | Yes | Có phương án dùng thuần Rule (Commitizen + Template tay), nhưng phương án này không tự sinh được nội dung ngữ nghĩa và không giải thích được conflict. |

**Decision:**

```text
Go
```

**Lý do (3-4 câu dựa trên bằng chứng):**

```text
Bài toán đáp ứng xuất sắc toàn bộ 6 tiêu chí thẩm định kỹ thuật. Nhu cầu thực tế cao, tác động đo đếm được rõ ràng bằng số phút tiết kiệm được của cả đội ngũ phát triển. Ranh giới an toàn được thiết kế đa tầng, đảm bảo tính ổn định tuyệt đối cho sản phẩm ngay cả khi hệ thống AI gặp sự cố. Đặc biệt, việc tự xây dựng agent nội bộ mang lại giá trị chiến lược kép: bảo vệ an toàn 100% tài sản trí tuệ và bí mật mã nguồn doanh nghiệp (không bị gửi bừa bãi ra dịch vụ ngoài), đồng thời đạt được quyền tự chủ công nghệ cao nhất, hoàn toàn không bị lệ thuộc vào nhà cung cấp AI độc quyền nào (Zero Vendor Lock-in).
```

**Nếu Go — pilot nhỏ nhất (data nào, chạy tay ra sao, đo 3 số nào):**

```text
- Phạm vi áp dụng: Thử nghiệm trên 1 repository nội bộ của nhóm trong 2 tuần, với tối thiểu 20 Pull Requests thực tế.
- Cách vận hành thử nghiệm: Cài đặt pre-commit hook gọi AI sinh commit message; cấu hình GitHub Actions chạy Commitlint và test tự động; áp dụng template PR có AI tóm tắt; bật Branch Protection Rule trên nhánh develop và main.
- 3 chỉ số cốt lõi cần đo:
  1. Thời gian trung bình từ lúc mở PR đến khi hoàn tất merge (mục tiêu giảm từ 25 phút xuống dưới 15 phút).
  2. Tỷ lệ commit và branch tuân thủ 100% chuẩn Conventional Commits.
  3. Số lần push trực tiếp hoặc merge lỗi chưa được duyệt vào nhánh chính (mục tiêu giữ vững bằng 0).
```

**Nếu Not Yet — cần validate gì trước:**

```text
Không áp dụng vì dự án đã đủ điều kiện triển khai ngay lập tức.
```

**Nếu No-Go — làm gì thay AI:**

```text
Không áp dụng. Nếu không dùng AI, nhóm sẽ áp dụng bộ công cụ thuần Rule gồm Commitizen CLI ép dev chọn menu từng bước, kết hợp viết tay mô tả PR theo mẫu Markdown cố định.
```

**Exit / rollback (khi nào dừng AI, quay về cách cũ):**

```text
Hệ thống sẽ lập tức dừng sử dụng AI và quay về quy trình thủ công truyền thống nếu xảy ra một trong hai điều kiện sau:
1. Chi phí gọi API AI vượt quá 10 USD/tháng cho mỗi lập trình viên mà không đem lại mức tiết kiệm thời gian tương xứng.
2. Tỷ lệ gợi ý commit hoặc tóm tắt của AI bị lập trình viên từ chối quá 40% trong 2 tuần liên tiếp, hoặc AI gây ra sự cố sinh thông tin sai lệch nghiêm trọng ảnh hưởng đến quyết định merge của Tech Lead.
Khi rollback: Chỉ cần gỡ bỏ hook AI ở local và workflow AI trên GitHub Actions; toàn bộ hệ thống kiểm tra quy chuẩn Commitlint và Branch Protection Rules vẫn được giữ nguyên vẹn để bảo vệ mã nguồn.
```

---

### Self-check nộp phần 02 (nhóm)
- [x] Có nhật ký hội tụ 9-12 → 1 (cluster + shortlist + score)
- [x] Có validation (quote thật) + research (link kiểm được)
- [x] Có workflow trước/sau đủ thời gian, handoff, bottleneck, boundary, fallback
- [x] Có PS v0 → v1, metric có trước/sau + cách đo, boundary có làm/không làm
- [x] Có so sánh Rule/Workflow/Agent + Decision Go/Not Yet/No-Go có lý do
