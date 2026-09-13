# 📊 BÁO CÁO THU HOẠCH NGHIỆM THU BÀI LAB 3 (BƯỚC 3 — SUBMISSION ARTIFACT)

> **Họ và Tên Học viên:** Cao Đức Anh
> **Mã Sinh Viên / Mã Học viên:** 2A202602754
> **Chủ đề Lựa chọn:** Trợ lý Học vụ & Tra cứu Lịch thi VinUni

---

## 1. BẢNG CHẤM ĐIỂM AGENTIC FIT SCORING MATRIX (ĐÁNH GIÁ CHỦ ĐỀ)

| Tiêu chí Đánh giá | Mức độ (1 - 5) | Giải trình chi tiết lý do chọn điểm |
| :--- | :---: | :--- |
| **1. Multi-step Reasoning** | 2 / 5 | Phần lớn yêu cầu dừng ở mức tra cứu 1–2 bước. Ít công việc cần suy luận phức tạp |
| **2. Tool Interaction** | 3 / 5 | Cần tích hợp công cụ lấy lịch thi cá nhân và tra cứu sổ tay sinh viên |
| **3. Dynamic Decision** | 2 / 5 | Luồng xử lý cố định, kết quả của đầu ra không làm thay đổi bản chất của mục tiêu hay hệ thống |
| **4. Long Horizon Goal** | 2 / 5 | Tương tác theo phiên, người dùng hỏi và nhận câu trả lời xong là kết thúc, không cần giữ trạng thái hay theo dõi mục tiêu kéo dài |
| **TỔNG ĐIỂM AGENTIC FIT** | **9 / 20** | *Nếu tổng điểm > 12/20: Bài toán rất phù hợp triển khai Agentic System.* |

---

## 2. TRÍCH XUẤT KẾT QUẢ WATERFALL TRACE LOG (SAU KHI CHẠY TEST SUITE TRÊN API THẬT)

> ⚠️ **YÊU CẦU NGHIỆM THU:** Mở tệp `.env` điền `GEMINI_API_KEY` (hoặc `OPENAI_API_KEY`) để kết nối LLM thật trước khi thực thi `python src/app.py --all`. Bài nộp chỉ dùng Mock Offline Provider sẽ không đạt điểm nghiệm thực tế.

Dán 1 đoạn trích xuất log tiêu biểu từ file `docs/trace_waterfall.json` sinh ra từ phản hồi LLM API thật:

```json
[
  {
    "step": 1,
    "query": "Chào bạn, bạn có thể giới thiệu quy chế học vụ cơ bản của Đại học VinUni không?",
    "action_type": "FINAL_ANSWER",
    "thought": "Gemini phản hồi trực tiếp bằng văn bản (không cần gọi công cụ).",
    "output": "Chào bạn! Đại học VinUni áp dụng các tiêu chuẩn học vụ quốc tế theo định dạng của các trường đại học hàng đầu thế giới (đặc biệt theo chuẩn kiểm định của Ivy League). Dưới đây là một số điểm cơ bản trong quy chế học vụ của VinUni:\n\n1. **Hệ thống tín chỉ và Đánh giá học tập:**\n   * VinUni áp dụng hệ thống tín chỉ (Credit System).\n   * Điểm số thường được đánh giá theo hệ thống chữ cái (A, B, C, D, F) tương ứng với Thang điểm GPA hệ 4.0.\n\n2. **Yêu cầu về Tiến độ và Điểm số (Academic Standing):**\n   * Sinh viên cần duy trì mức Điểm trung bình tích lũy (Cumulative GPA - CGPA) tối thiểu theo quy định của trường/chương trình (thường là từ 2.0/4.0 trở lên) để đảm bảo tình trạng học tập tốt (Good Standing).\n   * Nếu CGPA hoặc GPA học kỳ rơi xuống dưới mức quy định, sinh viên có thể bị đưa vào diện Cảnh báo học vụ (Academic Warning) hoặc xem xét buộc thôi học nếu không cải thiện sau thời gian quy định.\n\n3. **Thời gian đào tạo:**\n   * Thời gian chuẩn cho chương trình Cử nhân thường là 4 năm (bao gồm các học kỳ chính và học kỳ hè tùy theo chương trình).\n\n4. **Đăng ký môn học và Cố vấn học tập (Academic Advising):**\n   * Mỗi sinh viên sẽ được phân công một Cố vấn học tập (Advisor) để đồng hành, định hướng lộ trình học tập và phê duyệt danh sách môn học đăng ký mỗi học kỳ.\n\nNếu bạn cần tra cứu thông tin học vụ cá nhân (như điểm số, tình trạng học tập, v.v.) hoặc cần đặt lịch hẹn với Cố vấn học tập, vui lòng cung cấp **Mã sinh viên** (ví dụ: SV2026001) để tôi hỗ trợ bạn nhé!",
    "latency_ms": 5155.57
  }
]
```

---

## 3. TỔNG KẾT KẾT QUẢ NGHIỆM THU & NỘP BÀI

- [X] Đã điền API Key thật trong `.env` và xác nhận Agent chạy mượt mà trên LLM API thật (Gemini/OpenAI).
- **Tổng số Test Cases đã chạy thành công:** 5 / 5 test cases.
- **Số lượt gọi Tool qua MCP Server chính xác:** 4 lượt.
- **Kết quả đẩy Repo nộp bài:** [X] Đã Commit và Push mã nguồn thành công lên GitHub cá nhân.

---

> ✅ **HOÀN TẤT NỘP BÀI:** Sao chép đường link GitHub Repository cá nhân của bạn và dán vào ô nộp bài trên hệ thống LMS VLearn để hoàn tất Bài Lab 3!
