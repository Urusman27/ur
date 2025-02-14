# ur<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>For My Rahmeen 💖</title>
  <style>
    /* General Styles */
    body {
      font-family: 'Arial', sans-serif;
      text-align: center;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      margin: 0;
      padding: 20px;
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: flex-start; /* Align to top for scrolling */
      overflow-y: auto; /* Allow vertical scrolling */
      position: relative;
    }

    .container {
      background: rgba(255, 255, 255, 0.9);
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
      max-width: 500px;
      width: 90%;
      animation: fadeIn 1s ease-in-out;
      position: relative;
      z-index: 1; /* Ensure container is above petals */
      margin: 20px 0; /* Add margin for better spacing */
    }

    h1 {
      color: #ff4d4d;
      font-size: 2.5rem;
      margin-bottom: 20px;
      animation: float 3s ease-in-out infinite;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
      margin-bottom: 20px;
    }

    button {
      background: #ff4d4d;
      color: white;
      border: none;
      padding: 15px 30px;
      font-size: 1.2rem;
      cursor: pointer;
      border-radius: 10px;
      transition: all 0.3s ease;
    }

    button:hover {
      background: #e60000;
      transform: scale(1.1);
    }

    .hidden {
      display: none;
    }

    .letter {
      margin-top: 20px;
      font-size: 1.1rem;
      color: #333;
      text-align: left;
      line-height: 1.6;
      animation: slideIn 1s ease-in-out;
    }

    .letter h2 {
      color: #ff4d4d;
      font-size: 1.8rem;
      margin-bottom: 10px;
    }

    .images {
      display: flex;
      justify-content: center;
      gap: 10px;
      margin-top: 20px;
    }

    img {
      width: 150px;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
      animation: popUp 1s ease-in-out;
    }

    .heart {
      position: absolute;
      top: -50px;
      left: 50%;
      transform: translateX(-50%);
      font-size: 3rem;
      color: #ff4d4d;
      animation: float 3s ease-in-out infinite;
    }

    .surprise {
      margin-top: 20px;
      font-size: 1.2rem;
      color: #ff4d4d;
      animation: blink 1.5s infinite;
    }

    /* Falling Rose Petals */
    .petal {
      position: fixed; /* Fixed position for petals */
      top: -10%;
      width: 20px;
      height: 20px;
      background-image: url('https://i.imgur.com/rose-petal.png'); /* Rose petal image */
      background-size: cover;
      animation: fall linear infinite;
      z-index: 0; /* Ensure petals are behind the container */
    }

    @keyframes fall {
      0% { transform: translateY(-10%) rotate(0deg); }
      100% { transform: translateY(110vh) rotate(360deg); }
    }

    /* Hello Kitty Animation */
    .hello-kitty {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 100px;
      height: 100px;
      background-image: url('https://i.imgur.com/hello-kitty.png'); /* Hello Kitty image */
      background-size: cover;
      animation: bounce 2s ease-in-out infinite;
    }

    @keyframes bounce {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }

    /* Animations */
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes slideIn {
      from { transform: translateY(20px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes popUp {
      0% { transform: scale(0); opacity: 0; }
      50% { transform: scale(1.2); opacity: 1; }
      100% { transform: scale(1); opacity: 1; }
    }

    @keyframes float {
      0% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
      100% { transform: translateY(0); }
    }

    @keyframes blink {
      0% { opacity: 1; }
      50% { opacity: 0.5; }
      100% { opacity: 1; }
    }
  </style>
</head>
<body>
  <!-- Falling Rose Petals -->
  <div class="petal" style="left: 10%; animation-duration: 8s;"></div>
  <div class="petal" style="left: 20%; animation-duration: 6s;"></div>
  <div class="petal" style="left: 30%; animation-duration: 10s;"></div>
  <div class="petal" style="left: 40%; animation-duration: 7s;"></div>
  <div class="petal" style="left: 50%; animation-duration: 9s;"></div>
  <div class="petal" style="left: 60%; animation-duration: 5s;"></div>
  <div class="petal" style="left: 70%; animation-duration: 8s;"></div>
  <div class="petal" style="left: 80%; animation-duration: 6s;"></div>
  <div class="petal" style="left: 90%; animation-duration: 7s;"></div>

  <!-- Hello Kitty -->
  <div class="hello-kitty"></div>

  <div class="container">
    <div class="heart">💖</div>
    <h1>Do You Love Me? 💌</h1>
    <div class="buttons">
      <button onclick="showLetter()">Yes 💖</button>
      <button onclick="showLetter()">Han 🌸</button>
      <button onclick="showLetter()">Hanji 🌹</button>
      <button onclick="showLetter()">G 🍫</button>
      <button onclick="showLetter()">G Zaroor 🍬</button>
      <button onclick="showLetter()">Of Course 💕</button>
      <button onclick="showLetter()">Always 💘</button>
      <button onclick="showLetter()">Forever 💍</button>
    </div>

    <div id="letter" class="hidden">
      <h2>My Dearest Rahmeen, 💖</h2>
      <p>
        From the moment I saw you, my heart knew it was you. You are the most beautiful soul I have ever met, and every day with you feels like a blessing. I love you more than words can ever express. I love the way you smile, the way you laugh, and the way you say my name, "Usman." It’s like music to my ears, and it makes my heart skip a beat every time. 💖
      </p>
      <p>
        You are my everything, Rahmeen. Your kindness, your strength, and the way you love me so deeply have changed my life forever. I can’t imagine a single day without you. You are my best friend, my partner, and my soulmate. I am so grateful for you, and I thank God every day for bringing you into my life. 🌸
      </p>
      <p>
        I want you to know that my love for you is endless. I dream of a future with you—a future where we are together, always. I want to wake up every morning with you by my side, and I want to fall asleep every night holding you close. I want to build a life with you, filled with love, laughter, and endless happiness. I want to marry you, Rahmeen, and spend the rest of my life making you feel loved, cherished, and adored. 💍
      </p>
      <p>
        You are my forever, and I promise to love you with all my heart, today and always. Happy Valentine’s Day, my love. I can’t wait to create so many beautiful memories with you. 💕
      </p>
      <p>With all my love,</p>
      <p>Usman 💌</p>
      <div class="images">
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRY7EKaZbxknzbbjYDJVJZaFB376PEqIrp4Fg&s" alt="Flowers"> <!-- Flower image -->
        <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTE_rzoig8DHp_lpeiG-M5ev2T42ajxKgkHeA&s"> <!-- Chocolate image -->
      </div>
      <div class="surprise">
        💖 You are my forever Valentine! 💖
      </div>
    </div>
  </div>

  <script>
    function showLetter() {
      const letter = document.getElementById('letter');
      letter.classList.remove('hidden');

      // Make Hello Kitty "speak"
      const message = new SpeechSynthesisUtterance("I love you, Rahmeen!");
      message.voice = speechSynthesis.getVoices().find(voice => voice.name === "Google US English");
      message.pitch = 1.5; // Higher pitch for a cute voice
      message.rate = 1.2; // Slightly faster speed
      speechSynthesis.speak(message);
    }

    // Create more rose petals dynamically
    for (let i = 0; i < 20; i++) {
      const petal = document.createElement('div');
      petal.classList.add('petal');
      petal.style.left = `${Math.random() * 100}%`;
      petal.style.animationDuration = `${Math.random() * 5 + 5}s`;
      document.body.appendChild(petal);
    }
  </script>
</body>
</html>
