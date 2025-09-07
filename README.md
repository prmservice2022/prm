# prm
soluçôesauto
<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PRM Service - Reprogramação & Diagnóstico</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #fff;
      color: #222;
    }
    header {
      background: #8B0000;
      color: #fff;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
    }
    nav a {
      color: #fff;
      margin-left: 20px;
      text-decoration: none;
      font-weight: bold;
    }
    .hero {
      background: url("https://via.placeholder.com/1600x500") center/cover;
      color: #fff;
      padding: 120px 30px;
      text-align: center;
    }
    .hero h2 {
      font-size: 2.5rem;
      margin: 0 0 20px;
    }
    .btn {
      background: #8B0000;
      color: #fff;
      padding: 12px 25px;
      border: none;
      border-radius: 8px;
      text-decoration: none;
      font-size: 1rem;
      margin: 10px;
      display: inline-block;
    }
    .section {
      padding: 50px 30px;
      text-align: center;
    }
    .services {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }
    .service-card {
      border: 1px solid #ccc;
      border-radius: 8px;
      padding: 20px;
    }
    footer {
      background: #111;
      color: #eee;
      text-align: center;
      padding: 20px;
      position: relative;
    }
    .whatsapp-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25D366;
      color: #fff;
      padding: 15px;
      border-radius: 50%;
      font-size: 24px;
      text-decoration: none;
    }
    /* Página de Login */
    .login-page {
      display: none;
      height: 100vh;
      background: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .login-box {
      background: #fff;
      padding: 40px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.2);
      width: 300px;
      text-align: center;
    }
    .login-box h2 {
      margin-bottom: 20px;
    }
    .login-box input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
    .login-box button {
      background: #8B0000;
      color: #fff;
      border: none;
      padding: 12px;
      border-radius: 6px;
      width: 100%;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <header>
    <h1>PRM Service</h1>
    <nav>
      <a href="#inicio">Início</a>
      <a href="#servicos">Serviços</a>
      <a href="#" onclick="showLogin()">Portal</a>
      <a href="#contactos">Contactos</a>
    </nav>
  </header>

  <section class="hero" id="inicio">
    <h2>Soluções em Reprogramação e Diagnóstico</h2>
    <a href="#servicos" class="btn">Ver Serviços</a>
    <a href="#" onclick="showLogin()" class="btn">Entrar no Portal</a>
  </section>

  <section class="section" id="servicos">
    <h2>Serviços</h2>
    <div class="services">
      <div class="service-card">Filtro de Partículas</div>
      <div class="service-card">Válvula EGR</div>
      <div class="service-card">AdBlue</div>
      <div class="service-card">Aumento de Potência</div>
      <div class="service-card">Pesados & Ligeiros</div>
      <div class="service-card">Máquinas Agrícolas & Construção</div>
      <div class="service-card">Diagnóstico Multimarcas</div>
      <div class="service-card">Reprogramação de Caixas</div>
    </div>
  </section>

  <section class="section" id="contactos">
    <h2>Contactos</h2>
    <p>Email: prmservice2022@gmail.com</p>
    <p>Telefone: 932337388</p>
  </section>

  <footer>
    <p>© 2025 PRM Service</p>
  </footer>

  <!-- Botão WhatsApp -->
  <a href="https://wa.me/351932337388" class="whatsapp-btn">💬</a>

  <!-- Página de Login -->
  <div class="login-page" id="loginPage">
    <div class="login-box">
      <h2>Login</h2>
      <input type="email" placeholder="Email">
      <input type="password" placeholder="Senha">
      <button>Entrar</button>
      <br><br>
      <button onclick="hideLogin()">Voltar</button>
    </div>
  </div>

  <script>
    function showLogin() {
      document.querySelector('.hero').style.display = 'none';
      document.querySelector('.section').style.display = 'none';
      document.querySelector('#loginPage').style.display = 'flex';
    }
    function hideLogin() {
      document.querySelector('.hero').style.display = 'block';
      document.querySelector('.section').style.display = 'block';
      document.querySelector('#loginPage').style.display = 'none';
    }
  </script>

</body>
</html>
