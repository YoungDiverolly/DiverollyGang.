<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DIVEROLLY GANG | Official</title>

    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;900&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

    <style>
        /* Обнуляем всё лишнее, чтобы сайт был на весь экран */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html, body {
            width: 100%;
            height: 100%;
            background-color: #000; /* Глубокий черный */
            color: #fff;
            font-family: 'Inter', sans-serif;
            overflow-x: hidden;
        }

        /* Главный экран на всю высоту (Viewport Height) */
        header {
            width: 100%;
            height: 100vh; 
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
            background: radial-gradient(circle at center, #1a1a1a 0%, #000 100%);
            padding: 20px;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2.5rem, 8vw, 6rem); /* Адаптивный размер шрифта */
            font-weight: 900;
            letter-spacing: 0.15em;
            color: #c9b37e;
            text-transform: uppercase;
            margin-bottom: 10px;
            border-bottom: 2px solid #c9b37e;
            padding-bottom: 10px;
        }

        .line-accent {
            width: 80px;
            height: 2px;
            background: #c9b37e;
            margin: 30px 0;
        }

        header p {
            max-width: 800px;
            font-size: clamp(1rem, 2vw, 1.4rem);
            line-height: 1.8;
            font-weight: 300;
            color: #aaa;
            text-transform: uppercase;
            letter-spacing: 4px;
        }

        /* Секция с качеством — теперь она идет следом */
        .features {
            min-height: 50vh;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            align-items: center;
            background: #fff;
            color: #000;
            padding: 80px 10%;
        }

        .feature-box {
            flex: 1;
            min-width: 300px;
            padding: 30px;
            text-align: center;
        }

        .feature-box h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            margin-bottom: 15px;
            text-transform: uppercase;
        }

        /* Кнопка действия */
        .cta-button {
            margin-top: 50px;
            padding: 15px 40px;
            border: 1px solid #c9b37e;
            color: #c9b37e;
            text-decoration: none;
            font-size: 0.9rem;
            letter-spacing: 3px;
            transition: all 0.4s ease;
            text-transform: uppercase;
        }

        .cta-button:hover {
            background: #c9b37e;
            color: #000;
        }

        footer {
            padding: 40px;
            background: #000;
            text-align: center;
            color: #444;
            font-size: 0.7rem;
            letter-spacing: 2px;
        }
    </style>
</head>
<body>

    <header>
        <h1>DIVEROLLY GANG</h1>
        <div class="line-accent"></div>
        <p>НОВАЯ ЭРА УЛИЧНОЙ МОДЫ.<br>БЕСКОМПРОМИССНОЕ КАЧЕСТВО. ЭСТЕТИКА ХАОСА И ПОРЯДКА.</p>
        
        <a href="#collection" class="cta-button">Смотреть дроп</a>
    </header>

    <section class="features">
        <div class="feature-box">
            <h3>QUALITY</h3>
            <p>Премиальный хлопок 480g. Износостойкость, проверенная улицами.</p>
        </div>
        <div class="feature-box">
            <h3>DESIGN</h3>
            <p>Уникальный крой и внимание к каждой детали фурнитуры.</p>
        </div>
        <div class="feature-box">
            <h3>EXCLUSIVE</h3>
            <p>Лимитированные тиражи без повторов. Только для своих.</p>
        </div>
    </section>

    <footer>
        © 2026 DIVEROLLY GANG — ALL RIGHTS RESERVED
    </footer>

</body>
</html>
