1. Perbedaan React Router v5 dan v6?
React Router v5 menggunakan <Switch> sedangkan v6 menggunakan <Routes>, penggunaan <Routes> memudahkan nesting.

2. Apa fungsi <Routes> pada React Router v6?
<Routes> memiliki fungsi diantaranya adalah sebagai "kontainer" dari seluruh <Route>, yang berisi path menuju laman lain pada suatu project React.

3. Bagaimana cara mendefinisikan rute dasar di React Router v6?
Untuk mendefinisikan Route, dapat dilakukan dengan membuat <Routes> yang berfungsi sebagai wrapper dari <Route> yang berisi path, code nya kurang lebih seperti ini:

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" element={<Halaman1 />} />
        <Route path="/about" element={<Halaman2 />} />
        <Route path="/products" element={<Halaman3 />} />
      </Routes>
    </BrowserRouter>
  );
}  

4. Apa itu nested route dan bagaimana cara menerapkannya?
Nested route memungkinkan kita untuk membuat sebuah struktur hierarki dari route-route project React kita. Nested reoute berlaku seperti parent component-child component. Penerapannya seperti code di bawah ini:

import { BrowserRouter, Routes, Route, Outlet } from 'react-router-dom';

function App() {
  return (
    <BrowserRouter>
      <Routes>
        <Route path="/" >
          /* Nested routes */
          <Route path="/products" element={<Products />}>
         		<Route path="/products/:productId" />
          </Route>
        </Route>
      </Routes>
    </BrowserRouter>
  );
}

5. Apa fungsi dari hook useNavigate di React Router?
useNavigate adalah hook yang dapat melakukan navigasi di dalam komponen react. Artinya, kita dapat mengatur perpindahan halaman memakai menggunakan hook ini.

6. Bagaimana cara melakukan redirect di React Ruoter?
Ada dua cara untuk melakukan redirect, pertama adalah: Menggunakan hook 'useNavigate' dan mmebuat komponen '<Redirect>'.

7. Apa kegunaan dari useParams hook?
Hook useParams memungkinan kita membuat parameter dinamis dari URL di dalam komponen React.Hook ini berguna untuk handling Route yang fleksibel.

8. Bagaimana cara mengakses query string?
Query string dapat diakses menggunakan hook 'useLocation' dan mendpatkan query yang dicari dengan memakai search property.

9. Apa itu Outlet dan bagaimana cara penggunaannya?
'<Outlet>' berguna untuk mengelola nested route. '<Outlet>' berperan sebagai placeholder untuk child routes. Contoh penggunaanya seperti di bawah:

import { Routes, Route, Outlet } from 'react-router-dom';

function App() {
  return (
    <Routes>
      <Route path="/" element={<Layout />}>
        <Route path="/products" element={<Products />}>
          <Route path="/products/:productId" element={<ProductDetails />} />
        </Route>
      </Route>
    </Routes>
  );
}

function Layout() {
  return (
    <div>
      <Outlet />
    </div>
  );
}

function Products() {
  return (
    <div>
      <h2>Products</h2>
      <Outlet />
    </div>
  );
}


10. Bagaimana cara melindungi route yang memerlukan autentikasi?
Melindungi rute yang memerlukan autentikasi dalam React Router v6 dapat dilakukan dengan menggunakan komponen '<ProtectedRoute>'. Workflownya adalah 
- Buat component '<ProtectedRoute>' yang membungkus komponen yang ingin dilindungi.
- Periksa status autentikasi pengguna sebelum merender komponen yang dilindungi.
- Jika pengguna tidak atau belum autentikasi, redirect ke halaman lainnya yang public.