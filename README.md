<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Login Page</title>
    <style>
        * {
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
        }

        .login-container {
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            width: 100%;
            max-width: 350px;
            text-align: left;
        }

        label {
            display: block;
            font-weight: bold;
            margin-top: 10px;
        }

        input {
            width: 100%;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 16px;
        }

        .btn-sign-up, .btn-logout {
            width: 100%;
            padding: 10px;
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
            margin-top: 15px;
        }

        .btn-sign-up:hover,
        .btn-logout:hover {
            background-color: #218838;
        }

        .error-message {
            color: red;
            font-size: 14px;
            height: 20px;
            margin-top: 5px;
        }

        .hidden {
            display: none;
        }

        img {
            max-width: 100%;
            height: auto;
        }

        @media (max-width: 480px) {
            h1 {
                font-size: 1.5em;
            }
            .login-container {
                padding: 15px;
            }
        table {
                border-collapse: collapse;
                width: 100%;
            }

        th, td {
                border: 1px solid black;
                padding: 8px;
                text-align: center;
            }

        th {
                background-color: #f2f2f2;
            }
        }
    </style>
</head>
<body>
    <div id="login-page">
        <h1>Selamat Datang</h1>
        <p>Silakan masukkan username dan password yang sudah diberikan.</p>
        <div class="login-container">
            <label for="username">Username</label>
            <input type="text" id="username" placeholder="Masukkan username">
            <p id="error-username" class="error-message"></p>

            <label for="password">Password</label>
            <input type="password" id="password" placeholder="Masukkan password">
            <p id="error-password" class="error-message"></p>

            <button type="button" class="btn-sign-up">MASUK</button>
        </div>
    </div>

    <div id="content-page" class="hidden">
        <h1>HTML</h1>
        <h3>apa sih html itu?</h3>
        <p>HTML atau <strong>HyperText Markup Language</strong> adalah bahasa markah standar untuk dokumen yang ditampilkan di browser. Bisa dikombinasikan dengan CSS dan JavaScript.</p>

        <h4>Terus HTML itu buat apa?</h4>
        <p>HTML menggunakan tag untuk memberikan instruksi pada browser. Misalnya membuat teks tebal seperti ini: <b>TAMPIL TEBAL</b>. Cara menulisnya adalah:
        <code>&lt;b&gt;TAMPIL TEBAL&lt;/b&gt;</code></p>

        <p>Fungsi lainnya:</p>
        <ol>
            <li>Mengintegrasikan gambar dengan tulisan.</li>
            <li>Membuat pranala (link).</li>
            <li>Memutar suara atau video.</li>
            <li>Membuat form interaktif.</li>
        </ol>

        <h5>Contoh dokumen HTML</h5>
        <img src="https://i.postimg.cc/fy4XnVJh/Screenshot-2025-04-04-20-38-15-73.jpg" alt="contoh dokumen html">

        <p>
            <code>&lt;!DOCTYPE html&gt;</code> menyatakan tipe dokumen HTML (HTML5).<br>
            <code>&lt;html lang="en"&gt;</code> menandai awal dokumen dan menyatakan bahasa isi halaman.<br>
            <code>&lt;head&gt;</code> berisi informasi meta tentang dokumen (tidak terlihat langsung di halaman web), biasanya berisi:
        </p>
        <ol>
            <li>Judul halaman <code>&lt;title&gt;</code></li>
            <li>Pengaturan karakter <code>&lt;meta charset="UTF-8"&gt;</code></li>
            <li>Link ke CSS</li>
            <li>Script (JavaScript)</li>
            <li>Deskripsi SEO</li>
        </ol>
        <p><code>&lt;title&gt;</code> berfungsi menentukan judul halaman yang muncul di tab browser.<br>
        <code>&lt;body&gt;</code>bagian utama yang berisi semua konten yang ditampilkan ke pengguna di browser.<br>
        </p>
        <h3>bagaimana HTML di gunakan dalam pembuatan website?</h3>
        <p>bayangin kamu lagi bikin rumah.</p>
        
        <p>dan HTML itu seperti rangka rumah. Dia yang bikin bentuk dasarnya: ada pintu, jendela, tembok, atap. Tapi ya... kalau cuma HTML doang, tampilannya kayak rumah tanpa cat. Polos. Kaku. Kurang vibes-nya.</p> 
        <p>contoh:<br>
        <code>&lt;p&gt;ini paragraf&lt;p&gt;</code><br>
         >“HTML itu polos, kayak chat pacarlu yang cuma<br> ‘ok’.”
        </p>
        <h3>lalu css itu apa?</h3>
        <p>Nah, CSS (Cascading Style Sheets) itu kayak interior design-nya rumah.<br>
        •Dia yang ngatur warna, font, ukuran, posisi, dan vibes halaman kamu.<br>
        •Kalau HTML bilang "ini paragraf", CSS bilang: "Oke, kita kasih warna pink, font aesthetic, dan letaknya tengah biar kayak story Instagram." contoh:<br>
        <code>&lt;p style="color:hotpink; text-align:center;"&gt;Ini paragraf kece.&lt;/p&gt;</code><br>
        >CSS bikin HTML dari ‘biasa aja’ jadi ‘cakep maksimal’, kayak glow-up setelah libur semester.”
        </p>
        <h3>Terus JavaScript Apa?</h3>
        <p>Nah ini... JavaScript itu otaknya. Dia yang bikin web kamu bisa gerak, bisa klik, bisa interaktif.</p>
        <p>•Mau tombol yang bisa diklik?<br>

           •Mau slideshow otomatis?<br>

           •Mau muncul popup yang bilang “Hai manis, semangat ngodingnya.!”<br>


           Itu kerjaannya JavaScript.<br></p>
           <p>contoh:
           alert("Hai, selamat datang di web kami!");<br>
           >“JavaScript itu kayak barista di kafe: bikin semuanya ngga cuma enak dilihat, tapi juga bisa berinteraksi. Klik dikit, langsung respon.”
           </p>
           <p>Web itu gabungan 3 serangkai kayak trio K-Pop:</p>
           <table>
               <tr>
                   <th>elemen</th>
                   <th>peran</th>
                   <th>analoginya</th>
               </tr>
               <tr>
                   <td>HTML</td>
                   <td>struktur</td>
                   <td>Tulang(biar berdiri walau masi kaku)</td>
               </tr>
               <tr>
               <td>CSS</td>
               <td>gaya & tampilan</td>
               <td>outfit & filter ig</td>
             </tr>
             <tr>
                 <td>java script</td>
                 <td>interaksi & diamika</td>
                 <td>otak + mood booster</td>
             </tr>
           </table>
           <p>“HTML, CSS, dan JavaScript tuh kayak kombinasi nasi, ayam geprek, dan sambel. Gak lengkap kalau satu doang!”</p>
           
           <p>Sekarang kalian sudah kenalan sama HTML? Keren! Tapi tunggu dulu, petualangan ngoding belum selesai—ada CSS buat ngasih style biar web kamu nggak kayak tugas Excel, dan JavaScript buat bikin web-nya hidup, interaktif, dan gak boring kayak chat mantan.</p>

            <p>Kalau kamu mau lanjut belajar, coba cek <a href="https://www.w3schools.com/">W3Schools</a> atau <a href="https://developer.mozilla.org/en-US/">MDN Web Docs</a>— itu tempat belajar paling ramah dan gratis, cocok buat yang pengen jadi web developer tanpa pusing.</p>

            <p>Sekarang, gak ada alasan buat nunda—ayo mulai bangun web pertamamu! Siapa tahu, project kecil hari ini jadi startup miliaran besok. Ya minimal, bisa pamerin ke temen, “Nih, web bikinan gue.”</p>

        <button class="btn-logout" onclick="logout()">LOGOUT</button>
    </div>

    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const usernameInput = document.getElementById("username");
            const passwordInput = document.getElementById("password");
            const errorUsername = document.getElementById("error-username");
            const errorPassword = document.getElementById("error-password");
            const loginButton = document.querySelector(".btn-sign-up");
            const loginPage = document.getElementById("login-page");
            const contentPage = document.getElementById("content-page");

            const correctUsername = "Saya tidak tahu";
            const correctPassword = "bodo amat";

            // Cek status login dari localStorage
            if (localStorage.getItem("isLoggedIn") === "true") {
                loginPage.classList.add("hidden");
                contentPage.classList.remove("hidden");
            }

            loginButton.addEventListener("click", function () {
                let isValid = true;

                if (usernameInput.value !== correctUsername) {
                    errorUsername.textContent = "Username salah.";
                    isValid = false;
                } else {
                    errorUsername.textContent = "";
                }

                if (passwordInput.value !== correctPassword) {
                    errorPassword.textContent = "Password salah.";
                    isValid = false;
                } else {
                    errorPassword.textContent = "";
                }

                if (isValid) {
                    localStorage.setItem("isLoggedIn", "true");
                    loginPage.classList.add("hidden");
                    contentPage.classList.remove("hidden");
                }
            });
        });

        function logout() {
            localStorage.removeItem("isLoggedIn");
            location.reload();
        }
    </script>
</body>
</html>
