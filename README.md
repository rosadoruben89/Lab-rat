<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT · Tu primera PC</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta name="description" content="Guía sencilla de partes de PC para personas que van a armar su primera computadora." />

<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
body{
font-family:system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
color:#f9fafb;
background:radial-gradient(circle at top left,#0b4fbf 0,#021631 40%,#000 100%);
min-height:100vh;
}
a{color:inherit;text-decoration:none}
.wrapper{min-height:100vh;display:flex;flex-direction:column}
.site-header{
background:linear-gradient(180deg,rgba(3,16,46,.95),rgba(2,22,49,.95));
border-bottom:1px solid rgba(148,163,184,.35);
}
.header-inner{
max-width:1150px;
margin:auto;
padding:.75rem 1.25rem;
display:flex;
align-items:center;
gap:1rem;
flex-wrap:wrap;
}
.brand{
display:flex;
gap:.75rem;
align-items:center;
margin-right:auto;
}
.brand-logo{
width:52px;
height:52px;
border-radius:999px;
overflow:hidden;
border:2px solid rgba(255,255,255,.8);
background:#020617;
}
.brand-logo img{
width:100%;
height:100%;
object-fit:cover;
}
.brand-name{
font-size:1.4rem;
text-transform:uppercase;
letter-spacing:.20em;
font-weight:700;
}
.navbar{
display:flex;
gap:1.5rem;
font-size:.86rem;
text-transform:uppercase;
letter-spacing:.16em;
}
.navbar a{opacity:.7}
.navbar a:hover,.navbar a.active{opacity:1}

.container{
max-width:1150px;
margin:auto;
padding:2rem 1.25rem;
flex:1;
}

.card{
background:rgba(15,23,42,.9);
border-radius:1rem;
border:1px solid rgba(148,163,184,.55);
padding:1.5rem;
}

.hero-title{
font-size:1.6rem;
letter-spacing:.18em;
text-transform:uppercase;
margin-bottom:1rem;
}
.section-intro{
color:#e5e7eb;
margin-bottom:1.3rem;
max-width:40rem;
}

.parts-grid{
display:grid;
grid-template-columns:repeat(2,1fr);
gap:1rem;
}
.part-block{
background:rgba(15,23,42,.95);
border-radius:.8rem;
border:1px solid rgba(148,163,184,.4);
padding:1rem;
}
.part-title{
font-weight:600;
margin-bottom:.3rem;
}
.part-title span{
display:block;
font-size:.8rem;
text-transform:uppercase;
color:#93c5fd;
}

.site-footer{
border-top:1px solid rgba(148,163,184,.4);
background:rgba(3,7,18,.95);
padding:1rem;
text-align:center;
font-size:.8rem;
color:#9ca3af;
}

@media(max-width:768px){
.parts-grid{grid-template-columns:1fr}
}
</style>
</head>

<body>
<div class="wrapper">
<header class="site-header">
<div class="header-inner">
<a href="index.html" class="brand">
<div class="brand-logo">
<img src="ratas.jpg" alt="LAB RAT logo">
</div>
<div class="brand-name">LAB RAT</div>
</a>

<nav class="navbar">
<a href="index.html" class="active">Home</a>
<a href="build.html">Build</a>
<a href="guia.html">Guia</a>
<a href="contacto.html">Contactanos</a>
</nav>
</div>
</header>

<main class="container">
<section class="card">
<h1 class="hero-title">Partes básicas de una PC</h1>
<p class="section-intro">
Si vas a armar tu primera computadora, estas son las piezas principales que debes conocer.
</p>

<div class="parts-grid">
<div class="part-block">
<h2 class="part-title">CPU <span>El cerebro</span></h2>
<p>Procesa todas las instrucciones.</p>
</div>

<div class="part-block">
<h2 class="part-title">GPU <span>Gráficos</span></h2>
<p>Dibuja juegos y video.</p>
</div>

<div class="part-block">
<h2 class="part-title">RAM <span>Memoria</span></h2>
<p>Permite abrir varios programas.</p>
</div>

<div class="part-block">
<h2 class="part-title">SSD <span>Almacenamiento</span></h2>
<p>Guarda sistema y archivos.</p>
</div>
</div>
</section>
</main>

<footer class="site-footer">
© 2025 LAB RAT
</footer>
</div>
</body>
</html>
