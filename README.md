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
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%201.html" class="brand">
<div class="brand-logo">
<img src="ratas.jpg" alt="LAB RAT logo">
</div>
<div class="brand-name">LAB RAT</div>
</a>
<nav class="navbar">
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%201.html">Home</a>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%202.html">Build</a>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%205.html">Guia</a>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%203.html">Contactanos</a>
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
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%204.html" class="article-link">Leer más</a>
</article>
<article class="article-card">
<h3 class="article-title">Errores comunes al armar tu primera PC</h3>
<p class="article-desc">
Cosas que deberías evitar: fuentes genéricas, mala ventilación, incompatibilidades y más.
</p>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%206.html" class="article-link">Leer más</a>
</article>
<article class="article-card">
<h3 class="article-title">Cómo planear un presupuesto para tu PC</h3>
<p class="article-desc">
Aprende a repartir tu dinero entre CPU, GPU, RAM y otros componentes sin romper la alcancía.
</p>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%207.html" class="article-link">Leer más</a>
</article>
</div>
</section>
</main>
<footer class="site-footer">
<div class="footer-inner">
<footer>
© <span id="year"></span> LAB RAT
</footer>
</div>
</footer>
</div>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT PC Builder · Opciones</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
*,
*::before,
*::after {
box-sizing: border-box;
margin: 0;
padding: 0;
}
body {
font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
sans-serif;
color: #f9fafb;
background: radial-gradient(circle at top left, #0b4fbf 0, #021631 40%, #000000 100%);
min-height: 100vh;
line-height: 1.5;
}
a {
color: inherit;
text-decoration: none;
}
img {
max-width: 100%;
display: block;
}
.wrapper {
min-height: 100vh;
display: flex;
flex-direction: column;
}
.container {
width: 100%;
max-width: 1150px;
margin: 0 auto;
padding: 1.5rem 1.25rem 2.5rem;
flex: 1;
}
.site-header {
background: rgba(3, 16, 46, 0.9);
backdrop-filter: blur(18px);
border-bottom: 1px solid rgba(148, 163, 184, 0.35);
box-shadow: 0 10px 30px rgba(0, 0, 0, 0.55);
}
.header-inner {
max-width: 1150px;
margin: 0 auto;
padding: 0.75rem 1.25rem;
display: flex;
align-items: center;
justify-content: space-between;
gap: 1rem;
flex-wrap: wrap;
}
.brand {
display: flex;
align-items: center;
gap: 0.75rem;
}
.brand-logo {
width: 52px;
height: 52px;
border-radius: 999px;
overflow: hidden;
border: 2px solid rgba(248, 250, 252, 0.8);
box-shadow: 0 0 20px rgba(15, 23, 42, 0.9);
background: #020617;
}
.brand-logo img {
width: 100%;
height: 100%;
object-fit: cover;
}
.brand-text {
display: flex;
flex-direction: column;
gap: 0.1rem;
}
.brand-name {
font-size: 1.4rem;
text-transform: uppercase;
letter-spacing: 0.20em;
font-weight: 700;
}

.brand-tagline {
font-size: 0.75rem;
color: #cbd5f5;
}
.navbar {
display: flex;
align-items: center;
gap: 1.5rem;
font-size: 0.86rem;
text-transform: uppercase;
letter-spacing: 0.16em;

margin-left: auto;
margin-right: auto; 
}
.navbar a {
position: relative;
padding-bottom: 0.25rem;
opacity: 0.85;
transition: opacity 0.2s ease, transform 0.2s ease;
}
.navbar a::after {
content: "";
position: absolute;
left: 0;
bottom: 0;
width: 0;
height: 2px;
border-radius: 999px;
background: linear-gradient(90deg, #ffffff, #3b82f6);
transition: width 0.2s ease;
}
.navbar a:hover {
opacity: 1;
transform: translateY(-1px);
}
.navbar a:hover::after,
.navbar a.active::after {
width: 100%;
}

main {
margin-top: 1.5rem;
}
.card {
background: rgba(15, 23, 42, 0.9);
border-radius: 1rem;
border: 1px solid rgba(148, 163, 184, 0.55);
box-shadow: 0 22px 60px rgba(0, 0, 0, 0.8);
padding: 1.4rem 1.5rem;
}
.card-title {
font-size: 1.1rem;
text-transform: uppercase;
letter-spacing: 0.18em;
margin-bottom: 0.8rem;
}
.card-subtitle {
font-size: 0.9rem;
color: #d1d5db;
margin-bottom: 1rem;
}
.hero-title {
font-size: 1.7rem;
text-transform: uppercase;
letter-spacing: 0.18em;
margin-bottom: 0.5rem;
}
.hero-title span.blue {
color: #60a5fa;
}
.hero-title span.cyan {
color: #22d3ee;
}
.hero-text {
font-size: 0.95rem;
color: #e5e7eb;
max-width: 32rem;
margin-bottom: 1.2rem;
}
.hero-badges {
display: flex;
flex-wrap: wrap;
gap: 0.5rem;
margin-bottom: 1.2rem;
font-size: 0.75rem;
}
.badge {
padding: 0.25rem 0.6rem;
border-radius: 999px;
border: 1px solid rgba(148, 163, 184, 0.7);
background: rgba(15, 23, 42, 0.9);
text-transform: uppercase;
letter-spacing: 0.14em;
color: #cbd5f5;
}
.hero-meta {
margin-top: 0.9rem;
display: flex;
flex-wrap: wrap;
gap: 1.5rem;
font-size: 0.78rem;
color: #9ca3af;
text-transform: uppercase;
letter-spacing: 0.14em;
margin-bottom: 1.2rem;
}
.hero-meta span strong {
color: #e5e7eb;
font-weight: 600;
}
.btn-main {
border-radius: 999px;
border: none;
padding: 0.7rem 1.4rem;
font-size: 0.8rem;
text-transform: uppercase;
letter-spacing: 0.18em;
cursor: pointer;
background: linear-gradient(120deg, #38bdf8, #ffffff);
color: #020617;
box-shadow: 0 16px 40px rgba(0, 0, 0, 0.8);
transition: transform 0.2s ease, box-shadow 0.2s ease, filter 0.2s ease;
}
.btn-main:hover {
transform: translateY(-1px) scale(1.01);
box-shadow: 0 18px 46px rgba(0, 0, 0, 0.85);
filter: brightness(1.02);
}
.parts-table-wrapper {
overflow-x: auto;
margin-top: 0.8rem;
}

table {
width: 100%;
border-collapse: collapse;
font-size: 0.86rem;
min-width: 650px;
}

thead {
background: rgba(15, 23, 42, 0.98);
}

th,
td {
padding: 0.65rem 0.75rem;
text-align: left;
border-bottom: 1px solid rgba(55, 65, 81, 0.8);
}

th {
font-size: 0.75rem;
text-transform: uppercase;
letter-spacing: 0.15em;
color: #9ca3af;
}

tbody tr:nth-child(even) {
background: rgba(15, 23, 42, 0.85);
}

tbody tr:hover {
background: rgba(30, 64, 175, 0.55);
}

.col-category {
width: 140px;
font-weight: 600;
color: #e5e7eb;
}

.col-part {
width: 45%;
}

.col-price {
white-space: nowrap;
}

.part-select {
width: 100%;
padding: 0.4rem 0.5rem;
border-radius: 0.5rem;
border: 1px solid rgba(148, 163, 184, 0.8);
background: rgba(15, 23, 42, 0.95);
color: #e5e7eb;
font-size: 0.85rem;
}

.part-note {
font-size: 0.74rem;
color: #9ca3af;
margin-top: 0.25rem;
}

.price {
font-variant-numeric: tabular-nums;
}

.total-row {
margin-top: 1.4rem;
display: flex;
justify-content: space-between;
align-items: flex-start;
flex-wrap: wrap;
gap: 0.8rem;
}

.total-label {
font-size: 0.85rem;
color: #9ca3af;
text-transform: uppercase;
letter-spacing: 0.18em;
}

.total-amount {
font-size: 1.2rem;
font-weight: 700;
color: #bbf7d0;
font-variant-numeric: tabular-nums;
}

/* breakdown styling */
.breakdown {
margin-top: 0.4rem;
font-size: 0.8rem;
color: #e5e7eb;
}
.breakdown-item {
display: flex;
justify-content: space-between;
gap: 0.75rem;
}
.breakdown-item span:first-child {
opacity: 0.9;
}
.breakdown-item span:last-child {
font-variant-numeric: tabular-nums;
}

/* Footer */
.site-footer {
border-top: 1px solid rgba(148, 163, 184, 0.4);
background: rgba(3, 7, 18, 0.95);
padding: 0.75rem 1.25rem;
font-size: 0.78rem;
color: #9ca3af;
}
.footer-inner {
max-width: 1150px;
margin: 0 auto;
display: flex;
justify-content: space-between;
align-items: center;
gap: 0.75rem;
flex-wrap: wrap;
}
.footer-links {
display: flex;
gap: 1rem;
flex-wrap: wrap;
}
.footer-links a {
opacity: 0.85;
transition: opacity 0.2s ease;
}
.footer-links a:hover {
opacity: 1;
}

/* Responsive */
@media (max-width: 900px) {
.container {
padding-inline: 1rem;
}
table {
font-size: 0.82rem;
}
}
@media (max-width: 520px) {
.card {
padding-inline: 1.1rem;
}
.hero-title {
font-size: 1.4rem;
letter-spacing: 0.14em;
}
}
</style>
</head>
<body>
<div class="wrapper">
<header class="site-header">
<div class="header-inner">
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%201.html" class="brand">
<div class="brand-logo">
<img src="ratas.jpg" alt="LAB RAT logo">
</div>
<div class="brand-name">LAB RAT</div>
</a>
<nav class="navbar">
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%201.html">Home</a>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%202.html">Build</a>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%205.html">Guia</a>
<a href="file:///C:/Users/rosad/OneDrive/Manga%20Iguana/INTER/WEB%20DEV%20CLIENT%20%20front%20end/final%20project/index%203.html">Contactanos</a>
</nav>
</div>
</header>
<div class="container">
<main>
<section class="card" id="builder">
<h1 class="hero-title">
Construye tu <span class="blue">PC</span><br />
eligiendo entre <span class="cyan">varias opciones</span>
</h1>
<p class="hero-text">
Selecciona una opción para cada categoría. Cada opción tiene un precio asociado
y el total se calcula automáticamente.
</p>
<div class="parts-table-wrapper">
<table>
<thead>
<tr>
<th>Categoría</th>
<th>Componente</th>
<th>Precio</th>
</tr>
</thead>
<tbody>
<tr data-row>
<td class="col-category">CPU</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona un CPU –</option>
<option data-price="90">Ryzen 3 · Básico (US$90)</option>
<option data-price="145">Ryzen 5 · Gaming medio (US$145)</option>
<option data-price="230">Ryzen 7 · Gaming/creador (US$230)</option>
</select>
<div class="part-note">El procesador afecta rendimiento general y FPS.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
<tr data-row>
<td class="col-category">GPU</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona una GPU –</option>
<option data-price="180">GTX 1660 Super (US$180)</option>
<option data-price="270">RTX 3060 (US$270)</option>
<option data-price="420">RTX 4070 (US$420)</option>
</select>
<div class="part-note">La tarjeta gráfica es clave para gaming y apps 3D.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
<tr data-row>
<td class="col-category">RAM</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona la RAM –</option>
<option data-price="35">8GB DDR4 (US$35)</option>
<option data-price="55">16GB DDR4 (US$55)</option>
<option data-price="95">32GB DDR4 (US$95)</option>
</select>
<div class="part-note">Más RAM ayuda con multitarea y programas pesados.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
<tr data-row>
<td class="col-category">Almacenamiento</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona almacenamiento –</option>
<option data-price="35">SSD 480GB SATA (US$35)</option>
<option data-price="55">SSD 1TB NVMe (US$55)</option>
<option data-price="90">SSD 1TB NVMe + HDD 2TB (US$90)</option>
</select>
<div class="part-note">SSD hace que el sistema se sienta mucho más rápido.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
<tr data-row>
<td class="col-category">Motherboard</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona motherboard –</option>
<option data-price="75">B450 básica (US$75)</option>
<option data-price="95">B550 con M.2 extra (US$95)</option>
<option data-price="140">X570 más completa (US$140)</option>
</select>
<div class="part-note">Afecta compatibilidad y puertos disponibles.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
<tr data-row>
<td class="col-category">Case</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona el case –</option>
<option data-price="45">Case básico con 1 fan (US$45)</option>
<option data-price="65">Case airflow 3 fans (US$65)</option>
<option data-price="90">Case con vidrio + RGB (US$90)</option>
</select>
<div class="part-note">El airflow ayuda a mantener la temperatura baja.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
<tr data-row>
<td class="col-category">Fuente (PSU)</td>
<td class="col-part">
<select class="part-select">
<option value="" data-price="0">– Selecciona la fuente –</option>
<option data-price="45">500W 80+ White (US$45)</option>
<option data-price="60">650W 80+ Bronze (US$60)</option>
<option data-price="90">750W 80+ Gold (US$90)</option>
</select>
<div class="part-note">Una buena PSU da estabilidad y seguridad.</div>
</td>
<td class="col-price price" data-price="0">$0.00</td>
</tr>
</tbody>
</table>
</div>
<div class="total-row" id="resumen">
<div>
<div class="total-label">Costo total estimado</div>
<div id="totalAmount" class="total-amount">$0.00</div>
<div id="breakdown" class="breakdown">
</div>
</div>
<button type="button" class="btn-main" id="recalcBtn">
Reset
</button>
</div>
</section>
</main>
</div>
<footer class="site-footer">
<div class="footer-inner">
<span>© <span id="year"></span> LAB RAT</span>
<div class="footer-links">
</div>
</div>
</footer>
</div>
<script>
function recalcTotal() {
let total = 0;
const rows = document.querySelectorAll("tr[data-row]");
const breakdownItems = [];

rows.forEach(function (row) {
const categoryCell = row.querySelector(".col-category");
const select = row.querySelector(".part-select");
const priceCell = row.querySelector(".price");
if (!select || !priceCell || !categoryCell) return;

const option = select.options[select.selectedIndex];
const price = parseFloat(option.getAttribute("data-price")) || 0;
const partName = option.value === "" ? "" : option.textContent.trim();
const categoryName = categoryCell.textContent.trim();
priceCell.setAttribute("data-price", price.toString());
priceCell.textContent = "$" + price.toFixed(2);
total += price;
if (price > 0 && partName) {
breakdownItems.push({
category: categoryName,
part: partName,
price: price
});
}
});
document.getElementById("totalAmount").textContent = "$" + total.toFixed(2);
const breakdownDiv = document.getElementById("breakdown");
if (breakdownItems.length === 0) {
breakdownDiv.innerHTML = "<em>No has seleccionado componentes aún.</em>";
} else {
breakdownDiv.innerHTML = breakdownItems.map(item => `
<div class="breakdown-item">
<span>${item.category}: ${item.part}</span>
<span>$${item.price.toFixed(2)}</span>
</div>
`).join("");
}
}
function resetBuilder() {
const selects = document.querySelectorAll(".part-select");
selects.forEach(select => {
select.selectedIndex = 0;
});
recalcTotal();
}
recalcTotal();
document.querySelectorAll(".part-select").forEach(function (select) {
select.addEventListener("change", recalcTotal);
});
document.getElementById("recalcBtn").addEventListener("click", resetBuilder);
document.getElementById("year").textContent = new Date().getFullYear();
const currentFile = decodeURIComponent(location.pathname.split("/").pop());
document.querySelectorAll(".navbar a").forEach(link => {
const href = link.getAttribute("href");
if (!href) return;
const linkFile = decodeURIComponent(
href.split("/").pop().split("#")[0].split("?")[0]
);
if (linkFile === currentFile) {
link.classList.add("active");
} else {
link.classList.remove("active");
}
});
</script>
</body>
</html>
