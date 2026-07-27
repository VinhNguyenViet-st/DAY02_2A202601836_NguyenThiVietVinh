# 03 — Individual Reflection Example

## Đóng góp của Mình trong nhóm

| Hoạt động | Mình đã làm gì? | Kết quả |
|---|---|---|
| Scan cá nhân | Đưa ra 7 vấn đề liên quan đến quá trình tìm việc của sinh viên năm cuối | Nhóm có thêm candidate về hỗ trợ tìm việc và tối ưu hồ sơ ứng tuyển |
| Pitch | Pitch bài toán Phân tích Job Description và gợi ý chỉnh CV | Bài toán được đưa vào shortlist và được nhóm chọn làm đề tài chính |
| Challenge | Đề xuất thu hẹp phạm vi từ "viết CV" sang "phân tích JD và gợi ý chỉnh CV", nhấn mạnh AI chỉ hỗ trợ gợi ý thay vì tự tạo nội dung | Giúp nhóm xác định scope rõ ràng, phù hợp phạm vi lab |
| Research | Tìm hiểu các giải pháp như ChatGPT, ResumeWorded, Kickresume AI và ATS Resume Checker | Nhóm xác định được các giải pháp hiện có và khoảng trống cần cải thiện |
| Rule | Phân tích và đề xuất chọn Workflow (AI phân tích JD → Gợi ý chỉnh CV → Người dùng review), không chọn Agent | Nhóm thống nhất chọn mô hình Workflow vì đơn giản, dễ triển khai và vẫn đảm bảo Human Review|

## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| Scan | Nhờ AI gợi ý thêm các vấn đề sinh viên năm cuối gặp khi tìm việc | Giúp mở rộng danh sách pain points như chỉnh CV, phân tích JD, ATS, Cover Letter | Một số ý quá chung hoặc không có workflow rõ ràng | Chỉ giữ các vấn đề có actor, workflow và metric cụ thể |
| Workflow | Nhờ AI xây dựng Current/Future Workflow và minh họa before/after | Giúp mô tả quy trình trực quan, xác định bottleneck | AI ban đầu gộp một số bước hoặc chưa thể hiện rõ bottleneck| Tách rõ bước Đọc JD → So sánh CV → Chỉnh CV, đánh dấu bottleneck ở bước chỉnh CV |
| Problem Statement | Nhờ AI góp ý Problem Statement, workflow và lựa chọn Rule/Workflow/Agent | AI giúp hoàn thiện Actor, Bottleneck, Success Metric và Human Boundary | Ban đầu AI mở rộng phạm vi sang Agent hoặc nhiều chức năng ngoài scope bài lab | Thu hẹp lại thành Workflow: AI phân tích JD → Gợi ý chỉnh CV → Người dùng review trước khi apply |

## Bài học của Mình

- Problem tốt không phải là problem có nhiều tính năng AI nhất, mà là problem có workflow rõ ràng, bottleneck cụ thể và có thể đo lường được.
- Vẽ workflow giúp xác định chính xác bước nào AI thực sự tạo ra giá trị, thay vì áp dụng AI cho toàn bộ quy trình.
- Workflow phù hợp hơn Agent trong bài toán này vì quy trình ứng tuyển có các bước cố định, AI chỉ hỗ trợ phân tích Job Description và gợi ý chỉnh CV, còn người dùng vẫn là người quyết định nội dung cuối cùng.
- Research giúp hiểu các sản phẩm hiện có như ChatGPT, ResumeWorded và Kickresume AI đang giải quyết vấn đề như thế nào, từ đó xác định khoảng trống và thiết kế giải pháp phù hợp thay vì sao chép tính năng của họ.
-Human review vẫn là bước quan trọng để đảm bảo CV phản ánh đúng năng lực thật của ứng viên và tránh AI đề xuất những nội dung không chính xác.

Nếu làm lại:

```text
Tôi sẽ validate với nhiều PM hơn trước khi chốt metric 90 phút → 30 phút, vì baseline hiện tại chủ yếu đến từ trải nghiệm của tôi.
```
