<template>
  <div id="app">
    <header class="navbar">
      <nav>
        <a href="#home" class="logo"></a>

        <button class="hamburger-menu" @click="toggleMobileMenu">
          <span :class="{ 'line': true, 'line-1': true, 'menu-open': isMenuOpen }"></span>
          <span :class="{ 'line': true, 'line-2': true, 'menu-open': isMenuOpen }"></span>
          <span :class="{ 'line': true, 'line-3': true, 'menu-open': isMenuOpen }"></span>
        </button>

        <ul :class="['nav-links', { 'menu-open': isMenuOpen }]">
          <li><a href="#especializacao" @click="closeMobileMenu">Especialização</a></li>
          <li><a href="#quem-atendemos" @click="closeMobileMenu">Quem Atendemos</a></li>
          <li><a href="#sobre-nos" @click="closeMobileMenu">Sobre Nós</a></li>
          <li><a href="#contato" @click="closeMobileMenu">Contato</a></li>
        </ul>
      </nav>
    </header>

    <section id="home" class="hero">
      <div class="hero-content">
        <div class="hero-text-container">
          <h1>Defesa Jurídica Especializada para Profissionais de Saúde</h1>
          <p>Oferecemos assessoria jurídica estratégica e humanizada, com foco na defesa dos direitos de médicos, dentistas e enfermeiros. Nossa missão é garantir que você tenha o suporte necessário para navegar com segurança pelo complexo universo médico-legal, protegendo sua carreira e sua reputação.</p>
          <a href="#contato" class="btn-contato">Entre em Contato</a>
        </div>
        <img src="../assets/ise.png" alt="Foto da Advogada" class="advogada-photo">
      </div>
    </section>

    <section id="especializacao" class="section">
      <h2>Nossa Especialização</h2>
      <p class="section-description">Atuamos exclusivamente em causas relacionadas aos direitos médicos e da saúde, oferecendo suporte jurídico abrangente para <span class="highlight">profissionais como você</span>, em diversas áreas, tais como:</p>
      <ul class="specialization-list">
        <li>
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <line x1="12" y1="5" x2="12" y2="19"></line>
              <line x1="5" y1="12" x2="19" y2="12"></line>
            </svg>
          </div>
          <h3>Defesa em processos éticos e administrativos</h3>
          <p>Suporte jurídico em processos administrativos e éticos junto aos conselhos de medicina, odontologia e enfermagem.</p>
        </li>
        <li>
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <line x1="12" y1="1" x2="12" y2="23"></line>
              <path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"></path>
            </svg>
          </div>
          <h3>Responsabilidade civil e erro profissional</h3>
          <p>Defesa de médicos, dentistas e enfermeiros em processos de responsabilidade civil decorrentes de supostos erros.</p>
        </li>
        <li>
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <circle cx="12" cy="7" r="4"></circle>
              <path d="M2 21v-2a4 4 0 0 1 4-4h12a4 4 0 0 1 4 4v2"></path>
            </svg>
          </div>
          <h3>Contratos e consultoria preventiva</h3>
          <p>Elaboração e revisão de contratos, e consultoria para evitar litígios na prática profissional.</p>
        </li>
        <li>
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <circle cx="12" cy="12" r="10"></circle>
              <line x1="4.93" y1="4.93" x2="19.07" y2="19.07"></line>
            </svg>
          </div>
          <h3>Questões regulatórias e sanitárias</h3>
          <p>Assessoria em conformidade com normas da ANS, ANVISA e outras regulamentações do setor de saúde.</p>
        </li>
        <li>
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                  <path d="M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
                  <circle cx="8.5" cy="7" r="4"></circle>
                  <line x1="18" y1="10" x2="18" y2="16"></line>
                  <line x1="15" y1="13" x2="21" y2="13"></line>
                </svg>
          </div>
          <h3>Processos judiciais cíveis e criminais</h3>
          <p>Defesa em ações que envolvam a prática profissional, garantindo seus direitos e minimizando riscos.</p>
        </li>
        <li>
          <div class="card-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                  <path d="M14 9V5a3 3 0 0 0-3-3l-4 9v11h11a3 3 0 0 0 3-3V9h-3z"></path>
                  <path d="M4 15V9a3 3 0 0 1 3-3h10a3 3 0 0 1 3 3v6"></path>
                  <line x1="8" y1="21" x2="8" y2="15"></line>
                  <line x1="16" y1="21" x2="16" y2="15"></line>
                </svg>
          </div>
          <h3>Defesa de honorários e questões financeiras</h3>
          <p>Suporte jurídico para cobrança de honorários e resolução de pendências financeiras.</p>
        </li>
      </ul>
    </section>

    <section id="quem-atendemos" class="section">
      <h2>Quem Atendemos</h2>
      <p class="section-description">Nossa atuação é focada em oferecer suporte jurídico especializado para:</p>
      <ul class="who-we-serve-list">
        <li>
          <div class="list-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
              <circle cx="9" cy="7" r="4"></circle>
              <path d="M23 21v-2a4 4 0 0 0-3-3.87"></path>
              <circle cx="16" cy="7" r="4"></circle>
            </svg>
          </div>
          <p><strong>Médicos e Cirurgiões:</strong> Em todas as especialidades, necessitando de defesa em processos éticos, cíveis ou criminais.</p>
        </li>
        <li>
          <div class="list-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M16 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"></path>
              <circle cx="8.5" cy="7" r="4"></circle>
              <line x1="18" y1="8" x2="23" y2="13"></line>
              <line x1="23" y1="8" x2="18" y2="13"></line>
            </svg>
          </div>
          <p><strong>Dentistas e Odontólogos:</strong> Oferecendo suporte em questões de responsabilidade profissional e regulatórias.</p>
        </li>
        <li>
          <div class="list-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <path d="M2 3a2 2 0 0 1 2-2h16a2 2 0 0 1 2 2v18a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V3z"></path>
              <polyline points="3 7 12 13 21 7"></polyline>
              <polyline points="21 21 12 15 3 21"></polyline>
            </svg>
          </div>
          <p><strong>Enfermeiros e Equipe de Enfermagem:</strong> Auxiliando na defesa de direitos e em processos disciplinares.</p>
        </li>
        <li>
          <div class="list-icon">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
              <polyline points="22 12 16 12 14 15 10 15 8 12 2 12"></polyline><path d="M5.45 5.11L2 12v6a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2v-6l-3.45-6.89A2 2 0 0 0 16.76 4H7.24a2 2 0 0 0-1.79 1.11z"></path>
            </svg>
          </div>
          <p><strong>Clínicas e Consultórios:</strong> Buscando assessoria jurídica preventiva e contenciosa para a instituição.</p>
        </li>
      </ul>
    </section>

    <section id="sobre-nos" class="section">
      <div class="sobre-nos-content">
        <img src="../assets/ise.png" alt="Foto da Advogada" class="advogada-photo-small">
        <div class="text-content">
          <h2>Sobre Nós</h2>
          <p>Com anos de experiência e um profundo conhecimento da legislação em saúde, nossa missão é garantir que os direitos de médicos, dentistas e enfermeiros sejam defendidos com rigor e excelência. Nosso compromisso é com a <span class="highlight">justiça e a proteção dos interesses</span> daqueles que nos confiam suas carreiras.</p>
          <p>Nossa fundadora, [Nome da Advogada], é uma advogada dedicada e apaixonada por direitos médicos, reconhecida por sua atuação ética e resultados consistentes na defesa de profissionais da saúde.</p>
        </div>
      </div>
    </section>

    <section id="contato" class="section">
      <h2>Entre em Contato</h2>
      <p class="section-description">Estamos prontos para defender sua carreira. Clique no botão abaixo para falar diretamente conosco:</p>
      
      <div class="contact-button-container">
        <a href="#" target="_blank" class="btn-contato">Fale Conosco</a> 
      </div>

      <div class="contact-info-container">
        <p class="contact-info">Telefone: (XX) XXXX-XXXX</p>
        <p class="contact-info">Email: contato@defesasaude.com.br</p> 
        <p class="contact-info">Endereço: Rua [Nome da Rua], [Número], [Bairro], [Cidade] - [Estado]</p>
      </div>
    </section>

    <footer class="footer">
      <p>&copy; {{ new Date().getFullYear() }} Advocacia de Direitos Médicos. Todos os direitos reservados.</p>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      isMenuOpen: false, // Controla o estado do menu hambúrguer
    };
  },
  methods: {
    toggleMobileMenu() {
      this.isMenuOpen = !this.isMenuOpen;
      // Opcional: Impedir scroll do body quando o menu está aberto
      if (this.isMenuOpen) {
        document.body.style.overflow = 'hidden';
      } else {
        document.body.style.overflow = '';
      }
    },
    closeMobileMenu() {
      // Fecha o menu ao clicar em um item (opcional, mas melhora a UX)
      this.isMenuOpen = false;
      document.body.style.overflow = ''; // Permite scroll novamente
    },
  },
};
</script>

