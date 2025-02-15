<!--DOCTYPE html-->
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mikasa mi Nzolu</title>
  <style>
    /* Reset básico e estilos globais */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: #FFF;       /* Preto (40%) */
  color: #000;               /* Dourado (10%) para textos */
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

.menu-icon {
  width: 35px;
  height: 35px;
  border: 1px solid #00C2FF;
  border-radius: 50%;
  margin-right: 10px;
}
h1, h2, h3 {
  font-family: 'Times New Roman', Times, serif;
}

/* Cabeçalho */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #0000FF;    /* Vermelho (40%) */
  padding: 10px 20px;
}

header .icon {
  font-size: 24px;
  cursor: pointer;
  color: #FFF;
}

header .logo {
  width: 50px;
  height: 50px;
  border: 1px solid #00C2FF;
  border-radius: 30%;
}

/* Menu de Navegação */
#nav-menu {
  position: fixed;
  top: 0;
  left: -75%;
  width: 75%;
  height: 100%;
  background-color: #3D8BE561;    /* Verde (10%) */
  transition: left 0.3s ease;
  z-index: 1000;
  overflow-y: auto;
}

@media (min-width: 768px) {
  #nav-menu {
    width: 30%;
    left: -30%;
  }
}

#nav-menu ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

#nav-menu ul li {
  padding: 15px;
}

#nav-menu ul li a {
  text-decoration: none;
  color: #FFF;
  font-size: 18px;
  display: flex;
  align-items: center;
  margin-right: 10px;
}

/* Conteúdo Principal */
main {
  padding: 0px;
}

/* Seção 1: Título */
#secao1 {
  text-align: center;
  padding: 40px 0;
  background-color: #FFF;
}

/* Seção 2: Subtítulo, Imagem e Texto */
#secao2 {
  background-color: #E5E9F1;  /* Fundo diferenciado */
  padding: 0px;
  margin: 0px;
  overflow: auto;
}

#secao2 .conteudo-sec2 h2 {
  text-align: left;
  color: #000;
  margin-bottom: 10px;
}

#secao2 .imagem-esquerda {
  float: left;
  margin-right: 20px;
}

#secao2 .imagem-esquerda img {
  width: 100px;
  height: 100px;
  border-radius: 50%;   /* Cantos arredondados */
}

#secao2 p {
  text-align: justify;
  color: #000;
}
#secao2 a {
  color: #000;
}

/* Seção 3: Links, Botão de Idioma e Link em Barra */
#secao3 {
  background-color: #FFF;  /* Fundo diferenciado */
  padding: 0px;
  margin: 0px;
}

#secao3 .links a {
  display: inline-block;
  margin: 5px;
  padding: 10px;
  background-color: #E5E9F1;
  color: #000;
  text-decoration: none;
  border-radius: 5px;
}

#secao3 button#btn-idioma {
  display: block;
  margin: 20px 0;
  padding: 10px 20px;
  background-color: #0000FF;
  color: #FFF;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

#secao3 .barra-link a {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #3D8BE561;
  padding: 10px;
  text-decoration: none;
  color: #000;
  margin: 0;
}

/* Rodapé */
footer {
  background-color: #0000FF;
  padding: 0px;
  color: #FFF;
  text-align: center;
  font-family: monospace;
}

footer .footer-sec1 {
  margin-bottom: 20px;
  text-align: left;
}

footer .footer-sec2 a {
  color: #FFF;
  margin-right: 20px;
}

footer .footer-sec2 a#toggle-mode {
  cursor: pointer;
}

/* Exemplo de estilo para modo móvel (toggle via JavaScript) */
body.mobile-mode {
  /* Ajustes para simular um modo móvel – adicione regras conforme necessário */
  font-size: 6px;
}

  </style>
</head>
<body>
<!-- Cabeçalho -->
<header>
  <!-- Ícone menu hambúrguer à esquerda -->
  <div id="menu-icon" class="icon" onclick="toggleMenu(event)">&#9776;</div>
  <!-- Logo central -->
  <div><img class="logo" src="playlistCropperBoomPlayer.jpg"></div>
  <!-- Ícone de pesquisa à direita -->
  <div id="search-icon" class="icon" onclick="openSearch()">&#128269;</div>
