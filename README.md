<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Не обижайся, Махаббат</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      height: 100vh;
      background: linear-gradient(145deg, #1f1f1f, #2c2c2c);
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    .message {
      color: #ffffff;
      font-size: 3rem;
      font-weight: bold;
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 2s ease forwards;
      animation-delay: 0.5s;
      text-align: center;
      text-shadow: 0 0 10px rgba(255,255,255,0.2);
    }

    .button {
      margin-top: 30px;
      padding: 12px 24px;
      font-size: 1.2rem;
      background-color: #4CAF50;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 2s ease forwards;
      animation-delay: 2s;
      transition: background-color 0.3s ease;
    }

    .button:hover {
      background-color: #45a049;
    }

    @keyframes fadeInUp {
      0% {
        opacity: 0;
        transform: translateY(20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }

    @media (max-width: 600px) {
      .message {
        font-size: 2rem;
        padding: 0 20px;
      }

      .button {
        font-size: 1rem;
        padding: 10px 20px;
      }
    }
  </style>
</head>
<body>
  <div class="message">Не обижайся, Махаббат</div>
  <button class="button" onclick="handleForgive()">Я тебя прощаю</button>

  <script>
    function handleForgive() {
      const msg = document.querySelector('.message');
      msg.textContent = 'Спасибо 💖';
    }
  </script>
</body>
</html>
