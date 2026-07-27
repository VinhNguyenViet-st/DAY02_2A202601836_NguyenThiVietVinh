# Group Report — Day 02

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|-----|-----------|-------------|--------------------|
| 1   |Vũ Văn Huy      |2A202601342|Đóng góp nội dung|
| 2   |Hoàng Văn Quang |2A202601334|Người trình bày|
| 3   |Nguyễn Thị Việt Vinh|2A202601836|Đóng góp nội dung|
| 4   |Trịnh Bá Khánh Trình|2A202601531|Đóng góp nội dung|

## Trình bày top 3

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh |
|---|---|---|---|---|---|
| 1 | Hoàng Văn Quang | Tổng hợp bản tin AI buổi sáng (Daily AI Digest) | Người quan tâm đến AI | Lọc tin rác và bài viết không đúng trọng tâm | Workflow |
| 2 | Hoàng Văn Quang | Tóm tắt nhanh Video/Bài báo kỹ thuật dài | Người quan tâm đến AI | Tiêu thụ toàn bộ nội dung để tìm ra vài ý chính | Workflow |
| 3 | Hoàng Văn Quang | Phân loại & tra cứu Bookmark/Notes cá nhân | Người quan tâm đến AI | Hệ thống tag cứng nhắc, không tìm lại được thông tin | Agent |
| 4 | Vũ Văn Huy | Tìm kiếm, dịch sát nghĩa & tóm tắt tài liệu tiếng Anh | Sinh viên đại học / Thực tập sinh | Dịch sát nghĩa tiếng Việt và đọc lọc ý tóm tắt | Workflow |
| 5 | Vũ Văn Huy | Tailor CV & Viết Cover Letter theo từng Job Description (JD) | Sinh viên năm cuối / Fresher, Junior | So sánh từ khóa JD và viết Cover Letter | Workflow |
| 6 | Vũ Văn Huy | Gom bài & theo dõi tiến độ bài tập nhóm rải rác trên Zalo | Nhóm trưởng môn học (Leader) | Nhắc nhở và đi gom bài | Rule, Workflow |
| 7 | Trịnh Bá Khánh Trình | Tổng hợp Weekly Report từ CSV xuất ra từ Grafana | PM hoặc QC lead | Viết narrative từ số liệu và ghép nhiều nguồn | Workflow |
| 8 | Trịnh Bá Khánh Trình | Gán nhãn ảnh CVAT thủ công | CTV labeling / QC | Vẽ bounding box thủ công cho từng object | Workflow |
| 9 | Trịnh Bá Khánh Trình | QC human-loop ảnh AI nhận diện dưới ngưỡng | QC reviewer | Mở tuần tự ảnh dưới ngưỡng, so sánh ground truth | Workflow |
| 10 | Nguyễn Thị Việt Vinh | Phân tích JD và gợi ý chỉnh CV | Sinh viên năm cuối | Đọc JD và xác định nên chỉnh phần nào của CV | Workflow |
| 11 | Nguyễn Thị Việt Vinh | Theo dõi job phù hợp trên nhiều nền tảng | Sinh viên năm cuối | Mở nhiều website tuyển dụng, dễ bỏ lỡ job | AI |
| 12 | Nguyễn Thị Việt Vinh | Viết cover letter cho từng công ty | Sinh viên năm cuối | Viết Cover Letter riêng cho từng công ty | AI |


 ## Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A (Tìm việc & Xin việc) | 5, 10, 11, 12 | Tự động hóa tìm việc, phân tích JD, tinh chỉnh CV và viết Cover Letter. | Đều là nhu cầu thiết yếu của sinh viên năm cuối. |
| B (Xử lý thông tin & Tóm tắt) | 1, 2, 4 | Lọc, dịch thuật và tóm tắt thông tin/tài liệu/video thành ý chính. | Tập trung vào giải quyết việc quá tải thông tin, giảm thời gian đọc hiểu. |
| C (Tổng hợp dữ liệu & Báo cáo) | 3, 6, 7 | Gom nhóm, phân loại và tổng hợp dữ liệu rải rác thành hệ thống hoặc báo cáo. | Cần workflow tốt để gom dữ liệu trước khi dùng AI. |
| D (Xử lý ảnh & Labeling) | 8, 9 | Tác vụ thủ công lặp lại trong Computer Vision (gán nhãn, kiểm tra chất lượng). | Đặc thù ngành CV, có thể áp dụng mô hình AI có sẵn (như SAM) để rút ngắn thời gian. |



## Shortlist và score

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Daily AI Digest | 5 | 5 | 5 | 5 | 5 | 5 | 5 | 35 |
| Tìm & Dịch tài liệu tiếng Anh | 4 | 4 | 4 | 4 | 5 | 4 | 5 | 30 |
| Tổng hợp Weekly Report | 4 | 5 | 4 | 4 | 3 | 4 | 4 | 28 |

Nhóm chọn: **Daily AI Digest (Tổng hợp bản tin AI buổi sáng)**.

Vì sao chọn:

