# Dasar Git dan GitHub

## 1. Install Tools
Sebelum mulai, pastikan sudah meng-install:
- [Visual Studio Code](https://code.visualstudio.com/download)
- [Git](https://git-scm.com/downloads)
- [GitHub](https://github.com) → buat akun terlebih dahulu

Cek instalasi Git:
```bash
git --version
```

## 2. Konfigurasi Git
Atur nama dan email (harus sama dengan email GitHub):
```bash
git config --global user.name "yourname"
git config --global user.email "youremail@mail.com"
```

## 3. Hubungkan Git dengan GitHub (SSH)
Langkah-langkah membuat SSH key:
```bash
ssh-keygen -t ed25519 -C "youremail@mail.com"
```

Salin isi file id_ed25519.pub, lalu tambahkan ke GitHub:
GitHub → Settings → SSH and GPG keys
Klik New SSH key → paste isi key → Add SSH key

Cek koneksi:
```bash
ssh -T git@github.com
```

## 4. Workflow Dasar Git
1. Buat repository di GitHub.
2. Clone repository:
   ```bash
   git clone git@github.com:username/reponame.git
   ```
3. Pull:
   ```bash
   git pull origin main
   ```
4. Buka folder repository di Visual Studio Code dan buat file baru.
5. Tambahkan file ke staging area:
   ```bash
   git add filename
   ```
   atau
   ```bash
   git add
   ```.
6. Commit perubahan:
   ```bash
   git commit -m "pesan commit"
   ```
7. Push:
   ```bash
   git push origin main
   ```
## 5. Alternatif Menggunakan GitHub Desktop
Jika ingin lebih mudah tanpa terminal, bisa pakai GitHub Desktop.
