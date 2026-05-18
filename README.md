# Luan-Pereira-
Meu Repositório 

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>

<title>Luan Pereira | Full Stack Developer</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"/>

<style>

/* =========================
RESET
========================= */
*{
margin:0;
padding:0;
box-sizing:border-box;
scroll-behavior:smooth;
}

body{
font-family:'Poppins',sans-serif;
background:#050816;
color:#fff;
overflow-x:hidden;
}

/* =========================
SCROLLBAR
========================= */
::-webkit-scrollbar{
width:10px;
}

::-webkit-scrollbar-track{
background:#050816;
}

::-webkit-scrollbar-thumb{
background:#00bfff;
border-radius:20px;
}

/* =========================
BACKGROUND
========================= */
.bg{
position:fixed;
width:100%;
height:100%;
top:0;
left:0;
background:
radial-gradient(circle at top left,#00bfff22,transparent 30%),
radial-gradient(circle at bottom right,#8b5cf622,transparent 30%),
#050816;
z-index:-1;
}

/* =========================
NAVBAR
========================= */
nav{
position:fixed;
top:0;
left:0;
width:100%;
padding:20px 8%;
display:flex;
justify-content:space-between;
align-items:center;
backdrop-filter:blur(14px);
background:rgba(5,8,22,.7);
border-bottom:1px solid rgba(255,255,255,.08);
z-index:999;
}

.logo{
font-size:24px;
font-weight:800;
color:#00bfff;
}

nav ul{
display:flex;
gap:25px;
list-style:none;
}

nav a{
text-decoration:none;
color:#cbd5e1;
font-weight:500;
transition:.3s;
}

nav a:hover{
color:#00bfff;
}

/* =========================
HERO
========================= */
.hero{
min-height:100vh;
display:flex;
justify-content:center;
align-items:center;
padding:120px 8%;
}

.hero-content{
display:grid;
grid-template-columns:1fr 400px;
align-items:center;
gap:80px;
width:100%;
max-width:1300px;
}

.hero-text h3{
font-size:22px;
color:#00bfff;
margin-bottom:10px;
}

.hero-text h1{
font-size:72px;
line-height:1.1;
margin-bottom:20px;
}

.hero-text span{
background:linear-gradient(90deg,#00bfff,#8b5cf6);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
}

.hero-text p{
font-size:18px;
color:#94a3b8;
margin-bottom:35px;
max-width:600px;
line-height:1.8;
}

.hero-buttons{
display:flex;
gap:20px;
flex-wrap:wrap;
}

/* =========================
BUTTONS
========================= */
.btn{
padding:16px 32px;
border-radius:60px;
text-decoration:none;
font-weight:700;
transition:.3s;
display:inline-flex;
align-items:center;
gap:10px;
}

.btn-primary{
background:linear-gradient(90deg,#00bfff,#2563eb);
color:white;
box-shadow:0 0 30px #00bfff55;
}

.btn-primary:hover{
transform:translateY(-5px);
box-shadow:0 0 45px #00bfff88;
}

.btn-secondary{
border:1px solid rgba(255,255,255,.15);
color:white;
background:rgba(255,255,255,.04);
}

.btn-secondary:hover{
background:#ffffff10;
transform:translateY(-5px);
}

/* =========================
PHOTO
========================= */
.hero-photo{
position:relative;
display:flex;
justify-content:center;
}

.hero-photo img{
width:100%;
max-width:380px;
border-radius:30px;
border:2px solid rgba(255,255,255,.1);
box-shadow:
0 0 40px #00bfff33,
0 0 120px #8b5cf622;
animation:float 4s ease-in-out infinite;
}

@keyframes float{
0%{ transform:translateY(0px); }
50%{ transform:translateY(-15px); }
100%{ transform:translateY(0px); }
}

/* =========================
SECTION
========================= */
section{
padding:120px 8%;
}

.section-title{
font-size:48px;
margin-bottom:60px;
text-align:center;
}

.section-title span{
color:#00bfff;
}

/* =========================
ABOUT
========================= */
.about-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:30px;
}

.about-card{
background:rgba(255,255,255,.04);
padding:35px;
border-radius:25px;
border:1px solid rgba(255,255,255,.08);
transition:.3s;
}

.about-card:hover{
transform:translateY(-10px);
border-color:#00bfff;
}

.about-card i{
font-size:40px;
color:#00bfff;
margin-bottom:20px;
}

/* =========================
STACK
========================= */
.stack{
display:flex;
justify-content:center;
flex-wrap:wrap;
gap:20px;
}

.tech{
padding:18px 25px;
background:rgba(255,255,255,.04);
border-radius:18px;
border:1px solid rgba(255,255,255,.08);
font-weight:600;
transition:.3s;
}

.tech:hover{
background:#00bfff;
transform:translateY(-8px);
}

/* =========================
PROJECTS
========================= */
.projects-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(320px,1fr));
gap:30px;
}

.project-card{
background:rgba(255,255,255,.04);
border-radius:25px;
overflow:hidden;
border:1px solid rgba(255,255,255,.08);
transition:.4s;
}

.project-card:hover{
transform:translateY(-12px);
border-color:#00bfff;
}

.project-image{
height:220px;
background:linear-gradient(135deg,#00bfff,#8b5cf6);
display:flex;
justify-content:center;
align-items:center;
font-size:70px;
}

.project-content{
padding:30px;
}

.project-content h3{
margin-bottom:15px;
font-size:24px;
}

.project-content p{
color:#94a3b8;
line-height:1.7;
margin-bottom:25px;
}

/* =========================
SOCIAL
========================= */
.socials{
display:flex;
justify-content:center;
gap:20px;
flex-wrap:wrap;
margin-top:50px;
}

.socials a{
width:70px;
height:70px;
display:flex;
justify-content:center;
align-items:center;
font-size:28px;
text-decoration:none;
border-radius:20px;
background:rgba(255,255,255,.04);
border:1px solid rgba(255,255,255,.08);
color:white;
transition:.3s;
}

.socials a:hover{
background:#00bfff;
transform:translateY(-8px) scale(1.08);
}

/* =========================
FOOTER
========================= */
footer{
padding:40px 8%;
text-align:center;
border-top:1px solid rgba(255,255,255,.08);
color:#94a3b8;
}

/* =========================
RESPONSIVO
========================= */
@media(max-width:980px){

.hero-content{
grid-template-columns:1fr;
text-align:center;
}

.hero-text h1{
font-size:52px;
}

.hero-buttons{
justify-content:center;
}

}

@media(max-width:768px){

nav{
padding:18px 5%;
flex-direction:column;
gap:15px;
}

nav ul{
flex-wrap:wrap;
justify-content:center;
}

.hero{
padding-top:180px;
}

.hero-text h1{
font-size:42px;
}

.section-title{
font-size:36px;
}

.hero-photo img{
max-width:300px;
}

}

</style>
</head>

<body>

<div class="bg"></div>

<!-- NAVBAR -->
<nav>

<div class="logo">
LUAN.dev
</div>

<ul>
<li><a href="#inicio">Início</a></li>
<li><a href="#sobre">Sobre</a></li>
<li><a href="#stack">Stack</a></li>
<li><a href="#projetos">Projetos</a></li>
<li><a href="#contato">Contato</a></li>
</ul>

</nav>

<!-- HERO -->
<section class="hero" id="inicio">

<div class="hero-content">

<div class="hero-text">

<h3>👋 Olá, eu sou</h3>

<h1>
Luan Pereira <br>
<span>Full Stack Developer</span>
</h1>

<p>
Desenvolvedor focado em aplicações modernas, sistemas escaláveis,
interfaces premium e experiências digitais de alto impacto.
Construindo projetos reais com JavaScript, React e Node.js.
</p>

<div class="hero-buttons">

<a href="https://github.com/AFRICANTU" target="_blank" class="btn btn-primary">
<i class="fa-brands fa-github"></i>
GitHub
</a>

<a href="https://www.linkedin.com" target="_blank" class="btn btn-secondary">
<i class="fa-brands fa-linkedin"></i>
LinkedIn
</a>

</div>

</div>

<div class="hero-photo">

<img src="sua-foto.jpg" alt="Luan Pereira">

</div>

</div>

</section>

<!-- SOBRE -->
<section id="sobre">

<h2 class="section-title">
Sobre <span>Mim</span>
</h2>

<div class="about-grid">

<div class="about-card">
<i class="fa-solid fa-code"></i>
<h3>Desenvolvimento Web</h3>
<p>
Criação de aplicações modernas, interfaces premium e sistemas responsivos.
</p>
</div>

<div class="about-card">
<i class="fa-solid fa-server"></i>
<h3>Backend</h3>
<p>
Estudando Node.js, APIs REST, autenticação e arquitetura escalável.
</p>
</div>

<div class="about-card">
<i class="fa-solid fa-rocket"></i>
<h3>Objetivo</h3>
<p>
Evoluir para atuar em projetos Full Stack de alto nível e produtos digitais modernos.
</p>
</div>

</div>

</section>

<!-- STACK -->
<section id="stack">

<h2 class="section-title">
Minha <span>Stack</span>
</h2>

<div class="stack">

<div class="tech">HTML5</div>
<div class="tech">CSS3</div>
<div class="tech">JavaScript</div>
<div class="tech">React</div>
<div class="tech">Node.js</div>
<div class="tech">Git</div>
<div class="tech">GitHub</div>
<div class="tech">UI/UX</div>

</div>

</section>

<!-- PROJETOS -->
<section id="projetos">

<h2 class="section-title">
Projetos <span>Recentes</span>
</h2>

<div class="projects-grid">

<div class="project-card">

<div class="project-image">
🦷
</div>

<div class="project-content">

<h3>Sistema Odontológico</h3>

<p>
Sistema moderno com login, agendamento online,
persistência local e integração WhatsApp.
</p>

<a href="#" class="btn btn-primary">
Ver Projeto
</a>

</div>

</div>

<div class="project-card">

<div class="project-image">
🍰
</div>

<div class="project-content">

<h3>Sweet Snake Delivery</h3>

<p>
Landing page premium focada em branding,
conversão e experiência moderna.
</p>

<a href="#" class="btn btn-primary">
Ver Projeto
</a>

</div>

</div>

<div class="project-card">

<div class="project-image">
💅
</div>

<div class="project-content">

<h3>Gabriela Art Unhas</h3>

<p>
Landing page premium com estrutura moderna,
branding forte e conversão otimizada.
</p>

<a href="#" class="btn btn-primary">
Ver Projeto
</a>

</div>

</div>

</div>

</section>

<!-- CONTATO -->
<section id="contato">

<h2 class="section-title">
Entre em <span>Contato</span>
</h2>

<p style="text-align:center;color:#94a3b8;font-size:18px;">
Vamos construir algo incrível juntos 🚀
</p>

<div class="socials">

<a href="https://github.com/AFRICANTU" target="_blank">
<i class="fa-brands fa-github"></i>
</a>

<a href="https://linkedin.com" target="_blank">
<i class="fa-brands fa-linkedin"></i>
</a>

<a href="https://instagram.com/mutasenji" target="_blank">
<i class="fa-brands fa-instagram"></i>
</a>

<a href="https://tiktok.com/@l_senji" target="_blank">
<i class="fa-brands fa-tiktok"></i>
</a>

<a href="https://youtube.com/@l-senji" target="_blank">
<i class="fa-brands fa-youtube"></i>
</a>

</div>

</section>

<!-- FOOTER -->
<footer>

<p>
© 2026 Luan Pereira • Full Stack Developer
</p>

</footer>

<script>

/* =========================
NAVBAR EFFECT
========================= */
window.addEventListener("scroll", () => {

const nav = document.querySelector("nav");

if(window.scrollY > 50){
nav.style.background = "rgba(5,8,22,.95)";
}else{
nav.style.background = "rgba(5,8,22,.7)";
}

});

/* =========================
SCROLL REVEAL
========================= */
const observer = new IntersectionObserver((entries) => {

entries.forEach(entry => {

if(entry.isIntersecting){
entry.target.style.opacity = 1;
entry.target.style.transform = "translateY(0)";
}

});

}, { threshold:0.15 });

document.querySelectorAll("section").forEach(section => {

section.style.opacity = 0;
section.style.transform = "translateY(40px)";
section.style.transition = ".8s";

observer.observe(section);

});

</script>

</body>
</html>