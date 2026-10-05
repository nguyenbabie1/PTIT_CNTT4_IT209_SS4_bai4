# Bài 2: Kết hợp cập nhật từ main và feature-update

## Báo cáo giải quyết xung đột

1. Tạo README.md trên main và commit nội dung ban đầu.
2. Tạo nhánh feature-update, sửa dòng tiêu đề và commit.
3. Quay lại main, sửa cùng dòng tiêu đề thành nội dung khác và commit.
4. Chạy git merge feature-update và nhận thông báo xung đột.
5. Mở README.md bằng Notepad, đọc nội dung của cả hai nhánh.
6. Sửa tiêu đề thành nội dung kết hợp và xóa thủ công các dấu xung đột.
7. Lưu file, chạy git add và git commit để hoàn thành merge.

## Cơ chế 3-Way Merge

Git so sánh ba phiên bản: commit tổ tiên chung, phiên bản trên main
và phiên bản trên feature-update.

Hai nhánh sửa cùng một dòng thành nội dung khác nhau nên xảy ra
xung đột. Sau khi sửa và commit, merge commit có hai commit cha.

## Minh chứng

![Lịch sử commit](git-log.png)