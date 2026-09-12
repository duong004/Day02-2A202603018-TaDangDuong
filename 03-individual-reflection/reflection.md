# 03 - Individual Reflection

## Thông tin cá nhân

- **Họ và tên:** Tạ Đăng Dương
- **Mã học viên:** 2A202603018
- **Nhóm:** Nhóm X
- **Vai trò trong nhóm:** Phụ trách Validation & Research, đóng vai người phản biện kỹ thuật trong nhóm, và tham gia xây dựng ranh giới an toàn (Boundary) cũng như kiến trúc kiểm soát (Governed Workflow).

---

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| **Scan cá nhân** | Quét 10 bài toán từ trải nghiệm học tập và nghiên cứu thực tế của mình - đọc paper AI, trích xuất metric, tra Discord, gán nhãn dữ liệu. | Đóng góp 2 candidate (#10 và #11) vào ngân hàng ý tưởng chung. |
| **Pitch Problem Card** | Trình bày bài toán trích xuất metric từ paper học thuật và bài toán tìm kiếm quyết định kỹ thuật trong Discord. | Nhóm thấy bài toán có cấu trúc rõ, nhưng cuối cùng ưu tiên bài toán Git của Đăng vì phù hợp với cả 6 người hơn. |
| **Challenge bài của bạn khác** | Chất vấn khá thẳng với đề xuất Git của Đăng: "Tại sao phải dùng AI khi Commitlint và Branch Protection đã giải quyết được 80% rồi?" và "AI có làm mất code khi xử lý conflict không?" | Nhóm phải ngồi lại định nghĩa lại phạm vi: cấm AI tự merge, không cho AI tự giải quyết xung đột logic, chuyển thành mô hình Rule + AI kết hợp. |
| **Gom trùng / cluster** | Cùng nhóm gom 12 bài toán thành 4 cụm (Quy trình phần mềm, Xử lý tài liệu, CSKH, Quản lý tác vụ). | Xác định cụm Quy trình phần mềm là thế mạnh chung, dễ kiểm chứng trong lab. |
| **Chọn candidate problem** | Tham gia chấm điểm theo 7 tiêu chí trong bảng Score, đồng ý chọn đề tài Git sau khi các rủi ro kỹ thuật đã được khoanh vùng rõ. | Candidate số 1 đạt 35/35 điểm, làm nền cho các bước triển khai sau. |
| **Validation / research** | Cùng thiết kế bảng hỏi phỏng vấn nhanh cho Tech Lead/Backend Dev, phân tích 30 Pull Request thực tế để lấy baseline, tra thêm các công cụ tương tự (GitHub Copilot, Semantic Release). | Có số liệu thật: 65% commit vi phạm chuẩn, trung bình mất 22 phút/PR. Từ đó thấy cần workflow nội bộ tự chủ, tránh Vendor Lock-in. |
| **Workflow nhóm** | Góp ý các chốt chặn kiểm soát trong Future Workflow (Bước 3 Sanity Check, Bước 6 Lead Review) và cơ chế Fallback khi lỗi. | Quy trình tương lai rõ ràng hơn: bước nào máy chạy, bước nào AI làm, người duyệt ở đâu, và đường lui khi AI sai. |
| **Problem Statement** | Tham gia chuyển Success Metric từ kiểu định tính ("nhanh hơn") sang 6 chỉ số cụ thể (giảm 30% thời gian xử lý PR, 100% commit chuẩn, 0 lần push lỗi). | Problem Statement v0 và v1 chặt hơn, phạm vi In-Scope / Out-of-Scope rõ. |
| **Rule / Workflow / Agent** | Phản đối phương án xây một Autonomous Agent tự do merge code, đề xuất Governed Workflow - khung là Workflow & Rule, AI chỉ dùng cục bộ để tạo commit và tóm tắt PR. | Nhóm chốt giải pháp Workflow kết hợp: tự động hóa được nhiều nhưng vẫn an toàn. |
| **Decision** | Cùng nhóm rà 6 câu hỏi thẩm định kỹ thuật, thống nhất Go với pilot 1 repo nội bộ trong 2 tuần / 20 PR. | Bản quyết định có tiêu chí đo được, điều kiện dừng pilot và kế hoạch rollback cụ thể. |

---

## 2. Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **Scan** | Hỏi thêm góc nhìn về những điểm nghẽn tốn thời gian trong quy trình nghiên cứu kỹ thuật. | Gợi ý được vài điểm như đọc traceback lỗi dài nhiều tầng, hay chuyển công thức toán từ PDF sang LaTeX. | Có lúc đưa ra ý viển vông kiểu "AI tự code cả đồ án từ A đến Z". | Loại bỏ luôn những gợi ý không gắn với workflow thực tế hoặc phạm luật tính trung thực học thuật. |
| **Problem Card** | Nhờ AI đóng vai một PM khó tính để bới lỗi trong Card trích xuất paper. | Chỉ ra đúng nguy cơ ảo giác (hallucination) làm sai số thập phân và các metric khó đo. | Gợi ý nhảy thẳng sang làm Agent tự cập nhật Sheets mà không cần người duyệt. | Thêm bước Human Boundary - dành 18/30 phút để người đối chiếu số liệu trước khi lưu. |
| **Workflow** | Tham khảo cách vẽ các chốt chặn CI/CD có tích hợp AI. | Giúp hình dung nhanh chuỗi bước từ Local Hook lên GitHub Actions. | Hay bỏ qua các trường hợp ngoại lệ (test fail, merge conflict), mặc định lúc nào quy trình cũng chạy êm. | Tự thêm nhánh Exception/Retry khi có xung đột, quy định dev phải sửa tay trong IDE. |
| **Research** | Tìm bài báo hoặc công cụ mã nguồn mở đã từng giải bài toán tương tự. | Gợi ý nhanh vài công cụ như Commitizen, Commitlint, Semantic Release. | Đưa số liệu ước tính về hiệu năng tiết kiệm thời gian nhưng không có nguồn để kiểm chứng. | Tự vào tài liệu chính thức của Conventional Commits và GitHub để đối chiếu lại. |
| **Problem Statement** | Nhờ phản biện xem các trường trong Problem Statement v0 đã đủ chặt chưa. | Nhắc đúng điểm: chỉ số đo lường ban đầu thiếu baseline và thiếu mốc thời gian thử nghiệm. | Có xu hướng viết lại câu chữ kiểu quảng cáo, nhiều mỹ từ sáo rỗng. | Giữ văn phong kỹ thuật, tự thêm bộ số liệu cụ thể cho 2 tuần / 20 PR. |
| **Rule / Workflow / Agent** | Hỏi về ranh giới giữa Workflow và Coding Agent trong môi trường Git. | Phân tích khá rõ khác biệt giữa AI can thiệp trên nhánh feature con và trên nhánh production. | Có xu hướng thiên về phương án Agent toàn năng vì nghe hoành tráng hơn. | Kéo nhóm về mức Workflow có kiểm soát, vì an toàn mã nguồn quan trọng hơn. |
| **Decision** | Rà lại điều kiện Rollback của một dự án có tích hợp AI. | Gợi ý tiêu chí như tỷ lệ người dùng từ chối gợi ý (rejection rate), ngưỡng chi phí API. | Gợi ý rollback chung chung kiểu "khi thấy không hiệu quả". | Cụ thể hóa: chi phí > 10 USD/dev/tháng hoặc tỷ lệ từ chối > 40% trong 2 tuần thì dừng. |

---

## 3. Reflection câu hỏi mở

### Tôi học được gì khi nghe top 3 problems của các bạn khác?
Nghe các bạn trình bày giúp tôi thoát ra khỏi cái khung nghiên cứu học thuật của riêng mình. Mỗi người gặp vấn đề trong một ngữ cảnh khác nhau - quản lý tin nhắn bán hàng, lọc log CI/CD, quản lý task họp - nhưng điểm chung của các bài toán tốt luôn là có người thật sự đau vì nó, quy trình lặp lại đều đặn, và điểm nghẽn đo được bằng thời gian. Bài học với tôi là một bài toán hay không nhất thiết cần mô hình phức tạp, mà cần đúng chỗ đau của số đông.

### Nhóm có lúc nào bị solution-first không?
Có, khá rõ ở đầu Phase 3. Khi Đăng đề xuất bài toán Git, phản xạ của mấy bạn trong nhóm là nghĩ ngay đến việc làm một Agent tự sửa code và tự merge kiểu Copilot Workspace. Cả nhóm bị cuốn theo cái "ngầu" của giải pháp tự động hóa hoàn toàn, quên mất rằng để AI tự merge vào production là rủi ro không nhỏ. May là nhóm dừng lại kịp, vẽ lại workflow và nhận ra Rule truyền thống (Branch Protection, Commitlint) mới là thứ bảo vệ hệ thống, còn AI chỉ nên hỗ trợ ở khâu sinh nội dung và tóm tắt.

### Tôi có thay đổi ý kiến sau khi bị challenge không?
Có. Ban đầu tôi khá tự tin với Problem Card #1 (trích xuất thông số từ paper học thuật) vì số liệu khá chi tiết. Nhưng khi bị hỏi lại: "Đề tài này hẹp quá, chỉ phục vụ nhu cầu cá nhân, 5 bạn còn lại đâu dùng hàng ngày nên khó cùng kiểm chứng", tôi mới nhận ra tính cộng tác của bài toán mới là yếu tố quyết định chứ không phải độ chi tiết của số liệu. Tôi bỏ bài của mình, dồn sức vào bài Git của nhóm.

### Tôi đóng góp gì thật sự vào artifact cuối?
Hai chỗ tôi thấy rõ nhất là:
1. **Ranh giới an toàn:** Tôi là người kiên quyết đòi đưa vào Problem Statement và Future Workflow điều khoản AI không được tự sửa code logic khi có conflict, và không được tự merge vào nhánh protected. Nhờ vậy giải pháp bớt mạo hiểm, kiểm soát được rủi ro hơn.
2. **Chỉ số đo lường:** Tôi chuyển các mục tiêu mơ hồ thành 6 chỉ số cụ thể có baseline - thời gian xử lý PR giảm từ 25–35 phút xuống dưới 15 phút, tỷ lệ commit chuẩn đạt 100%, số lần push lỗi vào production bằng 0. Nhờ đó Problem Statement v1 chặt hơn hẳn v0.

### Điều khó nhất khi viết Problem Statement là gì?
Khó nhất là xác định ranh giới và điểm can thiệp của AI. Rất dễ viết chung chung kiểu "AI hỗ trợ quy trình Git", nhưng khi phải nói rõ AI được chạm vào bước nào, dừng ở đâu, người phải can thiệp lúc nào, và nếu AI sai thì cứu bằng cách nào - lúc đó mới thấy ranh giới giữa một giải pháp thực tế và một ý tưởng nghe hay nhưng không làm được là rất mong manh.

### Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?
Nếu làm lại, tôi sẽ challenge mạnh hơn ngay từ Bước 3.1 khi gộp bài toán: đòi bỏ hẳn chữ "merge code" ra khỏi tên đề tài, chỉ giữ lại "chuẩn hóa commit message và tự động hóa mô tả Pull Request". Việc nhóm cứ giữ chữ "merge code" trong tên khiến Phase 5 và Phase 6 tốn khá nhiều thời gian chỉ để giải thích đi giải thích lại rằng AI không được tự merge. Nếu thu hẹp phạm vi dứt khoát từ sớm, nhóm đã có thêm thời gian để đào sâu vào thiết kế prompt và kịch bản pilot.

---

## Tự kiểm cuối bài (Self-check Phase 7)

- [x] Reflection nói rõ vai trò trong nhóm, cách dùng AI, điều học được và nếu làm lại sẽ đổi gì.
- [x] Đã phản tư trung thực việc AI sai/hời hợt ở đâu và bản thân đã sửa lại như thế nào.
- [x] Không để AI viết thay trải nghiệm thực tế; thể hiện rõ quan điểm và đóng góp cá nhân vào sản phẩm chung của nhóm.