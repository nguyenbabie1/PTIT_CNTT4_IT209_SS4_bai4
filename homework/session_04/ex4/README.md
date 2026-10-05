\# Bài 4: Quản lý .gitignore và sửa commit bằng Amend



\- Họ tên: Đoàn Trung Nguyên

\- Mã sinh viên: B24DTCN435

\- Lớp: HN-K24-CNTT4



\## Các bước thực hiện



1\. Tạo credentials.txt chứa thông tin giả phục vụ thực hành.

2\. Commit file với thông điệp:

&#x20;  oops: accidentally add credentials file.

3\. Tạo .gitignore với hai quy tắc: credentials.txt và \*.log.

4\. Chạy lệnh gỡ file khỏi Index của Git:



&#x20;  git rm --cached homework/session\_04/ex4/credentials.txt



5\. File vẫn tồn tại trên máy, kiểm tra bằng Test-Path trả về True.

6\. Đưa .gitignore và README.md vào Staging Area.

7\. Sửa nội dung và thông điệp commit gần nhất bằng:



&#x20;  git commit --amend -m "chore: ignore credentials and add exercise 4 report"



\## Giải thích



.gitignore giúp bỏ qua các file chưa được theo dõi. Nó không tự

gỡ bỏ file đã được Git theo dõi.



git rm --cached gỡ file khỏi Index nhưng giữ file vật lý trên máy.

Thao tác này được ghi vào commit khi chạy commit hoặc amend.



git commit --amend tạo commit thay thế commit gần nhất, có thể

thay đổi cả nội dung và thông điệp. Mã commit cũng thay đổi.



\## Kết quả kiểm tra



\- Test-Path trả về True: credentials.txt vẫn tồn tại trên máy.

\- git ls-files không liệt kê credentials.txt: Git không còn theo dõi file.

\- git status báo working tree clean sau khi hoàn tất.

\- git log -n 1 hiển thị thông điệp commit đã sửa.



Dán kết quả thực tế của git log -n 1 vào phần dưới đây trước khi nộp.

