<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LigSe – Economize com Energia Solar</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #f5f5f5;
      color: #333;
      text-align: center;
    }
    header {
      background: #009688;
      color: white;
      padding: 2rem 1rem;
    }
    h1 {
      font-size: 2rem;
      margin-bottom: 1rem;
    }
    p {
      font-size: 1.1rem;
      margin-bottom: 2rem;
    }
    form {
      max-width: 400px;
      margin: 2rem auto;
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    input {
      padding: 1rem;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      background: #25D366;
      color: white;
      padding: 1rem;
      font-size: 1.2rem;
      border: none;
      border-radius: 8px;
      cursor: pointer;
    }
    button:hover {
      background: #1ebe5d;
    }
    footer {
      margin-top: 3rem;
      font-size: 0.9rem;
      color: #888;
    }
    @media (max-width: 600px) {
      h1 { font-size: 1.5rem; }
      p { font-size: 1rem; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Economize na conta de luz com energia solar</h1>
    <p>Sem investimento, sem instalação. A LigSe conecta você à economia!</p>
  </header>

  <form id="leadForm">
    <input type="text" id="nome" placeholder="Seu nome" required>
    <input type="tel" id="telefone" placeholder="Telefone com DDD" required>
    <input type="text" id="cidade" placeholder="Cidade" required>
    <button type="submit">Quero economizar!</button>
  </form>

  <script>
    document.getElementById('leadForm').addEventListener('submit', function(event) {
      event.preventDefault();
      const nome = document.getElementById('nome').value;
      const telefone = document.getElementById('telefone').value;
      const cidade = document.getElementById('cidade').value;
      const msg = `Olá, meu nome é ${nome}, meu telefone é ${telefone} e sou de ${cidade}. Quero economizar na conta de luz!`;
      const url = `https://wa.me/5587988381709?text=${encodeURIComponent(msg)}`;
      window.open(url, '_blank');
    });
  </script>

  <footer>
    LigSe – Energias Renováveis © 2025
  </footer>
</body>
</html>
