## Git nâng cao
### 1. Kiểm tra các commit
` git log`
+ Bạn có thể thêm tùy chọn **--oneline** để xem log commit trên cùng một dòng có thể sẽ dễ quan sát hơn.<br>
`git log --oneline`
+ Để xem sự thay đổi trong một commit ta có thể sử dụng <br>
`git show [commit-id]`
+ So sánh sự thay đổi giữa 2 commit bằng lệnh <br>
`git diff [short-commit-id1]..[short-commit-id2].`
### 2. Chuyển một file về phiên bản cũ
Ví dụ: 
`$ git checkout ecd2a8a hello.txt`<br>
hello.txt đã quay về phiên bản trong quá khứ tương ứng với ecd2a8a, lúc này file không có nội dung gì (empty file).
### 3. Sửa lỗi commit
`$ git commit --amend`
### 4. Xung đột khi hợp nhất
### 5. Thiết lập .gitignore
Thông thường Git sẽ theo dõi mọi file trong dự án của bạn, tuy nhiên trong nhiều trường hợp chúng ta không muốn Git theo dõi một số thư mục hoặc file như:<br>
+ Thư mục node_modules không cần theo dõi vì mỗi thành viên chỉ cần chạy npm install là có thể tải được về thư mục này
+ Những file cấu hình local riêng của mỗi thành viên
+ Những file được tự động build ra từ các file code chính trong dự án.
-> Bạn có thể tạo file `.gitignore` (chú ý có dấu chấm phía trước nhé) để nói với Git rằng không cần theo dõi danh sách thư mục hoặc file được liệt kê bên trong nó.