# Prompt Templates — Dùng Nhanh với Claude Code

Thư mục này chứa các prompt mẫu dùng nhanh (copy → paste → gửi) đã được thiết kế tối ưu cho **Claude Code**. Các prompt này hỗ trợ gọi trực tiếp slash command hoặc thực thi đơn lẻ theo tiêu chuẩn chất lượng cao.

---

## Danh Sách Prompt Mẫu

| # | File | Command Tương Ứng | Skill Tích Hợp | Mô Tả & Cải Tiến Mới |
|---|------|-------------------|----------------|----------------------|
| 01 | `prompt_01_generate_requirements.txt` | `/generate_requirements_from_website` | `requirements_analyzer` | Phân tích website/sơ đồ để sinh tài liệu Yêu cầu |
| 02 | `prompt_02_generate_test_cases.txt` | `/generate_manual_testcases_rbt` | `rbt_manual_testing` | **[Nâng cấp mới]** Sinh Manual TCs chuẩn RBT, Checklist 15 loại input fields, Race condition, Session, A11y, AI Self-Quality Gate & Automation Metadata |
| 03 | `prompt_03_create_framework_playwright.txt` | `/generate_automation_framework` | `qa_automation_engineer` | Dựng khung dự án Automation Playwright TypeScript |
| 03 | `prompt_03_create_framework_selenium.txt` | `/generate_automation_framework` | `qa_automation_engineer` | Dựng khung dự án Automation Selenium Java |
| 04 | `prompt_04_generate_script_playwright.txt` | `/generate_automation_from_testcases` | `qa_automation_engineer` | Viết kịch bản tự động Playwright TypeScript theo POM |
| 04 | `prompt_04_generate_script_selenium.txt` | `/generate_automation_from_testcases` | `qa_automation_engineer` | Viết kịch bản tự động Selenium Java theo POM |
| 05 | `prompt_05_convert_manual_to_automation.txt` | `/generate_automation_from_testcases` | `qa_automation_engineer` | Chuyển đổi Manual Test Cases sang Automation Script |
| 07 | `prompt_07_generate_test_data.txt` | `/generate_test_data` | `test_data_generator` | Sinh dữ liệu kiểm thử có cấu trúc |
| 08 | `prompt_08_analyze_flaky_tests.txt` | `/analyze_flaky_tests` | `flaky_test_analyzer` | Phân tích và khắc phục Flaky Tests |
| 09 | `prompt_09_generate_api_tests.txt` | `/generate_api_tests_from_swagger` | `qa_automation_engineer` | **[Nâng cấp mới]** Sinh API tests từ Swagger/OpenAPI cover 12 HTTP Status Codes, OWASP API Security (BOLA/IDOR, Mass Assignment, ReDoS), SLA < 2s & Dynamic Auth Token |

*Lưu ý: Prompt 06 (Review Automation Code) thực thi trực tiếp bằng skill `qa_automation_engineer`.*

## Cách Sử Dụng Trong Claude Code

1. Chọn prompt phù hợp với nhu cầu.
2. Mở file `.txt` và thay thế các thông tin trong ngoặc vuông `[...]` bằng dữ liệu thực tế dự án của bạn.
3. Copy toàn bộ nội dung file → Paste vào ô chat của **Claude Code**.
4. Agent sẽ tự động nạp skill, nhận diện command và thực thi quy trình theo đúng chuẩn tiêu chuẩn cao.
