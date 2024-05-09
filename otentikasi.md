1. Apa itu otentikasi?
   Otentikasi web adalah proses pemeriksaan identitas pengguna untuk memastikan pengguna tersebut memang yang berhak mengakses situs web atau layanan web tertentu.       Dengan kata lain, ini seperti cara mengenali pengunjung sebelum diizinkan masuk ke suatu tempat.

2. Sebutkan tiga faktor otentikasi yang umum digunakan.
   Password, Biometrik, dan token autentikasi

3. Apa perbedaan antara otentikasi dua faktor dan otentikasi multifaktor?
   Otentikasi dua faktor (2FA)  memerlukan dua langkah verifikasi untuk masuk. Langkah pertama biasanya adalah sesuatu yang diketahui pengguna, seperti PIN atau password. Langkah kedua adalah sesuatu yang dimiliki pengguna, seperti OTP pada ponsel. Sedangkan otentikasi multifaktor (MFA) memerlukan tiga atau lebih langkah verifikasi untuk masuk. Hal ini menjadikn MFA lebih aman.
   
4. Apa itu Single Sign-On (SSO)?
   Single Sign-On (SSO) adalah sistem autentikasi yang memungkinkan pengguna untuk login ke beberapa aplikasi dan situs web  hanya dengan satu set kredensial. Dengan SSO, pengguna cukup login sekali ke dalam sistem SSO, dan kemudian Anda bisa langsung mengakses semua aplikasi lainnya yang terintegrasi dengan SSO tersebut. contohnya adalah webiste portal universitas, Google Workspace, dan Microsoft 365.

5. Mengapa password dianggap sebagai bentuk otentikasi yang lemah?
   Password sering dianggap sebagai bentuk otentikasi paling lemah karena rentan terhadap teknik peretasan seperti bruteforce atau menebak-nebak. Tetapi saya kurang berpendapat demikian, karena kuat dan lemah suatu password kembali kepada pengguna. Beberapa waktu lalu saya melihat riset yang menunjukkan interval waktu yang diperlukan teknik brute force untuk berhasil meretas berbagai kombinasi macam password. Password yang hanya berisi kombinasi huruf membutuhkan waktu lebih sedikit untuk diretas daripada password yang kombinasi antara huruf+angka+simbol.

6. Apa itu otentikasi biometrik dan berikan dua contoh.
   Otentikasi biometrik adalah metode otentikasi yang menggunakan atribut fisik individu untuk memverifikasi identitasnya. Contohnya adalah sidik jari (fingerprint) dan pengenalan wajah (face recognition). Kedua fitur ini biasa ada pada smartphone.

7. Sebutkan satu kelemahan dari otentikasi berbasis biometrik.
   Meskipun canggih, otentikasi biometrik memiliki kelemahan yang cukup menonjol yaitu permasalahan privasi. Pengguna khawatir bahwa data biometrik yang mereka daftarkan ke dalam sebuah gadget dipakai untuk mass surveillance pemerintah.

8. Apa fungsi dari token otentikasi?
   Token otentikasi secara garis besar memiliki fungsi sebagai berikut:

    - Verifikasi Identitas Pengguna: Token otentikasi berfungsi sebagai bukti bahwa pengguna telah berhasil login dan terverifikasi ke dalam suatu sistem.
    - Mencegah Akses Tidak Sah: Kepemilikan token otentikasi menjadi syarat tambahan selain kredensial login (username dan password) untuk mengakses layanan tertentu.

9. Apa itu OTP dan bagaimana cara kerjanya?
   OTP (One-Time-Password) adalah kode keamanan yang dirancang untuk digunakan hanya sekali pada saat login atau melakukan aktivitas tertentu. OTP berfungsi sebagai lapisan keamanan tambahan. Cara kerja dari OTP adalah di bawah ini:
  1 Permintaan Kode: Saat pengguna mencoba login ke akun atau melakukan transaksi yang memerlukan OTP, pengguna akan diminta untuk memasukkan username dan password. Setelah itu, sistem akan mengirimkan kode OTP ke perangkat terdaftar.
  2.Pengiriman Kode: Kode OTP dapat dikirimkan melalui berbagai cara, seperti SMS, Email, Push Notification.
  3. Verifikasi Kode: Setelah menerima kode OTP, pengguna harus memasukkannya ke dalam kolom yang disediakan pada halaman login atau transaksi. Jika kode yang dimasukkan sesuai dengan kode yang dikirimkan sistem, maka pengguna akan diizinkan untuk melanjutkan login atau transaksi.

