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
          <a href="https://wa.me/5514981411212?text=Olá, encontrei vocês através do site." class="btn-contato">Entre em Contato</a>
        </div>
        <img src="../assets/ise.png" alt="Foto da Advogada" class="advogada-photo">
      </div>
    </section>

    <section id="nossos-numeros" class="section">
      <h2>Nossos Números</h2>
      <p class="section-description">Resultados que comprovam nosso compromisso com a excelência na defesa da sua profissão.</p>
      <div class="stats-cards-container">
        <div class="stat-card">
          <h3>250+</h3>
          <p>Profissionais de Saúde Atendidos</p>
        </div>
        <div class="stat-card">
          <h3>98%</h3>
          <p>Taxa de Sucesso em Processos</p>
        </div>
        <div class="stat-card">
          <h3>8+</h3>
          <p>Anos de Experiência na Área</p>
        </div>
        <div class="stat-card">
          <h3>Nacional</h3>
          <p>Atendimento em Todo o Brasil</p>
        </div>
      </div>
    </section>
    <section id="especializacao" class="section">
      <h2>Nossa Especialização</h2>
      <p class="section-description">Atuamos exclusivamente em causas relacionadas aos direitos médicos e da saúde, oferecendo suporte jurídico abrangente para profissionais como você, em diversas áreas, tais como:</p>
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
            <svg fill="#CDA454" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M18.5,11H16.118L14.4,7.553A1,1,0,0,0,13.5,7h-6a1,1,0,0,0-.948.684l-2,6a1,1,0,1,0,1.9.632L7.5,11.162V22a1,1,0,0,0,2,0V16h2v6a1,1,0,0,0,2,0V10.236l1.105,2.211A1,1,0,0,0,15.5,13h3a1,1,0,0,0,0-2Zm-7,3h-2V9h2Zm-1-13A2.5,2.5,0,1,1,8,3.5,2.5,2.5,0,0,1,10.5,1Z"></path></g></svg>          </div>
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
<svg version="1.0" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 64 64" enable-background="new 0 0 64 64" xml:space="preserve" fill="#CDA454"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path fill="#CDA454" d="M60,56h-8V28h8c1.738,0,3.277-1.125,3.809-2.777c0.531-1.656-0.07-3.469-1.484-4.477l-28-20 c-1.391-0.992-3.258-0.992-4.648,0l-28,20c-1.414,1.008-2.016,2.82-1.484,4.477C0.723,26.875,2.262,28,4,28h8v28H4 c-2.211,0-4,1.789-4,4v4h64v-4C64,57.789,62.211,56,60,56z M28,56h-8V28h8V56z M44,56h-8V28h8V56z"></path> </g></svg>          </div>
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
          <svg viewBox="0 0 15 15" version="1.1" id="dentist" xmlns="http://www.w3.org/2000/svg" fill="#CDA454"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <path d="M4.36,14c-1,0-0.56-2.67-0.86-5c-0.1-0.76-1-1.49-1.12-2.06C2,5,1.39,1.44,3.66,1S6,3,7.54,3s1.57-2.36,3.85-2
            s1.59,3.9,1.29,5.9c-0.1,0.45-1.1,1.48-1.18,2.06c-0.33,2.4,0.32,5-0.8,5c-0.93,0-1.32-2.72-2-4.5C8.43,8.63,8.06,8,7.54,8
            C6,8,5.75,14,4.36,14z"></path> </g></svg>
          </div>
          <p><strong>Dentistas e Odontólogos:</strong> Oferecendo suporte em questões de responsabilidade profissional e regulatórias.</p>
        </li>
        <li>
          <div class="list-icon">
