# ĐỒ ÁN WEB (Đọc qua trước đi nha).

## I. Hướng dẫn chạy dự án:

- Tải [git](https://git-scm.com) và [Node.js](https://nodejs.org/en/download)
- Clone dự án về local.
  - Chạy dòng lệnh **`git clone https://github.com/cngk-2002/DoAn_IE104.git`**.
  - Chạy dòng lệnh **`run npm prod`**(chế độ minify) hoặc **`run npm dev`** trên terminal.
- Bật Live Server.

## II. Công nghệ:

- HTML
- TailwindCSS, PostCSS
- JavaScript
- git, Github
- npm

## III. Giới thiệu Git:

Tóm tắt: Git dùng để quản lý phiên bản code, rất thuận lợi trong làm việc nhóm thậm chí làm 1 mình.

## IV. Các khái niệm trong git:

- Repository (kho): là thư mục. Thư mục trên github.com gọi là **remote repository**, còn ở máy tính là **local repository**.
- Branch (nhánh): ví dụ t làm 1 phần trên 1 nhánh, m rẽ sang nhánh khác làm chức năng khác, sau này hộp lại (merge).
- Remote (máy chủ)
- add (thêm): sau khi làm gì đó thay đổi thì add (thêm) cái thay đổi đó vào.
- commit: chốt thay đổi kèm theo 1 message (tin nhắn).
- pull (kéo về): lấy code của thằng làm chung đã push (đẩy) lên.
  - Pull từ branch nào về branch hiện tại cũng được, nếu pull từ branch khác thì sẽ có "Merge" xảy ra, còn pull từ cũng branch thì là như update code base.
  - Khi mình làm thay đổi dưới local trùng với chỗ người nào đó đã sửa và push lên (nhưng mình chưa pull về trước đó), thì khi pull về sẽ có "conflict".
  - "Conflict" nghĩa là "đụng độ". Khi code pull về bị conflict, cần phải "Resolve conflict" bằng cách chọn thay đổi nào được giữ lại và thay đổi nào sẽ xóa đi hoặc giữ lại cả 2 và chỉnh sửa cho tụi nó hoạt động.
- push (đẩy): đưa code lên remote repository, nghĩa là đẩy lên cho tụi kia pull về.
- Collaborators: làm việc nhóm với git như nào:
  ai tạo repos thì vào đây: https://github.com/<tên_tài_khoản>/<tên_repos>/settings/collaboration
  gõ email github thành viên vào, thằng được mời làm chung đồng ý thì làm thôi.

## V. Ví dụ thực tế:

- Khi làm gì đó thay đổi trên thư mục ở máy nhà, phải ADD sau đó COMMIT sau đó PUSH lên github. Làm như sau:
  - ADD: mở git bash (màn hình console) lên, gõ: git add \*
  - COMMIT: cũng trên bash, gõ: git commit -m "nội dụng đã thực hiện" trong đó cái trong dấu ngoặc kép là ghi chú của việc commit, cái này bắt buộc nhập.
  - PUSH: cũng trên bash, gõ: git push origin master.
- Khi ai đó push gì mới lên thì ở máy lấy về bằng cách: gõ trên bash tại thư mục đã khởi tạo git (git init): git pull origin master
- Hết.
