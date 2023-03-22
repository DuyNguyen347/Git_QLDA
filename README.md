**Hướng dẫn chi tiết bài tập THỰC HÀNH GIT QUẢN LÝ DỰ ÁN**

1. Nhóm trưởng tạo repo mới để quản lý dự án bằng Github, thêm collaborators là các thành viên trong nhóm

2. Nhóm trưởng tiến hành protected branch main hoặc master bằng cách
        -> Settings -> Branches -> Rule

3. Nhóm trưởng cần khởi tạo source code ban đầu cho dự án
  
        + Nguồn code mẫu: https://github.com/NguyenPhuocDaiToan/bai-tap-QLDA
  
5. Mỗi thành viên cần clone Repository về và tạo một branch riêng để code từng phần của mình
        
        + Tạo branch bằng command: git branch new_branch
        
        + Chuyển nhánh bằng command: git checkout name_branch
        
        + Tạo và chuyển nhánh bằng command: git checkout -b name_branch
        
        + Quy ước đặt tên nhánh cho các thành viên do nhóm trưởng đề xuất


4. Sau khi code xong thì tiến hành dùng lệnh:

        + git add . (add tất cả file) hoặc git add name_file
        
        + git commit -m message_commit
        
5. Thay đổi nội dung message bằng command line: git commit --amend -m "New commit message."
   
        + Mục đích: ghi đè lên cam kết gần đây nhất với cam kết mới
   
6. Lấy lại code cũ dựa trên mã commit sau khi xoá nhánh
        + Tiến hành chuyển sang nhánh main (hoặc master) để xoá nhánh cá nhân vừa tạo bằng lệnh

        + git branch _D name_branch Hoặc git branch --delete name_banch
   
        + Sau đó dùng lệnh git reflog -1 để lấy lại id commit cuối cùng
   
        + Tiến hành tạo nhánh mới dựa trên code commit cũ
   
        
7. Thành viên đẩy code lên branch cá nhân và yêu cầu merge request

   + Tiến hành resolve conflict để tạo được yêu cầu merge request

8. Nhóm trưởng xác nhận merge code từ branch thành viên vào source code chính

9. Nhóm tiến hành Deploy bằng Github pages và gửi link vào MS Teams

* Các nhóm có thể tự tạo thêm bài tập để các thành viên hiểu được cách tương tác làm việc nhóm trong git