<style>
/* Estilos globais */
:root {
  --cor-fundo-escuro: #1A1A1A; /* Quase preto */
  --cor-texto-claro: #E0E0E0; /* Cinza claro para texto */
  --cor-destaque: #CDA454; /* Novo: Bronze/Dourado mais discreto */
  --cor-borda: #333; /* Um cinza um pouco mais claro para bordas e divisores */
  --cor-hover-sombra: rgba(0, 0, 0, 0.4); /* Sombra escura para o hover */
}

html, body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: var(--cor-fundo-escuro);
  color: var(--cor-texto-claro);
  line-height: 1.6; /* Levemente ajustado para melhor leitura */
  scroll-behavior: smooth;
}

h1,
h2,
h3 {
  color: var(--cor-destaque);
  text-align: center;
  margin-bottom: 25px;
}

h2 {
  font-size: 2em;
}

h3 {
  font-size: 1.6em;
}

p {
  margin-bottom: 15px;
}

.section-description {
  color: #A0A0A0;
  margin-bottom: 25px;
  text-align: center;
}

a {
  text-decoration: none;
  color: var(--cor-destaque);
  transition: color 0.3s ease;
}


/* Navbar */
.navbar {
  background-color: var(--cor-fundo-escuro);
  padding: 15px 0;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.5);
  position: fixed;
  width: 100%;
  z-index: 1000;
  display: flex;
  justify-content: center;
}

