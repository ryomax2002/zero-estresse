<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Zero Estresse</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(120deg, #a8edea, #fed6e3);
      color: #333;
      text-align: center;
    }

    header {
      padding: 50px 20px;
      background: rgba(255, 255, 255, 0.6);
      backdrop-filter: blur(10px);
    }

    h1 {
      font-size: 3em;
      margin: 0;
    }

    p {
      font-size: 1.2em;
    }

    .content {
      padding: 40px 20px;
    }

    .card {
      background: white;
      border-radius: 15px;
      padding: 20px;
      margin: 20px auto;
      max-width: 400px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }

    button {
      padding: 10px 20px;
      border: none;
      border-radius: 25px;
      background: #6c63ff;
      color: white;
      font-size: 1em;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #4a47d1;
    }

    footer {
      margin-top: 40px;
      padding: 20px;
      font-size: 0.9em;
      color: #555;
    }
  </style>
</head>
<body>

  <header>
    <h1>Zero Estresse</h1>
    <p>Respire fundo. Relaxe. Você está no controle.</p>
  </header>

  <section class="content">
    <div class="card">
      <h2>🌿 Dica do dia</h2>
      <p id="dica">Clique no botão para receber uma dica de relaxamento.</p>
      <button onclick="novaDica()">Nova dica</button>
    </div>
  </section>

  <footer>
    <p>© 2026 Zero Estresse</p>
  </footer>

  <script>
    const dicas = [
      "Respire profundamente por 1 minuto.",
      "Afaste-se das telas por alguns minutos.",
      "Beba um copo de água.",
      "Ouça uma música calma.",
      "Alongue seu corpo por 2 minutos.",
      "Dê uma pequena caminhada."
    ];

    function novaDica() {
      const random = Math.floor(Math.random() * dicas.length);
      document.getElementById("dica").innerText = dicas[random];
    }
  </script>

</body>
</html>
