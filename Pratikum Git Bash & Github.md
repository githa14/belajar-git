# Instalasi Git Bash
1. **Pertama**, kita harus mengunduh aplikasi **Git Bash** dari situs resmi **Git SCM** yaitu https://git-scm.com/ .
	![[foto_github/instal.png]]

2. Ketika sudah membuka situs resmi **Git SCM**, Pilih **Download for Windows untuk menginstal Git Bash pada laptop Windows** begitupun dengan Sistem Operasi lainnya.
	![[foto_github/2.png]]

# Loginkan Github
1.  Pertama, buka situs resmi **GitHub** yaitu https://github.com/.
	![[foto_github/3.png]]

2. Setelah membuka situs resmi **GitHub**, Klik **Sign In** untuk masuk ketika sudah mempunya akun dan **Sign Up** untuk membuat akun baru.
	![[foto_github/4.png]]

3. Inilah Tampilan Halaman ketika **Sign In**, disini kamu hanya akan diminta untuk memasukan **Email** serta **Password** akun yang telah kamu buat sebelumnya.
	![[foto_github/5.png]]

4. Inilah Tampilan Halaman ketika **Sign Up**, disini kamu akan diminta untuk mengisi beberapa pertanyaan untuk mengisi **Profil GitHubmu.**
	![[foto_github/6.png]]

5. Jika tampilannya sudah seperti gambar dibawah, maka proses **Login** telah berhasil kamu lakukan.
	![[foto_github/7.png]]

# Buat Repository
1.  Pertama, buka situs resmi **GitHub** yaitu https://github.com/.
	![[foto_github/8.png]]

2. Lalu Klik **Create New** dan Pilih **New Repository** untuk membuat Repository yang baru
	![[foto_github/99.png]]

3. Lalu kamu akan diminta untuk mengisi pilihan untuk membuat Repository yang baru, kamu dapat mengikuti pilihan yang tertera pada gambar dibawah ini.
	![[foto_github/11.png]]

4. Jika tampilannya sudah seperti gambar dibawah, maka proses **Membuat Repository yang baru** telah berhasil kamu lakukan.
	![[foto_github/13.png]]
# Konfigurasi Awal di Git Bash
1. Pertama, bukalah **Git Bash** dan ketikkan **"git config --list"** 
	![[foto_github/1 _baru.png]]

	Analisa : 
	- `git config --list` : digunakan untuk melihat konfigurasi Git yang saat ini aktif pada sistem .

2. Selanjutnya, aturlah konfigurasi username dan emailmu dengan menggetikkan **"git config --global user.name "username_githubmu"** untuk **username** dan **"git config --global user.email "akun_emailmu@gmail.com"** untuk **email**. 
	Code : 
	```bash
	git config --global user.name "username_githubmu"
	 ```

	```bash
	git config --global user.email "akun_emailmu@gmail.com"
	 ```

	![[foto_github/2_baruu.png]]

	Analisa : 
	- `git config --global user.name "githa14"` : digunakan untuk mengatur nama pengguna Git secara global. Artinya, setiap kali membuat commit pada semua repository Git di laptop ini, nama pengguna yang akan tercantum adalah "githa14".
	- `git config --global user.email "agathagithania@gmail.com"` : digunakan untuk mengatur alamat email Git secara global. Artinya, setiap kali membuat commit pada semua repository Git di laptop ini, alamat email yang akan tercantum adalah "[agathagithania@gmail.com](mailto:agathagithania@gmail.com)".

3. Setelah mengantur konfigurasi username dan emailmu, maka tampilannya akan seperti gambar dibawah ini.
	![[foto_github/3_baru.png]]
# Akses Folder Proyek di Git Bash
1. Pertama, buatlah Folder Baru di dalam Folder Obsidian.
	![[foto_github/9 _baru.png]]

2.  Selanjutnya, buka Git Bash dan ketikkan **"pwd"**
	![[foto_github/4 _baruu.png]]

	Analisa : 
	 - `pwd` : digunakan untuk mengetahui di direktori mana saat ini berada.

3. Lalu, gunakan perintah **"cd" (Change Directory)** dan **"ls"** sampai ke folder proyek/baru yaitu ***belajar-github***
	![[foto_github/11_baru.png]]
	![[foto_github/12_baru.png]]

	Analisa : 
	 - `cd e:` : adalah perintah untuk berpindah ke direktori "e:"
	 - `cd obsidian` : adalah perintah untuk berpindah ke folder bernama **"obsidian"**
	 - `ls` : adalah perintah untuk melihat daftar file dan folder yang ada di dalam direktori saat ini.
	 - `cd belajar-github` : adalah perintah untuk berpindah ke folder bernama **"belajar-github"**
# Hubungkan Folder Proyek Lokal ke Github
1. Pertama, kita dapat melakukan inisialisasi repository Git
	Code : 
	```bash
	git init
	 ```

	![[foto_github/14_baru.png]]

	Analisa : 
	- `git init` : digunakan untuk memulai repositori Git baru di direktori yang ada.

2. Selanjutnya, menambahkan repositori 'git remote" sebagai origin pada repositori lokal Git
	Code : 
	```bash
	git remote add origin "url_repositori"
	 ```

	![[foto_github/15_baru.png]]

	Analisa : 
	- `git remote add origin "url_repositori"` : digunakan untuk menghubungkan repository lokal dengan repository yang ada di server (remote repository).

3. Lalu, membuat commit baru di repositori Git dengan mengetikkan **"git commit -m "nama_commit_baru""**
	Code : 
	```bash
	git commit -m "nama_commit_baru"
	 ```

	![[foto_github/16_baru.png]]

	Analisa : 
	- `git commit -m "nama_commit_baru"` : digunakan untuk menyimpan (commit) perubahan yang telah dibuat pada repository Git lokal.

4. Selanjutnya, tambahkan semua file-file baru atau perubahan ke dalam direktori menggunakan **"git add ."**
	Code : 
	```bash
	git add .
	 ```

	![[foto_github/17_baru.png]]

	Analisa : 
	- `git add .`  : digunakan untuk menambahkan semua file yang telah diubah (modified) ke dalam staging area di Git.

5. Lalu, mengirim (push) perubahan dari Repository Lokal ke Repository Remote
	Code : 
	```bash
	git push origin master
	 ```

	![[foto_github/18_baru.png]]

	Analisa : 
	- `git push origin master`  : digunakan untuk mengunggah (push) perubahan yang telah disimpan (commit) pada repository lokal ke repository remote (server) yang bernama "origin".

6. Setelah melakukan perintah terakhir, maka akan tampil seperti pada gambar dibawah .
	![[foto_github/19_baru.png]]

7. Lalu klik **"Sign in with your browser"** dan masukkan password serta username akun GitHubmu dan Klik **Sign In**.
	![[foto_github/20_baru.png]]

8. Setelah masukkan username dan password, maka akan tampil seperti pada gambar dibawah dan klik **"Authorize git-ecosystem"**.
	![[foto_github/21_baru.png]]

9. Setelah mengklik  **"Authorize git-ecosystem"**, maka akan tampil seperti pada gambar dibawah yang berarti kamu berhasil menghubungkannya.
	![[foto_github/22_baru.png]]

10. Lalu setelah itu, buka https://github.com/ lalu bukalah repository yang telah dibuat tadi maka akan tampil seperti pada gambar yang berarti penyambungan folder proyek lokal ke Github telah berhasil dilakukan.
	![[foto_github/23_baru.png]]