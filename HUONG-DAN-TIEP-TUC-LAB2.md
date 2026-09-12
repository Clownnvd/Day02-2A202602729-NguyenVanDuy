# Hướng dẫn tiếp tục Lab 2 trên máy khác — Nguyễn Văn Duy

**Bối cảnh:** AI20K Cohort 4, buổi Lab 2 tại E403 ngày 12/09/2026. Học viên: **NGUYỄN VĂN DUY**, mã **2A202602729**, GitHub `Clownnvd`.

- **Repo cá nhân để làm và nộp:** https://github.com/Clownnvd/Day02-2A202602729-NguyenVanDuy
- **Đề và worksheet đúng của buổi này:** https://github.com/VinUni-AI20k/K4B-Day02-AI-Product-Labs
- **VLearn:** vào khóa `k4p1` → ngày `D03` → Lab 2, đọc hướng dẫn và mở mục **Nộp bài** khi đã đăng nhập. Đường dẫn trực tiếp tới mục nộp (nếu phiên đăng nhập cho phép): https://vlearn.dev/course/k4p1/reader?day=D03&part=codelab-8b284e92e52b4137a46f33b51e861643-submit

Đây là **Lab 2: Tìm Đúng Bài Toán Cho AI**, không phải codelab Day 02 cũ của GDGoC FPTU. Bài này tập trung vào problem, workflow, metric, boundary và quyết định Rule / Workflow / Agent; **không yêu cầu làm app hay prototype code** theo README/worksheet của repo trên. Fiprove không nằm trong Individual Scan theo lựa chọn của Duy.

## 1. Đầu ra phải có

Mỗi học viên có **một repo cá nhân public** gồm ba phần:

| File trong repo này | Yêu cầu chính | Trạng thái lúc chuyển máy |
|---|---|---|
| [`01-individual-problem-scan/individual-report.md`](01-individual-problem-scan/individual-report.md) | Phase 1: ít nhất 5 problems từ trải nghiệm thật, có actor và dấu hiệu; Phase 2: top 3 Problem Cards với workflow trước/sau. | **Đã có bản nháp 8 vấn đề**, đúng 4 lăng kính (mỗi lăng kính 2), và 3 card. Duy cần đọc, xác nhận/sửa điều chưa đúng trải nghiệm; chưa có số phút đo thật. |
| [`02-group-problem-statement/group-report.md`](02-group-problem-statement/group-report.md) | Phase 3–6: nhóm hội tụ candidates, kiểm chứng, research, workflow, Problem Statement v0/v1, so Rule/Workflow/Agent và quyết định Go/Not Yet/No-Go. Mỗi người đưa **cùng bản nhóm cuối** vào repo cá nhân. | Google Doc chung ghi **5 thành viên, 13 candidate, chọn món ăn**, shortlist/score và `Not Yet`; bản repo đã chuyển các phần có thể dùng. Interview/survey trong Doc được tab khác gọi là **kịch bản minh họa**, chưa dùng làm bằng chứng thật. Cần nhóm xác nhận và coach xác nhận nhóm 5 người. |
| [`03-individual-reflection/reflection.md`](03-individual-reflection/reflection.md) | Phase 7: reflection cá nhân 8–12 câu về vai trò, pitch/challenge, cách dùng AI, điều sửa sau phản biện và bài học. | **Dàn ý và dữ kiện**, chưa phải reflection cuối. Duy phải tự viết bằng trải nghiệm thật; worksheet không cho AI viết thay phần này. |

