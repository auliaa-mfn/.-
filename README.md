<DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Aulia | Personal Portfolio</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;700;800&display=swap" rel="stylesheet">

<style>
:root{
    --bg:#F7F4ED;
    --yellow:#FFD84D;
    --blue:#66B8FF;
    --pink:#FF6FAF;
    --green:#7CF27C;
    --orange:#FF9D42;
    --white:#ffffff;
    --black:#111111;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:'Space Grotesk',sans-serif;
    background:var(--bg);
    color:var(--black);
}

section{
    width:min(1150px,92%);
    margin:auto;
    padding:70px 0;
}

h1,h2,h3{
    font-weight:800;
}

.neo{
    border:4px solid var(--black);
    box-shadow:8px 8px 0 var(--black);
}

.btn{
    display:inline-block;
    text-decoration:none;
    color:var(--black);
    background:var(--yellow);
    padding:14px 28px;
    border:4px solid var(--black);
    font-weight:800;
    box-shadow:6px 6px 0 var(--black);
    transition:.15s;
}

.btn:hover{
    transform:translate(-4px,-4px);
    box-shadow:10px 10px 0 var(--black);
}

nav{
    position:sticky;
    top:0;
    z-index:1000;
    background:var(--white);
    border-bottom:4px solid var(--black);
}

.nav-container{
    width:min(1150px,92%);
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:18px 0;
}

.logo{
    font-size:30px;
    font-weight:800;
}

nav ul{
    display:flex;
    list-style:none;
    gap:20px;
}

nav a{
    text-decoration:none;
    color:var(--black);
    font-weight:700;
}

.hero{
    display:grid;
    grid-template-columns:1.2fr .8fr;
    gap:40px;
    align-items:center;
}

.hero-left{
    background:var(--yellow);
    padding:40px;
}

.hero-left h1{
    font-size:clamp(48px,8vw,90px);
    line-height:.95;
    margin-bottom:20px;
}

.hero-left p{
    font-size:20px;
    margin-bottom:30px;
    font-weight:500;
}

.hero-right{
    background:var(--blue);
    padding:35px;
    text-align:center;
}

.avatar{
    width:180px;
    height:180px;
    margin:auto;
    border-radius:50%;
    background:var(--white);
    border:4px solid var(--black);
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:70px;
    font-weight:800;
    box-shadow:6px 6px 0 var(--black);
}

.hero-right h2{
    margin-top:25px;
    font-size:34px;
}

.title{
    display:inline-block;
    padding:12px 20px;
    background:var(--pink);
    border:4px solid var(--black);
    box-shadow:6px 6px 0 var(--black);
    margin-bottom:35px;
}

.about{
    background:var(--green);
    padding:35px;
}

.about p{
    font-size:18px;
    line-height:1.8;
}

.skills{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
    gap:20px;
}

.skill{
    background:var(--orange);
    padding:28px;
    text-align:center;
    cursor:pointer;
    transition:.15s;
}

.skill h3{
    margin-bottom:10px;
}

.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.project{
    background:var(--white);
    overflow:hidden;
    cursor:pointer;
    transition:.15s;
}

.thumb{
    height:180px;
    background:var(--yellow);
    border-bottom:4px solid var(--black);
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:65px;
}

.project-content{
    padding:25px;
}

.project h3{
    margin-bottom:10px;
}

.contact{
    background:var(--blue);
    padding:35px;
}

