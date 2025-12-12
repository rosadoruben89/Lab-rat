<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT Web · Tu primera PC</title>
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
backdrop-filter:blur(18px);
border-bottom:1px solid rgba(148,163,184,.35);
}
.header-inner{
max-width:1150px;
margin:auto;
padding:.75rem 1.25rem;
display:flex;
align-items:center;
justify-content:flex-start;
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
align-items:center;
gap:1.5rem;
font-size:.86rem;
text-transform:uppercase;
letter-spacing:.16em;
margin-left:auto;
margin-right:auto;
}
.navbar a{
opacity:.7;
position:relative;
padding-bottom:.3rem;
transition:opacity .2s ease;
}
.navbar a:hover,
.navbar a.active{
opacity:1;
}
.navbar a::after{
content:"";
position:absolute;
left:0;
bottom:0;
width:100%;
height:2px;
background:linear-gradient(90deg,#fff,#38bdf8);
transform:scaleX(0);
transform-origin:left;
transition:transform .25s ease;
}
.navbar a:hover::after,
.navbar a.active::after{
transform:scaleX(1);
}
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
.card + .card{
margin-top:1.5rem;
}
.hero-title{
font-size:1.6rem;
letter-spacing:.18em;
text-transform:uppercase;
margin-bottom:1rem;
}
.section-intro{
font-size:.95rem;
color:#e5e7eb;
margin-bottom:1.3rem;
max-width:40rem;
}
.articles-title{
font-size:.9rem;
text-transform:uppercase;
letter-spacing:.16em;
color:#bfdbfe;
margin-bottom:.6rem;
}
.articles-list{
display:grid;
grid-template-columns:repeat(3,minmax(0,1fr));
gap:.85rem;
font-size:.85rem;
}
.article-card{
background:rgba(15,23,42,.95);
border-radius:.7rem;
border:1px solid rgba(148,163,184,.45);
padding:.7rem .8rem;
}
.article-title{
font-size:.9rem;
font-weight:600;
margin-bottom:.25rem;
}
.article-desc{
color:#e5e7eb;
margin-bottom:.35rem;
}
.article-link{
font-size:.78rem;
text-transform:uppercase;
letter-spacing:.14em;
color:#93c5fd;
}
.parts-grid{
display:grid;
grid-template-columns:repeat(2,minmax(0,1fr));
gap:1rem 1.5rem;
}
.part-block{
background:rgba(15,23,42,.95);
border-radius:.8rem;
border:1px solid rgba(148,163,184,.4);
padding:0.9rem 1rem;
font-size:.9rem;
}
.part-title{
font-size:.95rem;
font-weight:600;
margin-bottom:.3rem;
}
.part-title span{
font-size:.78rem;
text-transform:uppercase;
letter-spacing:.14em;
color:#93c5fd;
display:block;
}
.part-desc{color:#e5e7eb;margin-bottom:.35rem}
.part-tip{font-size:.8rem;color:#a5b4fc}
.site-footer{
border-top:1px solid rgba(148,163,184,.4);
background:rgba(3,7,18,.95);
padding:.75rem 1.25rem;
font-size:.78rem;
color:#9ca3af;
}
.footer-inner{
max-width:1150px;
margin:auto;
display:flex;
justify-content:space-between;
gap:1rem;
flex-wrap:wrap;
}
.footer-links{
display:flex;
gap:1rem;
flex-wrap:wrap;
}
@media (max-width:900px){
.articles-list{
grid-template-columns:repeat(2,minmax(0,1fr));
}
}
@media (max-width:768px){
.parts-grid{
grid-template-columns:minmax(0,1fr);
}
.articles-list{
grid-template-columns:minmax(0,1fr);
}
}
</style>
</head>
<body>
<div class="wrapper">
<header class="site-header">
<div class="header-inner">
<a href="index1.html" class="brand">
<div class="brand-logo">
<img src="ratas.jpg" alt="LAB RAT logo">
</div>
<div class="brand-name">LAB RAT</div>
</a>
<nav class="navbar">
<a href="index1.html">Home</a>
<a href="index2.html">Build</a>
<a href="index5.html">Guia</a>
<a href="index3.html">Contactanos</a>
</nav>
</div>
</header>
<main class="container">
<section class="card">
<h1 class="hero-title">Partes básicas de una PC</h1>
<p class="section-intro">
Si vas a armar tu primera computadora, estas son las piezas principales que
debes conocer y para qué sirve cada una.
</p>
<div class="parts-grid">
<article class="part-block">
<h2 class="part-title">CPU <span>El cerebro</span></h2>
<p class="part-desc">Procesa todas las instrucciones y tareas.</p>
<p class="part-tip">Tip: para estudiar y jugar, una CPU de gama media es suficiente.</p>
</article>
<article class="part-block">
<h2 class="part-title">GPU <span>Gráficos</span></h2>
<p class="part-desc">Dibuja juegos, videos y gráficos 3D.</p>
<p class="part-tip">Tip: es clave si piensas jugar o editar video.</p>
</article>
<article class="part-block">
<h2 class="part-title">RAM <span>Memoria</span></h2>
<p class="part-desc">Permite abrir varios programas sin lentitud.</p>
<p class="part-tip">Tip: 16 GB es el punto ideal hoy en día.</p>
</article>
<article class="part-block">
<h2 class="part-title">SSD / HDD <span>Almacenamiento</span></h2>
<p class="part-desc">Guarda tu sistema, programas y archivos.</p>
<p class="part-tip">Tip: usa SSD para velocidad.</p>
</article>
<article class="part-block">
<h2 class="part-title">Motherboard <span>Base</span></h2>
<p class="part-desc">Conecta todas las partes.</p>
<p class="part-tip">Tip: verifica compatibilidad con CPU y RAM.</p>
</article>
<article class="part-block">
<h2 class="part-title">PSU <span>Energía</span></h2>
<p class="part-desc">Alimenta todo el sistema.</p>
<p class="part-tip">Tip: nunca compres fuentes genéricas.</p>
</article>
</div>
</section>
<section class="card">
<h2 class="articles-title">Artículos recomendados para principiantes</h2>
<div class="articles-list">
<article class="article-card">
<h3 class="article-title">¿Qué PC me conviene para estudiar y jugar?</h3>
<p class="article-desc">
Guía sencilla para elegir componentes si quieres una PC que sirva tanto para clases como para gaming ligero.
</p>
<a href="index4.html" class="article-link">Leer más</a>
</article>
<article class="article-card">
<h3 class="article-title">Errores comunes al armar tu primera PC</h3>
<p class="article-desc">
Cosas que deberías evitar: fuentes genéricas, mala ventilación, incompatibilidades y más.
</p>
<a href="index6.html" class="article-link">Leer más</a>
</article>
<article class="article-card">
<h3 class="article-title">Cómo planear un presupuesto para tu PC</h3>
<p class="article-desc">
Aprende a repartir tu dinero entre CPU, GPU, RAM y otros componentes sin romper la alcancía.
</p>
<a href="index7.html" class="article-link">Leer más</a>
</article>
</div>
</section>
</main>
<footer class="site-footer">
<div class="footer-inner">
<div>© <span id="year"></span> LAB RAT</div>
</div>
</footer>
</div>
<script>
document.getElementById("year").textContent=new Date().getFullYear();
</script>
</body>
</html>