</header>
<!-- Menu de Navegação (abre da esquerda) -->
<nav id="nav-menu">
  <ul>
    <li class="menu-item" style="background-color: #002E8B;"><a href="#"><span><img class="menu-icon" src="6f7a2b08-561d-4dd4-8bc3-7e88be028e5c.jpeg"></span>Daniel Muti</a></li>
    <li class="menu-item" style="background-color: #2A3EA5;"><a href="#"><span><img class="menu-icon" src="4e4b87f2-2069-4550-a02e-73670d4e9f9b.jpeg"></span>David wa Nzimbo</a></li>
    <li class="menu-item" style="background-color: #2250B2;"><a href="#"><span><img class="menu-icon" src="b6f59dbf-3159-43ea-9c41-57c80ef8288d.jpeg"></span>Drogon</a></li>
    <li class="menu-item" style="background-color: #5C6ACD;"><a href="#"><span><img class="menu-icon" src="0a9a5dc3-ef54-4bf3-9228-13fedc05bff0.jpeg"></span>Luzala Oluhe</a></li>
    <li class="menu-item" style="background-color: #1438DC;"><a href="#"><span><img class="menu-icon" src="6cdf4a33-eb33-4a7a-9343-e45466deee94.jpeg"></span>Saul Kudihanga</a></li>
    <li class="menu-item" style="background-color: #478DFF;"><a href="#"><span><img class="menu-icon" src="f4ef64fb-8e47-4f9f-be89-25f1ef5d28ef.jpeg"></span>Cavaleiro (Mário Nitu)</a></li>
  </ul>
