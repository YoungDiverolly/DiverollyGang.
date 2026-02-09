<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DIVEROLLY GANG | Official</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Общие настройки — ТОТАЛЬНЫЙ ЧЕРНЫЙ */
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

        /* Манифест — ТЕПЕРЬ ТОЖЕ ЧЕРНЫЙ */
        .manifesto {
            padding: 100px 10%;
            text-align: center;
            background: #000; /* Убрал серый оттенок */
            border-top: 1px solid #1a1a1a;
            border-bottom: 1px solid #1a1a1a;
        }

        .manifesto h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            color: #c9b37e;
            margin-bottom: 30px;
            letter-spacing: 2px;
        }

        .manifesto p {
            max-width: 800px;
            margin: 0 auto 20px;
            line-height: 1.8;
            color: #ccc;
            font-size: 1.1rem;
            font-weight: 300;
        }

        .highlight {
            color: #fff;
            font-weight: 600;
            border-bottom: 1px solid #c9b37e;
        }

        /* Секция товара */
        .product-section {
            padding: 100px 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
            background: #000;
        }

        /* Переключатель вкладок */
        .tab-container {
            display: flex;
            gap: 20px;
            margin-bottom: 30px;
        }

        .tab-btn {
            background: none;
            border: 1px solid #333;
            color: #555;
            padding: 10px 25px;
            cursor: pointer;
            font-size: 0.8rem;
            letter-spacing: 2px;
            text-transform: uppercase;
            transition: 0.3s;
        }

        .tab-btn.active {
            border-color: #c9b37e;
            color: #c9b37e;
        }

        /* Контейнер картинки */
        .image-container {
            width: 100%;
            max-width: 500px;
            position: relative;
            overflow: hidden;
            border: 1px solid #1a1a1a;
            background: #000;
            box-shadow: 0 0 50px rgba(0,0,0,1);
        }

        .image-container img {
            width: 100%;
            display: block;
            transition: opacity 0.4s ease, transform 1s ease;
        }

        .image-container:hover img {
            transform: scale(1.03);
        }

        .product-info {
            text-align: center;
            margin-top: 40px;
        }

        .product-title {
            font-family: 'Playfair Display', serif;
            font-size: 2.3rem;
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
            display: inline-block;
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

    <section class="manifesto">
        <h2>ФИЛОСОФИЯ БРЕНДА</h2>
        <p>
            <span class="highlight">DIVEROLLY GANG</span> — это манифест тех, кто выбирает смыслы вместо массовости. 
            Мы известны своим фанатичным подходом к деталям и <span class="highlight">эксклюзивным кроем</span>.
        </p>
        <p>
            Каждая вещь — это <span class="highlight">Limited Edition</span>. Мы используем только тяжелый хлопок 480g, 
            создавая вещи, которые остаются в истории.
        </p>
    </section>

    <section class="product-section">
        <div class="tab-container">
            <button class="tab-btn active" onclick="changeImage('front', this)">Front</button>
            <button class="tab-btn" onclick="changeImage('back', this)">Back</button>
        </div>

        <div class="image-container">
            <img id="main-product-img" src="https://i.pinimg.com/736x/3d/59/94/3d5994ebe91a11cff3b1aacf40c7d3e6.jpg" alt="Diverolly Gang Front">
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

    <script>
        function changeImage(side, btn) {
            const img = document.getElementById('main-product-img');
            const buttons = document.querySelectorAll('.tab-btn');
            
            buttons.forEach(b => b.classList.remove('active'));
            btn.classList.add('active');

            img.style.opacity = 0;
            
            setTimeout(() => {
                if (side === 'front') {
                    // FRONT
                    img.src = "https://i.pinimg.com/736x/3d/59/94/3d5994ebe91a11cff3b1aacf40c7d3e6.jpg";
                } else {
                    // BACK
                    img.src = "https://i.pinimg.com/736x/fb/cb/da/fbcbda7a12925f55ffe19b5d35ea323d.jpg";
                }
                img.style.opacity = 1;
            }, 300);
        }
    </script>

</body>
</html>
