# Đồ án Thiết kế và Triển khai Hệ thống Điều khiển Nhiệt độ Hơi Quá nhiệt

## Tổng quan

Đồ án tập trung vào việc thiết kế và triển khai hệ thống điều khiển nhiệt độ hơi quá nhiệt trong nhà máy nhiệt điện, sử dụng PLC Siemens S7-1200. Dự án bao gồm:

- Thiết kế sơ đồ P&ID (Piping and Instrumentation Diagram)
- Nhận dạng đối tượng điều khiển
- Tổng hợp bộ điều khiển (PID, IMC, Robust)
- Mô phỏng và lập trình trên TIA Portal

## Cấu trúc Dự án

### Chương 1: Phân tích Hệ thống và Thiết kế Sơ đồ Công nghệ

**Mục tiêu:** Xây dựng nền tảng lý thuyết và thiết kế cho hệ thống điều khiển

**Nội dung chính:**
- Thu thập và phân tích thông số công nghệ của hơi quá nhiệt
- Phân tích đặc tính quá trình nhiệt động học
- Thiết kế sơ đồ P&ID chi tiết với:
  - Các tín hiệu đo lường (nhiệt độ, áp suất, lưu lượng)
  - Hệ thống điều khiển và rơ-le bảo vệ
  - Van điều khiển và thiết bị công nghệ
- Xác định biến điều khiển, biến nhiễu và thông số quan trọng

### Chương 2: Thiết kế, Nhận dạng và Tổng hợp Bộ điều khiển

**Mục tiêu:** Phát triển các thuật toán điều khiển tối ưu

**Nội dung chính:**
- Lựa chọn cấu trúc điều khiển cascade phù hợp
- Nhận dạng mô hình đối tượng bằng phương pháp số
- Xác định thông số động học quan trọng
- Tổng hợp bộ điều khiển theo các phương pháp:
  - **Ziegler-Nichols:** Phương pháp kinh điển
  - **IMC (Internal Model Control):** Điều khiển dựa trên mô hình nội
  - **Robust Control:** Điều khiển bền vững
- Mô phỏng và so sánh hiệu năng:
  - Tiêu chí quá độ và thời gian ổn định
  - Sai số tĩnh và khả năng chống nhiễu

### Chương 3: Triển khai Lập trình trên PLC S7-1200

**Mục tiêu:** Thực hiện hóa hệ thống điều khiển trên phần cứng thực tế

**Nội dung chính:**
- Xây dựng giao diện vận hành và giám sát HMI
- Lập trình hệ thống điều khiển trong TIA Portal
- Tích hợp các tham số đã tính toán từ Chương 2
- Thử nghiệm và kiểm tra trong môi trường PLCSIM:
  - Khả năng vận hành và đo lường tín hiệu
  - Điều khiển đầu ra và phản hồi
  - Đánh giá kết quả thực tế

## Kết quả Đạt được

### Thành tựu Kỹ thuật
- ✅ Hệ thống điều khiển nhiệt độ hơi quá nhiệt hoàn chỉnh
- ✅ Mô phỏng và lập trình thành công trên PLC S7-1200
- ✅ So sánh và đánh giá hiệu quả các phương pháp điều khiển

### Kết quả So sánh
- **Bộ điều khiển bền vững + PID cascade** cho hiệu quả cao nhất:
  - Hạn chế quá độ tối ưu
  - Giảm sai số tĩnh
  - Tăng khả năng chống nhiễu
  - Đảm bảo tính ổn định

### Khả năng Mở rộng
- Tích hợp HMI/SCADA cho giám sát trực quan
- Hỗ trợ điều khiển từ xa
- Kiến trúc mở rộng cho các ứng dụng công nghiệp

## Ứng dụng và Hướng phát triển

### Ứng dụng Thực tế
- **Nhà máy nhiệt điện:** Tăng hiệu quả vận hành và an toàn
- **Công nghiệp hóa chất:** Điều khiển quá trình nhiệt
- **Hệ thống HVAC:** Ứng dụng trong điều hòa không khí

### Hướng phát triển
- **SCADA/IoT Integration:** Kết nối mạng Modbus TCP/Profinet
- **Tích hợp hệ thống trung tâm:** Kết nối với DCS/SCADA
- **AI/ML Enhancement:** Tích hợp trí tuệ nhân tạo cho tối ưu hóa

## Công nghệ Sử dụng

### Phần cứng
- **PLC:** Siemens S7-1200
- **Mô phỏng:** PLCSIM Advanced

### Phần mềm
- **TIA Portal:** Môi trường phát triển tích hợp
- **MATLAB/Simulink:** Mô phỏng và thiết kế điều khiển

### Thuật toán
- **PID Control:** Điều khiển tỷ lệ-tích phân-vi phân
- **IMC:** Internal Model Control
- **Robust Control:** Điều khiển bền vững

## Từ khóa

`PLC S7-1200` `điều khiển nhiệt độ` `hơi quá nhiệt` `PID` `IMC` `bộ điều khiển bền vững` `TIA Portal` `P&ID` `mô phỏng PLCSIM` `cascade control` `thermal process control`