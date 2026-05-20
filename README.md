<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>

<title>Luan Pereira | Full Stack Developer</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Poppins',sans-serif;
    background:#070707;
    color:#fff;
    overflow-x:hidden;
}

/* BACKGROUND */

.bg{
    position:fixed;
    width:100%;
    height:100vh;
    background:
    radial-gradient(circle at top,#1b1b1b 0%,#070707 70%);
    z-index:-2;
}

.blur{
    position:fixed;
    width:500px;
    height:500px;
    background:#00bfff25;
    filter:blur(140px);
    z-index:-1;
    animation:float 8s infinite ease-in-out;
}

.blur2{
    right:0;
    bottom:0;
    background:#7b2cff2c;
}

@keyframes float{
    0%{transform:translateY(0px);}
    50%{transform:translateY(-30px);}
    100%{transform:translateY(0px);}
}

/* NAV */

nav{
    width:100%;
    padding:25px 8%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    position:fixed;
    top:0;
    backdrop-filter:blur(12px);
    z-index:999;
}

.logo{
    font-size:28px;
    font-weight:800;
    color:#fff;
}

.logo span{
    color:#00bfff;
}

nav ul{
    display:flex;
    gap:25px;
    list-style:none;
}

nav a{
    text-decoration:none;
    color:#d4d4d4;
    transition:.3s;
}

nav a:hover{
    color:#00bfff;
}

/* HERO */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:140px 8%;
    gap:60px;
}

.hero-left{
    max-width:650px;
}

.badge{
    display:inline-block;
    padding:10px 20px;
    border:1px solid #00bfff50;
    border-radius:40px;
    margin-bottom:25px;
    color:#00bfff;
    background:#00bfff10;
    font-size:14px;
}

.hero h1{
    font-size:75px;
    line-height:85px;
    margin-bottom:25px;
    font-weight:800;
}

.gradient{
    background:linear-gradient(90deg,#00bfff,#7b2cff);
    -webkit-background-clip:text;
    -webkit-text-fill-color:transparent;
}

.hero p{
    color:#bdbdbd;
    line-height:32px;
    font-size:18px;
    margin-bottom:35px;
}

.buttons{
    display:flex;
    gap:20px;
    flex-wrap:wrap;
}

.btn{
    padding:18px 35px;
    border-radius:16px;
    text-decoration:none;
    transition:.4s;
    font-weight:600;
}

.btn-main{
    background:linear-gradient(90deg,#00bfff,#7b2cff);
    color:#fff;
}

.btn-main:hover{
    transform:translateY(-5px);
    box-shadow:0 0 35px #00bfff50;
}

.btn-outline{
    border:1px solid #ffffff20;
    color:#fff;
}

.btn-outline:hover{
    background:#ffffff10;
}

/* CARD */

.hero-right{
    position:relative;
}

.card{
    width:420px;
    background:#101010;
    border:1px solid #1f1f1f;
    border-radius:35px;
    overflow:hidden;
    box-shadow:0 0 50px #000;
    transform:rotate(4deg);
    transition:.5s;
}

.card:hover{
    transform:rotate(0deg) scale(1.03);
}

.card img{
    width:100%;
    height:500px;
    object-fit:cover;
}

.card-content{
    padding:30px;
}

.card-content h2{
    font-size:32px;
    margin-bottom:10px;
}

.card-content p{
    color:#b8b8b8;
}

.tech{
    display:flex;
    gap:15px;
    margin-top:25px;
    flex-wrap:wrap;
}

.tech span{
    padding:10px 18px;
    border-radius:12px;
    background:#191919;
    color:#00bfff;
    font-size:14px;
}

/* SECTION */

section{
    padding:120px 8%;
}

.title{
    font-size:55px;
    margin-bottom:60px;
}

.title span{
    color:#00bfff;
}

/* ABOUT */

.about-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.about-card{
    background:#101010;
    padding:40px;
    border-radius:30px;
    border:1px solid #1f1f1f;
    transition:.4s;
}

.about-card:hover{
    transform:translateY(-10px);
    border-color:#00bfff50;
}

.about-card h3{
    margin-bottom:20px;
    font-size:26px;
}

.about-card p{
    color:#b8b8b8;
    line-height:30px;
}

/* PROJECTS */

.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(330px,1fr));
    gap:30px;
}

