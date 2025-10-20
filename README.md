<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>🌸 Bela Flor</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
  <style>
    /* Reset e fontes */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* Cabeçalho */
    header {
      height: 70px;
      background-color: #81C784;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0 40px;
      color: #2E7D32;
    }

    .logo {
      font-size: 22px;
    }

    nav a {
      margin-left: 24px;
      font-size: 16px;
      color: #2E7D32;
    }

    /* Seção Hero */
    .hero {
      height: 80vh;
      background: url('https://source.unsplash.com/1600x900/?flowers') center/cover no-repeat;
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background: rgba(255, 255, 255, 0.6);
    }

    .hero-content {
      position: relative;
      z-index: 1;
    }

    .hero-content h1 {
      font-family: Georgia, serif;
      font-size: 40px;
      color: #2E7D32;
      margin-bottom: 20px;
    }

    .hero-content a {
      background-color: #2E7D32;
      color: white;
      padding: 10px 20px;
      border-radius: 8px;
      font-size: 16px;
    }

    /* Seção Galeria */
    .galeria {
      background-color: #ffffff;
      padding: 60px 40px;
      text-align: center;
    }

    .galeria h2 {
      font-size: 26px;
      color: #2E7D32;
      margin-bottom: 40px;
    }

    .galeria-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 16px;
      justify-items: center;
    }

    .galeria-grid img {
      width: 200px;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
    }

    /* Seção Contato */
    .contato {
      background-color: #F1F8E9;
      padding: 40px;
    }

    .contato h2 {
      font-size: 26px;
      color: #2E7D32;
      text-align: center;
      margin-bottom: 30px;
    }

    form {
      max-width: 600px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 16px;
    }

    input, textarea {
      width: 100%;
      height: 40px;
      padding: 8px;
      border: 1px solid #C8E6C9;
      border-radius: 8px;
      font-family: 'Poppins', sans-serif;
    }

    textarea {
      height: 100px;
      resize: vertical;
    }

    button {
      background-color: #2E7D32;
      color: white;
      height: 44px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }

    /* Rodapé */
    footer {
      background-color: #81C784;
      color: #2E7D32;
      text-align: center;
      font-size: 14px;
      padding: 16px;
    }
  </style>
</head>
<body>

  <!-- Cabeçalho -->
  <header>
    <div class="logo">🌸 Bela Flor</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#galeria">Galeria</a>
      <a href="#contato">Contato</a>
    </nav>
  </header>

  <!-- Seção Hero -->
  <section class="hero" id="home">
    <div class="hero-content">
      <h1>Flores que encantam.</h1>
      <a href="#galeria">Ver Galeria</a>
    </div>
  </section>

  <!-- Seção Galeria -->
  <section class="galeria" id="galeria">
    <h2>Nossas Flores</h2>
    <div class="galeria-grid">
      <img src="https://source.unsplash.com/200x200/?flower1" alt="Flor 1">
      <img src="https://source.unsplash.com/200x200/?flower2" alt="Flor 2">
      <img src="https://source.unsplash.com/200x200/?flower3" alt="Flor 3">
      <img src="https://source.unsplash.com/200x200/?flower4" alt="Flor 4">
      <img src="https://source.unsplash.com/200x200/?flower5" alt="Flor 5">
      <img src="https://source.unsplash.com/200x200/?flower6" alt="Flor 6">
    </div>
  </section>

  <!-- Seção Contato -->
  <section class="contato" id="contato">
    <h2>Contato</h2>
    <form>
      <input type="text" placeholder="Nome" required>
      <input type="email" placeholder="E-mail" required>
      <textarea placeholder="Mensagem" required></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <!-- Rodapé -->
  <footer>
    &copy; 2025 Bela Flor. Todos os direitos reservados.
  </footer>

</body>
</html>
