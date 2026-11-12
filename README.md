
<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#260B12">
<meta name="description" content="ProspectivaAI. Inteligência de mercado, prospecção estratégica e desenvolvimento de negócios para empresas que querem crescer.">
<title>ProspectivaAI | Inteligência de Mercado e Oportunidades</title>

<style>
:root {
  --red: #981F35;
  --red-light: #B52B43;
  --wine: #260B12;
  --wine2: #3A101C;
  --gold: #D6B66F;
  --white: #FFFFFF;
  --muted: #BDAEB1;
  --bg: #16090D;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html { scroll-behavior: smooth; }

body {
  font-family: Arial, Helvetica, sans-serif;
  background: var(--bg);
  color: var(--white);
  line-height: 1.6;
}

a {
  color: inherit;
  text-decoration: none;
}

.container {
  width: min(1120px, 90%);
  margin: auto;
}

header {
  background: rgba(38,11,18,.97);
  border-bottom: 1px solid rgba(214,182,111,.2);
  position: sticky;
  top: 0;
  z-index: 10;
}

.nav {
  min-height: 76px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
}

.logo {
  font-size: 25px;
  font-weight: 800;
  letter-spacing: 1px;
}

.logo span { color: var(--gold); }

nav {
  display: flex;
  gap: 25px;
  font-size: 14px;
  color: #E8DDE0;
}

nav a:hover { color: var(--gold); }

.hero {
  padding: 105px 0 95px;
  background:
    radial-gradient(ellipse at 80% 20%, rgba(152,31,53,.38), transparent 45%),
    linear-gradient(135deg, #260B12, #16090D 75%);
}

.tag {
  display: inline-block;
  border: 1px solid rgba(214,182,111,.5);
  color: var(--gold);
  padding: 7px 14px;
  border-radius: 30px;
  font-size: 12px;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  margin-bottom: 24px;
}

.hero h1 {
  font-size: clamp(38px, 6vw, 68px);
  line-height: 1.08;
  max-width: 850px;
  margin-bottom: 25px;
}

.hero h1 span { color: var(--gold); }

.hero p {
  color: #D2C3C6;
  max-width: 650px;
  font-size: 18px;
  margin-bottom: 32px;
}

.btn {
  display: inline-block;
  background: var(--red);
  color: white;
  padding: 14px 24px;
  border-radius: 5px;
  font-weight: bold;
  transition: .2s;
}

.btn:hover {
  background: var(--red-light);
  transform: translateY(-2px);
}

.btn-outline {
  background: transparent;
  border: 1px solid var(--gold);
  color: var(--gold);
  margin-left: 10px;
}

.btn-outline:hover {
  background: var(--gold);
  color: var(--wine);
}

section { padding: 82px 0; }

.section-title {
  text-align: center;
  max-width: 750px;
  margin: 0 auto 45px;
}

.section-title small {
  color: var(--gold);
  text-transform: uppercase;
  letter-spacing: 2px;
}

.section-title h2 {
  font-size: clamp(28px, 4vw, 40px);
  margin: 12px 0;
}

.section-title p { color: var(--muted); }

.services {
  background: #1D0B11;
}

.cards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
}

.card {
  background: linear-gradient(145deg, #35121D, #220B12);
  border: 1px solid rgba(214,182,111,.19);
  padding: 28px;
  border-radius: 9px;
  transition: .25s;
}

.card:hover {
  transform: translateY(-5px);
  border-color: var(--gold);
}

.card .number {
  color: var(--gold);
  font-size: 13px;
  letter-spacing: 2px;
}

.card h3 {
  font-size: 20px;
  margin: 14px 0;
}

.card p {
  color: var(--muted);
  font-size: 15px;
}

.sectors-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 14px;
}

.sector {
  padding: 20px 12px;
  text-align: center;
  background: #2A1018;
  border: 1px solid rgba(214,182,111,.15);
  border-radius: 7px;
  color: #E9DDE0;
}

.sector:hover {
  border-color: var(--gold);
  color: var(--gold);
}

.method {
  background: linear-gradient(120deg, #3A101C, #1A090E);
}

.steps {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 22px;
}

.step {
  border-top: 2px solid var(--gold);
  padding-top: 20px;
}

.step strong {
  color: var(--gold);
  font-size: 27px;
}

.step h3 { margin: 10px 0; }

.step p {
  color: var(--muted);
  font-size: 14px;
}

.about {
  background: #1D0B11;
}

.about-content {
  max-width: 820px;
  margin: auto;
  text-align: center;
}

.about-content p {
  color: #D2C3C6;
  margin-top: 15px;
}

.contact {
  background:
    radial-gradient(ellipse at center, rgba(152,31,53,.32), transparent 65%),
    #200A11;
  text-align: center;
}

.contact h2 {
  font-size: clamp(30px, 5vw, 45px);
  margin-bottom: 15px;
}

.contact p {
  color: var(--muted);
  margin-bottom: 28px;
}

footer {
  border-top: 1px solid rgba(214,182,111,.2);
  padding: 27px 0;
  text-align: center;
  color: #A9959A;
  font-size: 13px;
}

footer span { color: var(--gold); }

@media(max-width: 800px) {
  .cards { grid-template-columns: repeat(2, 1fr); }
  .steps { grid-template-columns: repeat(2, 1fr); }
  .sectors-grid { grid-template-columns: repeat(2, 1fr); }
  nav { gap: 12px; font-size: 12px; }
}

@media(max-width: 560px) {
  .nav {
    flex-direction: column;
    padding: 15px 0;
  }
  nav {
    flex-wrap: wrap;
    justify-content: center;
  }
  .hero { padding: 75px 0; }
  .cards, .steps { grid-template-columns: 1fr; }
  .btn { display: block; text-align: center; margin: 10px 0; }
  .btn-outline { margin-left: 0; }
  section { padding: 65px 0; }
}
</style>
</head>

<body>

<header>
  <div class="container nav">
    <a href="#" class="logo">PROSPECTIVA<span>AI</span></a>
    <nav>
      <a href="#inicio">Início</a>
      <a href="#servicos">Soluções</a>
      <a href="#setores">Setores</a>
      <a href="#metodo">Método</a>
      <a href="#contato">Contato</a>
    </nav>
  </div>
</header>

<main>

<section class="hero" id="inicio">
  <div class="container">
    <span class="tag">Estratégia • Mercado • Expansão</span>
    <h1>Enxergue oportunidades que seus <span>concorrentes ainda não perceberam.</span></h1>
    <p>
      Identificamos oportunidades de mercado, novos clientes,
      parceiros estratégicos e caminhos de expansão para
      empresas que desejam crescer com inteligência e direção.
    </p>
    <a class="btn" href="#contato">Descubra novas oportunidades</a>
    <a class="btn btn-outline" href="#servicos">Conheça nossas soluções</a>
  </div>
</section>

<section class="services" id="servicos">
  <div class="container">
    <div class="section-title">
      <small>Nossas soluções</small>
      <h2>Informação estratégica que gera oportunidades.</h2>
      <p>
        Transformamos informações de mercado em caminhos
        concretos para desenvolvimento comercial e crescimento.
      </p>
    </div>

    <div class="cards">

      <article class="card">
        <span class="number">01 / MERCADO</span>
        <h3>Radar de Mercado</h3>
        <p>
          Análise de segmentos, regiões, tendências,
          concorrentes e oportunidades de posicionamento.
        </p>
      </article>

      <article class="card">
        <span class="number">02 / PROSPECÇÃO</span>
        <h3>Radar de Oportunidades</h3>
        <p>
          Identificação e organização de potenciais clientes,
          distribuidores, representantes e parceiros comerciais.
        </p>
      </article>

      <article class="card">
        <span class="number">03 / EXPANSÃO</span>
        <h3>Expansão Comercial</h3>
        <p>
          Mapeamento de novos territórios, canais de venda
          e possibilidades de desenvolvimento de negócios.
        </p>
      </article>

      <article class="card">
        <span class="number">04 / ESTRATÉGIA</span>
        <h3>Inteligência Competitiva</h3>
        <p>
          Estudos sobre posicionamento, movimentações do setor
          e oportunidades para fortalecer sua competitividade.
        </p>
      </article>

      <article class="card">
        <span class="number">05 / ANÁLISE</span>
        <h3>Estudos Estratégicos</h3>
        <p>
          Relatórios e análises para apoiar decisões comerciais,
          investimentos e planejamento de expansão.
        </p>
      </article>

      <article class="card">
        <span class="number">06 / NEGÓCIOS</span>
        <h3>Desenvolvimento de Negócios</h3>
        <p>
          Aproximação entre empresas, identificação de sinergias
          e construção de novas oportunidades comerciais.
        </p>
      </article>

    </div>
  </div>
</section>

<section id="setores">
  <div class="container">
    <div class="section-title">
      <small>Áreas de atuação</small>
      <h2>Conhecimento aplicado a diferentes mercados.</h2>
      <p>
        Atuamos na identificação de oportunidades em setores
        com potencial de crescimento e desenvolvimento.
      </p>
    </div>

    <div class="sectors-grid">
      <div class="sector">Energia Solar</div>
      <div class="sector">Armazenamento de Energia</div>
      <div class="sector">Telecomunicações</div>
      <div class="sector">Tecnologia</div>
      <div class="sector">Segurança Eletrônica</div>
      <div class="sector">Mobilidade Elétrica</div>
      <div class="sector">Indústria</div>
      <div class="sector">Novos Mercados</div>
    </div>
  </div>
</section>

<section class="method" id="metodo">
  <div class="container">
    <div class="section-title">
      <small>Nossa metodologia</small>
      <h2>Da informação à oportunidade.</h2>
      <p>
        Um processo estruturado para transformar conhecimento
        de mercado em decisões e ações comerciais.
      </p>
    </div>

    <div class="steps">
      <div class="step">
        <strong>01</strong>
        <h3>Entender</h3>
        <p>Compreendemos o negócio, os objetivos e os desafios da empresa.</p>
      </div>

      <div class="step">
        <strong>02</strong>
        <h3>Investigar</h3>
        <p>Mapeamos o mercado, os agentes envolvidos e as oportunidades.</p>
      </div>

      <div class="step">
        <strong>03</strong>
        <h3>Identificar</h3>
        <p>Organizamos informações e priorizamos caminhos estratégicos.</p>
      </div>

      <div class="step">
        <strong>04</strong>
        <h3>Direcionar</h3>
        <p>Apresentamos recomendações para apoiar a ação comercial.</p>
      </div>
    </div>
  </div>
</section>

<section class="about">
  <div class="container about-content">
    <div class="section-title">
      <small>Sobre a ProspectivaAI</small>
      <h2>Antecipar oportunidades é uma vantagem competitiva.</h2>
    </div>

    <p>
      A ProspectivaAI é uma iniciativa dedicada à inteligência
      de mercado, prospecção estratégica e desenvolvimento
      de negócios.
    </p>

    <p>
      Nosso trabalho conecta informações, visão comercial
      e análise estratégica para ajudar empresas a identificar
      oportunidades, fortalecer relacionamentos e explorar
      novos caminhos de crescimento.
    </p>
  </div>
</section>

<section class="contact" id="contato">
  <div class="container">
    <span class="tag">Vamos conversar</span>
    <h2>O próximo grande negócio pode estar mais perto do que você imagina.</h2>
    <p>
      Conte-nos sobre sua empresa e seus objetivos.
      Vamos identificar caminhos para novas oportunidades.
    </p>

    <a class="btn"
       href="https://wa.me/5511994793854?text=Olá!%20Gostaria%20de%20conhecer%20as%20soluções%20da%20ProspectivaAI."
       target="_blank" rel="noopener noreferrer">
       Fale com a ProspectivaAI
    </a>
  </div>
</section>

</main>

<footer>
  <div class="container">
    <div class="logo">PROSPECTIVA<span>AI</span></div>
    <p>Inteligência para encontrar oportunidades antes dos seus concorrentes.</p>
    <p>© 2026 ProspectivaAI. Todos os direitos reservados.</p>
  </div>
</footer>

</body>
</html>
# index.html
