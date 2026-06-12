<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Agro Forte Sustentável | O Futuro do Agro Brasileiro</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

:root{
    --verde:#1b5e20;
    --verde-claro:#4caf50;
    --verde-neon:#7cff6b;
    --escuro:#081c15;
    --cinza:#f5f7f6;
    --texto:#2d3436;
    --branco:#ffffff;
}

html{
    scroll-behavior:smooth;
}

body{
    background:var(--cinza);
    color:var(--texto);
    overflow-x:hidden;
}

/* HEADER */

header{
    position:fixed;
    top:0;
    width:100%;
    z-index:999;
    backdrop-filter:blur(20px);
    background:rgba(255,255,255,.85);
    border-bottom:1px solid rgba(0,0,0,.08);
}

.nav{
    max-width:1300px;
    margin:auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:18px 30px;
}

.logo{
    font-size:1.6rem;
    font-weight:800;
    color:var(--verde);
}

.logo span{
    color:var(--verde-claro);
}

.nav-links{
    display:flex;
    gap:30px;
}

.nav-links a{
    text-decoration:none;
    color:#222;
    font-weight:500;
    transition:.3s;
}

.nav-links a:hover{
    color:var(--verde);
}

/* HERO */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    background:
    linear-gradient(rgba(0,0,0,.55),rgba(0,0,0,.55)),
    url('https://images.unsplash.com/photo-1500937386664-56d1dfef3854?q=80&w=1920');
    background-size:cover;
    background-position:center;
    text-align:center;
    color:white;
    padding:120px 20px 80px;
}

.hero-content{
    max-width:900px;
}

.hero h1{
    font-size:4rem;
    font-weight:800;
    margin-bottom:20px;
    line-height:1.1;
}

.hero p{
    font-size:1.2rem;
    margin-bottom:35px;
    opacity:.9;
}

.btn{
    display:inline-block;
    padding:16px 35px;
    background:linear-gradient(45deg,var(--verde),var(--verde-claro));
    color:white;
    text-decoration:none;
    border-radius:50px;
    font-weight:600;
    transition:.4s;
    box-shadow:0 10px 25px rgba(0,0,0,.2);
}

.btn:hover{
    transform:translateY(-5px);
}

/* STATS */

.stats{
    max-width:1200px;
    margin:-80px auto 80px;
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
    padding:0 20px;
}

.stat-card{
    background:white;
    border-radius:20px;
    padding:30px;
    text-align:center;
    box-shadow:0 10px 30px rgba(0,0,0,.08);
}

.stat-card h2{
    color:var(--verde);
    font-size:2.3rem;
}

.stat-card p{
    margin-top:10px;
}

/* SECTION */

section{
    padding:90px 8%;
}

.section-title{
    text-align:center;
    margin-bottom:60px;
}

.section-title h2{
    font-size:2.8rem;
    color:var(--escuro);
}

.section-title p{
    margin-top:10px;
    color:#666;
}

/* SOBRE */

