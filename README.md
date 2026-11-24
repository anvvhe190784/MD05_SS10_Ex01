# Bài tập 1: Khởi tạo và kết nối VPS

## 1. Checklist khởi tạo VPS trên Cloud (AWS EC2 / Google Cloud / DigitalOcean / Vultr)
- **Hệ điều hành:** Ubuntu 22.04 LTS (hoặc 24.04 LTS).
- **Cấu hình tối thiểu:** Free Tier / 1 vCPU – 1 GB RAM.
- **Cloud Security Group / Firewall (Inbound Rules):** Mở sẵn các cổng TCP `22` (SSH), `8080` và `8081` (để kiểm thử so sánh UFW ở Bài 4).
- **Ghi lại thông số sau khi tạo:** Địa chỉ **IPv4 Public** và thông tin đăng nhập ban đầu (`root` hoặc `ubuntu` + file `.pem`).

## 2. Kết nối từ PowerShell trên máy cá nhân
Xem chi tiết câu lệnh trong [`commands.txt`](./commands.txt):
```powershell
ssh root@<VPS_PUBLIC_IP>
# hoặc (AWS EC2):
ssh -i "C:\Users\vanan\.ssh\<your-key>.pem" ubuntu@<VPS_PUBLIC_IP>
```

## 3. Ảnh minh chứng kết quả (sẽ bổ sung sau khi chạy trên VPS)
- `homework/session_10/exercise_01/vps_config.png` — Ảnh cấu hình thông số VPS trên giao diện Cloud.
- `homework/session_10/exercise_01/ssh_login.png` — Ảnh PowerShell/Terminal đăng nhập SSH thành công vào VPS.
