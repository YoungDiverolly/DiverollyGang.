<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Шрифты (жирные веса подключены) -->
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
            padding: 40px 20px; /* меньше воздуха */
            background: rgba(255,255,255,0.75);
            backdrop-filter: blur(20px);
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4.2rem;
            font-weight: 900;      /* жирнее */
            letter-spacing: 8px;
            margin-top: -50px;     /* выше */
        }

        .line {
            width: 40px;           /* короче */
            height: 2px;
            background: #ffffff;   /* белая */
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
        }

        section h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.6rem;
            font-weight: 800;
            margin-bottom: 30px;
        }

        section p {
            max-width: 750px;
            font-size: 1.05rem;
            line-height: 1.8;
            font-weight: 500;
            color: #333;
        }

        .grid {
            margin-top: 60px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 35px;
        }

        .box {
            background: rgba(255,255,255,0.85);
            border-radius: 22px;
            padding: 45px;
            box-shadow: 0 25px 60px rgba(0,0,0,0.12);
            transition: 0.4s ease;
        }

        .box:hover {
            transform: translateY(-12px);
            box-shadow: 0 40px 80px rgba(0,0,0,0.18);
        }

        .box h3 {
            font-family: 'Playfair Display', serif;
            margin-bottom: 15px;
            font-size: 1.4rem;
            font-weight: 700;
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
    <h2>Концепция бренда</h2>
    <p>
        DIVEROLLY GANG — это дизайнерский проект в сфере моды,
        направленный на создание визуальной идентичности,
        передающей уверенность, статус и индивидуальность.
    </p>
</section>

<section>
    <h2>Коллекции</h2>

    <div class="grid">
        <div class="box">
            <h3>Минимализм</h3>
            <p>
                Чистые формы, спокойные оттенки и внимание к деталям.
            </p>
        </div>

        <div class="box">
            <h3>Street Luxury</h3>
            <p>
                Слияние уличной моды и люкса с премиальным ощущением.
            </p>
        </div>

        <div class="box">
            <h3>Лимитированные дропы</h3>
            <p>
                Ограниченные коллекции, подчёркивающие эксклюзивность.
            </p>
        </div>
    </div>
</section>

<section>
    <h2>Уникальность бренда</h2>
    <p>
        Каждая вещь создаётся как кастомный элемент стиля,
        отражающий индивидуальность владельца.
    </p>
</section>

<footer>
    © 2026 DIVEROLLY GANG — Fashion Design Concept
</footer>

</body>
</html>
