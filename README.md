DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Meu Portfólio</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    body {
      background-color: #f4f6f8;
      color: #222;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(135deg, #0f172a, #2563eb);
      color: white;
      padding: 20px 8%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      font-size: 24px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: bold;
    }

    nav a:hover {
      color: #93c5fd;
    }

    .hero {
      min-height: 90vh;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 60px 8%;
      background: white;
    }

    .hero-text {
      max-width: 600px;
    }

    .hero-text h2 {
      font-size: 48px;
      color: #0f172a;
      margin-bottom: 15px;
    }

    .hero-text h2 span {
      color: #2563eb;
    }

    .hero-text p {
      font-size: 18px;
      margin-bottom: 25px;
      color: #444;
    }

    .btn {
      display: inline-block;
      padding: 12px 25px;
      background-color: #2563eb;
      color: white;
      text-decoration: none;
      border-radius: 8px;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn:hover {
      background-color: #1e40af;
      transform: scale(1.05);
    }

    .hero-card {
      background-color: #0f172a;
      color: white;
      padding: 40px;
      border-radius: 20px;
      max-width: 350px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.2);
      text-align: center;
    }

    .hero-card h3 {
      font-size: 28px;
      margin-bottom: 10px;
    }

    section {
      padding: 70px 8%;
    }

    section h2 {
      text-align: center;
      font-size: 34px;
      margin-bottom: 40px;
      color: #0f172a;
    }

    .sobre {
      background-color: #f8fafc;
      text-align: center;
    }

    .sobre p {
      max-width: 800px;
      margin: auto;
      font-size: 18px;
      color: #444;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 25px;
    }

    .card {
      background-color: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      box-shadow: 0 5px 15px rgba(0,0,0,0.08);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-8px);
    }

    .card h3 {
      color: #2563eb;
      margin-bottom: 10px;
    }

    .projetos {
      background-color: white;
    }

    .projeto-card {
      background-color: #f1f5f9;
      padding: 25px;
      border-radius: 15px;
      border-left: 5px solid #2563eb;
    }

    .contato {
      background-color: #0f172a;
      color: white;
      text-align: center;
    }

    .contato h2 {
      color: white;
    }

    .contato p {
      margin-bottom: 20px;
      font-size: 18px;
    }

    form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    input, textarea {
      padding: 14px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
    }

    textarea {
      resize: none;
      height: 120px;
    }

    button {
      padding: 14px;
      border: none;
      background-color: #2563eb;
      color: white;
      font-size: 16px;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
    }

    button:hover {
      background-color: #1d4ed8;
    }

    footer {
      background-color: #020617;
      color: white;
      text-align: center;
      padding: 20px;
    }

    .menu-btn {
      display: none;
      font-size: 28px;
      cursor: pointer;
    }

    @media (max-width: 768px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }

      nav {
        display: none;
        flex-direction: column;
        width: 100%;
        margin-top: 15px;
      }

      nav a {
        margin: 10px 0;
      }

      nav.ativo {
        display: flex;
      }

      .menu-btn {
        display: block;
        position: absolute;
        right: 8%;
        top: 18px;
      }

      .hero {
        flex-direction: column;
        text-align: center;
        gap: 40px;
      }

      .hero-text h2 {
        font-size: 36px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>Meu Portfólio</h1>

    <div class="menu-btn" onclick="abrirMenu()">☰</div>

    <nav id="menu">
      <a href="#inicio">Início</a>
      <a href="#sobre">Sobre</a>
      <a href="#habilidades">Habilidades</a>
      <a href="#projetos">Projetos</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

  <main>

    <section class="hero" id="inicio">
      <div class="hero-text">
        <h2>Olá, eu sou <span>João</span></h2>
        <p>
          Estudante de Engenharia de Software, apaixonado por tecnologia,
          desenvolvimento web e criação de soluções digitais.
        </p>
        <a href="#contato" class="btn">Fale comigo</a>
      </div>

      <div class="hero-card">
        <h3>Desenvolvedor</h3>
        <p>HTML • CSS • JavaScript • Python • SQL</p>
      </div>
    </section>

    <section class="sobre" id="sobre">
      <h2>Sobre mim</h2>
      <p>
        Sou uma pessoa dedicada, em constante aprendizado, buscando crescer na área
        de tecnologia. Tenho interesse em desenvolvimento de sistemas, sites,
        aplicações web e soluções que ajudem pessoas e empresas.
      </p>
    </section>

    <section id="habilidades">
      <h2>Minhas Habilidades</h2>

      <div class="cards">
        <div class="card">
          <h3>HTML</h3>
          <p>Criação da estrutura de páginas web.</p>
        </div>

        <div class="card">
          <h3>CSS</h3>
          <p>Estilização, layout responsivo e design moderno.</p>
        </div>

        <div class="card">
          <h3>JavaScript</h3>
          <p>Interatividade e lógica para páginas web.</p>
        </div>

        <div class="card">
          <h3>Python</h3>
          <p>Automação, lógica de programação e sistemas.</p>
        </div>
      </div>
    </section>

    <section class="projetos" id="projetos">
      <h2>Projetos</h2>

      <div class="cards">
        <div class="projeto-card">
          <h3>Sistema de Estoque</h3>
          <p>
            Sistema simples para controlar entrada e saída de produtos.
          </p>
        </div>

        <div class="projeto-card">
          <h3>Site Institucional</h3>
          <p>
            Página profissional para empresas, igrejas ou projetos pessoais.
          </p>
        </div>

        <div class="projeto-card">
          <h3>Portfólio Pessoal</h3>
          <p>
            Site para apresentar habilidades, experiências e contatos.
          </p>
        </div>
      </div>
    </section>

    <section class="contato" id="contato">
      <h2>Contato</h2>
      <p>Entre em contato comigo preenchendo o formulário abaixo.</p>

      <form onsubmit="enviarMensagem(event)">
        <input type="text" id="nome" placeholder="Seu nome" required />
        <input type="email" id="email" placeholder="Seu e-mail" required />
        <textarea id="mensagem" placeholder="Sua mensagem" required></textarea>
        <button type="submit">Enviar mensagem</button>
      </form>
    </section>

  </main>

  <footer>
    <p>&copy; 2026 - Meu Portfólio. Todos os direitos reservados.</p>
  </footer>

  <script>
    function abrirMenu() {
      const menu = document.getElementById("menu");
      menu.classList.toggle("ativo");
    }

    function enviarMensagem(event) {
      event.preventDefault();

      const nome = document.getElementById("nome").value;
      const email = document.getElementById("email").value;
      const mensagem = document.getElementById("mensagem").value;

      if (nome && email && mensagem) {
        alert("Mensagem enviada com sucesso, " + nome + "!");
        
        document.getElementById("nome").value = "";
        document.getElementById("email").value = "";
        document.getElementById("mensagem").value = "";
      }
    }
  </script>

</body>
</html>