10. Bagaimana otentikasi dapat diperkuat dalam sistem online?
   - Gunakan password yang kuat dan kombinasi dari huruf, angka dan simbol.
   - Menggunakan 2FA seperti OTP, utnuk mengurangi resiko penyalahgunaan password.

11. Apa itu otorisasi?
    Otorisasi adalah proses dalam keamanan komputer dan informasi yang menentukan hak akses pengguna ke layanan tertentu. Dengan kata lain, otorisasi  menetapkan  apa yang boleh dan tidak boleh dilakukan.

12. Apa perbedaan utama antara otentikasi dan otorisasi?
    Otentikasi berfokus pada memverifikasi identitas pengguna atau program. Otentikasi memastikan apakah pengguna memiliki identittas valid. Sedangkan otorisasi baru berperan setelah proses otentikasi berhasil. Otorisasi menentukan apa yang dapat dilakukan pengguna tersebut berdasarkan identitas dan kredensial mereka.

13. Sebutkan dua metode otorisasi yang sering digunakan dalam sistem komputer.
    RBAC (Role-Based Access Control) dan ABAC (Attribute-Based Access Control)


14. Apa itu Role-based Access Control?
    RBAC adalah metode otorisasi yang menetapkan hak akses berdasarkan peran (role) pengguna dalam sistem. Setiap peran memiliki serangkaian izin yang menentukan apa yang dapat dilakukan pengguna dengan peran tersebut.

15. Apa itu Policy-based Access Control?
    Policy-Based Access Control - PBAC adalah metode otorisasi yang  memungkinkan administrator untuk menentukan hak akses pengguna atau program ke sebuah layanan atau sistem berdasarkan kebijakan yang telah ditetapkan. Kebijakan tersebut dapat berupa identitas user, role user, lokasi user atau kondisi lainnya.

16. Apa keuntungan menggunakan ABAC dibandingkan dengan RBAC?
    ABAC adalah metode otorisasi yang lebih fleksibel. ABAC memungkinkan administrator untuk  menentukan hak akses berdasarkan berbagai atribut, seperti identitas pengguna, peran pengguna, lokasi pengguna, dan lain-lain.

17. Apa itu JSON Web Token (JWT) dan bagaimana hubungannya dengan otorisasi?
    JSON Web Token (JWT) adalah standar untuk mentransmisikan informasi denagn aman. JWT sering digunakan dalam otentikasi dan otorisasi aplikasi web dan mobile.

18. Apa yang dimaksud dengan "least privilege" dalam konteks otorisasi?
    Least privilage dalam konteks otorisasi adalah konsep yang menyatakan bahwa pengguna hanya boleh diberikan akses yang seminimal mungkin yang diperlukan untuk menyelesaikan tugas atau pekerjaan mereka. Contohnya adalah akun guest.

19. Mengapa penting untuk sering memeriksa dan memperbarui kebijakan otorisasi?
    Penting karena ancaman terus-menerus berkembang dalam bentuk malware maupun teknik hacking. Kebijakan otorisasi yang tidak up-to-date mungkin tidak dapat mengimbangi terhadap ancaman-ancaman terbaru itu.

20. Apa itu Access Control List (ACL)?
    ACL adalah mekanisme keamanan yang digunakan untuk mengatur akses ke dalam sistem komputer. ACL berfungsi dengan cara menentukan pengguna mana yang diizinkan atau ditolak untuk mengakses sistem, serta jenis akses seperti apa yang diizinkan.

21. Bagaimana otentikasi dan otorisasi bekerja bersama dalam keamanan sistem informasi?
    Otentikasi memverifikasi identitas pengguna, memastikan mereka valid. Otorisasi menentukan akses yang dimiliki pengguna ke sistem setelah diautentikasi.
Bentuk kerjasama keduanya dapat berbentuk: Memastikan hanya pengguna sah yang mengakses sistem dan membatasi akses ke data dan fungsionalitas berdasarkan peran dan izin pengguna.

