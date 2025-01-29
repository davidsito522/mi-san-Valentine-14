<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Te amo mucho, mi amor</title>
  <style>
    /* Estiliza el cuerpo */
    body {
      margin: 0;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      font-family: 'Arial', sans-serif;
      color: white;
      overflow: hidden;
      text-align: center;
    }

    /* Contenedor principal */
    .container {
      position: relative;
      z-index: 2;
    }

    h1 {
      font-size: 2.5em;
      text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
    }

    .button {
      background-color: #f06292;
      border: none;
      padding: 15px 30px;
      color: white;
      font-size: 1em;
      cursor: pointer;
      margin-top: 20px;
      border-radius: 30px;
      box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.2);
    }

    .button:hover {
      background-color: #e91e63;
      transform: scale(1.05);
    }

    /* Animación tulipanes */
    .tulip {
      position: absolute;
      width: 50px;
      height: 100px;
      background: url('https://i.imgur.com/rUMH9Yk.png') no-repeat center/contain;
      animation: floatTulips 6s infinite;
      opacity: 0.7;
    }

    /* Posición aleatoria de tulipanes */
    @keyframes floatTulips {
      0% {
        transform: translateY(100vh) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(-20vh) rotate(360deg);
        opacity: 0;
      }
    }

    /* Tulipanes distribuidos aleatoriamente */
    .tulip:nth-child(1) { left: 10%; animation-duration: 5s; }
    .tulip:nth-child(2) { left: 30%; animation-duration: 6s; }
    .tulip:nth-child(3) { left: 50%; animation-duration: 7s; }
    .tulip:nth-child(4) { left: 70%; animation-duration: 4.5s; }
    .tulip:nth-child(5) { left: 90%; animation-duration: 5.5s; }

  </style>

  <script>
    function changeMessage() {
      document.querySelector("h1").innerText = "¿Quieres ser mi San Valentín?";
      document.querySelector(".button").style.display = "none";
    }
  </script>
</head>
<body>
  <div class="container">
    <h1>Te amo mucho, mi amor</h1>
    <button class="button" onclick="changeMessage()">Click aquí</button>
  </div>

  <!-- Tulipanes flotantes -->
  <div class="tulip"></div>
  <div class="tulip"></div>
  <div class="tulip"></div>
  <div class="tulip"></div>
  <div class="tulip"></div>
</body>
</html>