.navbar nav {
  display: flex;
  justify-content: center;
  align-items: center;
  max-width: 1100px;
  margin: 0 auto;
  padding: 0 20px;
  width: 100%; /* Garante que a nav ocupe a largura máxima permitida */
}
/* Menu de navegação (desktop) */
.nav-links {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex; /* Visível por padrão em desktop */
}

.nav-links li {
  margin-left: 30px;
}

.nav-links li a {
  color: var(--cor-texto-claro);
  font-weight: bold;
  transition: color 0.3s ease;
}

.nav-links li a:hover {
  color: var(--cor-destaque);
}

/* Estilos para o Botão Hamburguer CSS */
.hamburger-menu {
  /* Escondido por padrão em desktop */
  display: none; 
  background: none;
  border: none;
  width: 30px; /* Largura do botão */
  height: 25px; /* Altura do botão */
  position: relative;
  cursor: pointer;
  z-index: 1001;
  padding: 0;
  flex-direction: column;
  justify-content: space-between; /* Espaça as linhas */
  align-items: center; /* Centraliza as linhas */
}

.hamburger-menu .line {
  display: block;
  width: 100%;
  height: 3px; /* Espessura da linha */
  background-color: var(--cor-texto-claro); /* Cor das linhas */
  border-radius: 2px;
  transition: all 0.3s ease-in-out; /* Transição para a animação */
}