<svg fill="#CDA454" height="200px" width="200px" version="1.1" id="Layer_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 512 512" xml:space="preserve"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"> <g> <g> <polygon points="266.534,81.856 266.534,40.928 246.07,40.928 246.07,81.856 205.142,81.856 205.142,102.321 246.07,102.321 246.07,143.249 266.534,143.249 266.534,102.321 307.463,102.321 307.463,81.856 "></polygon> </g> </g> <g> <g> <path d="M399.266,175.204L429.77,12.519c0.559-2.993-0.24-6.279-2.183-8.622C425.643,1.556,422.758,0,419.713,0H92.287 c-3.045,0-5.93,1.556-7.874,3.897c-1.944,2.343-2.743,5.53-2.183,8.522l30.504,162.739 c-18.128,32.463-28.515,69.946-30.351,109.289c-0.312,1.28-0.38,2.621-0.185,3.938c-0.092,2.903-0.143,5.819-0.143,8.739 C82.055,415.606,160.087,512,256,512c95.913,0,173.945-96.389,173.945-214.871C429.945,253.143,419.336,211.128,399.266,175.204z M104.615,20.464h302.77l-26.859,143.249H131.474L104.615,20.464z M256,491.539c-84.629,0-153.481-87.211-153.481-194.409 c0-1.533,0.042-3.056,0.07-4.585c18.523-11.096,89.341-49.699,145.777-28.388c4.496,9.521,17.314,34.101,38.77,55.558 c24.511,24.512,52.177,36.925,81.582,36.924c11.339,0,22.937-1.872,34.71-5.582C384.923,432.095,325.856,491.539,256,491.539z M405.681,328.56c-38.113,15.243-73.001,7.528-103.687-22.929c-23.999-23.815-36.432-53.081-36.549-53.363 c-1.024-2.458-2.968-4.421-5.416-5.47c-57.175-24.501-124.438,4.187-155.786,21.024c3.547-30.018,12.6-58.065,26.694-83.645 H381.06c18.588,33.254,28.42,72.012,28.42,112.752c0,10.517-0.684,21.034-1.961,31.102 C406.903,328.153,406.286,328.318,405.681,328.56z"></path> </g> </g> </g></svg>
          </div>
          <p><strong>Enfermeiros e Equipe de Enfermagem:</strong> Auxiliando na defesa de direitos e em processos disciplinares.</p>
        </li>
        <li>
          <div class="list-icon">
<svg fill="#CDA454" viewBox="0 0 50 50" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><g id="SVGRepo_bgCarrier" stroke-width="0"></g><g id="SVGRepo_tracerCarrier" stroke-linecap="round" stroke-linejoin="round"></g><g id="SVGRepo_iconCarrier"><path d="M24.964844 1 A 1.0001 1.0001 0 0 0 24.382812 1.2128906L4.421875 16.835938L1.3828125 19.212891 A 1.0002305 1.0002305 0 1 0 2.6171875 20.787109L4 19.705078L4 46 A 1.0001 1.0001 0 0 0 5 47L45 47 A 1.0001 1.0001 0 0 0 46 46L46 19.705078L47.382812 20.787109 A 1.0002308 1.0002308 0 1 0 48.617188 19.212891L45.632812 16.878906L25.617188 1.2128906 A 1.0001 1.0001 0 0 0 24.964844 1 z M 25 3.2695312L44 18.138672L44 45L6 45L6 18.138672L25 3.2695312 z M 23 20L23 27L16 27L16 31L23 31L23 38L27 38L27 31L34 31L34 27L27 27L27 20L23 20 z"></path></g></svg>
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
          <p>Com anos de experiência e um profundo conhecimento da legislação em saúde, nossa missão é garantir que os direitos de médicos, dentistas e enfermeiros sejam defendidos com rigor e excelência. Nosso compromisso é com a justiça e a proteção dos interesses daqueles que nos confiam suas carreiras.</p>
          <p>Nossa fundadora, [Nome da Advogada], é uma advogada dedicada e apaixonada por direitos médicos, reconhecida por sua atuação ética e resultados consistentes na defesa de profissionais da saúde.</p>
        </div>
      </div>
    </section>

    <section id="contato" class="section">
      <h2>Entre em Contato</h2>
      <p class="section-description">Estamos prontos para defender sua carreira. Clique no botão abaixo para falar diretamente conosco:</p>
      
      <div class="contact-button-container">
        <a href="https://wa.me/5514981411212?text=Olá, encontrei vocês através do site." target="_blank" class="btn-contato">Fale Conosco</a> 
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
  padding: 80px 20px; /* ORIGINAL */
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
  width: 52px; /* Tamanho fixo para o SVG */
  height: 52px; /* Tamanho fixo para o SVG */
  color: var(--cor-destaque); /* A cor de preenchimento do SVG */
  margin-bottom: 10px;
  transition: transform 0.3s ease;
  display: flex; /* Centralizar o SVG dentro do div */
  align-items: center;
  justify-content: center;
}

/* Garante que o SVG dentro do container use a cor definida e tenha tamanho */
.card-icon svg {
  width: 90%; /* Ajuste o tamanho do ícone dentro do container */
  height: 90%; /* Ajuste o tamanho do ícone dentro do container */
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
  width: 36px; /* Tamanho do ícone para Quem Atendemos */
  height: 36px; /* Tamanho do ícone para Quem Atendemos */
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
  background-color: var(--cor-fundo-escuro); 
  height: auto; 
  min-height: 80vh; 
  display: flex;
  flex-direction: column; 
  align-items: center;
  justify-content: center;
  padding-top: 70px;
  padding-bottom: 20px; 
  box-sizing: border-box;
}