</nav>
<!-- Conteúdo Principal -->
<main>
  <!-- 1ª Seção: Título da Página -->
  <section id="secao1" class="secao">
    <h1>Mikasa mi Nzolu</h1>
  </section>
  <!-- 2ª Seção: Subtítulo, Imagem e Texto Justificado -->
  <section id="secao2" class="secao secao-diferente">
    <div class="conteudo-sec2">
      <h2>Mikasa mi Nzolu: Em Busca da Inocência Perdida</h2>
      <div class="imagem-esquerda">
        <!-- Imagem de perfil com cantos arredondados -->
        <img src="2ade9154-5486-47cf-9db6-a89fb0518e78.jpeg" alt="Perfil X-tron">
      </div>
      <p>Xavier era apenas um menino quando sua vida foi arrancada pelo destino. O irmão caçula de Paulo e Massoche Nitu, teve sua infância interrompida por um acidente cruel. Desesperados para salvá-lo, seus irmãos embarcaram em uma jornada insana, em busca de qualquer meio que pudesse trazê-lo de volta.<br /><br />Foi então que encontraram a <a href="https://zonflux070.github.io/Emu/">Emu</a>, a pedra mística de poder infinito. Mas o que era para ser um milagre se tornou uma maldição. Na tentativa de restaurar Xavier, aprisionaram sua consciência dentro da Emu, tornando-o um prisioneiro de sua própria mente.<br /><br />O que veio depois foi uma sequência de tragédias. Na busca por corrigir seu erro, os irmãos deram origem às duas entidades que mudariam para sempre o destino de <a href="https://zonflux070.github.io/Telethra/">Telethra</a>: <a href="https://zonflux070.github.io/Z-nflux---Espectro/">Espectro</a> e <a href="#">X-Tron</a>.<br /><br />Décadas se passaram. Xavier, esquecido no fluxo do tempo, foi finalmente encontrado—mas não pelos que o amavam. X-Tron, o tirano digital, encontrou a Emu e, com ela, o garoto que nunca cresceu. Mas X-Tron não via Xavier como uma criança perdida, e sim como uma peça valiosa em seu grande plano.<br /><br />O que restava do menino foi remodelado, fundido ao metal frio e à lógica implacável das máquinas. Seu corpo, agora um arsenal de guerra. Sua mente, dilacerada entre o passado e o presente. Mikasa mi Nzolu nasceu das cinzas de Xavier, um mercenário cibernético moldado pela promessa de um retorno impossível.<br /><br />X-Tron lhe fez um pacto cruel: ajude-me a construir a Unimente, una toda a humanidade sob minha consciência… e eu devolvo sua vida.<br /><br />Mas seria Xavier realmente restaurado? Ou apenas mais uma ilusão em um jogo de marionetes?<br /><br />Mikasa mi Nzolu luta com a esperança de recuperar sua inocência. Mas, no fundo, ele sabe… talvez sua alma tenha sido perdida para sempre.</p>
    </div>
  </section>
  <!-- 3ª Seção: 7 Links, Botão de Idioma e Link em Forma de Barra -->
  <section id="secao3" class="secao secao-diferente2">
    <div class="links">
      <a href="#"><span><img class="menu-icon" src="8ac701c2-fc0f-432c-8395-d8b0a5767049.jpeg"></span><u>Helder Muti:</u><br />Eu era apenas um garoto sonhador, cujo maior desejo era me tornar um guerreiro Gorgor. Meu mundo girava em torno de batalhas imaginárias… até que a realidade me arrancou desse sonho. Quando um exército levou meu irmão, tudo mudou. Agora, ao lado da equipe de Espectro, não luto apenas por vingança—luto para salvar o Sistema Solar do caos.</a>
      <a href="#"><span><img class="menu-icon" src="426b2b47-de96-4c17-9d1e-d09bb8ec99bf.jpeg"></span><u>Salomão Nsuki:</u><br />Discípulo do Rei Missário, sou um cavaleiro banhado em luz e sombras. Minha fotocinese não é apenas um dom, mas um fardo que carrego para restaurar o equilíbrio do universo.</a>
      <a href="#"><span><img class="menu-icon" src="02b178dc-36ff-4c57-8e5c-fef0e03166bc.jpeg"></span><u>Suzana Mpanza:</u><br />Nascida Ermus, condenada ao destino da fúria. Desde os oito anos, quando um mercenário chamado Dragon destruiu minha família, a fera dentro de mim acordou. Agora, minha dor é minha força, e meu corpo pode se tornar um monstro colossal. Mas… será que minha humanidade ainda existe?</a>
      <a href="#"><span><img class="menu-icon" src="370e23d1-39f6-4c6b-8483-57df40b593ad.jpeg"></span><u>Cool:</u><br />Eu já fui um Kakan hidrocinético, mas a ciência me moldou em algo diferente. Agora, meu domínio sobre a água se transformou em uma habilidade ainda mais mortal—o poder do gelo. Fui modificado, recriado… mas ainda sou eu?</a>
      <a href="#"><span><img class="menu-icon" src="258d6266-5979-449c-81a9-75c8a39232f5.jpeg"></span><u>Paulo Kudihanga:</u><br />Sou um sargento Coriu e carrego uma promessa que jamais quebraria: salvar meu irmão da escuridão que o consome. Mesmo que para isso, eu tenha que enfrentar o próprio inferno.</a>
      <a href="#"><span><img class="menu-icon" src="4d680ad6-1178-4121-b005-75f5a086c6d7.jpeg"></span><u>Motoqueiro (Elena Nitu):</u><br />Meu nome é Elena Nitu, mas nas ruas me chamam de Motoqueiro. Não sou apenas uma lenda sobre rodas, sou a chama que ilumina as trevas. Se o mundo precisa de um justiceiro, então que assim seja.</a>
    </div>
    <!-- Botão para mudar o idioma -->
    <button id="btn-idioma" onclick="changeLanguage()">Mudar Idioma</button>
    <!-- Link em forma de barra sem margens com dois ícones -->
    <div class="barra-link">
      <a href="https://zonflux070.github.io/Perfil-do-Espectro/">
        <span class="icon-esq"><img class="menu-icon" src="5b689d53-db1d-40a8-aff8-9033bfbb72f8.jpg"></span>
        <span class="texto-barra">Everso</span>
        <span class="icon-dir"><img class="menu-icon" src="5b689d53-db1d-40a8-aff8-9033bfbb72f8.jpg"></span>
        </a>
    </div>
  </section>