.project{
    background:#101010;
    border-radius:30px;
    overflow:hidden;
    border:1px solid #1f1f1f;
    transition:.4s;
}

.project:hover{
    transform:translateY(-10px);
}

.project img{
    width:100%;
    height:220px;
    object-fit:cover;
}

.project-content{
    padding:30px;
}

.project-content h3{
    margin-bottom:15px;
    font-size:28px;
}

.project-content p{
    color:#b8b8b8;
    line-height:28px;
}

.project-buttons{
    display:flex;
    gap:15px;
    margin-top:25px;
}

/* STATS */

.stats{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
    gap:25px;
}

.stat{
    background:#101010;
    padding:40px;
    border-radius:25px;
    text-align:center;
    border:1px solid #1f1f1f;
}

.stat h2{
    font-size:55px;
    color:#00bfff;
}

.stat span{
    color:#bdbdbd;
}

/* SOCIAL */

.social{
    display:flex;
    justify-content:center;
    gap:25px;
    flex-wrap:wrap;
}

.social a{
    width:70px;
    height:70px;
    border-radius:20px;
    display:flex;
    align-items:center;
    justify-content:center;
    background:#101010;
    border:1px solid #1f1f1f;
    transition:.4s;
}

.social a:hover{
    transform:translateY(-10px);
    box-shadow:0 0 30px #00bfff40;
}

.social img{
    width:35px;
}

/* FOOTER */

footer{
    padding:60px;
    text-align:center;
    color:#8d8d8d;
}

/* RESPONSIVO */

@media(max-width:1000px){

.hero{
    flex-direction:column;
    text-align:center;
}

.hero h1{
    font-size:55px;
    line-height:65px;
}

.buttons{
    justify-content:center;
}

.card{
    width:100%;
}

nav ul{
    display:none;
}

.title{
    font-size:40px;
}

}

</style>
</head>

<body>

<div class="bg"></div>
<div class="blur"></div>
<div class="blur blur2"></div>

<!-- NAV -->

<nav>

<div class="logo">
Luan<span>.</span>
</div>

<ul>
<li><a href="#about">Sobre</a></li>
<li><a href="#projects">Projetos</a></li>
<li><a href="#stats">Estatísticas</a></li>
<li><a href="#contact">Contato</a></li>
</ul>

</nav>

<!-- HERO -->

<section class="hero">

<div class="hero-left">

<div class="badge">
🚀 Full Stack Developer
</div>

<h1>
Construindo o
<span class="gradient">
futuro digital
</span>
com experiências premium.
</h1>

<p>
Desenvolvedor Full Stack focado em aplicações modernas,
interfaces premium, experiências futuristas e sistemas escaláveis.
Especialista em React, Node.js e UI/UX de alto impacto.
</p>

<div class="buttons">

<a href="#projects" class="btn btn-main">
Ver Projetos
</a>

<a href="https://github.com/luanpereira-dev" class="btn btn-outline">
GitHub
</a>

</div>

</div>

<div class="hero-right">

<div class="card">

<img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?q=80&w=1200&auto=format&fit=crop" alt="">

<div class="card-content">

<h2>Luan Pereira</h2>

<p>
Full Stack Engineer • UI/UX Builder
</p>

<div class="tech">
<span>React</span>
<span>Node.js</span>
<span>JavaScript</span>
<span>UI/UX</span>
</div>

</div>

</div>

</div>

</section>

<!-- ABOUT -->

