
1. What is Virtual Dom in React?
Virtual DOM adalah Document Object Model yang digunakan pada React. Virtual DOM bisa dibilang seperti representasi dari document object model yang disimpan di memori komputer. 
		
2. What is JSX?
JSX adalah sintaks khusus yang dipakai untuk menulis kode yang mirip HTML tapi sebenarnya adalah JavaScript. JSX membuat kita bisa menulis kode React dengan gaya mirip HTML, tapi dengan kemampuan tambahan dari JavaScript.  Ini membuat kode React lebih mudah dibaca.
		
3. Explain the steps to create a react application and print Hello World.
DEngan mengasumsikan kita sudah menginstal node.js, pada IDE buka terminal dan ketikkan '`npm create vite@latest`'. Setelah itu command line akan meminta kita memasukkan nama project dan memilih framework. Pada tahap ini pilih 'react'. Setelah selesai masuk ke folder project kita dengan '`cd nama-project`', klik enter dan ketikkan '`npm run dev`'. Browser akan terbuka secara otomatis. Buka file src/App.jsx dan ganti isi elemen h1 dengan yang diinginkan.

4. How to Create Event in React?
Event handler adalah fungsi yang dijalankan ketika event tertentu terjadi pada elemen React. Membuat event di React dapat memakai Event Handler. Sebagai contoh, berikut Langkah-langkah Event Handler dengan pada button untuk mengeksekusi log "Halo".
	`<button onClick={eventKlik}>Klik</button>` dimana event onClick akan mengeksekusi function bernama 'eventKlik'. 
	
	`function eventKlik(event) { console.log("Halo"); }` adalah isi function 'eventKlik' yang akan menampilkan log "Halo". Event pada React tidak terbatas hanya pada event klik pada button saja.
	
   
5. Explain Props in React?
Props ( kependekan dari properties) adalah mekanisme penting untuk mengirim data antar komponen React. Komponen React seringkali membutuhkan data untuk menampilkan sesuatu atau menjalankan fungsinya, dan Props lah yang berperan untuk memberikan data tersebut ke komponen. Props juga membuat komponen menjadi reusable.

6. What is higher-order component in React?
Higher-Order Component (HOC) adalah pola di React yang memungkinkan developer untuk membungkus komponen dan menambahkan fungsionalitas baru ke dalamnya tanpa mengubah komponen yang ada. HOC sering digunakan untuk menggunakan kembali logika komponen.

7. Explain the difference between functional and class component?
Functional Component dan Class Component adalah dua cara untuk membuat komponen di React. Functional component lebih ringkas dan sering dipakai dalam pengembangan aplikasi react modern dan dokumentasi React sendiri merekomendasikan memakai functional component. Class component lebih kompleks secara penulisan karena menggunakan konsep class pada Javascript.

8. What are Hooks?
React Hooks adalah fitur baru yang memungkinkan kamu untuk "mengaitkan" state dan fitur React lainnya dari functional components. Hooks membuat functional components lebih powerful dan fleksibel. Beberapa hooks yang penting adalah useState berguna untuk mengelola state di dalam functional components; useEffects untuk menjalankan side effects di functional components; useReducer untuk mengelola state yang lebih kompleks.

9. Explain the useState hook?
useState adalah salah satu React Hook yang paling banyak digunakan.  Hook ini berguna untuk mengelola state di dalam functional components. State adalah data yang tersimpan di dalam komponen dan dapat diubah-ubah.

10. Explain "useEffect"?
useEffect adalah react hook yang memungkinkan developer untuk menjalankan efek samping di dalam functional components, diantaranya adalah rendering dan fetching data.

11. What is prop drilling and its disadvantages?
Prop Drilling adalah teknik untuk mengirim props antar komponen. Kekurangannya adalah prop drilling dapat membuat kode menjadi berantakan dan sulit dibaca ketika aplikasi semakin kompleks. Untuk menghindari prop drilling dapat memakai Redux (library third party) atau React Context (built-in).

12. Explain props and state with differences
Props adalah data yang dikirim dari komponen induk (parent component) ke komponen anak (child component) untuk dirender. Nilai props bersifat read-only yang tidak dapat diubah oleh komponen anak.
State adalah data tersimpan di dalam komponen yang dapat berubah-ubah seiring waktu. State hanya dapat diakses dan diubah oleh tiap komponen yang memilikinya. Sedangkan props adalah data yang dikirim dari komponen induk (parent component) ke komponen anak. Props adalah nilai read-only yang tidak dapat diubah oleh komponen anak.

13. What is the use  of ref in React?
React 'useRef' adalah fitur yang memungkinkan kita mengakses element DOM secara langsung yang dirender oleh komponen. Biasanya, di React kita memanipulasi UI melalui state dan props, namun ref menawarkan cara alternatif untuk itu.

14. What is 'this.setState' function in React?
this.setState adalah sebuah metode yang digunakan untuk memperbarui state di dalam functional component. Ketika nilai dalam objek state berubah, komponen akan melakukan render ulang, yang berarti output akan berubah sesuai dengan nilai baru. Memanggil this.setState akan melakukan re-rendering parent component dan child component. 

15. What are benefit of using react-Redux?
Redux adalah  library third-party yang dapat diandalkan untuk membangun project React yang kompleks dan memiliki state management yang terpusat. Semua state terpusat menjadikan komponen di projec dapat mengakses dan memperbarui state dengan mudah dan menghindari kebingungan akibat state hell. Selain itu, pengelolaan state secara terpusat dengan Redux jadi lebih efisien.