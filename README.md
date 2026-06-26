<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Meu Universo</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Arial', sans-serif;
    }

    body {
      height: 100vh;
      overflow-x: hidden;
      background: #0a0a0f;
      color: white;
    }

    .background {
      position: fixed;
      width: 100%;
      height: 100%;
      background: radial-gradient(circle at top, #1a1a2e, #0a0a0f);
      overflow: hidden;
      z-index: -1;
    }

    .stars {
      position: absolute;
      width: 200%;
      height: 200%;
      animation: moveStars 60s linear infinite;
    }

    .stars::before,
    .stars::after {
      content: "";
      position: absolute;
      width: 100%;
      height: 100%;
      background-image: radial-gradient(white 1px, transparent 1px);
      background-size: 50px 50px;
      opacity: 0.15;
    }

    @keyframes moveStars {
      from { transform: translateY(0px); }
      to { transform: translateY(-1000px); }
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      backdrop-filter: blur(10px);
      background: rgba(10,10,15,0.5);
      border-bottom: 1px solid rgba(255,255,255,0.1);
      z-index: 10;
    }

    header h1 {
      font-size: 18px;
      letter-spacing: 2px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      opacity: 0.7;
      transition: 0.3s;
    }

    nav a:hover {
      opacity: 1;
    }

    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
    }

    .hero h2 {
      font-size: 48px;
      margin-bottom: 20px;
      letter-spacing: 2px;
    }

    .hero p {
      max-width: 600px;
      opacity: 0.7;
      line-height: 1.6;
    }

    .btn {
      margin-top: 30px;
      padding: 12px 24px;
      border: 1px solid white;
      background: transparent;
      color: white;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background: white;
      color: black;
    }

    @media (max-width: 768px) {
      .hero h2 {
        font-size: 32px;
      }

      header {
        padding: 15px 20px;
      }
    }
  </style>
</head>

<body>

  <div class="background">
    <div class="stars"></div>
  </div>

  <header>
    <h1>MEU UNIVERSO</h1>
    <nav>
      <a href="#">Início</a>
      <a href="#">Poemas</a>
      <a href="#">Músicas</a>
      <a href="#">Contato</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Um espaço onde a arte respira</h2>
    <p>
      Poemas, ideias e fragmentos de um universo pessoal em construção.
      Aqui, tudo é sentimento transformado em linguagem.
    </p>
    <button class="btn">Explorar</button>
  </section>

</body>
</html>      z-index: -1;
    }

    .stars {
      position: absolute;
      width: 200%;
      height: 200%;
      background: transparent;
      animation: moveStars 60s linear infinite;
    }

    .stars::before,
    .stars::after {
      content: "";
      position: absolute;
      width: 100%;
      height: 100%;
      background-image: radial-gradient(white 1px, transparent 1px);
      background-size: 50px 50px;
      opacity: 0.15;
    }

    @keyframes moveStars {
      from { transform: translateY(0px); }
      to { transform: translateY(-1000px); }
    }

    /* Header */
    header {
      position: fixed;
      top: 0;
      width: 100%;
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      backdrop-filter: blur(10px);
      background: rgba(10,10,15,0.5);
      border-bottom: 1px solid rgba(255,255,255,0.1);
      z-index: 10;
    }

    header h1 {
      font-size: 18px;
      letter-spacing: 2px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      opacity: 0.7;
      transition: 0.3s;
    }

    nav a:hover {
      opacity: 1;
    }

    /* Hero */
    .hero {
      height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 0 20px;
    }

    .hero h2 {
      font-size: 48px;
      margin-bottom: 20px;
      letter-spacing: 2px;
    }

    .hero p {
      max-width: 600px;
      opacity: 0.7;
      line-height: 1.6;
    }

    .btn {
      margin-top: 30px;
      padding: 12px 24px;
      border: 1px solid white;
      background: transparent;
      color: white;
      cursor: pointer;
      transition: 0.3s;
    }

    .btn:hover {
      background: white;
      color: black;
    }

    /* Responsivo */
    @media (max-width: 768px) {
      .hero h2 {
        font-size: 32px;
      }

      header {
        padding: 15px 20px;
      }
    }
  </style>
</head>

<body>

  <div class="background">
    <div class="stars"></div>
  </div>

  <header>
    <h1>MEU UNIVERSO</h1>
    <nav>
      <a href="#">Início</a>
      <a href="#">Poemas</a>
      <a href="#">Músicas</a>
      <a href="#">Contato</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Um espaço onde a arte respira</h2>
    <p>
      Poemas, ideias e fragmentos de um universo pessoal em construção.
      Aqui, tudo é sentimento transformado em linguagem.
    </p>
    <button class="btn">Explorar</button>
  </section>

</body>
</html>
