# Nhựt Trần — Portfolio

Director of Photography · Camera Operator · Photographer — Sài Gòn

Trang chính: `Nhuttranshowreels.html` (`index.html` tự chuyển sang trang này).

## Cấu trúc

```
Nhuttranshowreels.html   trang web (HTML + CSS + JS trong 1 file)
index.html               chuyển hướng sang Nhuttranshowreels.html
media/
  hero.mp4               montage nền trang chủ (1080p, ~6MB)
  hero-poster.jpg        ảnh hiện trong lúc video tải
  nhut.jpg               ảnh chân dung phần About
  previews/<dự-án>.mp4   montage 6s mỗi dự án (1080p, ~2.7MB) — chạy khi rê chuột + nền trang dự án
  stills/<dự-án>/01–06   still grab từ video (01 = ảnh đại diện)
  reels/short-NN.mp4     13 clip ngắn
  photos/<hạng-mục>/     126 ảnh (street, portrait, lifestyle, landscape, bts)
```

Sửa nội dung: mở `Nhuttranshowreels.html`, tìm khối `CONFIG`, `PROJECTS`, `REELS`, `LOGOS`.

## Đưa lên GitHub + mở trang web miễn phí (GitHub Pages)

Folder có 270 file (~150MB). Cách dễ nhất là **GitHub Desktop**.
Upload qua trình duyệt cũng được, nhưng mỗi lần chỉ kéo được tối đa 100 file.

### Cách 1 — GitHub Desktop (khuyên dùng)
1. Tạo tài khoản tại github.com (nếu chưa có), tải GitHub Desktop: desktop.github.com
2. Mở GitHub Desktop → đăng nhập → **File → Add Local Repository…** → chọn folder `nhuttranshowreels`
3. Nó báo "not a Git repository" → bấm **create a repository** → Name: `nhuttranshowreels` → **Create Repository**
4. Bấm **Publish repository** → **bỏ tick "Keep this code private"** (GitHub Pages miễn phí cần repo public) → **Publish**

### Cách 2 — Terminal
Máy chưa khai báo tên/email cho git, làm 1 lần trước (dùng email tài khoản GitHub):
```bash
git config --global user.name "Tên của bạn"
git config --global user.email "email-github@example.com"
```
```bash
cd "/Users/huynhbakhoa/Downloads/Nhựt Trần showreels/nhuttranshowreels"
git init -b main
git add .
git commit -m "Nhựt Trần portfolio"
```
Tạo repo trống tên `nhuttranshowreels` trên github.com (Public, không tick README), rồi:
```bash
git remote add origin https://github.com/<tên-tài-khoản>/nhuttranshowreels.git
git push -u origin main
```

### Bật trang web
Trên github.com, vào repo → **Settings → Pages** → Source: **Deploy from a branch** → Branch: **main**, folder **/(root)** → **Save**.
Đợi 1–2 phút, trang sẽ ở: `https://<tên-tài-khoản>.github.io/nhuttranshowreels/`

Cập nhật sau này: sửa file → GitHub Desktop → **Commit to main** → **Push origin** (hoặc `git add . && git commit -m "..." && git push`).

## Lưu ý
- Repo public = ai có link cũng tải được ảnh/video. Muốn riêng tư thì để Private (khi đó GitHub Pages cần gói trả phí).
- Mỗi file < 100MB (giới hạn của GitHub); file lớn nhất ở đây ~6MB.
- Gắn tên miền riêng (vd nhuttran.com): Settings → Pages → Custom domain (cần mua tên miền).
