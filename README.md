<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NOGA OFFICIAL</title>
    <style>
        /* Global Styles */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #9E0E0F, #1D1D1D); /* Latar belakang merah darah dan hitam */
            color: white;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        /* Container untuk judul utama */
        .main-header {
            padding: 40px;
            background-color: rgba(0, 0, 0, 0.8);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.8);
            position: relative;
        }

        .main-header h1 {
            font-size: 48px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 5px;
            margin: 0;
        }

        .main-header h2 {
            font-size: 24px;
            font-weight: 300;
            margin-top: 10px;
        }

        /* Transisi slide */
        .slide-container {
            display: flex;
            transition: transform 1s ease-in-out;
            overflow: hidden;
        }

        .slide {
            min-width: 100%;
            padding: 40px;
            background: rgba(0, 0, 0, 0.6);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.9);
            text-align: center;
            position: relative;
        }

        /* Subjudul untuk tiap slide */
        .slide h3 {
            font-size: 32px;
            font-weight: bold;
            margin-bottom: 20px;
            letter-spacing: 2px;
        }

        .slide p {
            font-size: 18px;
            line-height: 1.8;
            margin-bottom: 20px;
        }

        .nav-buttons {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }

        .nav-buttons button {
            background-color: rgba(0, 0, 0, 0.7);
            border: none;
            padding: 10px;
            color: white;
            font-size: 24px;
            cursor: pointer;
            border-radius: 50%;
        }

        .nav-buttons button:hover {
            background-color: rgba(0, 0, 0, 0.9);
        }

        /* Konten footer */
        footer {
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.8);
            font-size: 16px;
            text-align: center;
            margin-top: 40px;
        }

        footer a {
            text-decoration: none;
            color: white;
            font-weight: bold;
        }

    </style>
</head>
<body>

    <!-- Judul utama -->
    <header class="main-header">
        <h1>WELCOME to PERGURUAN SENI BELA DIRI “NOGA”</h1>
        <h2>“Membangun Karakter melalui Bela Diri Islami”</h2>
    </header>

    <!-- Slide Container -->
    <div class="slide-container" id="slides">
        <!-- Slide 1: Tentang Kami -->
        <div class="slide">
            <h3>Tentang Kami</h3>
            <p>
                NOGA (Nur Raga) adalah perguruan seni bela diri Islami yang berbasis di Desa Anjani, Lombok Timur. Didirikan pada tahun 2000 oleh Syuhada Ahmad, perguruan ini berfokus pada penguatan fisik dan spiritual dengan prinsip-prinsip Islam. Keunikan kami terletak pada perpaduan seni bela diri dengan nilai-nilai luhur Islami.
            </p>
        </div>

        <!-- Slide 2: Sejarah -->
        <div class="slide">
            <h3>Sejarah dan Kiprah NOGA</h3>
            <p>
                NOGA dimulai pada tahun 2000 sebagai komunitas kecil yang kini telah berkembang menjadi organisasi besar di Lombok Timur, dengan kontribusi dalam bidang sosial, keagamaan, dan pembinaan generasi muda.
            </p>
            <p><strong>Makna Nama “NOGA”:</strong><br>
                • N: Nabi/Para Nabi<br>
                • O: Orang Tua<br>
                • G: Guru-Guru<br>
                • A: Anggota dan Aulia Allah SWT
            </p>
        </div>

        <!-- Slide 3: Program -->
        <div class="slide">
            <h3>Program Kami</h3>
            <ul>
                <li>Pelatihan Fisik: Seni bela diri tingkat dasar hingga lanjutan.</li>
                <li>Pembinaan Spiritual: Kajian Islam dan pembangunan akhlak.</li>
                <li>Kompetisi: Pertandingan bela diri Islami tahunan.</li>
                <li>Kegiatan Sosial: Bakti sosial untuk masyarakat sekitar.</li>
            </ul>
        </div>

        <!-- Slide 4: Kontak -->
        <div class="slide">
            <h3>Kontak Kami</h3>
            <p>
                Untuk informasi lebih lanjut, Anda dapat menghubungi kami melalui media sosial atau langsung ke lokasi perguruan di Desa Anjani, Lombok Timur:
            </p>
            <p>
                <strong>Email:</strong> <a href="mailto:nogaofficial@gmail.com">nogaofficial@gmail.com</a><br>
                <strong>Instagram:</strong> <a href="https://www.instagram.com/nogaofficial" target="_blank">@nogaofficial</a><br>
                <strong>TikTok:</strong> <a href="https://www.tiktok.com/@nogaofficial1" target="_blank">@nogaofficial1</a>
            </p>
        </div>
    </div>

    <!-- Navigation Buttons -->
    <div class="nav-buttons">
        <button onclick="prevSlide()">❮</button>
        <button onclick="nextSlide()">❯</button>
    </div>

    <!-- Footer -->
    <footer>
        <p>Hak Cipta: © 2024 NOGA Official. All rights reserved.</p>
    </footer>

    <!-- JavaScript untuk navigasi slide -->
    <script>
        let currentSlide = 0;
        const slides = document.getElementById('slides');
        const totalSlides = document.querySelectorAll('.slide').length;

        function showSlide(index) {
            if (index >= totalSlides) {
                currentSlide = 0;
            } else if (index < 0) {
                currentSlide = totalSlides - 1;
            } else {
                currentSlide = index;
            }
            slides.style.transform = 'translateX(' + (-100 * currentSlide) + '%)';
        }

        function nextSlide() {
            showSlide(currentSlide + 1);
        }

        function prevSlide() {
            showSlide(currentSlide - 1);
        }
    </script>

</body>
</html>