/* Animação do X */
.hamburger-menu .line-1.menu-open {
  transform: translateY(11px) rotate(45deg); /* Move para o centro e gira */
}

.hamburger-menu .line-2.menu-open {
  opacity: 0; /* Esconde a linha do meio */
}

.hamburger-menu .line-3.menu-open {
  transform: translateY(-11px) rotate(-45deg); /* Move para o centro e gira */
}

/* Seções */
.section {
  padding: 80px 20px;
  max-width: 1000px;
  margin: 0 auto;
  text-align: center;
  border-bottom: 1px solid var(--cor-borda);
}

.section:last-of-type {
  border-bottom: none;
}

.section ul {
  list-style: none;
  padding: 0;
  margin-top: 25px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

/* === ESTILOS DA SEÇÃO DE ESPECIALIZAÇÃO MELHORADOS === */
.specialization-list li {
  background-color: #282828;
  padding: 30px 25px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
  font-weight: 500;
  text-align: center;
  transition: transform 0.3s ease, background-color 0.3s ease;
  flex-basis: calc(33.333% - 40px);
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  min-height: 220px;
}

.specialization-list li::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 5%;
  background-color: transparent;
  transition: background-color 0.6s ease;
  z-index: 1;
}

.specialization-list li:hover {
  transform: translateY(-10px);
}

.specialization-list li:hover::before {
  background-color: var(--cor-destaque);
}

.specialization-list li h3 {
  font-size: 1.3em;
  margin-top: 15px;
  margin-bottom: 10px;
  color: var(--cor-destaque);
}

.specialization-list li p {
  font-size: 0.95em;
  color: #B0B0B0;
  line-height: 1.4;
}

.card-icon {
  width: 48px; /* Tamanho fixo para o SVG */
  height: 48px; /* Tamanho fixo para o SVG */
  color: var(--cor-destaque); /* A cor de preenchimento do SVG */
  margin-bottom: 10px;
  transition: transform 0.3s ease;
  display: flex; /* Centralizar o SVG dentro do div */
  align-items: center;
  justify-content: center;
}

/* Garante que o SVG dentro do container use a cor definida e tenha tamanho */
.card-icon svg {
  width: 60%; /* Ajuste o tamanho do ícone dentro do container */
  height: 60%; /* Ajuste o tamanho do ícone dentro do container */
  fill: currentColor; /* Para SVGs com fill */
  stroke: currentColor; /* Para SVGs com stroke */
  stroke-width: 2; /* Mantém a largura do traço para ícones de linha */
}

.specialization-list li:hover .card-icon {
  transform: scale(1.1);
}

/* Estilos para a seção "Quem Atendemos" */
.who-we-serve-list li {
  background-color: #282828;
  padding: 15px 25px; /* Reduzi um pouco o padding vertical */
  border-radius: 8px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
  font-weight: 500;
  transition: transform 0.3s ease, background-color 0.3s ease;
  flex-basis: calc(33.333% - 40px); /* Mantido para 3 colunas em desktop */
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  display: flex; /* Torna o item da lista um container flex */
  flex-direction: column; /* Coloca o ícone e o texto em coluna */
  align-items: center; /* Centraliza o ícone e o texto horizontalmente no card */
  gap: 10px; /* Espaço entre o ícone e o texto */
}

.who-we-serve-list li::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 5%;
  background-color: transparent;
  transition: background-color 0.6s ease;
  z-index: 1;
}

.who-we-serve-list li:hover {
  transform: translateY(-8px);
}

.who-we-serve-list li:hover::before {
  background-color: var(--cor-destaque);
}

.list-icon {
  width: 32px; /* Tamanho do ícone para Quem Atendemos */
  height: 32px; /* Tamanho do ícone para Quem Atendemos */
  color: var(--cor-destaque);
  flex-shrink: 0; /* Impede que o ícone encolha se o texto for muito longo */
  display: flex; /* Para centralizar o SVG */
  align-items: center;
  justify-content: center;
}