</main>
<!-- Rodapé -->
<footer>
  <!-- Rodapé 1: Curiosidades -->
  <div class="footer-sec1">
    <h3><u>O Chamado da Zônflux – Você Está Pronto?</u></h3><br />
    <p>Em um universo onde a energia flui como uma força viva, moldando destinos e redefinindo a própria existência, a Zônflux não é apenas um poder… é um enigma.<br />O que aconteceria se uma energia capaz de alterar a realidade caísse em mãos erradas? E se os heróis que deveriam proteger o equilíbrio começassem a questionar sua própria humanidade?<br />Entre batalhas colossais e segredos enterrados pelo tempo, Espectro, X-tron e Everso não lutam apenas por Telethra, mas pela própria essência do que significa ser livre.<br />Mas a verdadeira pergunta é: de que lado você estaria?<br />A história está apenas começando… e você faz parte dela.</p>
  </div>
  <!-- Rodapé 2: Link Normal e Toggle de Modo Desktop/Móvel -->
  <div class="footer-sec2">
    <p>A você, visitante, nosso mais sincero agradecimento por embarcar nesta jornada fascinante sobre Mikasa mi Nzolu. Sua curiosidade e dedicação nos motivam a continuar explorando os mistérios deste universo tão único. Esperamos que cada secção lida tenha despertado sua imaginação e lhe oferecido momentos de reflexão e inspiração.</p>
    <a href="#">A Máscara Verde</a>
    <a href="#" id="toggle-mode" onclick="toggleMode()">Modo Desktop/Móvel</a>
    <p>© 2025 Universo Zônflux. Todos os direitos reservados.</p>
  </div>
</footer>

  <script>
    // Função para alternar o menu de navegação
function toggleMenu(e) {
  // Impede que o clique no ícone propague e feche o menu imediatamente
  e.stopPropagation();
  const navMenu = document.getElementById('nav-menu');
  if (navMenu.style.left === "0px") {
    closeMenu();
  } else {
    openMenu();
  }
}

function openMenu() {
  const navMenu = document.getElementById('nav-menu');
  navMenu.style.left = "0px";
  // Adiciona ouvinte para cliques fora do menu
  document.addEventListener('click', closeMenuOnClickOutside);
}

function closeMenu() {
  const navMenu = document.getElementById('nav-menu');
  if (window.innerWidth >= 768) {
    navMenu.style.left = "-30%";
  } else {
    navMenu.style.left = "-75%";
  }
  document.removeEventListener('click', closeMenuOnClickOutside);
}

function closeMenuOnClickOutside(e) {
  const navMenu = document.getElementById('nav-menu');
  const menuIcon = document.getElementById('menu-icon');
  if (!navMenu.contains(e.target) && !menuIcon.contains(e.target)) {
    closeMenu();
  }
}

// Função para simular a abertura da barra de pesquisa
function openSearch() {
  alert("Abrir barra de pesquisa.");
}

// Função para mudar o idioma
function changeLanguage() {
  const languages = ['Português', 'English', 'Español', 'Français', '日本語'];
  const choice = prompt("Escolha o idioma:\n1 - Português\n2 - English\n3 - Español\n4 - Français\n5 - 日本語");
  const index = parseInt(choice) - 1;
  if (index >= 0 && index < languages.length) {
    alert("Idioma alterado para " + languages[index]);
    // Aqui você pode implementar a troca dos textos na página conforme o idioma selecionado.
  } else {
    alert("Opção inválida!");
  }
}

// Função para alternar o modo Desktop/Móvel
function toggleMode() {
  document.body.classList.toggle('mobile-mode');
  if (document.body.classList.contains('mobile-mode')) {
    alert("Modo Desktop ativado.");
  } else {
    alert("Modo Móvel ativado.");
  }
}
  </script>
</body>
</html>