.contact-grid{
    margin-top:25px;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.item{
    background:var(--white);
    padding:20px;
    border:4px solid var(--black);
    box-shadow:5px 5px 0 var(--black);
}

footer{
    text-align:center;
    padding:30px;
    font-weight:700;
    border-top:4px solid var(--black);
}

@media(max-width:850px){

.hero{
    grid-template-columns:1fr;
}

nav ul{
    gap:12px;
    flex-wrap:wrap;
    justify-content:flex-end;
}

.hero-left{
    padding:30px;
}

.hero-right{
    padding:30px;
}

}

@media(max-width:600px){

nav .nav-container{
    flex-direction:column;
    gap:15px;
}

.hero-left h1{
    font-size:56px;
}

.hero-left p{
    font-size:18px;
}

.title{
    font-size:22px;
}

}
</style>
</head>

<body>

<nav>
<div class="nav-container">

<div class="logo">AULIA</div>

<ul>
<li><a href="#about">Tentang</a></li>
<li><a href="#skills">Skill</a></li>
<li><a href="#projects">Proyek</a></li>
<li><a href="#contact">Kontak</a></li>
</ul>

</div>
</nav>

<section class="hero">

<div class="hero-left neo">

<h1>Halo!<br>Saya<br>Aulia.</h1>

<p>
Seorang pengembang web yang senang menciptakan website modern,
responsif, dan memiliki karakter visual yang kuat dengan gaya
Neo-Brutalism.
</p>

<a href="#projects" class="btn">Lihat Portofolio</a>

</div>

<div class="hero-right neo">

<div class="avatar">A</div>

<h2>Creative Web Developer</h2>

<p>HTML • CSS • JavaScript</p>

</div>

</section>

<section id="about">

<h2 class="title">Tentang Saya</h2>

<div class="about neo">

<p>
Halo! Nama saya <strong>Aulia</strong>. Saya memiliki minat dalam
pengembangan website, UI sederhana, dan desain antarmuka yang unik.
Saya percaya bahwa website tidak hanya harus berfungsi dengan baik,
tetapi juga memiliki identitas visual yang menarik.
</p>

<br>

<p>
Saya terus belajar teknologi web modern dan senang membuat website
yang cepat, responsif, serta nyaman digunakan di berbagai perangkat.
</p>

</div>

</section>

<section id="skills">

<h2 class="title">Skill & Keahlian</h2>

<div class="skills">

<div class="skill neo">
<h3>HTML5</h3>
<p>Semantic Markup</p>
</div>

<div class="skill neo">
<h3>CSS3</h3>
<p>Responsive Design</p>
</div>

<div class="skill neo">
<h3>JavaScript</h3>
<p>Interactive UI</p>
</div>

<div class="skill neo">
<h3>UI Design</h3>
<p>Modern Layout</p>
</div>

<div class="skill neo">
<h3>Git</h3>
<p>Version Control</p>
</div>

<div class="skill neo">
<h3>Responsive</h3>
<p>Mobile First</p>
</div>

</div>

</section>

<section id="projects">

<h2 class="title">Proyek</h2>

<div class="projects">

<div class="project neo">

<div class="thumb">💻</div>

<div class="project-content">

<h3>Landing Page</h3>

<p>
Website promosi dengan tampilan modern dan cepat.
</p>

</div>

</div>

<div class="project neo">

<div class="thumb">📱</div>

<div class="project-content">

<h3>Portfolio Website</h3>

<p>
Website pribadi bergaya Neo-Brutalism yang responsif.
</p>

</div>

</div>

<div class="project neo">

<div class="thumb">🚀</div>

<div class="project-content">

<h3>Dashboard</h3>

<p>
Dashboard sederhana menggunakan HTML, CSS, dan JavaScript.
</p>

</div>

</div>

</div>

</section>

<section id="contact">

<h2 class="title">Kontak</h2>

<div class="contact neo">

<p>
Terima kasih telah mengunjungi portofolio saya.
Mari berkolaborasi untuk membuat sesuatu yang luar biasa!
</p>

<div class="contact-grid">

<div class="item">
<h3>Email</h3>
<p>aulia@email.com</p>
</div>

<div class="item">
<h3>Instagram</h3>
<p>@aulia.dev</p>
</div>

<div class="item">
<h3>GitHub</h3>
<p>github.com/aulia</p>
</div>

<div class="item">
<h3>Lokasi</h3>
<p>Indonesia</p>
</div>

</div>

</div>

</section>

<footer>
© 2026 Aulia • Dibuat menggunakan HTML, CSS & JavaScript
</footer>

<script>
// Efek interaktif kartu skill
document.querySelectorAll(".skill").forEach(card=>{

card.addEventListener("mouseenter",()=>{

card.style.transform="translate(-6px,-6px)";
card.style.boxShadow="14px 14px 0 #111";

});

card.addEventListener("mouseleave",()=>{

card.style.transform="translate(0,0)";
card.style.boxShadow="8px 8px 0 #111";

});

});

// Efek interaktif proyek
document.querySelectorAll(".project").forEach(card=>{

card.addEventListener("mouseenter",()=>{

card.style.transform="rotate(-1deg) scale(1.02)";
card.style.boxShadow="14px 14px 0 #111";

});

card.addEventListener("mouseleave",()=>{

card.style.transform="rotate(0deg) scale(1)";
card.style.boxShadow="8px 8px 0 #111";

});

});

// Efek klik tombol
document.querySelector(".btn").addEventListener("click",function(){

this.textContent="🚀 Terima Kasih!";

setTimeout(()=>{

this.textContent="Lihat Portofolio";

},1500);

});
</script>

</body>
</html>