22. Sebutkan contoh aplikasi yang menggunakan otentikasi dan otorisasi.
    Contohnya adalah sistem KMS (Knowledge Management System) internal perusahaan dimana setiap karyawan memiliki akun untuk bisa menggunakan webapp tersebut, tetapi tidak semua akun memiliki privilege yang sama. Ada dokumen atau konten yang hanya dapat diakses oleh C-level. Contoh lain adalah situs manajemen perpustakaan. Pengguna perpustakaan dapat mendaftar dan hanya memiliki otorisasi untuk membuat profil, melihat daftar buku dan meminjam sedangkan pengelola perpustakaan memiliki admin akses kepada data pengguna dan buku apa yang mereka pinjam.

23. Apa yang terjadi jika proses otentikasi gagal?
    Pengguna tidak akan diizinkan untuk mengakses website atau aplikasi yang mereka coba akses. Dalam sebuah sistem yang lebih canggih, IP pengguna yang terus-menerus gagal masuk dapat diblokir sementara. Selain itu website/aplikasi dapat menawarkan fitur 'forget password'.

24. Mengapa penting untuk log aktivitas otentikasi dan otorisasi?
    Logging penting dalam investigasi bilamana terdapat suatu insiden, misalnya hacking. Selain itu logging dapat membantu identifikasi aktivitas seperti serangan brute force atau upaya akses tidak sah lainnya.

25. Bagaimana cara sistem menangani perubahan kebijakan otorisasi tanpa mengganggu pengguna?
- Implementasi Bertahap: Lakukan perubahan secara bertahap dan mengkomunikasikannya dengan jelas.
- Pendekatan Just-in-Time : Berikan akses hanya saat dibutuhkan.
- Access Control List (ACL): Perbarui ACL secara dinamis, tentukan aturan akses fleksibel, dan pantau akses.
- Manajemen Akses Berbasis Peran (RBAC): Tetapkan peran dan izin, kelola akses berdasarkan peran, dan perbarui dengan mudah.

26. Apa pengaruh kegagalan sistem otentikasi terhadap proses otorisasi?
    Kegagalan sistem otentikasi dapat mengakibatkan penghentian layanan atau kehilangan akses ke protected resource. Hal ini terutama terjadi jika sistem memutuskan untuk memblokir akses ke semua pengguna sebagai tindakan pencegahan terhadap potensi ancaman keamanan.

27. Bagaimana implementasi kebijakan "zero trust" mempengaruhi otentikasi dan otorisasi?
    Dengan pendekatan "zero trust", asumsi dasar adalah bahwa tidak ada yang bisa dipercaya secara default, termasuk pengguna yang ada di dalam jaringan internal. Hal ini dapat berbentuk penggabungan beberapa metode autentikasi, seperti password, biometrik, dan token kode, untuk meningkatkan keamanan. Selain itu, pemantauan aktivitas pengguna menjadi sangat penting di bawah kebijakan "zero trust" untuk mendeteksi tanda-tanda potensial dari perilaku yang mencurigakan atau akses yang tidak sah.

28. Apa dampak dari serangan keamanan pada sistem otentikasi dan otorisasi?
    Serangan keamanan dapat memmberikan berbagai dampak negatif seperti pencurian identitas user, penanaman backdoor, serta kehilangan data-data penting yang berdampak kepada kerugian finansial.

29. Bagaimana teknologi blockchain dapat mempengaruhi otentikasi dan otorisasi?
    - Sistem otentikasi dan otorisasi berbasis blockchain tidak memiliki otoritas pusat, sehingga lebih tahan terhadap peretasan dan manipulasi data.
    - Data yang disimpan di blockchain bersifat immutable dan dienkripsi, membuatnya sangat sulit untuk dipalsukan.
    - Semua transaksi pada blockchain dicatat dan dapat diakses oleh semua orang, yang meningkatkan transparansi.

30. Apa peran administrator sistem dalam pengelolaan otentikasi dan otorisasi?
    Administrator bertanggung jawab dalam menetapkan kebijakan otentikasi dan otorisasi, mengkonfigurasi dan memelihara sistem, mengelola akun penggunna dan memantau aktivitas mereka untuk mencegah akses tidak sah atau perilaku tidak bertanggungjawab.


