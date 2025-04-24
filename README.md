# 1. Quy trình làm việc với git
Bước 1: Clone Repo về máy <br>
git clone https://github.com/luuquangphu/DAn_QuanLyNhaHangBuffet.git

Bước 2: Chuyển vào thư mục đã clone<br>
cd DAn_QuanLyNhaHangBuffet

Bước 3: Cấu hình thông tin Git cá nhân<br>
git config --global user.name "(thay ngoặc này bằng Họ tên)"<br>
git config --global user.email "(thay ngoặc này bằng Email)"

Bước 4: Checkout sang đúng nhánh của mình(Xem trên GitHub vào phần Branches xem nhánh theo đúng tên)<br>
git checkout (Tên nhánh)

Bước 5: Quy trình push code lên nhánh làm việc  
git add . ("." để thêm tất cả các file hoặc có thể sài git add a.txt để chỉ định 1 hay nhiều file muốn add)  
git commit -m "(thay ngoặc bằng file đã thêm hay việc đã làm)"  
git push (đối với git push lần đầu hãy kéo xuống mục dưới)  
  
Bước 6: Quy trình lấy code từ main repo về  
Bước 6.1: Dùng git pull(lệnh này sẽ lấy code về và tự động merge code kéo xuống dưới để xem git pull)  
Bước 6.2: Dùng git fetch(lệnh này sẽ lấy code về nhưng sẽ không merge vào nhánh đang làm việc xem cách làm ở mục 2.1)

# 2.Note: Quan trọng

# 2.1 Muốn xem sự thay đổi của main repo sài git fecth và git status để kiểm tra sự thay đổi code

git fetch origin<br>
git status<br>
--Nếu có thay đổi/commit từ nhánh khác và muốn cập nhật code hãy sử dụng, để hợp nhất thay đổi<br>
git merge origin/main

# 2.2 Mỗi khi commit nếu có thêm file hay làm chức năng gì thì khi rõ trong phần message

# 2.3 Khuyến khích sử dụng git fetch rồi merge để tránh conflict theo lệnh ở trên

==== Khi sài [git push] lần đầu ====

+ Sử dụng: git push -u origin (Tên nhánh) (lệnh này sẽ push lên nhánh đang làm việc)

+ Những lần sau sài git push bình thường

+ Nếu push từ các nhánh thì những commit chỉ ở trong nhánh đang làm việc thôi nên sẽ chưa được cập nhật trong main repo

 ==== Khi sài [git pull] lần đầu ====

+ Sử dụng: git pull origin main

+ Những lần sau sài git pull bình thường

