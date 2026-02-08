<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>DIVEROLLY GANG</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Google Font -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;800&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #ffffff, #f2f2f2);
            color: #111;
            min-height: 100vh;
        }

        header {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 40px;
        }

        header h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            letter-spacing: 6px;
            font-weight: 800;
        }

        header p {
            margin-top: 20px;
            max-width: 600px;
            font-size: 1.1rem;
            color: #555;
        }

        .divider {
            width: 80px;
            height: 2px;
            background: #000;
            margin: 30px 0;
        }

        section {
            padding: 100px 10%;
        }

        section h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 30px;
        }

        section p {
            max-width: 700px;
            line-height: 1.7;
            color: #444;
        }

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .card {
            background: rgba(255,255,255,0.7);
            border-radius: 20px;
            padding: 40px;
            backdrop-filter: blur(10px);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        .card h3 {
            margin-bottom: 15px;
            font-family: 'Playfair Display', serif;
        }

        footer {
            text-align: center;
            padding: 40px;
            font-size: 0.9rem;
            color: #777;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2.8rem;
            }
        }
    </style>
</head>
<body>

<header>
    <h1>DIVEROLLY GANG</h1>
    <div class="divider"></div>
    <p>
        A luxury fashion concept inspired by modern street culture, minimalism,
        and high-end design aesthetics.
    </p>
</header>

<section>
    <h2>Brand Concept</h2>
    <p>
        DIVEROLLY GANG is a fashion design project focused on expressing identity,
        confidence, and exclusivity through clean silhouettes and premium style.
        The brand combines street culture with luxury fashion.
    </p>
</section>

<section>
    <h2>Our Collection</h2>

    <div class="cards">
        <div class="card">
            <h3>Minimal Wear</h3>
            <p>
                Clean colors, oversized shapes, and premium materials
                inspired by modern luxury brands.
            </p>
        </div>

        <div class="card">
            <h3>Street Luxury</h3>
            <p>
                Streetwear mixed with high fashion aesthetics,
                designed for confidence and individuality.
            </p>
        </div>

        <div class="card">
            <h3>Limited Pieces</h3>
            <p>
                Exclusive drops that emphasize rarity, uniqueness,
                and artistic expression.
            </p>
        </div>
    </div>
</section>

<section>
    <h2>IB Project Focus</h2>
    <p>
        This website was created as part of an IB design project.
        It demonstrates branding, visual identity, web design,
        and fashion concept development.
    </p>
</section>

<footer>
    © 2026 DIVEROLLY GANG — Fashion Design Concept
</footer>

</body>
</html>