.list-icon svg {
  width: 100%; /* SVG ocupa todo o espaço do container list-icon */
  height: 100%;
  fill: currentColor; /* Para SVGs com fill */
  stroke: currentColor; /* Para SVGs com stroke */
  stroke-width: 2; /* Largura do traço para ícones de linha */
}

/* Ajuste de estilo para o parágrafo dentro do li de "Quem Atendemos" */
.who-we-serve-list li p {
  margin-bottom: 0; /* Remove margem inferior padrão para alinhamento */
  text-align: center; /* Centraliza o texto do parágrafo no card */
}


/* Hero Section */
.hero {
  /* Fundo da seção hero agora cinza escuro, sem gradiente ou imagem */
  background-color: var(--cor-fundo-escuro); 
  height: 105vh; /* Mantido para ocupar a tela toda */
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 70px;
  box-sizing: border-box;
}

.hero-content {
  max-width: 1000px;
  display: flex;
  flex-direction: row; /* PADRÃO: Foto e Texto lado a lado */
  align-items: center;
  justify-content: center; /* Centraliza o conteúdo horizontalmente */
  gap: 50px;
  padding: 0 20px;
}

.advogada-photo {
  width: 400px;
  height: 400px;
  border-radius: 8px;
  object-fit: cover;
  box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.6);
  /* Removido margin-right: 50px; pois flex-direction-reverse já controla o espaçamento */
}

.hero-text-container {
  flex: 1;
  text-align: left; /* Texto alinhado à esquerda */
}

.hero h1 {
  font-size: 3.2em;
  margin-bottom: 20px;
  color: var(--cor-texto-claro);
  text-align: left;
}

.hero p {
  font-size: 1.2em;
  margin-bottom: 30px;
  color: var(--cor-texto-claro);
  text-align: left;
}

.btn-contato {
  display: inline-block;
  background-color: var(--cor-destaque);
  color: var(--cor-fundo-escuro);
  padding: 16px 30px;
  border-radius: 5px;
  font-weight: bold;
  font-size: 1em;
  transition: background-color 0.3s ease, transform 0.3s ease;
}

.btn-contato:hover {
  background-color: #A98745;
  transform: translateY(-3px);
}

/* Sobre Nós Section */
.sobre-nos-content {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
  text-align: left;
  flex-wrap: wrap;
}

.advogada-photo-small {
  width: 300px;
  height: 300px;
  border-radius: 8px;
  object-fit: cover;
  box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.5);
}

.text-content {
  max-width: 600px;
}

.text-content h2 {
  text-align: left;
}

.text-content p {
  margin-bottom: 15px;
}

/* Formulário de Contato REMOVED, NEW STYLES BELOW */
.contact-button-container {
  margin: 30px auto;
  text-align: center; /* Centraliza o botão */
}

.contact-info-container {
  margin-top: 30px;
  text-align: center;
}

.contact-info {
  margin-bottom: 10px;
}

/* Footer */
.footer {
  background-color: var(--cor-fundo-escuro);
  padding: 20px;
  text-align: center;
  border-top: 1px solid var(--cor-borda);
  color: #888;
  font-size: 0.85em;
  margin-top: 40px;
}

/* Marca Texto */
.highlight {
  background-color: var(--cor-destaque);
  color: var(--cor-fundo-escuro); /* Garante que o texto seja legível sobre o destaque */
  padding: 2px 5px; /* Adiciona um pequeno padding para o "grifo" */
  border-radius: 3px; /* Cantos levemente arredondados */
  display: inline; /* Garante que se comporte como texto em linha */
}