.hero-content {
  max-width: 1000px;
  display: flex;
  flex-direction: row; 
  align-items: center;
  justify-content: center; 
  gap: 50px;
  padding: 0 20px;
  flex-grow: 1; 
}

.advogada-photo {
  width: 400px;
  height: 400px;
  border-radius: 8px;
  object-fit: cover;
  box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.6);
}

.hero-text-container {
  flex: 1;
  text-align: left; 
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

.contact-button-container {
  margin: 30px auto;
  text-align: center; 
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

/* Estilos para a Seção "Nossos Números" */
.stats-cards-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  padding: 0px 20px 40px; 
  max-width: 1000px; 
  margin: 0 auto; 
}

.stat-card {
  background-color: #282828;
  padding: 25px;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4);
  flex-basis: calc(25% - 30px); 
  box-sizing: border-box;
  text-align: center;
  display: flex;
  flex-direction: column;
  /* NOVO: Propriedades para alinhamento e altura fixa */
  justify-content: space-around; /* Distribui espaço entre o h3 e o p */
  align-items: center;
  height: 150px; /* DEFINIDO UMA ALTURA FIXA PARA PADRONIZAR */
  transition: transform 0.3s ease, background-color 0.3s ease;
  position: relative; 
  overflow: hidden;
  width: 100%;
}

.stat-card::before {
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

.stat-card:hover {
  transform: translateY(-8px);
  background-color: #383838; 
}

.stat-card:hover::before {
  background-color: var(--cor-destaque);
}

.stat-card h3 {
  font-size: 2.5em; 
  color: var(--cor-destaque); 
  margin-bottom: 0px; /* REMOVIDO MARGIN-BOTTOM PARA MELHOR ALINHAMENTO COM SPACE-AROUND */
  margin-top: 0;
  line-height: 1;
  z-index: 2; 
  position: relative; 
}

.stat-card p {
  font-size: 0.9em;
  color: var(--cor-texto-claro);
  margin-bottom: 0;
  line-height: 1.2;
  z-index: 2; 
  position: relative; 
}

/* Ajuste do padding do hero para acomodar a nova seção */
.hero {
    min-height: 80vh; 
    padding-bottom: 20px; 
}

#nossos-numeros {
    padding-top: 40px; 
    padding-bottom: 40px; 
}


/* RESPONSIVIDADE DO MENU HAMBÚRGUER */
@media (max-width: 900px) { 
  .navbar nav {
    flex-direction: row; 
    justify-content: space-between; 
    padding: 0 20px; 
  }

  .nav-links {
    display: none; 
    flex-direction: column;
    position: fixed; 
    top: 60px; 
    right: 0; 
    width: 100%; 
    background-color: var(--cor-fundo-escuro);
    box-shadow: -2px 0 10px rgba(0, 0, 0, 0.5); 
    padding: 20px 0;
    transition: transform 0.3s ease-in-out; 
    transform: translateX(100%); 
    height: calc(100vh - 60px); 
    overflow-y: auto; 
    z-index: 999; 
  }

  .nav-links.menu-open {
    display: flex; 
    transform: translateX(0); 
  }

  .nav-links li {
    margin: 15px 0; 
    text-align: center;
  }

  .nav-links li a {
    display: block; 
    padding: 10px 0; 
    color: var(--cor-texto-claro);
    font-size: 1.2em;
  }

  .nav-links li a:hover {
    background-color: #282828; 
  }

  .hamburger-menu {
    display: flex; 
  }

  .hero-content {
    flex-direction: column; 
    text-align: center; 
  }

  .stats-cards-container {
    flex-direction: column; 
    align-items: center;
  }

  .stat-card {
    flex-basis: 90%;
    width: 100%;
    max-width: 300px; 
    height: 300px; /* MANTIDO: Altura fixa no mobile */
  }
}

@media (max-width: 768px) {
  .hero {
    padding-top: 100px;
    min-height: auto; 
    padding-bottom: 20px; 
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
    font-size: 2.2em; 
  }

  .who-we-serve-list li {
    flex-direction: column; 
    align-items: center; 
    gap: 5px; 
    padding: 15px; 
  }

  .list-icon {
    width: 28px; 
    height: 28px; 
    margin-bottom: 5px; 
  }

  .who-we-serve-list li p {
    text-align: center; 
  }

  .stats-cards-container {
      padding: 30px 15px; 
  }

  .stat-card h3 {
      font-size: 2em; 
  }
  .stat-card p {
      font-size: 0.85em; 
  }

  #nossos-numeros {
    padding-top: 30px; 
    padding-bottom: 30px; 
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

  .contact-button-container {
    padding: 0 15px;
  }
}
</style>