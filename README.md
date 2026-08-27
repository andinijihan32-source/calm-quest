# 🌿 Calm Quest

Board game edukasi kesehatan mental (100 kotak, gaya ular tangga) untuk membantu remaja mengenali dan menghadapi kecemasan lewat 5 zona: Akademik, Pertemanan, Keluarga, Masa Depan, dan Media Sosial.

Ini adalah aplikasi single-file (HTML + CSS + JS, tanpa build step), jadi bisa langsung di-deploy ke **GitHub Pages** tanpa proses build apapun.

## 🚀 Cara Deploy ke GitHub Pages

### 1. Buat repository baru di GitHub
- Buka https://github.com/new
- Beri nama repo, misalnya `calm-quest`
- Set ke **Public** (GitHub Pages gratis butuh repo public, kecuali kamu punya GitHub Pro/Team)
- Klik **Create repository**

### 2. Upload file ini ke repo
Ada dua cara:

**Cara A — lewat browser (paling gampang, tanpa command line):**
1. Di halaman repo yang baru dibuat, klik **"uploading an existing file"**
2. Drag & drop file `index.html` (dan `README.md` ini kalau mau)
3. Klik **Commit changes**

**Cara B — lewat git command line:**
```bash
git init
git add .
git commit -m "Initial commit: Calm Quest"
git branch -M main
git remote add origin https://github.com/USERNAME/calm-quest.git
git push -u origin main
```

### 3. Aktifkan GitHub Pages
1. Di repo, buka tab **Settings**
2. Di sidebar kiri, klik **Pages**
3. Di bagian **Build and deployment** → **Source**, pilih **Deploy from a branch**
4. Pilih branch **main** dan folder **/ (root)**
5. Klik **Save**

### 4. Selesai! 🎉
Tunggu 1–2 menit, lalu situs akan aktif di:
```
https://USERNAME.github.io/calm-quest/
```
(ganti `USERNAME` dengan username GitHub kamu, dan `calm-quest` kalau nama repo-nya beda)

## 📝 Catatan
- Tidak perlu server, database, atau build tool — semua logic ada di `index.html` (vanilla JS).
- Progress permainan **tidak tersimpan** kalau halaman di-refresh (state hanya di memory browser) — ini sesuai desain aslinya untuk dimainkan sekali jalan bersama teman-teman.
- Kalau mau custom domain (misal `calmquest.id`), bisa diatur juga di halaman **Settings → Pages → Custom domain**.

## 🛠️ Update konten
Semua data situasi (pertanyaan, catatan konselor, dll) ada di dalam file `index.html`, di bagian `const SITUATIONS = {...}`. Edit langsung di sana, commit, dan GitHub Pages otomatis re-deploy dalam 1–2 menit.
