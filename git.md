# Tạo repos

1. git init
   => nhánh chính : master

## git inint -b main

=> tạo repos local vs nhánh chính có tên main

#git remote add origin
=> liên kết repos remote vs repos local

##file .gitignore quy định những thư mục hay file kg dc phép đẩy lên respo remote
=> .gitignore nằm ở thư mục root

## git status

=> Kiểm tra sự thay đổi các file trong dự án

## git add

## git add . => dùng để thêm tất cả các file ở trong thư mục hiện tại vào staging

## git add -A => dùng để thêm tất cả các file ở trong dự án vào trong staging

## git add <đường dẫn file> => chỉ thêm file cụ thể vào trong staging

=> Thêm file vào trong staging

## working directory (file mau dỏ)

## staging (file màu xanh) =>file đã sẵn sàng đưa lên repos remote (có thể đưa file lên git repos remote)

## config git chỉ chạy duy nhất 1 lần

### git config --global user.name "tên"

### git config --global user.email "email"

## git commit -m "<message>"

=> dùng để gắn message vào trong những file đang ở staging dc phép đưa lên repos remote
=> mỗi commit có một mã sha (id)

## git log

=> kiểm tra lịch sử commit

## git push -u origin <tên nhánh>

=> đưa code lên repo remote
=> từ lần push code thứ 2 : git push

## git reset

=> đưa file từ staging về lại working

## git restore -S . (đưa tất cả các file đang ở staging về working)

## git restore -S <url file> (chỉ đưa duy nhất file về working)

## git checkout <url file>

=> 1. đưa 1 file đang dc chỉnh sửa về trạng thái trước đó

## git check out -b <tên nhánh>

=> tương đương với 2 lệnh git branch + git switch

## git checkout <tên nhánh>

=> tương đương vs lệnh git switch
=> dùng đẻ chuyển qua <tên nhánh>

## branch

// dev => Kiểm thử QA và dev

// staging => QA kiểm thử 1 lần nữa

// production => end user

git branch <tên nhánh>
=> tạo ra 1 nhánh mới
=> nhánh mới sẽ chứa toàn bộ code của nhánh đang đứng

git brach -a
=> liệt kê tất cả các branch đang có trong repos

git switch <tên nhánh>
=> chuyển qua nhánh <tên nhánh>

## git pull

=> pull code ở repo remote về local

## git pull --no-ff (dùng khi git pull lỗi)