- Có workflow rõ nhất, đang là pain point thực tế mỗi ngày.
- Impact dễ đo lường trực tiếp bằng thời gian (so với 30-60 phút/sáng).
- Có thể dùng nhiều tool AI hiện có để test nhanh (LLM summarization, Agent).
- Có thể vẽ before/after rất rõ ràng.

Vì sao không chọn các bài khác:

- Tìm & Dịch tài liệu tiếng Anh: Dễ làm, nhưng chưa tạo ra business/personal value vượt trội (hiện tại Google Translate/ChatGPT cơ bản đã làm khá tốt mà không cần custom workflow phức tạp).
- Tổng hợp Weekly Report: Phụ thuộc nhiều vào data nội bộ công ty (Jira/Grafana), khó test và validate nhanh trong phạm vi lab.

## Quick validation

Nhóm hỏi nhanh 3 người học/làm trong ngành IT/AI.

| Nguồn | Số người | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Quick interview | 3 | 2/3 người cũng mất nhiều thời gian lướt xem tin tức rác; muốn có bản tóm tắt ngắn | 1 người chỉ đọc 1 trang web quen thuộc nên không thấy ngợp | Thu hẹp problem: Tập trung vào "người muốn theo dõi nhiều nguồn tin đa dạng" |
| Mini poll trong lớp | 6 | 5/6 người muốn có một bản cập nhật công nghệ ngắn gọn hàng ngày | Một số sợ bản tóm tắt bỏ sót thông tin kỹ thuật chuyên sâu | Thêm AI fallback: Có link đến bài gốc để người dùng đọc chi tiết |

Insight sau validation:

```text
Pain không phải là "không có tin để đọc", mà là "có quá nhiều tin, lẫn lộn tin rác, tốn thời gian tự lọc để tìm thông tin chất lượng".
```

## Research giải pháp

Nhóm tìm các hướng đã có sẵn, không giả định phải tự build từ đầu.

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| TLDR Newsletter | https://tldr.tech/ | Tổng hợp tin tức công nghệ mỗi ngày | Đã lọc sẵn tin hay | Nội dung tiếng Anh, chung chung, không customize theo sở thích cá nhân | Cần hướng đến cá nhân hóa (Personalized) |
| Feedly AI | https://feedly.com/ai | Gom RSS và dùng AI lọc | Lọc theo chủ đề rất tốt | Setup phức tạp, chi phí cao | Workflow nên tự động gom các nguồn quen thuộc và tóm tắt nhanh |
| ChatGPT / Claude | https://chatgpt.com/ | Dùng prompt tóm tắt link cụ thể | Khả năng tóm tắt xuất sắc | Phải tự đi tìm link rồi paste vào thủ công mỗi ngày | Cần tự động hóa bước "đi tìm link" đầu vào |

Research takeaway:

```text
Không nên chỉ dùng LLM để tóm tắt thuần túy. Hướng giải quyết: Workflow tự động lấy link từ RSS/YouTube/News → LLM đánh giá độ liên quan & lọc tin rác → LLM tóm tắt các tin pass → Gửi digest (email/Telegram) mỗi sáng.
```

## Workflow before/after

File nhóm nộp kèm:

```text
02-group-problem-statement-workflow.png/pdf/md
```

Nội dung workflow:

```text
CURRENT STATE — 5 bước, 45 phút

[1 Mở YouTube xem feed: 10']
→ [2 Mở Google News tìm tin AI: 10']
→ [3 Vào Hacker News / Blog chuyên ngành: 15']
→ [4 Lọc thủ công bài viết hữu ích: 5'] <-- bottleneck (lọc tin rác)
→ [5 Đọc chi tiết từng bài: 5']

FUTURE STATE — 3 bước, 7 phút

[1 Auto-pull từ RSS/Youtube (Make/Zapier): 1'] -- Rule/script
→ [2 AI lọc & draft digest (LLM): 1'] -- Workflow step
→ [3 Người dùng đọc Digest trên Telegram/Email: 5'] -- Human boundary

Fallback:
Nếu AI bỏ sót tin hoặc tóm tắt sai → Người dùng có sẵn link gốc để click vào xem chi tiết.

Bottleneck mới:
AI đánh giá sai độ "relevant" của bài viết với sở thích người dùng. Có thể khắc phục bằng cách tinh chỉnh prompt tiêu chí lọc.
```

Before/after impact:

| Metric | Trước | Sau kỳ vọng | Ghi chú |
|---|---:|---:|---|
| Tổng thời gian | 45 phút | Dưới 10 phút | Target chính |
| Số bước | 5 | 3 | Tự động hóa hoàn toàn phần thu thập thông tin |
| Bước thủ công | 5/5 | 1/3 | Người dùng chỉ việc đọc Digest cuối cùng |
| Bottleneck chính | Tự lọc tin rác | Chất lượng lọc của AI | Có thể tinh chỉnh prompt để AI lọc tốt hơn |
| Risk mới | Lãng phí thời gian, mỏi mắt | AI bỏ sót tin quan trọng | Có kèm link gốc cho mỗi tin |

## Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Người làm IT / quan tâm đến AI muốn cập nhật kiến thức mới mỗi sáng. |
| **Workflow** | Truy cập thủ công nhiều nguồn (YouTube, Google, Blogs), tự lướt lọc tin clickbait, chọn lọc bài hay rồi mới đọc chi tiết. |
| **Bottleneck** | Bước lọc tin rác và bài viết không đúng trọng tâm mất nhiều thời gian (30-45 phút), dễ gây ngợp thông tin và mệt mỏi. |
| **Impact** | Mất nhiều thời gian mỗi buổi sáng nhưng lượng kiến thức thu lượm lại ít, hiệu quả thấp, dễ bỏ cuộc. |
| **Success Metric** | Giảm tổng thời gian gom và lọc tin xuống dưới 10 phút/ngày; giữ nguyên hoặc tăng số lượng tin hữu ích đọc được. |
| **Boundary** | AI không được thay đổi sự thật trong bản tin (hallucination); bắt buộc phải trích dẫn link gốc. |

## Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Dùng RSS feed reader gom tin vào 1 nơi | Đủ nếu người dùng có thời gian tự lướt đọc tiêu đề | Vẫn bị ngợp thông tin, phải tự đọc để lọc | Không |
| **Workflow** | Tool gom tin tự động (RSS) → AI lọc tin rác → AI tóm tắt → Gửi qua Telegram/Email | Hợp lý, chạy tự động theo lịch (ví dụ 7h sáng mỗi ngày) | AI lọc sai, bỏ sót tin quan trọng | Chọn |
| **Agent** | Agent tự động search internet tìm trend mới, tổng hợp báo cáo chuyên sâu tự động đổi chủ đề | Cần thiết nếu muốn phân tích trend sâu rộng, tự đi tìm nguồn mới liên tục | Quá phức tạp, chi phí API token cao | Chưa chọn |

Mức chọn:

```text
Workflow.
```

Vì sao:

- Bước gom nguồn tin cố định (RSS, YouTube) hoàn toàn có thể dùng tool (Make/Zapier) làm trigger.
- AI chỉ can thiệp vào đúng bước nó mạnh nhất: lọc văn bản rác và tóm tắt ý chính.
- Rủi ro thấp do người dùng là người cuối cùng đọc và kiểm chứng qua link gốc.
- Dễ dàng thực thi và test nhanh trong thời gian lab.

## Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | Người làm IT / quan tâm AI cần cập nhật tin tức mỗi sáng. |
| **Workflow** | Gom tin tự động từ các nguồn yêu thích → AI lọc tin → AI tóm tắt → Người dùng đọc Daily Digest qua Email/Telegram. |
| **Bottleneck** | Việc AI phân loại tin rác/clickbait và tóm tắt sao cho đúng trọng tâm mà không làm mất thông tin kỹ thuật cốt lõi. |
| **Impact** | Giảm đáng kể thời gian lướt tin từ 45 phút xuống dưới 10 phút, tăng cường sự tập trung vào kiến thức. |
| **Success Metric** | Giảm thời gian tự đi gom và lọc tin xuống bằng 0; thời gian đọc digest mỗi sáng dưới 10 phút. |
| **Boundary** | AI không tự chế ra tin tức (hallucination); luôn đính kèm link gốc để người dùng có thể tự đối chiếu. |
| **AI intervention point** | Sau khi tin thô được tự động kéo về từ web/RSS, và trước khi gửi đến tay người dùng. |
| **Mức chọn** | Workflow: dùng tool (Make/RSS) kéo data, AI thực hiện tóm tắt & đánh giá, bắn thông báo tự động. |
| **Rủi ro & người thật kiểm tra** | Risk: AI tóm tắt sai sự thật hoặc bỏ sót bài hay. Người thật kiểm tra: Người dùng trực tiếp đọc Digest, nếu thấy lạ có thể click link gốc để kiểm chứng. |

## Final decision

Decision:

```text
Go với scope nhỏ (Workflow tự động lấy tin và AI tóm tắt).
```

Pilot nhỏ nhất:

- Dùng tool automation (ví dụ: Make.com) tạo một luồng lấy tin (RSS) từ 2 trang tin AI uy tín.
- Gọi API (OpenAI/Gemini) truyền vào toàn bộ text bài viết, yêu cầu AI đánh giá độ phù hợp (0-10) và tóm tắt thành 3 gạch đầu dòng.
- Bắn tin nhắn tóm tắt qua Telegram cá nhân.
- Đo lường thời gian đọc và tần suất phải click vào link gốc trong vòng 3 ngày.

Exit / rollback:

- Nếu AI tóm tắt quá hời hợt hoặc bịa đặt (hallucinate) liên tục trong 2 ngày, quay lại cách đọc tin thủ công truyền thống qua RSS.

Decision rationale:

- Vấn đề có thật, xảy ra mỗi ngày với mọi người học IT/AI.
- AI tham gia vào đúng một bước cụ thể là tóm tắt NLP, không ôm đồm cả quá trình search động.
- Dễ dàng setup bằng các tool tự động hóa (No-code/Low-code) kết nối với LLM.
- Việc có người thật (Human in the loop) xem lại link gốc giúp triệt tiêu hoàn toàn rủi ro hallucination.
