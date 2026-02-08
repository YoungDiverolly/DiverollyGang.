<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<title>IB PROJECT</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;600;900&display=swap" rel="stylesheet">

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Inter', sans-serif;
}

body {
    background: radial-gradient(circle at top, #12002e, #050008);
    color: white;
    overflow-x: hidden;
}

/* HEADER */
header {
    position: fixed;
    width: 100%;
    padding: 28px 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 10;
    background: linear-gradient(to bottom, rgba(5,0,8,0.8), transparent);
}

.logo {
    font-size: 34px;
    font-weight: 900;
    letter-spacing: 6px;
    background: linear-gradient(90deg, #8b5cf6, #ec4899, #f59e0b);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

nav a {
    margin-left: 36px;
    text-decoration: none;
    color: #ddd;
    font-weight: 300;
}

nav a:hover {
    color: white;
}

/* HERO */
.hero {
    height: 100vh;
    display: flex;
    align-items: center;
    padding-left: 80px;
    position: relative;
}

.hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background:
      radial-gradient(circle at 70% 20%, #8b5cf644, transparent 40%),
      radial-gradient(circle at 20% 60%, #ec489944, transparent 40%);
}

.hero-content {
    position: relative;
    max-width: 700px;
}

.hero h1 {
    font-size: 96px;
    font-weight: 900;
    line-height: 1;
    background: linear-gradient(90deg, #fff, #d4d4d4);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.hero p {
    margin-top: 30px;
    font-size: 22px;
    opacity: 0.8;
}

.buttons {
    margin-top: 50px;
}

.buttons a {
    padding: 18px 46px;
    margin-right: 20px;
    border-radius: 50px;
    font-weight: 600;
    text-decoration: none;
    color: white;
    display: inline-block;
}

.primary {
    background: linear-gradient(90deg, #8b5cf6, #ec4899);
    box-shadow: 0 0 40px #8b5cf688;
}

.secondary {
    border: 1px solid #ffffff33;
}

/* INFO */
.info {
    display: flex;
    justify-content: space-around;
    padding: 100px 60px;
    background: linear-gradient(to top, #050008, #070010);
}

.block {
    text-align: center;
}

.block h2 {
    font-size: 52px;
    background: linear-gradient(90deg, #8b5cf6, #ec4899);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.block p {
    margin-top: 10px;
    opacity: 0.7;
}

/* FOOTER */
footer {
    text-align: center;
    padding: 50px;
    opacity: 0.5;
}
</style>
</head>

<body>

<header>
    <div class="logo">IB</div>
    <nav>
        <a href="#">Главная</a>
        <a href="#">Коллекции</a>
        <a href="#">Контакты</a>
    </nav>
</header>

<section class="hero">
    <div class="hero-content">
        <h1>IB CLOTHING</h1>
        <p>Премиальный дизайн одежды нового уровня</p>
        <div class="buttons">
            <a href="#" class="primary">Смотреть дроп</a>
            <a href="#" class="secondary">О проекте</a>
        </div>
    </div>
</section>

<section class="info">
    <div class="block">
        <h2>12+</h2>
        <p>Коллекций</p>
    </div>
    <div class="block">
        <h2>500+</h2>
        <p>Моделей</p>
    </div>
    <div class="block">
        <h2>IB</h2>
        <p>Эксклюзив</p>
    </div>
</section>

<footer>
    © IB PROJECT • Premium Style
</footer>

</body>
</html>
