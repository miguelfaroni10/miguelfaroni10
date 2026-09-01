<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <style>
    body {
      background-color: #000000;
      color: #00ff66;
      font-family: 'Courier New', Courier, monospace;
      margin: 0;
      padding: 20px;
      overflow-x: hidden;
    }
    .matrix-card {
      position: relative;
      background: #050505;
      border: 1px solid #004411;
      border-radius: 8px;
      padding: 20px;
      box-shadow: 0 0 15px rgba(0, 255, 102, 0.2);
    }
      .matrix-card::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 4px;
      background: linear-gradient(90deg, transparent, #005511, #00ff66, #005511, transparent);
      background-size: 200% 100%;
      animation: borderGlow 3s infinite linear;
      border-bottom-left-radius: 8px;
      border-bottom-right-radius: 8px;
    }
    @keyframes borderGlow {
      0% { background-position: 200% 0; }
      100% { background-position: -200% 0; }
    }
    .matrix-text-fade {
      display: inline-block;
      animation: matrixFade 2s infinite ease-in-out alternate;
      color: #00ff66;
      text-shadow: 0 0 8px #00ff66;
    }
    @keyframes matrixFade {
      0% { opacity: 0.1; transform: translateY(-2px); }
      50% { opacity: 1; text-shadow: 0 0 12px #00ff66; }
      100% { opacity: 0.2; transform: translateY(2px); }
    }
  </style>
</head>
<body>

  <div class="matrix-card">
    <h2><span class="matrix-text-fade">SYS.MATRIX //</span> MIGUEL FARONI</h2>
    <p>curto uns programa dahora ai...</p>
  </div>

</body>
</html>
