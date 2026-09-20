<head>

<style>

/* =========================
   CONFIGURACIÓN GENERAL
========================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    width: 100%;
    overflow-x: hidden;
    scroll-behavior: smooth;
}

body {
    width: 100%;
    min-height: 100vh;
    overflow-x: hidden;

    font-family: Arial, Helvetica, sans-serif;

    color: white;

    background:
        linear-gradient(
            135deg,
            #0c0599 0%,
            #3b0bb5 45%,
            #de12d7 100%
        );
}


/* =========================
   DESTELLOS
========================= */

.sparkles {
    position: fixed;

    top: 0;
    left: 0;

    width: 100%;
    height: 100%;

    pointer-events: none;

    overflow: hidden;

    z-index: 0;
}

.sparkles span {
    position: absolute;

    top: -20px;

    width: 4px;
    height: 4px;

    border-radius: 50%;

    background: #00ffff;

    box-shadow:
        0 0 10px #00ffff,
        0 0 20px #00ffff;

    animation: caer linear infinite;
}

.sparkles span:nth-child(1) {
    left: 5%;
    animation-duration: 8s;
}

.sparkles span:nth-child(2) {
    left: 15%;
    animation-duration: 10s;
    background: white;
}

.sparkles span:nth-child(3) {
    left: 25%;
    animation-duration: 7s;
}

.sparkles span:nth-child(4) {
    left: 35%;
    animation-duration: 12s;
    background: #a0e9ff;
}

.sparkles span:nth-child(5) {
    left: 45%;
    animation-duration: 9s;
    background: white;
}

.sparkles span:nth-child(6) {
    left: 55%;
    animation-duration: 11s;
}

.sparkles span:nth-child(7) {
    left: 65%;
    animation-duration: 8s;
}

.sparkles span:nth-child(8) {
    left: 75%;
    animation-duration: 10s;
    background: white;
}

.sparkles span:nth-child(9) {
    left: 85%;
    animation-duration: 7s;
    background: #a0e9ff;
}

.sparkles span:nth-child(10) {
    left: 95%;
    animation-duration: 9s;
}


