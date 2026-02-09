<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DIVEROLLY GANG | Official Concept</title>

    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700;800;900&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            /* Градиент стал более мягким и премиальным */
            background: linear-gradient(135deg, #0f0f0f 0%, #1a1a1a 100%);
            color: #ffffff;
            min-height: 100vh;
            overflow-x: hidden;
        }

        header {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 40px 20px;
            background: rgba(0, 0, 0, 0.6);
            backdrop-filter: blur(15px);
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 5rem;
            font-weight: 900;
            letter-spacing: 12px;
            color: #c9b37e; /* Золотистый акцент */
            margin-bottom: 20px;
        }

        .line {
            width: 60px;
            height: 2px;
            background: #c9b37e;
            margin: 20px 0;
        }

        header p {
            max-width: 700px;
            font-size: 1.2rem;
            line-height: 1.6;
            font-weight: 300;
            color: #ddd;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* ==== NEW: QUALITY SECTION ==== */
        .quality-section {
            padding: 100px 10%;
            background: #ffffff;
            color: #111;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            text-align: center;
        }

        .quality-item h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            margin-bottom: 15px;
        }

        .quality-item p {
            font-size: 0.95rem;
            color: #555;
            line-height: 1.5;
        }

        /* ==== PRODUCT ==== */
        section.collection {
            padding: 120px 10%;
            text-align: center;
        }

        section h2 {
            font-family: 'Playfair Display', serif;
            font-size: 3rem;
            font-weight: 800;
            margin-bottom: 60px;
            color: #fff;
        }

        .product-card {
            width: 450px;
            margin: 0 auto;
            position: relative;
            cursor: crosshair;
        }

        .product-card img {
            width: 100%;
            border-radius: 5px; /* Более строгие углы для люкса */
            transition: all 0.6s cubic-bezier(0.23, 1, 0.32, 1);
            filter: grayscale(20%);
        }

        .product-card:hover img {
            transform: scale(1.02);
            filter: grayscale(0%);
        }

        .price-tag {
            margin-top: 25px;
            font-size: 1.5rem;
            font-weight: 600;
            color: #c9b37e;
        }

        footer {
            text-align: center;
            padding: 60px;
            background: #000;
            color: #555;
            font-size: 0.8rem;
            letter-spacing: 3px;
            text-transform: uppercase;
        }

        @media (max-width: 768px) {
            header h1 { font-size: 2.5rem; letter-spacing: 5px; }
            .product-card { width: 100%; }
            .quality-section { padding: 60px 5%; }
        }
    </style>
</head>
<body>

<header>
    <h1>DIVEROLLY GANG</h1>
    <div class="line"></div>
    <p>
        Новая эра уличной моды. <br>
        Бескомпромиссное качество. Эстетика хаоса и порядка.
    </p>
</header>

<section class="quality-section">
    <div class="quality-item">
        <h3>PREMIUM TEXTILE</h3>
        <p>Используем только плотный хлопок высшего сорта (450g+). Ткань, которая держит форму и приятна к телу годами.</p>
    </div>
    <div class="quality-item">
        <h3>HANDMADE DETAILS</h3>
        <p>Каждый принт и шов проходят ручной контроль. Мы не делаем масс-маркет — мы создаем артефакты.</p>
    </div>
    <div class="quality-item">
        <h3>NEW GEN CULTURE</h3>
        <p>DIVEROLLY GANG — это не просто одежда. Это манифест свободы, объединяющий тех, кто диктует свои правила.</p>
    </div>
</section>

<section class="collection">
    <h2>DROP #01</h2>

    <div class="product-card" 
         onmouseenter="startFlip()" 
         onmouseleave="stopFlip()">
        
        <img id="productImage" src="front.png" alt="Diverolly Gang Limited Edition">
        <div class="price-tag">LIMITED DROP</div>
    </div>
</section>

<footer>
    © 2026 DIVEROLLY GANG — DEFINING THE NEW STANDARD
</footer>

<script>
    let flipTimer;

    function startFlip() {
        // Уменьшил задержку до 1 секунды, чтобы юзер сразу видел эффект
        flipTimer = setTimeout(() => {
            const img = document.getElementById("productImage");
            img.style.opacity = "0.7";
            setTimeout(() => {
                img.src = "back.png";
                img.style.opacity = "1";
            }, 200);
        }, 800);
    }

    function stopFlip() {
        clearTimeout(flipTimer);
        const img = document.getElementById("productImage");
        img.src = "front.png";
    }
</script>

</body>
</html>
