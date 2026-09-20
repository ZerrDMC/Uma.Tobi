
<!DOCTYPE html>
<html lang="es">

<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Emprendimiento Uma Tobi</title>

<style>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

:root {
    --blanco: #ffffff;
    --rosa: #ff69b4;
    --violeta: #cab8ff;
    --oscuro: #0c0599;
}

body {
    font-family: Arial, sans-serif;
    color: white;
    min-height: 100vh;
    background: linear-gradient(135deg, #0c0599, #de12d7);
}

/* Destellos animados */

.sparkles {
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: 0;
    overflow: hidden;
}

.sparkles span {
    position: absolute;
    top: -20px;
    width: 4px;
    height: 4px;
    border-radius: 50%;
    background: #00ffff;
    box-shadow: 0 0 15px #00ffff;
    animation: fall linear infinite;
}

.sparkles span:nth-child(1) { left: 5%; animation-duration: 8s; }
.sparkles span:nth-child(2) { left: 15%; animation-duration: 10s; background: white; }
.sparkles span:nth-child(3) { left: 25%; animation-duration: 7s; }
.sparkles span:nth-child(4) { left: 35%; animation-duration: 12s; background: #a0e9ff; }
.sparkles span:nth-child(5) { left: 45%; animation-duration: 9s; background: white; }
.sparkles span:nth-child(6) { left: 55%; animation-duration: 11s; }
.sparkles span:nth-child(7) { left: 65%; animation-duration: 8s; }
.sparkles span:nth-child(8) { left: 75%; animation-duration: 10s; background: white; }
.sparkles span:nth-child(9) { left: 85%; animation-duration: 7s; background: #a0e9ff; }
.sparkles span:nth-child(10) { left: 95%; animation-duration: 9s; }

@keyframes fall {
    0% {
        transform: translateY(-20px);
        opacity: 0;
    }

    10% {
        opacity: 1;
    }

    100% {
        transform: translateY(110vh);
        opacity: 0;
    }
}

/* Contenido */

header {
    background: rgba(0, 0, 0, 0.25);
    color: white;
    padding: 30px 15px;
    text-align: center;
    position: relative;
    z-index: 1;
}

header h2 {
    font-size: 28px;
}

nav {
    background: rgba(255, 105, 180, 0.9);
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    position: relative;
    z-index: 1;
}

nav a {
    color: white;
    padding: 15px 20px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    background: #000000;
}

.container {
    max-width: 1000px;
    margin: auto;
    padding: 20px;
    position: relative;
    z-index: 1;
}

.card {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(10px);
    padding: 25px;
    margin: 20px 0;
    border-radius: 15px;
    box-shadow: 0 0 15px rgba(0, 0, 0, 0.2);
}

.card h2 {
    margin-bottom: 15px;
}

.card p {
    margin: 10px 0;
    font-size: 17px;
}

.precios {
    display: grid;
    gap: 10px;
}

.precio {
    background: rgba(0, 0, 0, 0.2);
    padding: 15px;
    border-radius: 10px;
    font-weight: bold;
}

footer {
    text-align: center;
    padding: 20px;
    position: relative;
    z-index: 1;
}

.contacto {
    background: rgba(0, 0, 0, 0.25);
    padding: 20px;
    border-radius: 15px;
}

@media (max-width: 700px) {
    header h2 {
        font-size: 22px;
    }

    nav a {
        padding: 12px;
        font-size: 14px;
    }

    .container {
        padding: 10px;
    }
}

</style>

</head>

<body>

<!-- Destellos -->

<div class="sparkles">
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
    <span></span>
</div>

<header>
    <h2>Emprendimiento Uma Tobi</h2>
    <p>Productos caseros hechos con amor 💖</p>
</header>

<nav>
    <a href="#cosas-saladas">Cosas Saladas</a>
    <a href="#precios">Precios</a>
    <a href="#contacto">Contacto</a>
</nav>

<div class="container">

    <div class="card" id="cosas-saladas">
        <h2>🥪 Cosas Saladas</h2>
        <p><strong>Pizzetas:</strong></p>
        <p>Próximamente agregaremos más productos.</p>
    </div>

    <div class="card" id="precios">
        <h2>💰 Precios</h2>

        <div class="precios">
            <div class="precio">Budín de Vainilla: $4.500</div>
            <div class="precio">Budín Marmolado: $4.500</div>
            <div class="precio">Budín de Limón: $4.500</div>
            <div class="precio">Budín con Chispas de Chocolate: $4.500</div>
        </div>
    </div>

    <footer id="contacto">
        <div class="contacto">
            <h2>📞 Contacto</h2>
            <p>WhatsApp: +54 9 11 6258-0452</p>
        </div>

        <p style="margin-top: 20px;">
            © 2026 Emprendimiento Uma Tobi
        </p>
    </footer>

</div>

</body>
</html>
