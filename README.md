# STM32F103C8T6 LCD1602 8-Bit Parallel HAL Library

[![GitHub License](https://img.shields.io/github/license/phongtrinh1234523/lcd1602?color=blue)](LICENSE)
[![STM32CubeHAL](https://img.shields.io/badge/HAL-STM32Cube-orange.svg)](https://www.st.com/)
[![MCU](https://img.shields.io/badge/MCU-STM32F103C8T6-blueviolet.svg)](https://www.st.com/)

Một thư viện nhỏ gọn, tường minh và được tối ưu hóa theo hướng hướng đối tượng (Object-Oriented C) giúp giao tiếp màn hình **LCD1602/LCD2004** ở **chế độ song song 8-bit** sử dụng STM32CubeHAL.

A lightweight, object-oriented C library for interfacing **LCD1602/LCD2004** displays in **8-bit parallel mode** using STM32CubeHAL, tailored for STM32F103C8T6 (Blue Pill).

---

## 📌 Tính năng nổi bật / Key Features

* **Chế độ dữ liệu 8-bit đầy đủ (8-bit Parallel Mode):** Cho tốc độ truyền tải tối đa và xử lý lệnh cực kỳ tường minh.
* **Thiết kế hướng đối tượng (Object-Oriented Design):** Đóng gói toàn bộ cấu hình chân (GPIO Ports & Pins) vào cấu trúc `struct LCD`. Nhờ đó, bạn có thể quản lý và điều khiển **nhiều màn hình LCD cùng lúc** độc lập trên một vi điều khiển.
* **Linh hoạt phần cứng:** Không cố định chân cứng, cho phép gán bất kỳ chân GPIO nào (đã cấu hình `GPIO_Output`) thông qua mã nguồn ứng dụng mà không cần sửa lõi thư viện.

---

## 📂 Cấu trúc mã nguồn / Repository Structure

```text
├── LCD.h   # Định nghĩa cấu trúc dữ liệu, các Macro điều khiển và nguyên mẫu hàm API.
└── LCD.c   # Triển khai chi tiết các hàm khởi tạo, tạo xung ghi và dịch vị trí con trỏ.
