
Bước 1: Clone Repo về máy
git clone https://github.com/luuquangphu/DAn_QuanLyNhaHangBuffet.git

Bước 2: Chuyển vào thư mục đã clone
cd DAn_QuanLyNhaHangBuffet

Bước 3: Cấu hình thông tin Git cá nhân
git config --global user.name "(thay ngoặc này bằng Họ tên)"
git config --global user.email "(thay ngoặc này bằng Email)"

Bước 4: Checkout sang đúng nhánh của mình(Xem trên GitHub vào phần Branches xem nhánh theo đúng tên)
git checkout (Tên nhánh)

# Note: Quan trọng ***

# Mỗi lần làm việc hãy sài git fecth về để kiểm tra có thay đổi code gì không
git fetch origin
git status
--Nếu có thay đổi/commit từ nhánh khác và muốn cập nhật code hãy sử dụng, để hợp nhất thay đổi
git merge origin/main

# Mỗi khi commit nếu có thêm file hay làm chức năng gì thì khi rõ trong phần message

# Khuyến khích sử dụng git fetch rồi merge để tránh conflict theo lệnh ở trên

==== Khi sài [git push] lần đầu ====

+ Sử dụng: git push -u origin (Tên nhánh) (lệnh này sẽ push lên nhánh đang làm việc)

+ Những lần sau sài git push bình thường

+ Nếu push từ các nhánh thì những commit chỉ ở trong nhánh đang làm việc thôi nên sẽ chưa được cập nhật trong main repo

 ==== Khi sài [git pull] lần đầu ====

+ Sử dụng: git pull origin main

+ Những lần sau sài git pull bình thường

