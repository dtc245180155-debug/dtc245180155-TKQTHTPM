# Đồ án: Triển khai và Quản trị Hệ thống Phần mềm (TKQTHTPM)
- **Mã số sinh viên:** DTC245180155
- **Đề tài:** Đề 3 - Website Quảng bá Sản phẩm (WordPress)

---

## 🏗️ 1. Cấu trúc Hệ thống & Công nghệ
Hệ thống được đóng gói hoàn toàn bằng Docker Compose, bao gồm 9 container dịch vụ:
* **Nginx Alpine:** Làm Reverse Proxy, định tuyến và tích hợp Security Headers cơ bản.
* **WordPress & MySQL 8.0:** Nền tảng ứng dụng web quản lý sản phẩm và cơ sở dữ liệu.
* **phpMyAdmin:** Công cụ quản lý CSDL trực quan trên nền web.
* **Prometheus & cAdvisor:** Giám sát thông số tài nguyên hệ thống (CPU, RAM, Network).
* **Grafana:** Trực quan hóa Dashboard giám sát và hiển thị Log.
* **Loki & Promtail:** Hệ thống gom log tập trung và truy vấn LogQL.

---

## 🚀 2. Hướng dẫn Chạy hệ thống (Quick Start)

### Yêu cầu tiên quyết:
- Đã cài đặt **Docker** và **Docker Compose** trên Ubuntu Server.

### Các bước thực hiện:
1. Clone repository về máy ảo:
   ```bash
   git clone [https://github.com/dtc245180155-debug/dtc245180155-TKQTHTPM.git](https://github.com/dtc245180155-debug/dtc245180155-TKQTHTPM.git)
   cd dtc245180155-TKQTHTPM
