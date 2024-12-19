<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NOGA OFFICIAL</title>
    <style>
        /* Mengatur font global */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #9E0E0F, #1D1D1D); /* Latar belakang merah darah dan hitam */
            color: white;
            text-align: center;
            position: relative;
        }

        /* Header */
        header {
            padding: 40px;
            background-color: rgba(0, 0, 0, 0.8);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.8);
            position: relative;
        }

        header h1 {
            font-size: 48px;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 5px;
            margin: 0;
        }

        header h2 {
            font-size: 24px;
            font-weight: 300;
            margin-top: 10px;
        }

        /* Navigasi */
        nav {
            margin-top: 30px;
            background-color: rgba(0, 0, 0, 0.7);
            padding: 15px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.6);
        }

        nav a {
            text-decoration: none;
            color: white;
            margin: 0 20px;
            font-size: 18px;
            font-weight: bold;
            text-transform: uppercase;
        }

        nav a:hover {
            text-decoration: underline;
        }

        /* Konten utama */
        .content {
            margin-top: 60px;
            padding: 40px;
            background: rgba(0, 0, 0, 0.6);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.9);
            margin-left: 10%;
            margin-right: 10%;
            position: relative;
        }

        .section-title {
            font-size: 32px;
            margin-bottom: 20px;
            font-weight: bold;
            letter-spacing: 2px;
        }

        .section-content {
            font-size: 18px;
            line-height: 1.8;
        }

        /* Bayangan gerakan silat */
        .shadow-effect {
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-image: url('https://via.placeholder.com/1200x800'); /* Ganti dengan gambar gerakan silat */
            background-size: cover;
            background-position: center;
            opacity: 0.1;
            pointer-events: none;
            z-index: -1;
            animation: shadowAnimation 15s infinite;
        }

        @keyframes shadowAnimation {
            0% { opacity: 0.1; }
            50% { opacity: 0.3; }
            100% { opacity: 0.1; }
        }

        /* Footer */
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

    <header>
        <h1>NOGA OFFICIAL</h1>
        <h2>“Membangun Karakter melalui Bela Diri Islami”</h2>
    </header>

    <nav>
        <a href="#about">Tentang Kami</a>
        <a href="#history">Sejarah</a>
        <a href="#program">Program</a>
        <a href="#contact">Kontak</a>
    </nav>

    <!-- Elemen bayangan gerakan silat -->
    <div class="shadow-effect"></div>

    <div class="content" id="about">
        <h2 class="section-title">Tentang Kami</h2>
        <p class="section-content">
            NOGA (Nur Raga) adalah perguruan seni bela diri Islami yang berbasis di Desa Anjani, Lombok Timur. Didirikan pada tahun 2000 oleh Syuhada Ahmad, perguruan ini berfokus pada penguatan fisik dan spiritual dengan prinsip-prinsip Islam. Keunikan kami terletak pada perpaduan seni bela diri dengan nilai-nilai luhur Islami.
        </p>
    </div>

    <div class="content" id="history">
        <h2 class="section-title">Sejarah dan Kiprah NOGA</h2>
        <p class="section-content">
            NOGA dimulai pada tahun 2000 sebagai komunitas kecil yang kini telah berkembang menjadi organisasi besar di Lombok Timur, dengan kontribusi dalam bidang sosial, keagamaan, dan pembinaan generasi muda.
        </p>
        <p class="section-content"><strong>Makna Nama “NOGA”:</strong><br>
            • N: Nabi/Para Nabi<br>
            • O: Orang Tua<br>
            • G: Guru-Guru<br>
            • A: Anggota dan Aulia Allah SWT
        </p>
    </div>

    <div class="content" id="program">
        <h2 class="section-title">Program Kami</h2>
        <ul class="section-content">
            <li>Pelatihan Fisik: Seni bela diri tingkat dasar hingga lanjutan.</li>
            <li>Pembinaan Spiritual: Kajian Islam dan pembangunan akhlak.</li>
            <li>Kompetisi: Pertandingan bela diri Islami tahunan.</li>
            <li>Kegiatan Sosial: Bakti sosial untuk masyarakat sekitar.</li>
        </ul>
    </div>

    <div class="content" id="contact">
        <h2 class="section-title">Kontak Kami</h2>
        <p class="section-content">
            Untuk informasi lebih lanjut, Anda dapat menghubungi kami melalui media sosial atau langsung ke lokasi perguruan di Desa Anjani, Lombok Timur:
        </p>
        <p class="section-content">
            <strong>Email:</strong> <a href="mailto:nogaofficial@gmail.com">nogaofficial@gmail.com</a><br>
            <strong>Instagram:</strong> <a href="https://www.instagram.com/nogaofficial" target="_blank">@nogaofficial</a><br>
            <strong>TikTok:</strong> <a href="https://www.tiktok.com/@nogaofficial1" target="_blank">@nogaofficial1</a>
        </p>
    </div>

    <footer>
        <p>Hak Cipta: © 2024 NOGA Official. All rights reserved.</p>
    </footer>

</body>
</html>
