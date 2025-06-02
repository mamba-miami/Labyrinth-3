<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Лабиринт Порталов</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      overflow: hidden;
      height: 100%;
    }

    body {
      font-family: 'Trebuchet MS', sans-serif;
      background-image: url('https://i.postimg.cc/XqNWJwbd/9YkjNIZ.png');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
      color: #e0e0ff;
    }

    header {
      text-align: center;
      padding: 30px;
      font-size: 2em;
      background: rgba(40, 10, 70, 0.7);
      box-shadow: 0 0 20px #a070ff;
      position: relative;
      z-index: 2;
      color: #ffdfff;
      text-shadow: 0 0 10px #ffbbff;
    }

    #portals-container {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      display: flex;
      gap: 60px;
      z-index: 3;
    }

    .portal {
      width: 100px;
      height: 100px;
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      font-weight: bold;
      color: white;
      text-decoration: none;
      font-size: 0.9em;
      position: relative;
      transition: transform 0.3s ease;
      cursor: pointer;
      animation: pulse 3s infinite ease-in-out;
      overflow: hidden;
    }

    .portal:hover {
      transform: scale(1.1);
    }

    .portal::after {
      content: attr(data-tooltip);
      position: absolute;
      bottom: 120%;
      left: 50%;
      transform: translateX(-50%);
      background: rgba(0, 0, 0, 0.8);
      padding: 8px 12px;
      border-radius: 8px;
      font-size: 0.8em;
      opacity: 0;
      pointer-events: none;
      transition: opacity 0.3s ease;
      white-space: nowrap;
    }

    .portal:hover::after {
      opacity: 1;
    }

    @keyframes pulse {
      0%, 100% {
        transform: scale(1);
        box-shadow: 0 0 15px rgba(255,255,255,0.3);
      }
      50% {
        transform: scale(1.08);
        box-shadow: 0 0 30px rgba(255,255,255,0.6);
      }
    }

    .portal::before {
      content: '';
      position: absolute;
      width: 120%;
      height: 120%;
      border-radius: 50%;
      background: inherit;
      filter: blur(3px);
      animation: swirl 5s infinite linear;
      z-index: -1;
    }

    @keyframes swirl {
      0% {
        transform: rotate(0deg) scale(1.05);
      }
      100% {
        transform: rotate(360deg) scale(1.05);
      }
    }

    /* Стихии */
    .light {
      background: radial-gradient(circle at center, #fffce6, #b00040 70%, #400020);
      box-shadow: 0 0 20px #ff99bb, 0 0 40px #ff3377;
    }

    .electric {
      background: radial-gradient(circle at center, #ccffff, #003366 70%, #000022);
      box-shadow: 0 0 20px #66ffff, 0 0 40px #00ccff;
    }

    .earth {
      background: radial-gradient(circle at center, #e4ffcc, #4a3f28 70%, #1a130a);
      box-shadow: 0 0 20px #aaff88, 0 0 35px #5f5f2a;
    }

    /* Снежинки */
    .star {
      position: absolute;
      width: 2px;
      height: 2px;
      background: white;
      border-radius: 50%;
      opacity: 0.6;
      animation: snowfall linear infinite;
    }

    @keyframes snowfall {
      0% {
        transform: translateY(-10px);
        opacity: 0;
      }
      10% {
        opacity: 0.6;
      }
      100% {
        transform: translateY(110vh);
        opacity: 0;
      }
    }

    /* Кнопка запуска */
    #start-button {
      position: absolute;
      top: 75%;
      left: 50%;
      transform: translateX(-50%);
      padding: 15px 25px;
      font-size: 1.2em;
      background: rgba(0, 0, 0, 0.7);
      color: #fff0f5;
      border: 2px solid #ff66cc;
      border-radius: 12px;
      cursor: pointer;
      z-index: 10;
      box-shadow: 0 0 12px #ff99cc;
      transition: all 0.3s ease;
    }

    #start-button:hover {
      background: #ff66cc;
      color: black;
    }
  </style>
</head>
<body>

  <header>✨ Лабиринт Порталов ✨</header>

  <div id="portals-container">
    <a href="#" class="portal light" data-tooltip="Тайный алтарь света и чувственности">Храм<br>Алой Жрицы</a>
    <a href="#" class="portal electric" data-tooltip="Кибер-глаз в инфосферу">Всевидящее<br>Око</a>
    <a href="#" class="portal earth" data-tooltip="Убежище бывших птеродактилей">Лагерь<br>Птеродактилей</a>
  </div>

  <button id="start-button">🔮 Войти в Лабиринт</button>

  <!-- Аудио -->
  <audio id="bg-music" loop>
    <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
  </audio>
  <audio id="hover-sound">
    <source src="https://www.soundjay.com/button/sounds/button-16.mp3" type="audio/mpeg">
  </audio>
  <audio id="click-sound">
    <source src="https://www.soundjay.com/button/sounds/button-09.mp3" type="audio/mpeg">
  </audio>

  <script>
    // Снежинки
    for (let i = 0; i < 100; i++) {
      const star = document.createElement("div");
      star.className = "star";
      star.style.left = Math.random() * window.innerWidth + "px";
      star.style.animationDuration = (10 + Math.random() * 20) + "s";
      star.style.animationDelay = Math.random() * 10 + "s";
      document.body.appendChild(star);
    }

    const bgMusic = document.getElementById("bg-music");
    const hoverSound = document.getElementById("hover-sound");
    const clickSound = document.getElementById("click-sound");
    const startButton = document.getElementById("start-button");

    startButton.addEventListener("click", () => {
      bgMusic.volume = 0.3;
      bgMusic.play();
      startButton.style.display = "none";
    });

    document.querySelectorAll('.portal').forEach(portal => {
      portal.addEventListener("mouseenter", () => {
        hoverSound.volume = 0.3;
        hoverSound.currentTime = 0;
        hoverSound.play();
      });

      portal.addEventListener("click", () => {
        clickSound.volume = 0.5;
        clickSound.currentTime = 0;
        clickSound.play();
      });
    });
  </script>

</body>
</html>