.about{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.about img{
    width:100%;
    border-radius:25px;
    box-shadow:0 15px 35px rgba(0,0,0,.15);
}

.about-text h3{
    font-size:2rem;
    color:var(--verde);
    margin-bottom:20px;
}

.about-text p{
    line-height:1.8;
    margin-bottom:15px;
}

/* CULTURAS */

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.card{
    background:white;
    border-radius:25px;
    overflow:hidden;
    box-shadow:0 15px 35px rgba(0,0,0,.08);
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
}

.card img{
    width:100%;
    height:230px;
    object-fit:cover;
}

.card-content{
    padding:25px;
}

.card-content h3{
    color:var(--verde);
    margin-bottom:10px;
}

/* SUSTENTABILIDADE */

.sustentabilidade{
    background:linear-gradient(135deg,#0b3d0b,#1b5e20);
    color:white;
}

.features{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:25px;
}

.feature{
    background:rgba(255,255,255,.08);
    backdrop-filter:blur(15px);
    padding:30px;
    border-radius:20px;
}

.feature h3{
    margin-bottom:15px;
}

/* TIMELINE */

.timeline{
    position:relative;
    max-width:1000px;
    margin:auto;
}

.timeline::before{
    content:'';
    position:absolute;
    left:50%;
    width:4px;
    height:100%;
    background:var(--verde);
    transform:translateX(-50%);
}

.event{
    width:50%;
    padding:25px;
    position:relative;
}

.event:nth-child(odd){
    left:0;
    text-align:right;
}

.event:nth-child(even){
    left:50%;
}

.box{
    background:white;
    padding:25px;
    border-radius:18px;
    box-shadow:0 10px 25px rgba(0,0,0,.08);
}

/* CTA */

.cta{
    background:linear-gradient(135deg,var(--verde),#2e7d32);
    color:white;
    text-align:center;
}

.cta h2{
    font-size:3rem;
    margin-bottom:20px;
}

/* FOOTER */

footer{
    background:#06110c;
    color:white;
    text-align:center;
    padding:40px 20px;
}

footer p{
    opacity:.8;
}

/* RESPONSIVO */

@media(max-width:900px){

.hero h1{
    font-size:2.8rem;
}

.about{
    grid-template-columns:1fr;
}

.timeline::before{
    left:20px;
}

.event,
.event:nth-child(even),
.event:nth-child(odd){
    width:100%;
    left:0;
    text-align:left;
    padding-left:60px;
}

.nav-links{
    display:none;
}

}

</style>
</head>
<body>

<header>
    <nav class="nav">
        <div class="logo">Agro<span>Forte</span></div>

        <div class="nav-links">
            <a href="#inicio">Início</a>
            <a href="#agro">Agro Brasil</a>
            <a href="#culturas">Culturas</a>
            <a href="#sustentavel">Sustentabilidade</a>
        </div>
    </nav>
</header>

<section class="hero" id="inicio">
    <div class="hero-content">
        <h1>Agro Forte Sustentável</h1>
        <p>
            Tecnologia, produtividade e preservação ambiental caminhando juntas para construir o futuro do agronegócio brasileiro.
        </p>

        <a href="#agro" class="btn">Explorar o Agro</a>
    </div>
</section>

<div class="stats">

    <div class="stat-card">
        <h2>27%</h2>
        <p>Participação aproximada na economia nacional.</p>
    </div>

    <div class="stat-card">
        <h2>+200</h2>
        <p>Países recebem produtos brasileiros.</p>
    </div>

    <div class="stat-card">
        <h2>5M+</h2>
        <p>Empregos gerados pelo setor.</p>
    </div>

    <div class="stat-card">
        <h2>100%</h2>
        <p>Compromisso com a sustentabilidade.</p>
    </div>

</div>

<section id="agro">

    <div class="section-title">
        <h2>O Agro no Brasil</h2>
        <p>Uma potência mundial na produção de alimentos.</p>
    </div>

    <div class="about">

        <img src="https://images.unsplash.com/photo-1500382017468-9049fed747ef?q=80&w=1200">

        <div class="about-text">
            <h3>Força que Alimenta o Mundo</h3>

            <p>
                O Brasil é reconhecido internacionalmente como uma das maiores potências agrícolas do planeta. O agronegócio brasileiro combina inovação tecnológica, pesquisa científica e eficiência produtiva para atender mercados nacionais e internacionais.
            </p>

            <p>
                Com diversidade climática e vastas áreas produtivas, o país lidera a produção de diversas culturas agrícolas, contribuindo significativamente para a segurança alimentar global.
            </p>

            <p>
                Além da produtividade, o setor investe cada vez mais em práticas sustentáveis, agricultura de precisão e preservação ambiental.
            </p>
        </div>

    </div>

</section>

<section id="culturas">

    <div class="section-title">
        <h2>Principais Culturas</h2>
        <p>Produtos que destacam o Brasil no cenário mundial.</p>
    </div>

    <div class="cards">

        <div class="card">
            <img src="https://images.unsplash.com/photo-1447933601403-0c6688de566e?q=80&w=1200">
            <div class="card-content">
                <h3>☕ Café</h3>
                <p>
                    O Brasil é um dos maiores produtores e exportadores de café do mundo, reconhecido pela qualidade e diversidade de seus grãos.
                </p>
            </div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1464965911861-746a04b4bca6?q=80&w=1200">
            <div class="card-content">
                <h3>🍓 Morango</h3>
                <p>
                    Cultivado em diversas regiões do país, o morango se destaca pelo sabor, qualidade e crescente demanda do mercado.
                </p>
            </div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1592841200221-a6898f307baa?q=80&w=1200">
            <div class="card-content">
                <h3>🌱 Soja</h3>
                <p>
                    A soja é um dos principais motores da economia agrícola brasileira e líder nas exportações.
                </p>
            </div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1631301254694-cf9a79c6fbea?q=80&w=1200">
            <div class="card-content">
                <h3>🌽 Milho</h3>
                <p>
                    Essencial para a alimentação humana, animal e para a indústria, o milho possui enorme importância econômica.
                </p>
            </div>
        </div>

    </div>

</section>

<section class="sustentabilidade" id="sustentavel">

    <div class="section-title">
        <h2 style="color:white;">Sustentabilidade no Campo</h2>
        <p style="color:#d8ffd8;">
            Produzir mais preservando recursos naturais.
        </p>
    </div>

    <div class="features">

        <div class="feature">
            <h3>🌿 Agricultura de Precisão</h3>
            <p>
                Uso de sensores, drones e inteligência de dados para otimizar recursos.
            </p>
        </div>

        <div class="feature">
            <h3>💧 Uso Inteligente da Água</h3>
            <p>
                Sistemas modernos de irrigação reduzem desperdícios e aumentam a eficiência.
            </p>
        </div>

        <div class="feature">
            <h3>♻️ Preservação Ambiental</h3>
            <p>
                Conservação de matas, nascentes e biodiversidade nas propriedades rurais.
            </p>
        </div>

        <div class="feature">
            <h3>🚜 Tecnologia Rural</h3>
            <p>
                Máquinas modernas e automação elevam produtividade e sustentabilidade.
            </p>
        </div>

    </div>

</section>

<section>

    <div class="section-title">
        <h2>Evolução do Agro Brasileiro</h2>
    </div>

    <div class="timeline">

        <div class="event">
            <div class="box">
                <h3>1970</h3>
                <p>Modernização das técnicas agrícolas.</p>
            </div>
        </div>

        <div class="event">
            <div class="box">
                <h3>1990</h3>
                <p>Expansão da exportação para novos mercados.</p>
            </div>
        </div>

        <div class="event">
            <div class="box">
                <h3>2010</h3>
                <p>Agricultura digital e mecanização avançada.</p>
            </div>
        </div>

        <div class="event">
            <div class="box">
                <h3>2025+</h3>
                <p>Inteligência artificial, sustentabilidade e produção inteligente.</p>
            </div>
        </div>

    </div>

</section>

<section class="cta">

    <h2>O Futuro é Verde. O Futuro é Agro.</h2>

    <p style="max-width:700px;margin:auto;margin-bottom:30px;">
        Investir em inovação, sustentabilidade e tecnologia é garantir alimento, desenvolvimento e prosperidade para as próximas gerações.
    </p>

    <a href="#" class="btn">Saiba Mais</a>

</section>

<footer>
    <h3>Agro Forte Sustentável</h3>
    <br>
    <p>© 2026 - Projeto demonstrativo para agronegócio sustentável.</p>
</footer>

</body>
</html>
