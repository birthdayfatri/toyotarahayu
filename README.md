<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Profil perusahaan sales marketing mobil yang modern dan sporty.">
    <title>Profil Perusahaan - Dealer Mobil Sport</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            color: #fff;
            line-height: 1.6;
            overflow-x: hidden;
            position: relative;
            background-color: #000;
        }

        /* Global Background */
        .background {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: url('');
            background-size: cover;
            background-position: center;
            z-index: -1;
            opacity: 0.4;
        }

        /* Hero Section */
        .hero {
            position: relative; /* Pastikan elemen ini relative untuk z-index bekerja */
            height: 100vh;
            color: #fff;
            text-align: center;
            overflow: hidden;
        }

        .hero img.background {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1; /* Pastikan gambar background berada di belakang konten */
        }

        .hero-content {
            position: relative;
            z-index: 1; /* Konten berada di atas gambar background */
            max-width: 90%;
            margin: auto;
            padding: 0 20px;
            color: #fff;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 20px;
            font-weight: 800;
            text-transform: uppercase;
            letter-spacing: 2px;
            color: #e50914; /* Accent color */
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 30px;
        }

        .cta {
            background-color: #e50914;
            color: #fff;
            padding: 15px 30px;
            text-decoration: none;
            border-radius: 50px;
            font-size: 1.2rem;
            text-transform: uppercase;
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .cta:hover {
            background-color: #b20710;
            transform: scale(1.05);
        }

        /* About Us */
        .about {
            padding: 80px 20px;
            color: #fff;
            text-align: center;
            position: relative;
            z-index: 1;
            background-color: #222; /* Ganti latar belakang dengan warna solid atau hilangkan jika tidak diperlukan */
        }

        .about h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            font-weight: 800;
            color: #e50914;
        }

        .about p {
            font-size: 1.2rem;
            line-height: 1.8;
            margin: 0 auto;
            max-width: 800px;
        }

        /* Products & Services */
        .products {
            padding: 80px 20px;
            background-color: #1c1c1c;
            text-align: center;
        }

        .products h2 {
            font-size: 2.5rem;
            margin-bottom: 40px;
            color: #e50914;
            font-weight: 800;
        }

        .product-gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: auto;
        }

        .product-item {
            background-color: #333;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            cursor: pointer;
        }

        .product-item img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 15px;
            transition: transform 0.3s ease;
        }

        .product-item h3 {
            margin-top: 15px;
            font-size: 1.6rem;
            color: #e50914;
            font-weight: 600;
        }

        .product-item p {
            font-size: 1.1rem;
            color: #bbb;
        }

        .product-item:hover {
            transform: scale(1.05);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
        }

        .product-item:hover img {
            transform: scale(1.1);
        }

        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1000;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .modal-content {
            background-color: #fff;
            padding: 30px;
            border-radius: 15px;
            max-width: 600px;
            width: 100%;
            text-align: left;
            position: relative;
        }

        .modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            background-color: #e50914;
            color: #fff;
            border: none;
            padding: 10px;
            cursor: pointer;
            border-radius: 50%;
            font-size: 1.5rem;
        }

        .modal h3 {
            margin-bottom: 20px;
            font-size: 1.8rem;
            color: #333;
            font-weight: 800;
        }

        .modal p {
            font-size: 1.1rem;
            color: #555;
        }

        /* Photo Gallery Section */
        .photo-gallery {
            padding: 80px 20px;
            background-color: #222;
            text-align: center;
        }

        .photo-gallery h2 {
            font-size: 2.5rem;
            margin-bottom: 40px;
            color: #e50914;
            font-weight: 800;
        }

        .photo-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            max-width: 1200px;
            margin: auto;
        }

        .photo-grid img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .photo-grid img:hover {
            transform: scale(1.05);
            box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
        }

        /* Contact Us */
        .contact {
            padding: 80px 20px;
            background-color: #1c1c1c;
            text-align: center;
        }

        .contact h2 {
            font-size: 2.5rem;
            margin-bottom: 40px;
            color: #e50914;
            font-weight: 800;
        }

        .contact form {
            max-width: 600px;
            margin: auto;
        }

        .contact label {
            display: block;
            margin-bottom: 10px;
            font-size: 1.1rem;
            color: #fff;
        }

        .contact input, .contact textarea {
            width: 100%;
            padding: 15px;
            margin-bottom: 20px;
            border: none;
            border-radius: 5px;
            background-color: #333;
            color: #fff;
            font-size: 1rem;
        }

        .contact button {
            background-color: #e50914;
            color: #fff;
            padding: 15px 20px;
            border: none;
            border-radius: 5px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .contact button:hover {
            background-color: #b20710;
        }

        .map {
            margin-top: 30px;
        }

        .map iframe {
            border: none;
            width: 100%;
            height: 300px;
            border-radius: 5px;
        }

        /* Footer */
        footer {
            background-color: #111;
            color: #777;
            text-align: center;
            padding: 20px 0;
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media screen and (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.2rem;
            }

            .about h2 {
                font-size: 2rem;
            }

            .about p {
                font-size: 1rem;
            }

            .products h2 {
                font-size: 2rem;
            }

            .product-item h3 {
                font-size: 1.4rem;
            }

            .product-item p {
                font-size: 1rem;
            }

            .photo-gallery h2 {
                font-size: 2rem;
            }

            .contact h2 {
                font-size: 2rem;
            }

            .contact input, .contact textarea {
                font-size: 0.9rem;
            }

            .contact button {
                font-size: 0.9rem;
            }
        }

        @media screen and (max-width: 480px) {
            .hero h1 {
                font-size: 1.8rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .about h2 {
                font-size: 1.8rem;
            }

            .about p {
                font-size: 0.9rem;
            }

            .products h2 {
                font-size: 1.8rem;
            }

            .product-item h3 {
                font-size: 1.2rem;
            }

            .product-item p {
                font-size: 0.9rem;
            }

            .photo-gallery h2 {
                font-size: 1.8rem;
            }

            .contact h2 {
                font-size: 1.8rem;
            }

            .contact input, .contact textarea {
                font-size: 0.8rem;
            }

            .contact button {
                font-size: 0.8rem;
            }
        }
    </style>
</head>
<body>
    <!-- Global Background -->
    <div class="background"></div>

    <!-- Hero Section -->
    <header class="hero">
        <img src="foto4.png" alt="Background Hero" class="background">
        <div class="hero-content">
            <h1>Mengemudi Masa Depan Anda Hari Ini</h1>
            <p>Temukan mobil impian Anda dengan pelayanan terbaik.</p>
            <a href="#products" class="cta">Lihat Koleksi</a>
        </div>
    </header>

    <!-- About Us -->
    <section id="about" class="about">
        <h2>Tentang Kami</h2>
        <p>Kami adalah dealer mobil mewah yang berdedikasi untuk memberikan layanan terbaik dan pilihan kendaraan berkualitas tinggi. Dengan pengalaman bertahun-tahun dalam industri otomotif, kami berkomitmen untuk memenuhi kebutuhan pelanggan kami dengan sempurna.</p>
    </section>

    <!-- Products & Services -->
    <section id="products" class="products">
        <h2>Produk dan Layanan</h2>
        <div class="product-gallery">
            <div class="product-item" onclick="openModal('modal1')">
                <img src="foto1.jpg" alt="Mobil 1">
                <h3>Mobil Model X</h3>
                <p>Spesifikasi singkat mobil.</p>
            </div>
            <div class="product-item" onclick="openModal('modal2')">
                <img src="foto3.jpg" alt="Mobil 2">
                <h3>Mobil Model Y</h3>
                <p>Spesifikasi singkat mobil.</p>
            </div>
        <div class="product-item" onclick="openModal('modal2')">
            <img src="foto3.jpg" alt="Mobil 2">
            <h3>Mobil Model Y</h3>
            <p>Spesifikasi singkat mobil.</p>
        </div>
        <div class="product-gallery">
            <div class="product-item" onclick="openModal('modal1')">
                <img src="foto1.jpg" alt="Mobil 1">
                <h3>Mobil Model X</h3>
                <p>Spesifikasi singkat mobil.</p>
            </div>
            <div class="product-item" onclick="openModal('modal2')">
                <img src="foto3.jpg" alt="Mobil 2">
                <h3>Mobil Model Y</h3>
                <p>Spesifikasi singkat mobil.</p>
            </div>
        <div class="product-item" onclick="openModal('modal2')">
            <img src="foto3.jpg" alt="Mobil 2">
            <h3>Mobil Model Y</h3>
            <p>Spesifikasi singkat mobil.</p>
        </div>
        <div class="product-gallery">
            <div class="product-item" onclick="openModal('modal1')">
                <img src="foto1.jpg" alt="Mobil 1">
                <h3>Mobil Model X</h3>
                <p>Spesifikasi singkat mobil.</p>
            </div>
            <div class="product-item" onclick="openModal('modal2')">
                <img src="foto3.jpg" alt="Mobil 2">
                <h3>Mobil Model Y</h3>
                <p>Spesifikasi singkat mobil.</p>
            </div>
        <div class="product-item" onclick="openModal('modal2')">
            <img src="foto3.jpg" alt="Mobil 2">
            <h3>Mobil Model Y</h3>
            <p>Spesifikasi singkat mobil.</p>
        </div>
            <!-- Tambah produk lainnya -->
        </div>
    </section>

    <!-- Modal 1 -->
    <div id="modal1" class="modal">
        <div class="modal-content">
            <button class="modal-close" onclick="closeModal('modal1')">&times;</button>
            <h3>Mobil Model X</h3>
            <p>Spesifikasi Lengkap Mobil Model X:
                <ul>
                    <li>Mesin: V8 4.0L</li>
                    <li>Tenaga: 500 HP</li>
                    <li>Transmisi: Otomatis 8-percepatan</li>
                    <li>Fitur Keselamatan: ABS, Airbags, Lane Assist</li>
                    <li>Harga: Rp1.500.000.000</li>
                </ul>
            </p>
        </div>
    </div>

    <!-- Modal 2 -->
    <div id="modal2" class="modal">
        <div class="modal-content">
            <button class="modal-close" onclick="closeModal('modal2')">&times;</button>
            <h3>Mobil Model Y</h3>
            <p>Spesifikasi Lengkap Mobil Model Y:
                <ul>
                    <li>Mesin: V6 3.0L</li>
                    <li>Tenaga: 400 HP</li>
                    <li>Transmisi: Manual 6-percepatan</li>
                    <li>Fitur Keselamatan: ABS, Airbags, Traction Control</li>
                    <li>Harga: Rp1.200.000.000</li>
                </ul>
            </p>
        </div>
    </div>

    <!-- Photo Gallery Section -->
    <section id="photo-gallery" class="photo-gallery">
        <h2>Serah Terima Mobil</h2>
        <div class="photo-grid">
            <img src="serah-terima1.jpg" alt="Serah Terima Mobil 1">
            <img src="serah-terima2.jpg" alt="Serah Terima Mobil 2">
            <!-- Tambahkan lebih banyak gambar serah terima -->
        </div>
    </section>

    <!-- Contact Us -->
    <section id="contact" class="contact">
        <h2>Kontak Kami</h2>
        <form>
            <label for="name">Nama:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Pesan:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Kirim Pesan</button>
        </form>
        <div class="map">
            <h3>Lokasi Kami</h3>
            <iframe src="https://www.google.com/maps/embed?pb=..."></iframe>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Dealer Mobil Mewah. All rights reserved.</p>
    </footer>
   <!-- Audio Element -->
   <audio id="carSound" src="suaramobil.mp3" preload="auto"></audio>

   <script>
       // JavaScript untuk memutar efek suara saat halaman dimuat
       window.addEventListener('load', () => {
           const carSound = document.getElementById('carSound');
            const backgroundMusic = document.getElementById('background-music');
           carSound.play();
       });
   </script>
    <script>
        // Function to open modal
        function openModal(modalId) {
            document.getElementById(modalId).style.display = 'flex';
        }

        // Function to close modal
        function closeModal(modalId) {
            document.getElementById(modalId).style.display = 'none';
        }

        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Pesan Anda telah dikirim!');
        });
    </script>
</body>
</html>
