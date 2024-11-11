# Git basic
### 1. Git and how it works
![alt text](image.png)<br>
 **Remote**: This is the Git server side where the project’s source code is stored.<br>
 **Local**: This is the client side (your computer) where the source code is cloned from the remote repository.  
+ **git add**: Command to move files from "Working directory" to "Staging area".
+ **git commit**: The command to move files from the "Staging Area" to the "Repository."
+ **git checkout**: The command to switch to a different branch in the "Repository" (each repository can have multiple branches).
+ **git merge**: The command to merge code from one branch to another.
+ **git push**: The command to push code from the Local "Repository" to the Remote "Repository."
+ **git pull**: The command to fetch code from the Remote "Repository" to the Local "Repository."<br>
### 2. Các thao tác cơ bản
#### Tạo một kho lưu trữ - git init
#### Kiểm tra trạng thái - git status
#### git add 
+  Di chuyển 1 file có sự thay đổi tới Staging Area <br>
`$ git add hello.txt`
+  Thêm tất cả thay đổi trong thư mục.<br>
`$ git add -A` hoặc `$ git add .`
#### git commit - di chuyển files từ Staging Area tới vùng Local Repository
+ Ví dụ commit việc thêm file hello.txt vào dự án<br>
`$ git commit -m "Create hello.txt"`<br>
**-m** viết tắt của "message", tức là thông điệp của commit này nói lên điều gì.
### 3. Kho lưu trữ từ xa (remote repository)
Để tạo ra một remote repository ta đăng nhập một trong các bên cung cấp máy chủ Git như github, gitlab, v.v. Sau đó vào repository của bạn, chọn **Clone -> Clone with SSH -> Copy URL**
+ Thêm remote repository vào cài đặt phía local<br>
`$ git remote add origin git@.../myrepo.git` <br>
Lệnh trên sẽ thêm remote repository vào file cấu hình phía local tại my_project/.git/config.
#### Tải lên máy chủ - git push
Theo mặc định khi tạo mới repository (git init) sẽ có một nhánh (branch) tên là "master".  Vì vậy chúng ta có thể đẩy (push) nhánh "master" tại local lên remote ngay bây giờ với lệnh :<br>
`git push origin master`
#### Lấy các thay đổi từ máy chủ - git pull
Chạy `git pull origin master` để lấy các thay đổi từ nhánh "master" trên remote về nhánh "master" trên local.
### 4. Nhánh và thao tác với nhánh
Xin chào