Thang điểm trong [README đề gốc](https://github.com/VinUni-AI20k/K4B-Day02-AI-Product-Labs#ti%C3%AAu-ch%C3%AD-%C4%91%C3%A1nh-gi%C3%A1-100-%C4%91i%E1%BB%83m): **60 điểm nhóm + 40 điểm cá nhân**, bonus tối đa **+10**. Scan 8 vấn đề có thể đạt tiêu chí bonus về độ rộng nếu từng vấn đề thật và cụ thể; số lượng một mình không bảo đảm điểm.

## 2. Bài cá nhân đã chuẩn bị hôm nay

Phase 1 dùng đúng bốn lăng kính: **lặp lại, tốn thời gian, AI hỗ trợ tốt hơn, khó khăn từ người khác**. Tám vấn đề lấy từ buổi học này: hạn Lab 1 khác nhau giữa Discord/README; kiểm trạng thái nộp repo/VLearn; tìm đúng tài liệu; mở nhiều file khi pitch; phân biệt hai bộ Day 02; tổng hợp lý thuyết từ nhiều nguồn; khó truy vết ai thực sự đóng góp trong repo nhóm; câu hỏi công khai của bạn học về thông tin lớp/bài nộp. File scan có **tiêu chí riêng cho từng lăng kính** và **bảng giải thích vì sao lọc 8 xuống 3**. Các số đếm là quan sát của một phiên hoặc câu hỏi công khai, chưa phải khảo sát toàn khóa.

Phase 2 đã chọn ba card; [file 3 workflow](01-individual-problem-scan/01-individual-problem-scan-workflows.md) vẽ trước/sau cho từng card:

1. **Đối chiếu yêu cầu và hạn nộp** giữa Discord, VLearn, GitHub. Đây là card cá nhân Duy từng cân nhắc; Google Doc chung hiện ghi nhóm chọn **vấn đề chọn món ăn** từ candidate của thành viên khác.
2. **Kiểm tra repo trước khi nộp** đúng bài, đủ file, public và đúng cổng; baseline hợp lý là checklist/rule.
3. **Tìm đúng đoạn tài liệu** và giải thích ngắn có link, đúng khóa/phiên bản.

Mỗi card đã có problem một câu, actor, current workflow, bottleneck, metric mục tiêu, giải pháp không AI, giả thuyết AI, future workflow và fallback. **Metric phần trăm/20 case là mục tiêu pilot, không phải kết quả đã đạt.** Anh đọc từng card rồi sửa những chi tiết không đúng trải nghiệm của mình. Khi pitch, tự nói bằng lời của anh: *ai vướng → bước nào nghẽn → dấu hiệu nào đã thấy → cần hỏi nhóm điều gì*. Worksheet yêu cầu cá nhân tự pitch và tự challenge, không để AI nói/viết thay.

## 3. Việc cần làm theo thứ tự trên máy khác

1. **Mở repo cá nhân, đọc ba file trên và `01-worksheet.md`.** Xem thêm `02-deliverable-example.md` để hiểu hình dạng đầu ra. Giữ repo public. Nếu thấy bản scan mô tả sai trải nghiệm, sửa trước khi mang đi pitch.
2. **Xác nhận lại nhật ký hội tụ trong Google Doc với nhóm.** Doc đã ghi 13 candidates của 5 người, score 31/27/22 và chọn món ăn; cần từng thành viên xác nhận phần mình pitch/challenge, lý do chọn và disagreement thật. Hỏi coach về quy định nhóm 5 người vì worksheet mô tả nhóm 3–4.
3. **Kiểm chứng bài chọn món ăn bằng dữ liệu thật.** Hỏi nhanh **2–3 người** *hoặc* khảo sát/poll **5–10 người** theo worksheet. Tab “Thẻ 2” trong Doc gọi các quote/số hiện có là kịch bản minh họa, nên không nộp chúng như kết quả. Ghi cả phản hồi xác nhận lẫn phản bác, số phút/tần suất đo được. Nếu chưa đủ, ghi “chưa kiểm chứng” và giữ `Not Yet`.
4. **Research ít nhất 2–3 cách/tool đã tồn tại**, có **1–2 link nguồn** và so chúng xử lý bước nào của workflow; không chép số liệu AI không kiểm được. Bản nhóm đã có nguồn chính thức GrabFood, Grab AI Assistant và Uber Eats; nhóm cần tự kiểm và so với baseline bộ lọc/món quen.
5. **Vẽ workflow nhóm trước/sau** với actor, input/output, thời gian hoặc ghi rõ “chưa đo”, handoff, bottleneck, bước Rule/AI/người thật và fallback. Viết Problem Statement v0 có actor, workflow, bottleneck, impact, metric, boundary; phản biện rồi sửa thành v1.
6. **So No AI/process fix, Rule, Workflow, Agent; chốt Go/Not Yet/No-Go.** Với chọn món, thử bộ lọc giá/thời gian và đặt lại món cũ làm baseline; chỉ thêm AI để hiểu nhu cầu tự do/xếp ba món khi nó giúp nhanh hơn. Người dùng tự chọn và tự đặt. Google Doc hiện ghi `Not Yet`; nhóm cần xác nhận sau validation.
7. **Duy tự viết reflection 8–12 câu** sau hoạt động thật: card đã pitch, câu hỏi đã đặt, mình sửa gì, đóng góp nào vào bản nhóm, AI giúp/sai ở đâu, điều học được. Không nhận đã hỏi người dùng, đã pitch hay đã thống nhất nếu chưa xảy ra.
8. **Đưa bản nhóm cuối vào repo cá nhân, rà lại rồi nộp link repo trên VLearn.** Việc push GitHub **không tự điền ô nộp VLearn**. Mở mục Nộp bài của đúng Lab 2, dán URL repo cá nhân, bấm xác nhận và kiểm lại trạng thái trong tài khoản. Tại thời điểm lập hướng dẫn này, **chưa xác nhận đã nộp Lab 2 trên VLearn**.

## 4. Nếu chỉ có trình duyệt, không cần cài Git

Đăng nhập GitHub tài khoản `Clownnvd`, mở repo cá nhân ở trên. Vào file cần sửa → biểu tượng bút chì **Edit** → sửa → **Commit changes** vào `main`. Sau mỗi lần sửa, mở lại bản trên `main` để kiểm nội dung đã lên. Đừng xóa dữ kiện/bằng chứng gốc khi chưa có lý do; đánh dấu rõ phần chưa kiểm chứng. Sau khi ba file xong mới dán link **trang chủ repo** vào VLearn.

Nếu dùng Git trên máy mới:

```powershell
git clone https://github.com/Clownnvd/Day02-2A202602729-NguyenVanDuy.git
cd Day02-2A202602729-NguyenVanDuy
git pull origin main
# Sửa ba file báo cáo bằng editor, rồi:
git add 01-individual-problem-scan/individual-report.md 02-group-problem-statement/group-report.md 03-individual-reflection/reflection.md
git commit -m "Complete Lab 2 reports after group validation"
git push origin main
```

Nếu Git báo chưa đăng nhập, dùng GitHub Desktop hoặc đăng nhập GitHub theo hướng dẫn trên máy mới. **Không đưa token/API key hoặc mật khẩu vào repo hay cuộc chat.**

## 5. Tự kiểm trước khi gửi link

- [ ] Repo `Day02-2A202602729-NguyenVanDuy` ở chế độ public, trang `main` mở được khi không đăng nhập.
- [ ] Scan cá nhân giữ ít nhất 5 pain thật, 4 lăng kính, top 3 card có trước/sau và metric; Duy đã xác nhận nội dung.
- [ ] Có ghi nhận pitch/challenge và đóng góp thật của Duy, không gán việc của AI/người khác cho mình.
- [ ] Bản nhóm có dữ liệu nhóm thật, kết quả phỏng vấn/poll hoặc ghi rõ giới hạn, 2–3 giải pháp tham khảo, workflow, PS v0/v1, so Rule/Workflow/Agent và quyết định có lý do.
- [ ] Reflection cuối là 8–12 câu Duy tự viết sau khi làm, không còn placeholder.
- [ ] Repo public không chứa email/họ tên đầy đủ của **người khác** theo hướng dẫn VLearn; không chứa secret.
- [ ] Link repo đã được dán và xác nhận ở **VLearn Lab 2**, không nhầm Google Form/codelab cũ.

## 6. Đoạn chuyển giao để dán cho trợ lý trên máy khác

```text
Tôi là NGUYỄN VĂN DUY, mã học viên 2A202602729, làm AI20K Cohort 4 Day 02 Lab 2 ở E403. Repo cá nhân public của tôi: https://github.com/Clownnvd/Day02-2A202602729-NguyenVanDuy. Đề đúng: https://github.com/VinUni-AI20k/K4B-Day02-AI-Product-Labs. Hãy đọc README, 01-worksheet.md, HUONG-DAN-TIEP-TUC-LAB2.md và ba file báo cáo trong repo trước khi làm.

Phase 1 đã có 8 vấn đề theo bốn lăng kính; Phase 2 đã có top 3 Problem Cards cá nhân. Fiprove không được đưa vào scan. File nhóm đã chuyển sang vấn đề **chọn món ăn khi bận** từ Google Doc chung: Doc ghi 5 thành viên và 13 candidates, nhưng phần interview/survey trong tab “Thẻ 2” được ghi là kịch bản minh họa nên chưa thể dùng làm dữ liệu thật. Worksheet mô tả nhóm 3–4 người; cần coach xác nhận cách nộp nhóm 5. Reflection vẫn là dàn ý, chưa phải bài cuối. Hãy kiểm yêu cầu, chỉ ra chỗ thiếu, chỉnh theo dữ liệu thật tôi cung cấp. Đừng bịa phỏng vấn, số phút, đồng thuận hay đóng góp cá nhân. Không viết reflection/pitch/challenge thay tôi; chỉ gợi câu hỏi để tôi tự làm. Cuối cùng giúp kiểm repo public/main và hướng dẫn dán link vào đúng VLearn Lab 2.
```

**Nguồn ưu tiên khi có mâu thuẫn:** hướng dẫn trên VLearn của đúng khóa/buổi và [worksheet repo Lab 2 chính thức](https://github.com/VinUni-AI20k/K4B-Day02-AI-Product-Labs/blob/main/01-worksheet.md); nếu hạn hoặc quy định mới xung đột, hỏi người phụ trách/BTC và ghi lại xác nhận, không để AI tự đoán.
