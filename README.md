<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Шрифты -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700;800;900&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(
                135deg,
                #0f0f0f 0%,
                #1a1a1a 25%,
                #c9b37e 50%,
                #f5f5f5 75%,
                #ffffff 100%
            );
            color: #111;
            min-height: 100vh;
        }

        header {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 40px 20px;
            background: rgba(255,255,255,0.75);
            backdrop-filter: blur(20px);
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4.2rem;
            font-weight: 900;
            letter-spacing: 8px;
            margin-top: -50px;
        }

        .line {
            width: 40px;
            height: 2px;
            background: #ffffff;
            margin: 20px 0;
        }

        header p {
            margin-top: 20px;
            max-width: 650px;
            font-size: 1.15rem;
            font-weight: 500;
            color: #444;
        }

        section {
            padding: 110px 10%;
            text-align: center;
        }

        section h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.6rem;
            font-weight: 800;
            margin-bottom: 40px;
        }

        /* ==== PRODUCT ==== */
        .product-card {
            width: 420px;
            margin: 0 auto;
            transition: transform 0.4s ease;
        }

        .product-card img {
            width: 100%;
            border-radius: 20px;
            transition: transform 0.4s ease, opacity 0.4s ease;
        }

        .product-card:hover img {
            transform: scale(1.05);
        }

        footer {
            text-align: center;
            padding: 45px;
            background: rgba(0,0,0,0.9);
            color: #aaa;
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2.9rem;
                letter-spacing: 4px;
                margin-top: -30px;
            }

            .product-card {
                width: 90%;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>DIVEROLLY GANG</h1>
    <div class="line"></div>
    <p>
        Концептуальный бренд одежды, сочетающий уличную культуру,
        минимализм и эстетику люксовой моды.
    </p>
</header>

<section>
    <h2>Коллекция</h2>

    <div class="product-card"
         onmouseenter="startFlip()"
         onmouseleave="stopFlip()">

        <img id="productImage" src="front.png" alt="Diverolly Gang Sweatshirt">
    </div>
</section>

<footer>
    © 2026 DIVEROLLY GANG — Fashion Design Concept
</footer>

<script>
    let flipTimer;

    function startFlip() {
        flipTimer = setTimeout(() => {
            document.getElementById("productImage").src = "back.png";
        }, 3000);
    }

    function stopFlip() {
        clearTimeout(flipTimer);
        document.getElementById("productImage").src = "front.png";
    }
</script>

</body>
</html>