<section id="about">

<h2 class="title">
Sobre <span>Mim</span>
</h2>

<div class="about-grid">

<div class="about-card">
<h3>⚡ Minha Missão</h3>

<p>
Criar sistemas modernos, interfaces premium e aplicações
que entreguem experiências reais para usuários e empresas.
Meu foco é unir tecnologia, design e performance.
</p>
</div>

<div class="about-card">
<h3>🧠 Mentalidade</h3>

<p>
Construindo minha evolução diária como desenvolvedor Full Stack.
Aprendendo arquitetura escalável, APIs REST, bancos de dados
e engenharia de software moderna.
</p>
</div>

<div class="about-card">
<h3>🔥 Diferencial</h3>

<p>
Meu objetivo não é apenas programar.
É construir produtos digitais com identidade visual forte,
performance e experiência premium.
</p>
</div>

</div>

</section>

<!-- PROJECTS -->

<section id="projects">

<h2 class="title">
Projetos <span>Premium</span>
</h2>

<div class="projects">

<div class="project">

<img src="https://images.unsplash.com/photo-1588776814546-bb5cf5203b1d?q=80&w=1200&auto=format&fit=crop">

<div class="project-content">

<h3>Sistema Odontológico</h3>

<p>
Sistema premium com dashboard moderno,
agendamentos inteligentes, autenticação
e arquitetura Full Stack.
</p>

<div class="project-buttons">

<a href="#" class="btn btn-main">
Demo
</a>

<a href="#" class="btn btn-outline">
Código
</a>

</div>

</div>

</div>

<div class="project">

<img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?q=80&w=1200&auto=format&fit=crop">

<div class="project-content">

<h3>Sweet Snake Delivery</h3>

<p>
Landing page premium para delivery,
branding forte, experiência mobile
e estratégia visual de conversão.
</p>

<div class="project-buttons">

<a href="#" class="btn btn-main">
Demo
</a>

<a href="#" class="btn btn-outline">
Código
</a>

</div>

</div>

</div>

<div class="project">

<img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?q=80&w=1200&auto=format&fit=crop">

<div class="project-content">

<h3>Gabriela Art Unhas</h3>

<p>
Landing page moderna com identidade premium,
foco em branding, UX moderna
e conversão de clientes.
</p>

<div class="project-buttons">

<a href="#" class="btn btn-main">
Demo
</a>

<a href="#" class="btn btn-outline">
Código
</a>

</div>

</div>

</div>

</div>

</section>

<!-- STATS -->

<section id="stats">

<h2 class="title">
Minhas <span>Skills</span>
</h2>

<div class="stats">

<div class="stat">
<h2>95%</h2>
<span>Front-End</span>
</div>

<div class="stat">
<h2>85%</h2>
<span>UI/UX</span>
</div>

<div class="stat">
<h2>80%</h2>
<span>React</span>
</div>

<div class="stat">
<h2>70%</h2>
<span>Node.js</span>
</div>

</div>

</section>

<!-- SOCIAL -->

<section id="contact">

<h2 class="title">
Vamos <span>Conectar</span>
</h2>

<div class="social">

<a href="https://github.com/luanpereira-dev">
<img src="https://cdn-icons-png.flaticon.com/512/25/25231.png">
</a>

<a href="https://linkedin.com">
<img src="https://cdn-icons-png.flaticon.com/512/174/174857.png">
</a>

<a href="https://instagram.com">
<img src="https://cdn-icons-png.flaticon.com/512/2111/2111463.png">
</a>

<a href="https://youtube.com">
<img src="https://cdn-icons-png.flaticon.com/512/1384/1384060.png">
</a>

<a href="https://tiktok.com">
<img src="https://cdn-icons-png.flaticon.com/512/3046/3046121.png">
</a>

</div>

</section>

<footer>
© 2026 Luan Pereira • Full Stack Developer
</footer>

</body>
</html>