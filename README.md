<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Perfil - Hadassa Micaele</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #fff5f8;
      color: #4a4a4a;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
    }

    .card {
      background: #ffffff;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 25px rgba(255, 182, 217, 0.4);
      max-width: 400px;
      text-align: center;
      border: 2px solid #ffb6d9;
    }

    h1 {
      color: #d63384;
      margin-bottom: 5px;
    }

    .subtitle {
      font-size: 0.9em;
      color: #888;
      margin-bottom: 20px;
    }

    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      justify-content: center;
      margin: 20px 0;
    }

    .tag {
      background-color: #ffb6d9;
      color: #fff;
      padding: 6px 14px;
      border-radius: 15px;
      font-size: 0.85em;
      font-weight: bold;
    }

    button {
      background-color: #d63384;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 25px;
      cursor: pointer;
      font-size: 0.9em;
      transition: background 0.3s;
    }

    button:hover {
      background-color: #b02a6b;
    }

    #mensagem {
      margin-top: 15px;
      font-style: italic;
      color: #d63384;
    }
  </style>
</head>
<body>

  <div class="card">
    <h1>💄 Hadassa Micaele ✨</h1>
    <p class="subtitle">💻 Estudante de Informática • 🌱 Em constante evolução</p>
    
    <p>Construindo minha jornada na programação e explorando o mundo da tecnologia!</p>

    <div class="skills">
      <span class="tag">Python</span>
      <span class="tag">Java</span>
      <span class="tag">HTML</span>
      <span class="tag">CSS</span>
      <span class="tag">JavaScript</span>
      <span class="tag">Sistemas Operacionais</span>
    </div>

    <button onclick="mostrarInspiracao()">Clique para uma frase 🌷</button>
    <p id="mensagem"></p>
  </div>

  <script>
    function mostrarInspiracao() {
      const frases = [
        "Todo grande desenvolvedor começou digitando 'Hello World'!",
        "A prática constante leva à evolução constante. 🌱",
        "Código limpo é como arte: bonito e funcional. ✨"
      ];
      const fraseAleatoria = frases[Math.floor(Math.random() * frases.length)];
      document.getElementById("mensagem").innerText = fraseAleatoria;
    }
  </script>

</body>
</html>