@keyframes caer {

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


/* =========================
   CONTENIDO PRINCIPAL
========================= */

.page {
    position: relative;

    z-index: 1;

    width: 100%;
    max-width: 1100px;

    margin: 0 auto;
}


/* =========================
   ENCABEZADO
========================= */

header {

    width: 100%;

    padding: 45px 20px;

    text-align: center;

    background:
        rgba(0, 0, 0, 0.25);

    border-bottom:
        1px solid rgba(255,255,255,0.5);
}

header h1 {

    font-size: clamp(32px, 7vw, 60px);

    color: #00bfff;

    margin-bottom: 15px;

    word-wrap: break-word;
}

header p {

    font-size: clamp(16px, 4vw, 24px);

    color: white;
}


/* =========================
   MENÚ
========================= */

nav {

    width: 100%;

    display: flex;

    justify-content: center;

    align-items: center;

    flex-wrap: wrap;

    background: #e94cae;

    border-bottom:
        1px solid rgba(255,255,255,0.4);
}

nav a {

    display: block;

    padding: 16px 22px;

    color: white;

    text-decoration: none;

    font-weight: bold;

    font-size: 17px;

    transition: 0.2s;
}

nav a:hover {

    background: #c90078;
}


/* =========================
   CONTENEDOR
========================= */

.container {

    width: 100%;

    max-width: 1000px;

    margin: 0 auto;

    padding: 20px;
}


/* =========================
   TARJETAS
========================= */

.card {

    width: 100%;

    max-width: 100%;

    padding: 25px;

    margin: 20px 0;

    background:
        rgba(255,255,255,0.14);

    border:
        1px solid rgba(255,255,255,0.18);

    border-radius: 18px;

    box-shadow:
        0 8px 25px rgba(0,0,0,0.25);

    backdrop-filter: blur(10px);

    overflow: hidden;
}

.card h2 {

    width: 100%;

    font-size: clamp(24px, 5vw, 34px);

    margin-bottom: 18px;

    padding-bottom: 12px;

    border-bottom:
        2px solid rgba(255,255,255,0.7);

    word-wrap: break-word;
}

.card p {

    width: 100%;

    font-size: 18px;

    line-height: 1.6;

    margin: 10px 0;

    overflow-wrap: anywhere;

    word-break: normal;
}


/* =========================
   PRECIOS
========================= */

.precios {

    width: 100%;

    display: flex;

    flex-direction: column;

    gap: 12px;
}

.precio {

    width: 100%;

    padding: 16px;

    background:
        rgba(0,0,0,0.22);

    border:
        1px solid rgba(255,255,255,0.15);

    border-radius: 12px;

    font-size: 17px;

    overflow-wrap: anywhere;
}


/* =========================
   CONTACTO
========================= */

.contacto {

    width: 100%;

    padding: 25px;

    text-align: center;

    background:
        rgba(0,0,0,0.25);

    border-radius: 18px;

    border:
        1px solid rgba(255,255,255,0.2);
}

.contacto h2 {

    margin-bottom: 15px;
}

.contacto p {

    overflow-wrap: anywhere;
}


/* =========================
   FOOTER
========================= */

footer {

    width: 100%;

    padding: 10px 0 30px;

    text-align: center;
}

footer > p {

    margin-top: 20px;

    font-size: 14px;

    opacity: 0.8;
}


/* =========================
   CELULARES
========================= */

@media (max-width: 700px) {

    .container {

        width: 100%;

        padding:
            15px;
    }

    header {

        padding:
            35px 15px;
    }

    nav a {

        flex: 1 1 auto;

        text-align: center;

        padding:
            15px 10px;

        font-size: 15px;
    }

    .card {

        padding:
            20px;

        margin:
            15px 0;

        border-radius:
            15px;
    }

    .card h2 {

        font-size:
            26px;
    }

    .card p {

        font-size:
            16px;
    }

    .precio {

        font-size:
            16px;
    }

}


/* =========================
   CELULARES PEQUEÑOS
========================= */

@media (max-width: 400px) {

    .container {

        padding:
            10px;
    }

    header h1 {

        font-size:
            34px;
    }

    nav a {

        font-size:
            14px;

        padding:
            13px 7px;
    }

    .card {

        padding:
            17px;
    }

    .card h2 {

        font-size:
            23px;
    }

}

</style>

</head>


<body>


<!-- =========================
     DESTELLOS
========================= -->

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


<div class="page">


<!-- =========================
     ENCABEZADO
========================= -->

<header>

    <h1>Uma.Tobi</h1>

    <p>
        Emprendimiento Uma Tobi 💖
    </p>

</header>


<!-- =========================
     MENÚ
========================= -->

<nav>

    <a href="#saladas">
        Cosas Saladas
    </a>

    <a href="#precios">
        Precios
    </a>

    <a href="#contacto">
        Contacto
    </a>

</nav>


<!-- =========================
     CONTENIDO
========================= -->

<main class="container">


    <!-- COSAS SALADAS -->

    <section
        class="card"
        id="saladas"
    >

        <h2>
            🥪 Cosas Saladas
        </h2>

        <p>
            <strong>Pizzetas:</strong>
        </p>

        <p>
            Próximamente agregaremos más productos.
        </p>

    </section>


    <!-- PRECIOS -->

    <section
        class="card"
        id="precios"
    >

        <h2>
            💰 Precios
        </h2>


        <div class="precios">

            <div class="precio">
                Budín de Vainilla: $4.500
            </div>

            <div class="precio">
                Budín Marmolado: $4.500
            </div>

            <div class="precio">
                Budín de Limón: $4.500
            </div>

            <div class="precio">
                Budín con Chispas de Chocolate: $4.500
            </div>

        </div>

    </section>


    <!-- CONTACTO -->

    <footer id="contacto">

        <div class="contacto">

            <h2>
                📞 Contacto
            </h2>

            <p>
                WhatsApp:
                +54 9 11 6258-0452
            </p>

        </div>

        <p>
            © 2026 Uma.Tobi
        </p>

    </footer>


</main>

</div>

</body>

</html>