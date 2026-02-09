<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DIVEROLLY GANG | Official</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body {
            background-color: #000;
            color: #fff;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }

        /* Главный экран */
        header {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #111 0%, #000 100%);
            padding: 20px;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2rem, 10vw, 5rem);
            letter-spacing: 12px;
            color: #c9b37e;
            text-transform: uppercase;
            margin-bottom: 20px;
        }

        .desc {
            font-weight: 300;
            letter-spacing: 4px;
            color: #888;
            max-width: 700px;
            font-size: 0.9rem;
            text-transform: uppercase;
        }

        /* Секция с товаром */
        .product-section {
            padding: 100px 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            background: #000;
        }

        .image-container {
            width: 100%;
            max-width: 500px;
            position: relative;
            overflow: hidden;
            border: 1px solid #222; /* Тонкая рамка, чтобы серый фон фото плавно отделялся */
            box-shadow: 0 0 30px rgba(201, 179, 126, 0.05);
        }

        .image-container img {
            width: 100%;
            display: block;
            transition: transform 1s ease;
        }

        .image-container:hover img {
            transform: scale(1.05);
        }

        .product-info {
            text-align: center;
            margin-top: 40px;
        }

        .product-title {
            font-family: 'Playfair Display', serif;
            font-size: 2rem;
            margin-bottom: 10px;
        }

        .quality-tags {
            margin: 20px 0;
            color: #c9b37e;
            font-size: 0.8rem;
            letter-spacing: 2px;
            text-transform: uppercase;
        }

        .price {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 30px;
        }

        /* Кнопки */
        .btn {
            padding: 15px 60px;
            border: 1px solid #c9b37e;
            background: none;
            color: #c9b37e;
            text-transform: uppercase;
            letter-spacing: 3px;
            cursor: pointer;
            transition: 0.4s;
            text-decoration: none;
        }

        .btn:hover {
            background: #c9b37e;
            color: #000;
        }

        footer {
            padding: 60px;
            text-align: center;
            color: #333;
            font-size: 0.7rem;
            letter-spacing: 2px;
        }
    </style>
</head>
<body>

    <header>
        <h1>DIVEROLLY GANG</h1>
        <p class="desc">Quality over Quantity. Новый стандарт уличной эстетики.</p>
    </header>

    <section class="product-section">
        <div class="image-container">
            <img src="https://i.pinimg.com/736x/03/1b/8b/031b8b41efa5189f76b3d1bf28734906.jpg" alt="Diverolly Gang Custom Sweatshirt">
        </div>

        <div class="product-info">
            <h2 class="product-title">HANDS DROP #01</h2>
            <div class="quality-tags">Premium Cotton | 480g | Oversize Fit</div>
            <div class="price">5.500₽</div>
            <a href="#" class="btn">Заказать в Telegram</a>
        </div>
    </section>

    <footer>
        © 2026 DIVEROLLY GANG — DEFINING THE NEW STANDARD
    </footer>

</body>
</html>
