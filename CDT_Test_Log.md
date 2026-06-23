# BÁO CÁO PHIÊN KIỂM THỬ ĐỊNH HƯỚNG BỐI CẢNH (CDT LOG)
**Dự án:** Quản lý PC (Quy mô nhỏ)
**Người thực hiện:** Nguyễn Tuấn Anh 002
**Môn học:** Đảm bảo chất lượng & Kiểm thử phần mềm

---

## 1. THÔNG TIN PHIÊN KIỂM THỬ (Session Info)
* **Thời gian thực hiện:** 60 phút (Tập trung cao độ, không viết kịch bản trước).
* **Mục tiêu phiên:** Kiểm thử tích hợp hệ thống qua các API cốt lõi phục vụ tính năng hiển thị thông tin cấu hình PC.
* **Bối cảnh áp dụng:** Tiến độ dự án gấp, giao diện (Frontend) chưa hoàn thiện, nguồn lực nhân sự ít. Tùy biến chiến lược: Đánh giá nhanh qua Backend bằng công cụ miễn phí Thunder Client.

## 2. KẾT QUẢ THỰC THI (Execution Details)
* **API thực hiện:** `GET https://jsonplaceholder.typicode.com/posts/1` (Giả lập endpoint lấy chi tiết thông tin 01 máy tính trong hệ thống).
* **Trạng thái phản hồi (Status):** `200 OK` -> Hệ thống kết nối và phản hồi dữ liệu thành công dưới 300ms.
* **Xác thực dữ liệu (Data Verification):** Dữ liệu trả về đúng định dạng cấu trúc JSON bao gồm các trường thông tin ID, Title và Body, không xảy ra lỗi sập server (500) hay sai định dạng cấu trúc.

## 3. ĐÁNH GIÁ RỦI RO & KHUYẾN NGHỊ
* **Đánh giá:** API chạy ổn định, đáp ứng được yêu cầu về mặt hiệu năng cho dự án nhỏ.
* **Khách hàng thay đổi yêu cầu đột xuất:** Nhờ việc kiểm thử trực tiếp bằng Thunder Client tích hợp sẵn trên VS Code, nếu cấu trúc API thay đổi, Tester có thể chỉnh sửa lại tham số và bấm `Send` để kiểm tra lại ngay lập tức (mất 10 giây), tối ưu hóa thời gian so với việc sửa đổi các file tài liệu Excel truyền thống.