/* RESPONSIVIDADE DO MENU HAMBÚRGUER */
@media (max-width: 900px) { /* Ponto de interrupção para ativar o menu hambúrguer */
  .navbar nav {
    flex-direction: row; /* Mantém logo e hambúrguer na mesma linha */
    justify-content: space-between; /* Espaça logo e hambúrguer */
    padding: 0 20px; /* Garante padding em telas menores */
  }

  /* Esconde o menu de navegação padrão em telas menores */
  .nav-links {
    display: none; /* Esconde o menu por padrão no mobile */
    flex-direction: column;
    position: fixed; /* Fixa o menu */
    top: 60px; /* Abaixo da navbar */
    right: 0; /* Posiciona o menu no lado direito (inicialmente na tela) */
    width: 100%; /* Ocupa 100% da largura da tela */
    background-color: var(--cor-fundo-escuro);
    box-shadow: -2px 0 10px rgba(0, 0, 0, 0.5); /* Sombra à esquerda */
    padding: 20px 0;
    transition: transform 0.3s ease-in-out; /* Transição para o slide */
    transform: translateX(100%); /* Esconde o menu para fora da tela, à direita */
    height: calc(100vh - 60px); /* Ocupa o restante da tela */
    overflow-y: auto; /* Permite scroll se os itens excederem a altura */
    z-index: 999; /* Garante que o menu fique acima do conteúdo */
  }

  /* Mostra o menu quando "menu-open" está ativo */
  .nav-links.menu-open {
    display: flex; /* Mostra o menu quando aberto */
    transform: translateX(0); /* Desliza o menu para a posição 0 (dentro da tela) */
  }

  .nav-links li {
    margin: 15px 0; /* Espaçamento vertical para os itens */
    text-align: center;
  }

  .nav-links li a {
    display: block; /* Ocupa toda a largura do item */
    padding: 10px 0; /* Padding para a área clicável */
    color: var(--cor-texto-claro);
    font-size: 1.2em;
  }

  .nav-links li a:hover {
    background-color: #282828; /* Fundo sutil no hover */
  }

  .hamburger-menu {
    /* Mostra o hambúrguer no mobile */
    display: flex; 
  }

  /* RESPONSIVIDADE HERO SECTION (FOTO E TEXTO EMPILHADOS NO MOBILE) */
  .hero-content {
    flex-direction: column; /* Coloca foto e texto em coluna no mobile */
    text-align: center; /* Centraliza o conteúdo */
  }
}

@media (max-width: 768px) {
  .hero {
    padding-top: 100px;
  }

  .hero h1 {
    font-size: 2.8em;
  }

  .hero p {
    font-size: 1.1em;
  }

  .advogada-photo {
    width: 300px;
    height: 300px;
  }

  .advogada-photo-small {
    width: 250px;
    height: 250px;
  }

  .section {
    padding: 60px 15px;
  }

  h2 {
    font-size: 1.8em;
  }

  .section ul li {
    flex-basis: calc(100% - 30px);
  }

  .specialization-list li {
    padding: 25px 20px;
  }

  .specialization-list li h3 {
    font-size: 1.2em;
  }

  .card-icon {
    font-size: 2.2em; /* Ajuste para o tamanho do SVG em telas menores */
  }

  .who-we-serve-list li {
    flex-direction: column; /* Em telas menores, o ícone e o texto podem empilhar */
    align-items: center; /* Centraliza o conteúdo no card (mobile) */
    gap: 5px; /* Reduz o espaço entre o ícone e o texto quando empilhados */
    padding: 15px; /* Ajusta o padding do card para mobile */
  }

  .list-icon {
    width: 28px; /* Ajuste o tamanho do ícone em telas menores */
    height: 28px; /* Ajuste o tamanho do ícone em telas menores */
    margin-bottom: 5px; /* Espaço entre o ícone e o texto quando empilhados */
  }

  .who-we-serve-list li p {
    text-align: center; /* Centraliza o texto do parágrafo no card (mobile) */
  }
}

@media (max-width: 480px) {
  .navbar .logo {
    font-size: 1.4em;
  }

  .hero h1 {
    font-size: 2.2em;
  }

  .hero p {
    font-size: 1em;
  }

  .btn-contato {
    padding: 12px 25px;
    font-size: 0.9em;
  }

  /* Contact button container on mobile */
  .contact-button-container {
    padding: 0 15px;
  }
}
</style>