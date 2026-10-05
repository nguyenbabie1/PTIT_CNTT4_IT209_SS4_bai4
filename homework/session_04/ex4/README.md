\## Minh chứng thực tế sau khi amend



Kết quả lệnh `git log -n 1` tại thời điểm kiểm tra:



```text

commit 99c2cc9e0fb853d78aa1cfaa7e50e8952399757d (HEAD -> main)

Author: Đoàn Trung Nguyên <brokeniuem569@gmail.com>

Date:   Mon Oct 5 07:51:59 2026 +0700



&#x20;   chore: ignore credentials and add exercise 4 report

```



Các kết quả khác:



\- `git status`: nothing to commit, working tree clean.

\- `git ls-files -- homework/session\_04/ex4/credentials.txt`: không có kết quả.

\- `Test-Path homework/session\_04/ex4/credentials.txt`: True.

