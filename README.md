# me
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Important Question 💖</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #ffd6e8, #e9d6ff);
      overflow-x: hidden;
      text-align: center;
    }

    .container {
      max-width: 700px;
      margin: auto;
      padding: 60px 20px;
    }

    h1 {
      font-size: 2.5rem;
      color: #ff4d88;
    }

    p {
      font-size: 1.1rem;
      color: #444;
      line-height: 1.6;
    }

    .card {
      background: white;
      border-radius: 20px;
      padding: 30px;
      margin: 30px 0;
      box-shadow: 0 10px 30px rgba(0,0,0,0.1);
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 20px;
      flex-wrap: wrap;
    }

    button {
      font-size: 1.2rem;
      padding: 15px 30px;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      background: #ff4d88;
      color: white;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    button:hover {
      transform: scale(1.1) rotate(-2deg);
      box-shadow: 0 10px 20px rgba(0,0,0,0.2);
    }

    .footer {
      margin-top: 40px;
      font-size: 0.9rem;
      color: #555;
    }

    /* Floating hearts */
    .heart {
      position: fixed;
      bottom: -20px;
      font-size: 20px;
      animation: floatUp 6s linear infinite;
      opacity: 0.7;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) scale(1);
        opacity: 0.7;
      }
      100% {
        transform: translateY(-110vh) scale(1.5);
        opacity: 0;
      }
    }
  </style>
</head>
<body>

  <div class="container">
    <h1>Okay… this is me being brave 😳💖</h1>
    <p><em>Please appreciate the effort, I made a whole website and everything 😂</em></p>

    <div class="card">
      <p>
        So here’s the thing…<br>
        I like you.<br><br>
        And instead of overthinking it for 3–5 business years,
        I decided to do this ✨<br><br>
        You’re fun, you make me smile,
        and honestly… I’d love to hang out with you 🌸
      </p>
    </div>

    <div class="card">
      <h2>Would you like to go out with me sometime? 💌</h2>
      <p>(Yes, this is the official question 😌)</p>

      <div class="buttons">
        <button onclick="celebrate()">YES 😍</button>
        <button onclick="celebrate()">Obviously YES 💖</button>
      </div>

      <p style="margin-top:15px; font-size:0.9rem;">
        There is no “no” button because optimism ✨😂
      </p>
    </div>

    <div class="footer">
      Worst case scenario: you smile.<br>
      Best case scenario: we go on a cute date 🌸💘
    </div>
  </div>

  <script>
    function celebrate() {
      alert("YAY 💖✨ I knew it!!");

      for (let i = 0; i < 30; i++) {
        createHeart();
      }
    }

    function createHeart() {
      const heart = document.createElement("div");
      heart.className = "heart";
      heart.innerText = "💖";
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.animationDuration = (Math.random() * 3 + 3) + "s";
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    // background hearts
    setInterval(createHeart, 500);
  </script>

</body>
</html>
