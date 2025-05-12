# Rclone-Crontab

## 1. Tải Rclone và setup liên kiết giữa local và Google Drive

### Bước 0: Tải Rclone
```bash
sudo apt update
sudo apt install rclone
```

### Bước 1: Creating a Remote Connection to Google Drive using Rclone
```
rclone config
```
- Chọn n để tạo "New Remote"
- Nhập tên cho new remote (Ví dụ: "GoogleDrive")
- Chọn số ứng với Google Drive
- Requesting access from drive: **1**
- Edit advanced config?: **y**
- Những cái còn lại nhấn enter (Mặc định là default)

### Buóc 2: Đăng nhập để liên kết với Google Drive

- Sau khi liên kết xong thì chọn **q** để thoát setup Rclone

### Bước 3: Upload files from computer to Google Drive with rclone
```
rclone copy "<path_local>" "<Tên remote:Thư mục>"
```


