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
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT · Contacto</title>
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
font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
color: #f9fafb;
background: radial-gradient(circle at top left, #0b4fbf 0, #021631 40%, #000000 100%);
min-height: 100vh;
}
a {
color: inherit;
text-decoration: none;
}
.wrapper {
min-height: 100vh;
display: flex;
flex-direction: column;
}
.container {
max-width: 1150px;
margin: 0 auto;
padding: 2rem 1.25rem;
flex: 1;
}
.site-header {
background: linear-gradient(180deg, rgba(3,16,46,0.95), rgba(2,22,49,0.95));
backdrop-filter: blur(18px);
border-bottom: 1px solid rgba(148, 163, 184, 0.35);
box-shadow: 0 10px 30px rgba(0, 0, 0, 0.55);
}
.header-inner {
max-width: 1150px;
margin: auto;
padding: .75rem 1.25rem;
display: flex;
align-items: center;
justify-content: flex-start;
gap: 1rem;
flex-wrap: wrap;
}
.brand {
display: flex;
gap: .75rem;
align-items: center;
margin-right: auto;
}
.brand-logo {
width: 52px;
height: 52px;
border-radius: 999px;
overflow: hidden;
border: 2px solid rgba(248, 250, 252, 0.8);
background: #020617;
box-shadow: 0 0 20px rgba(15, 23, 42, 0.9);
}
.brand-logo img {
width: 100%;
height: 100%;
object-fit: cover;
}
.brand-name {
font-size: 1.4rem;
text-transform: uppercase;
letter-spacing: 0.20em;
font-weight: 700;
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
.card {
max-width: 620px;
margin: 3rem auto;
padding: 2rem;
background: rgba(15, 23, 42, 0.9);
border-radius: 1rem;
border: 1px solid rgba(148, 163, 184, 0.5);
box-shadow: 0 22px 60px rgba(0, 0, 0, 0.75);
text-align: left;
}
.card-title {
font-size: 1.1rem;
letter-spacing: 0.18em;
text-transform: uppercase;
margin-bottom: 1rem;
text-align: center;
}
.card-intro {
font-size: 0.95rem;
color: #e5e7eb;
margin-bottom: 0.75rem;
text-align: center;
}
.email {
text-align: center;
margin-bottom: 1.5rem;
font-size: 0.95rem;
}
.email a {
font-weight: 600;
text-decoration: underline;
}
.contact-form {
margin-top: 1rem;
display: flex;
flex-direction: column;
gap: 1rem;
}
.form-group {
display: flex;
flex-direction: column;
gap: 0.35rem;
}
.form-group label {
font-size: 0.8rem;
text-transform: uppercase;
letter-spacing: 0.14em;
color: #9ca3af;
}
.form-control {
width: 100%;
padding: 0.65rem 0.75rem;
border-radius: 0.5rem;
border: 1px solid rgba(148, 163, 184, 0.7);
background: rgba(15, 23, 42, 0.95);
color: #e5e7eb;
font-size: 0.95rem;
}
.form-control:focus {
outline: none;
border-color: #3b82f6;
box-shadow: 0 0 0 1px rgba(59, 130, 246, 0.6);
}
textarea.form-control {
min-height: 120px;
resize: vertical;
}
.btn-primary {
align-self: flex-start;
margin-top: 0.25rem;
padding: 0.6rem 1.4rem;
border-radius: 999px;
border: none;
background: linear-gradient(90deg, #2563eb, #3b82f6);
color: #f9fafb;
text-transform: uppercase;
letter-spacing: 0.16em;
font-size: 0.8rem;
font-weight: 600;
cursor: pointer;
box-shadow: 0 12px 30px rgba(15, 23, 42, 0.9);
transition: transform 0.15s ease, box-shadow 0.15s ease, opacity 0.15s ease;
}
.btn-primary:hover {
transform: translateY(-1px);
box-shadow: 0 18px 40px rgba(15, 23, 42, 1);
opacity: 0.95;
}
.comments-section {
margin-top: 2rem;
border-top: 1px solid rgba(148, 163, 184, 0.4);
padding-top: 1.25rem;
}
.comments-title {
font-size: 0.9rem;
text-transform: uppercase;
letter-spacing: 0.16em;
margin-bottom: 0.75rem;
color: #e5e7eb;
}
.comments-empty {
font-size: 0.85rem;
color: #9ca3af;
}
.comment-item {
padding: 0.75rem 0;
border-bottom: 1px solid rgba(31, 41, 55, 0.9);
}
.comment-header {
display: flex;
justify-content: space-between;
align-items: baseline;
margin-bottom: 0.25rem;
}
.comment-author {
font-weight: 600;
font-size: 0.9rem;
}
.comment-date {
font-size: 0.75rem;
color: #9ca3af;
}
.comment-body {
font-size: 0.9rem;
color: #e5e7eb;
white-space: pre-wrap;
}

footer {
background: rgba(3, 7, 18, 0.95);
border-top: 1px solid rgba(148, 163, 184, 0.3);
padding: 1rem;
font-size: 0.75rem;
text-align: center;
color: #9ca3af;
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
<section class="card">
<h2 class="card-title">Contacto</h2>
<p class="card-intro">
¿Tienes ideas, sugerencias o encontraste un bug en LAB RAT? Déjanos tu comentario o escríbenos directamente.
</p>
<p class="email">
También puedes contactarnos por email: 
<a href="mailto:labrat@gmail.com">labrat@gmail.com</a>
</p>
<form class="contact-form" id="commentForm">
<div class="form-group">
<label for="name">Nombre</label>
<input class="form-control" type="text" id="name" name="name" required placeholder="Tu nombre">
</div>
<div class="form-group">
<label for="email">Correo electrónico</label>
<input class="form-control" type="email" id="email" name="email" required placeholder="tucorreo@example.com">
</div>
<div class="form-group">
<label for="message">Comentario</label>
<textarea class="form-control" id="message" name="message" required placeholder="Escribe aquí tu comentario, sugerencia o reporte de error..."></textarea>
</div>
<button type="submit" class="btn-primary">Enviar comentario</button>
</form>
<div id="commentsList"></div>
</div>
</section>
</div>
<footer>
© 2025 LAB RAT
</footer>
</div>
<script>
const form = document.getElementById('commentForm');
const commentsList = document.getElementById('commentsList');
const commentsEmpty = document.getElementById('commentsEmpty');
form.addEventListener('submit', function (e) {
e.preventDefault();
const name = form.name.value.trim();
const email = form.email.value.trim();
const message = form.message.value.trim();
if (!name || !email || !message) {
alert('Por favor completa todos los campos.');
return;
}
const commentItem = document.createElement('div');
commentItem.className = 'comment-item';
const header = document.createElement('div');
header.className = 'comment-header';
const author = document.createElement('div');
author.className = 'comment-author';
author.textContent = name;
const date = document.createElement('div');
date.className = 'comment-date';
const now = new Date();
date.textContent = now.toLocaleString('es-ES', {
dateStyle: 'short',
timeStyle: 'short'
});
header.appendChild(author);
header.appendChild(date);
const body = document.createElement('div');
body.className = 'comment-body';
body.textContent = message;
commentItem.appendChild(header);
commentItem.appendChild(body);
if (commentsEmpty) {
commentsEmpty.style.display = 'none';
}
commentsList.prepend(commentItem);
form.reset();
});
</script>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT · PC para estudiar y jugar</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta name="description" content="Guía sencilla para elegir una PC equilibrada para estudiar y jugar sin gastar de más." />
<style>
*,*::before,*::after{
box-sizing:border-box;
margin:0;
padding:0;
}
body{
font-family:system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
color:#f9fafb;
background:radial-gradient(circle at top left,#0b4fbf 0,#021631 40%,#000 100%);
min-height:100vh;
line-height:1.5;
}
a{
color:inherit;
text-decoration:none;
}
.wrapper{
min-height:100vh;
display:flex;
flex-direction:column;
}
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
justify-content:space-between;
align-items:center;
gap:1rem;
flex-wrap:wrap;
}
.brand{
display:flex;
gap:.75rem;
align-items:center;
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
.brand-name {
font-size: 1.4rem;
text-transform: uppercase;
letter-spacing: 0.20em;
font-weight: 700;
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
.navbar a{
opacity:.7;
position:relative;
padding-bottom:.3rem;
transition:opacity .2s ease;
}
.navbar a.active,
.navbar a:hover{
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
transition:.25s;
}
.navbar a.active::after,
.navbar a:hover::after{
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
padding:1.75rem;
}
.hero-title{
font-size:1.5rem;
text-transform:uppercase;
letter-spacing:.18em;
margin-bottom:1rem;
}
.article-intro{
font-size:.95rem;
color:#e5e7eb;
max-width:45rem;
margin-bottom:1.5rem;
}
.article-grid{
display:grid;
grid-template-columns:repeat(2,minmax(0,1fr));
gap:1rem 1.5rem;
}
.article-block{
background:rgba(15,23,42,.95);
border-radius:.8rem;
border:1px solid rgba(148,163,184,.4);
padding:1rem 1.1rem;
}
.block-title{
font-size:.95rem;
font-weight:600;
margin-bottom:.3rem;
}
.block-title span{
display:block;
font-size:.75rem;
text-transform:uppercase;
letter-spacing:.14em;
color:#93c5fd;
}
.block-text{
color:#e5e7eb;
margin-bottom:.35rem;
}
.block-tip{
font-size:.8rem;
color:#a5b4fc;
}
.article-conclusion{
margin-top:1.5rem;
padding:1rem;
border-radius:.8rem;
border:1px solid rgba(148,163,184,.5);
background:rgba(15,23,42,.95);
font-size:.9rem;
}
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
@media (max-width:768px){
.article-grid{
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
<h1 class="hero-title">¿Qué PC me conviene para estudiar y jugar?</h1>
<p class="article-intro">
Elegir una PC para estudiar y jugar no tiene que ser complicado ni caro.
La clave está en balancear los componentes para que rindan bien en tareas académicas
y también en juegos, sin gastar más de lo necesario.
</p>
<div class="article-grid">
<article class="article-block">
<h2 class="block-title">CPU <span>Rendimiento general</span></h2>
<p class="block-text">
Para estudiar (Word, PowerPoint, navegar, programación básica) no necesitas
un procesador de gama alta.
</p>
<p class="block-tip">
Recomendación: Ryzen 5 o Intel i5 para un buen balance.
</p>
</article>
<article class="article-block">
<h2 class="block-title">GPU <span>Juegos</span></h2>
<p class="block-text">
Si quieres jugar títulos populares como Fortnite, GTA V o Valorant,
una GPU dedicada mejora mucho la experiencia.
</p>
<p class="block-tip">
Recomendación: GTX 1660 o RTX 3060 para 1080p.
</p>
</article>
<article class="article-block">
<h2 class="block-title">RAM <span>Multitarea</span></h2>
<p class="block-text">
Permite abrir varios programas a la vez sin que la PC se ponga lenta.
</p>
<p class="block-tip">
Recomendación: 16 GB como estándar actual.
</p>
</article>
<article class="article-block">
<h2 class="block-title">Almacenamiento <span>Velocidad</span></h2>
<p class="block-text">
Un SSD hace que todo cargue más rápido, desde Windows hasta juegos.
</p>
<p class="block-tip">
Recomendación: SSD NVMe de 1 TB.
</p>
</article>
</div>
<div class="article-conclusion">
<strong>Conclusión:</strong><br>
No necesitas la PC más cara para estudiar y jugar. Un equipo equilibrado
te dará buen rendimiento hoy y para varios años si eliges bien tus componentes.
</div>
</section>
</main>
<footer class="site-footer">
<div class="footer-inner">
<span>© <span id="year"></span> LAB RAT</span>
</div>
</footer>
</div>
<script>
document.getElementById("year").textContent = new Date().getFullYear();
</script>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT · Errores comunes al armar tu primera PC</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta name="description" content="Errores comunes al armar tu primera PC y cómo evitarlos, explicado de forma sencilla para principiantes." />
<style>
*,*::before,*::after{
box-sizing:border-box;
margin:0;
padding:0;
}
body{
font-family:system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
color:#f9fafb;
background:radial-gradient(circle at top left,#0b4fbf 0,#021631 40%,#000 100%);
min-height:100vh;
line-height:1.5;
}
a{
color:inherit;
text-decoration:none;
}
.wrapper{
min-height:100vh;
display:flex;
flex-direction:column;
}
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
justify-content:space-between;
align-items:center;
gap:1rem;
flex-wrap:wrap;
}
.brand{
display:flex;
gap:.75rem;
align-items:center;
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
.brand-name {
  font-size: 1.4rem;
  text-transform: uppercase;
  letter-spacing: 0.20em; /* opcional, puedes bajarlo si se ve muy separado */
  font-weight: 700;
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
.navbar a{
opacity:.7;
position:relative;
padding-bottom:.3rem;
transition:opacity .2s ease;
}
.navbar a.active,
.navbar a:hover{
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
transition:.25s;
}
.navbar a.active::after,
.navbar a:hover::after{
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
padding:1.75rem;
}
.hero-title{
font-size:1.5rem;
text-transform:uppercase;
letter-spacing:.18em;
margin-bottom:1rem;
}
.article-intro{
font-size:.95rem;
color:#e5e7eb;
max-width:45rem;
margin-bottom:1.5rem;
}
.article-grid{
display:grid;
grid-template-columns:repeat(2,minmax(0,1fr));
gap:1rem 1.5rem;
}
.article-block{
background:rgba(15,23,42,.95);
border-radius:.8rem;
border:1px solid rgba(148,163,184,.4);
padding:1rem 1.1rem;
font-size:.9rem;
}
.block-title{
font-size:.95rem;
font-weight:600;
margin-bottom:.3rem;
}
.block-title span{
display:block;
font-size:.75rem;
text-transform:uppercase;
letter-spacing:.14em;
color:#fca5a5;
}
.block-text{
color:#e5e7eb;
margin-bottom:.35rem;
}
.block-tip{
font-size:.8rem;
color:#a5b4fc;
}
.article-conclusion{
margin-top:1.5rem;
padding:1rem;
border-radius:.8rem;
border:1px solid rgba(248,113,113,.7);
background:rgba(15,23,42,.95);
font-size:.9rem;
color:#fee2e2;
}
.article-conclusion strong{
color:#fecaca;
}
.mini-list{
margin-top:.45rem;
padding-left:1.1rem;
font-size:.86rem;
color:#e5e7eb;
}
.mini-list li{
margin-bottom:.25rem;
}
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
@media (max-width:768px){
.article-grid{
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
<h1 class="hero-title">Errores comunes al armar tu primera PC</h1>
<p class="article-intro">
Armar una PC por primera vez puede dar miedo, pero la mayoría de los problemas
vienen de los mismos errores repetidos. Aquí verás los errores más comunes
y cómo evitarlos, explicado en lenguaje sencillo.
</p>
<div class="article-grid">
<article class="article-block">
<h2 class="block-title">1. No conectar todos los cables de la fuente <span>PC enciende, pero no da imagen</span></h2>
<p class="block-text">
Muchas veces se conecta solo el cable grande de 24 pines a la motherboard,
pero se olvida el cable de 8 pines (o 4+4) que alimenta el CPU.
</p>
<p class="block-tip">
Solución: revisa que el conector ATX de 24 pines y el conector EPS de 8 pines
estén bien puestos. Ambos son necesarios.
</p>
</article>
<article class="article-block">
<h2 class="block-title">2. Conectar el monitor a la salida equivocada <span>Sin señal de video</span></h2>
<p class="block-text">
Si tienes una tarjeta gráfica dedicada (GPU), el monitor debe ir conectado
a la GPU, no a los puertos de video de la motherboard.
</p>
<p class="block-tip">
Solución: conecta el cable HDMI/DisplayPort en la GPU (la que está más abajo,
en posición horizontal) y no en los puertos superiores.
</p>
</article>
<article class="article-block">
<h2 class="block-title">3. No encajar bien la RAM <span>Pitidos o pantalla negra</span></h2>
<p class="block-text">
A veces la RAM parece estar puesta, pero no hizo clic en ambos lados
y la PC no arranca correctamente.
</p>
<p class="block-tip">
Solución: saca el módulo, alinea la muesca y presiona con firmeza hasta que las trabas
se cierren solas. Verifica que no se vea “despareja”.
</p>
</article>
<article class="article-block">
<h2 class="block-title">4. Usar fuentes de poder genéricas <span>Riesgo para todos los componentes</span></h2>
<p class="block-text">
Una fuente de mala calidad puede fallar y dañar tu GPU, motherboard o disco.
Es de las peores formas de “ahorrar dinero”.
</p>
<p class="block-tip">
Solución: elige una fuente con certificación 80+ (White, Bronze, Gold) y de marca confiable.
Mejor gastar un poco más que perder toda la PC.
</p>
</article>
<article class="article-block">
<h2 class="block-title">5. Mala ventilación y manejo de cables <span>Temperaturas altas</span></h2>
<p class="block-text">
Si los cables quedan hechos un nudo y no hay buen flujo de aire,
la PC se calentará más de lo necesario.
</p>
<p class="block-tip">
Solución: usa las bridas que trae el case, organiza los cables por detrás
y asegúrate de que haya al menos un ventilador metiendo aire y otro sacándolo.
</p>
</article>
<article class="article-block">
<h2 class="block-title">6. No leer el manual de la motherboard <span>Cables frontales mal conectados</span></h2>
<p class="block-text">
Los pines del panel frontal (botón de encender, reset, LED, etc.)
son pequeños y se ven confusos, pero el manual los explica con un diagrama.
</p>
<p class="block-tip">
Solución: busca en el manual la sección “Front panel headers” o similar
y sigue el dibujo con calma. Es normal equivocarse al principio.
</p>
</article>
</div>
</section>
</main>
<footer class="site-footer">
<div class="footer-inner">
<span>© <span id="year"></span> LAB RAT</span>
</div>
</footer>
</div>
<script>
document.getElementById("year").textContent = new Date().getFullYear();
</script>
</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<title>LAB RAT · Cómo planear un presupuesto para tu PC</title>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<meta name="description" content="Guía para planear correctamente el presupuesto de tu PC y gastar el dinero donde realmente importa." />
<style>
*,*::before,*::after{
box-sizing:border-box;
margin:0;
padding:0;
}
body{
font-family:system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
color:#f9fafb;
background:radial-gradient(circle at top left,#0b4fbf 0,#021631 40%,#000 100%);
min-height:100vh;
line-height:1.5;
}
a{
color:inherit;
text-decoration:none;
}
.wrapper{
min-height:100vh;
display:flex;
flex-direction:column;
}
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
justify-content:space-between;
align-items:center;
gap:1rem;
flex-wrap:wrap;
}
.brand{
display:flex;
gap:.75rem;
align-items:center;
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
.brand-name {
font-size: 1.4rem;
text-transform: uppercase;
letter-spacing: 0.20em;
font-weight: 700;
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
.navbar a{
opacity:.7;
position:relative;
padding-bottom:.3rem;
}
.navbar a.active,
.navbar a:hover{
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
transition:.25s;
}
.navbar a.active::after,
.navbar a:hover::after{
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
padding:1.75rem;
}
.hero-title{
font-size:1.5rem;
text-transform:uppercase;
letter-spacing:.18em;
margin-bottom:1rem;
}
.article-intro{
font-size:.95rem;
color:#e5e7eb;
max-width:45rem;
margin-bottom:1.5rem;
}
.article-grid{
display:grid;
grid-template-columns:repeat(2,minmax(0,1fr));
gap:1rem 1.5rem;
}
.article-block{
background:rgba(15,23,42,.95);
border-radius:.8rem;
border:1px solid rgba(148,163,184,.4);
padding:1rem 1.1rem;
font-size:.9rem;
}
.block-title{
font-size:.95rem;
font-weight:600;
margin-bottom:.3rem;
}
.block-title span{
display:block;
font-size:.75rem;
text-transform:uppercase;
letter-spacing:.14em;
color:#86efac;
}
.block-text{
color:#e5e7eb;
margin-bottom:.35rem;
}
.block-tip{
font-size:.8rem;
color:#a5b4fc;
}
.article-conclusion{
margin-top:1.5rem;
padding:1rem;
border-radius:.8rem;
border:1px solid rgba(134,239,172,.7);
background:rgba(15,23,42,.95);
font-size:.9rem;
color:#dcfce7;
}
.article-conclusion strong{
color:#bbf7d0;
}
.budget-list{
margin-top:.4rem;
padding-left:1.2rem;
font-size:.85rem;
color:#e5e7eb;
}
.budget-list li{
margin-bottom:.25rem;
}
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
@media (max-width:768px){
.article-grid{
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
<h1 class="hero-title">Cómo planear un presupuesto para tu PC</h1>
<p class="article-intro">
Antes de comprar componentes al azar, es importante saber
cómo repartir bien tu dinero. Un buen presupuesto evita cuellos
de botella y te da mejor rendimiento por cada dólar gastado.
</p>
<div class="article-grid">
<article class="article-block">
<h2 class="block-title">1. Define para qué usarás la PC <span>El paso más importante</span></h2>
<p class="block-text">
No es lo mismo una PC para estudiar que una para gaming o edición.
El uso define dónde debes invertir más dinero.
</p>
<p class="block-tip">
Consejo: escribe tus prioridades antes de comprar.
</p>
</article>
<article class="article-block">
<h2 class="block-title">2. Invierte más en GPU o CPU según tu uso <span>Balance correcto</span></h2>
<p class="block-text">
En gaming, la GPU suele ser la parte más importante.
En programación o edición, la CPU y la RAM pesan más.
</p>
<p class="block-tip">
Consejo: evita gastar demasiado en un solo componente.
</p>
</article>
<article class="article-block">
<h2 class="block-title">3. No ahorres en la fuente <span>Protección del sistema</span></h2>
<p class="block-text">
Una fuente barata puede fallar y dañar todo el equipo.
</p>
<p class="block-tip">
Consejo: busca certificación 80+ y marcas conocidas.
</p>
</article>
<article class="article-block">
<h2 class="block-title">4. SSD antes que HDD <span>Velocidad diaria</span></h2>
<p class="block-text">
Un SSD mejora notablemente el arranque y la experiencia general.
</p>
<p class="block-tip">
Consejo: mínimo 500 GB, ideal 1 TB.
</p>
</article>
<article class="article-block">
<h2 class="block-title">5. No gastes de más en el case <span>Estética vs función</span></h2>
<p class="block-text">
Un case bonito no hace la PC más rápida.
Lo importante es el flujo de aire.
</p>
<p class="block-tip">
Consejo: prioriza airflow sobre RGB.
</p>
</article>
<article class="article-block">
<h2 class="block-title">6. Deja un margen extra <span>Imprevistos</span></h2>
<p class="block-text">
Siempre surgen gastos adicionales: cables, ventiladores o impuestos.
</p>
<p class="block-tip">
Consejo: guarda un 5–10% del presupuesto total.
</p>
</article>
</div>
<div class="article-conclusion">
<strong>Distribución recomendada del presupuesto:</strong>
<ul class="budget-list">
<li>GPU: 35–45%</li>
<li>CPU: 20–25%</li>
<li>RAM: 10–15%</li>
<li>Almacenamiento: 10–15%</li>
<li>PSU + Case: 10–15%</li>
</ul>
</div>
</section>
</main>
<footer class="site-footer">
<div class="footer-inner">
<span>© <span id="year"></span> LAB RAT</span>
</div>
</footer>
</div>
<script>
document.getElementById("year").textContent = new Date().getFullYear();
</script>
</body>
</html>
