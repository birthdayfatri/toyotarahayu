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
            position: relative;
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
            z-index: -1;
        }

        .hero-content {
            position: relative;
            z-index: 1;
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
            color: #e50914;
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
            background-color: #222;
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
            transition: background-color 0.3s ease, transform 0.3s ease;
        }

        .contact button:hover {
            background-color: #b20710;
            transform: scale(1.05);
        }

        /* Footer */
        .footer {
            padding: 20px;
            background-color: #111;
            text-align: center;
            color: #bbb;
        }

        .footer p {
            margin: 0;
            font-size: 1rem;
        }

        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.2rem;
            }

            .cta {
                font-size: 1rem;
                padding: 10px 20px;
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

            .photo-gallery h2 {
                font-size: 2rem;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 1.8rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .cta {
                font-size: 0.9rem;
                padding: 8px 15px;
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

            .photo-gallery h2 {
                font-size: 1.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="background"></div>
    <header class="hero">
        <img src="path_to_your_hero_image.jpg" alt="Hero Image" class="background">
        <div class="hero-content">
            <h1>Dealer Mobil Sport Terbaik</h1>
            <p>Kami menyediakan mobil-mobil sport terbaru dengan kualitas terbaik.</p>
            <a href="#contact" class="cta">Hubungi Kami</a>
        </div>
    </header>

    <section class="about">
        <h2>Tentang Kami</h2>
        <p>Kami adalah dealer mobil sport terkemuka dengan berbagai pilihan mobil sport premium. Dengan pengalaman bertahun-tahun, kami berkomitmen untuk memberikan layanan terbaik kepada pelanggan kami.</p>
    </section>

    <section class="products">
        <h2>Produk Kami</h2>
        <div class="product-gallery">
            <div class="product-item">
                <img src="path_to_your_product_image_1.jpg" alt="Produk 1">
                <h3>Mobil Sport 1</h3>
                <p>Deskripsi singkat tentang mobil sport 1.</p>
            </div>
            <div class="product-item">
                <img src="path_to_your_product_image_2.jpg" alt="Produk 2">
                <h3>Mobil Sport 2</h3>
                <p>Deskripsi singkat tentang mobil sport 2.</p>
            </div>
            <!-- Tambahkan lebih banyak produk sesuai kebutuhan -->
        </div>
    </section>

    <section class="photo-gallery">
        <h2>Galeri Foto</h2>
        <div class="photo-grid">
            <img src="path_to_your_photo_1.jpg" alt="Foto 1">
            <img src="path_to_your_photo_2.jpg" alt="Foto 2">
            <!-- Tambahkan lebih banyak foto sesuai kebutuhan -->
        </div>
    </section>

    <section class="contact" id="contact">
        <h2>Kontak Kami</h2>
        <form action="submit_form.php" method="post">
            <label for="name">Nama:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Pesan:</label>
            <textarea id="message" name="message" rows="5" required></textarea>
            <button type="submit">Kirim Pesan</button>
        </form>
    </section>

    <footer class="footer">
        <p>&copy; 2024 Dealer Mobil Sport. Semua hak dilindungi.</p>
    </footer>

    <!-- Modal -->
    <div id="modal" class="modal">
        <div class="modal-content">
            <button class="modal-close" onclick="closeModal()">×</button>
            <h3>Detail Produk</h3>
            <p>Informasi lebih lanjut tentang produk.</p>
        </div>
    </div>

    <script>
        function closeModal() {
            document.getElementById('modal').style.display = 'none';
        }
    </script>
</body>
</html>
