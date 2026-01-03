<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>To My Favorite Nonchalant Person</title>

  <style>
    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: linear-gradient(135deg, #fff6cc, #fffbea);
      font-family: "Segoe UI", sans-serif;
      color: #3b3b3b;
    }

    .card {
      background: #ffffff;
      padding: 35px 40px;
      border-radius: 18px;
      max-width: 500px;
      width: 90%;
      text-align: center;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    }

    h2 {
      margin-top: 0;
      color: #e3b300;
      font-weight: 600;
    }

    p {
      line-height: 1.6;
      margin: 15px 0;
      font-size: 15px;
    }

    button {
      background: #ffd84d;
      border: none;
      border-radius: 25px;
      padding: 12px 22px;
      margin: 12px 6px;
      font-size: 14px;
      cursor: pointer;
      transition: all 0.25s ease;
      box-shadow: 0 4px 10px rgba(0,0,0,0.1);
    }

    button:hover {
      background: #ffcf2f;
      transform: translateY(-2px);
      box-shadow: 0 6px 14px rgba(0,0,0,0.15);
    }

    #hiddenMessage {
      margin-top: 20px;
      font-size: 16px;
      color: #e3b300;
      font-weight: 600;
      animation: fadeIn 0.8s ease forwards;
    }

    footer {
      margin-top: 30px;
      font-size: 12px;
      color: #999;
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
        transform: translateY(5px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
  </style>
</head>

<body>

  <div class="card">

    <h2>To My Favorite Nonchalant Person ☝️</h2>

    <p>
      Happy <strong>2 months</strong> with you, my Nonchalant.<br>
      Even when you act calm and unbothered, you are my favorite person.
    </p>

    <p>
      Just like this song, everything feels brighter with you.<br>
      Thank you for choosing me every day 🤍
    </p>

    <!-- 🎵 Music -->
    <audio id="bgMusic" loop>
      <source src="music/yellow.mp3" type="audio/mpeg">
    </audio>

    <button onclick="toggleMusic()">Pause / Play Music 🎶</button>

    <p id="hiddenMessage" style="display:none;">
      You're my yellow 💛
    </p>

    <button onclick="showMessage()">Click Me 💗</button>

    <footer>
      Made by your Favorite QA Person
    </footer>

  </div>

  <script>
    const music = document.getElementById("bgMusic");

    function toggleMusic() {
      if (music.paused) {
        music.play();
      } else {
        music.pause();
      }
    }

    function showMessage() {
      document.getElementById("hiddenMessage").style.display = "block";
    }
  </script>

</body>
</html>
