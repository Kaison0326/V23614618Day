<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Valentine's Day Surprise</title>
  <style>
    body {
      font-family: 'Georgia', serif;
      background: url('love-writing-hearts-composition.jpg') no-repeat center center fixed;
      background-size: cover;
      text-align: center;
      margin: 0;
      padding: 0;
      position: relative;
      overflow: hidden;
      color: white;
    }
    .heart {
      color: red;
      font-size: 100rem;
      animation: heartbeat 1s infinite;
    }
    @keyframes heartbeat {
      0% { transform: scale(1); }
      50% { transform: scale(1.2); }
      100% { transform: scale(1); }
    }
    h1 {
      font-size: 4rem;
      color: #ff99cc;
      text-shadow: 2px 2px 4px #b30000;
      margin-top: 20px;
    }
    p {
      font-size: 2rem;
      color: #ff99cc;
      text-shadow: 1px 1px 2px #b30000;
      margin: 20px;
    }
    .envelope-container {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }
    .envelope {
      width: 250px;
      height: 150px;
      background: #ff6699;
      position: relative;
      border-radius: 10px;
      cursor: pointer;
      transition: transform 0.2s;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }
    .envelope:hover {
      transform: scale(1.1);
    }
    .button {
      background-color: #ff6699;
      color: white;
      padding: 15px 30px;
      text-decoration: none;
      border-radius: 5px;
      cursor: pointer;
      display: inline-block;
      margin-top: 20px;
      font-size: 1.5rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }
    .letter-container {
      padding: 40px;
    }
    .hidden {
      display: none;
    }
    .surprise-gif {
      max-width: 100%;
      height: auto;
      border: 4px solid #ff99cc;
      border-radius: 15px;
      box-shadow: 0 8px 12px rgba(0, 0, 0, 0.2);
    }
    .large-image {
      width: 500px;
      max-width: 80vw;
      height: auto;
    }
    #no-btn {
      position: absolute;
      transition: all 0.2s ease;
    }
    #options {
      position: relative;
    }
    .falling-heart {
      position: absolute;
      width: 40px;
      height: 40px;
      background: url('https://i.imgur.com/kLGNDM4.png') no-repeat center;
      background-size: contain;
      animation: fall 3s infinite;
    }
    @keyframes fall {
      0% { transform: translateY(-100px); opacity: 1; }
      100% { transform: translateY(100vh); opacity: 0; }
    }
    audio {
      margin-top: 20px;
      width: 80%;
      max-width: 500px;
    }
    .dynamic-yes {
      position: absolute;
      background-color: #ff6699;
      color: white;
      padding: 10px 20px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }
  </style>
</head>
<body>
  <!-- Falling hearts animation -->
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Romantic Heart Transition</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .heart {
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: red;
      transform: rotate(-45deg);
      animation: float 5s infinite;
    }

    /* Heart shape using pseudo-elements */
    .heart::before,
    .heart::after {
      content: '';
      position: absolute;
      width: 20px;
      height: 20px;
      background-color: red;
      border-radius: 50%;
    }

    .heart::before {
      top: -10px;
      left: 0;
    }

    .heart::after {
      left: 10px;
      top: 0;
    }

    @keyframes float {
      0% {
        transform: translateY(0px) rotate(-45deg);
        opacity: 1;
      }
      50% {
        opacity: 0.7;
      }
      100% {
        transform: translateY(-600px) rotate(-45deg);
        opacity: 0;
      }
    }

    /* Heart Animation Generator */
    @keyframes randomMove {
      0% {
        transform: translateX(0);
      }
      50% {
        transform: translateX(100px);
      }
      100% {
        transform: translateX(0);
      }
    }
  </style>
  <script>
    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('heart');
      document.body.appendChild(heart);
      
      const leftPos = Math.random() * 100;
      heart.style.left = leftPos + "vw";
      heart.style.animationDuration = Math.random() * 3 + 3 + "s";

      setTimeout(() => {
        heart.remove();
      }, 5000);
    }

    setInterval(createHeart, 300);
  </script>

  <!-- Music Player on Page 1 -->
  <div id="page1" class="envelope-container">
    <div class="envelope" onclick="playMusicAndOpenLetter()">
      <p style="font-size: 1.5rem; color: white; text-align: center;">To : <br>SHRYA CHETTY</br></p>
    </div>
  </div>

  <audio id="background-music" preload="auto">
    <source src=""D:\Die With A Smile.mp3"" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <div id="page2" class="letter-container hidden">
    <h1>To the Most Special Girl <span class="heart">❤</span></h1>
    <p>Shrya, my love, words cannot fully express how much you mean to me. Your laughter is the sweetest music to my soul, and your presence fills every moment with warmth and meaning. You are my greatest treasure, my rock, and my inspiration.

As I reflect on this day and what it signifies, I feel incredibly blessed to have you in my life. You have brought so much light, joy, and beauty into my world—more than I could ever have dreamed. Every moment with you feels like a gift, one I know I don't deserve but will cherish always.They say love is something that can't be fully explained—it is something you feel, something that grows over time. And every single day, I feel it for you in ways that words just can’t capture. Though nothing in life is ever certain, I know one thing for sure I will love you as long as I possibly can, And as I ask you this, my heart is filled with hope and the greatest amount of joy:</p>
    <button class="button" onclick="goToPage3()">Next</button>
  </div>

  <div id="page3" class="hidden">
    <h1>Will you be my Valentine?</h1>
    <div id="options">
      <button class="button" onclick="handleYesClick()">Yes</button>
      <button class="button" id="no-btn" onclick="handleNoClick()">No</button>
    </div>
  </div>

  <div id="page4" class="hidden">
    <h1>You said YES! This is from me to you!</h1>
    <img src=""D:\DALL·E 2025-02-04 16.07.36 - A romantic and heartwarming scene featuring two cute bears in a beautiful garden at sunset. The bear on the left, representing the boy, has the name '.webp"
" alt="Romantic Bears Scene">
  </div>

  <script>
    function playMusicAndOpenLetter() {
      const music = document.getElementById('background-music');
      music.play();
      document.getElementById('page1').classList.add('hidden');
      document.getElementById('page2').classList.remove('hidden');
    }

    function goToPage3() {
      document.getElementById('page2').classList.add('hidden');
      document.getElementById('page3').classList.remove('hidden');
    }

    function handleYesClick() {
      document.getElementById('page3').classList.add('hidden');
      document.getElementById('page4').classList.remove('hidden');
    }

    let yesButtonCount = 1;
    const noButton = document.getElementById('no-btn');

    function handleNoClick() {
      for (let i = 0; i < yesButtonCount; i++) {
        const yesButton = document.createElement('button');
        yesButton.innerText = 'Yes';
        yesButton.classList.add('dynamic-yes');
        yesButton.style.left = `${Math.random() * 80}vw`;
        yesButton.style.top = `${Math.random() * 60}vh`;
        yesButton.onclick = handleYesClick;
        document.getElementById('options').appendChild(yesButton);
      }
      yesButtonCount *= 2;
    }
  </script>
</body>
</html>
