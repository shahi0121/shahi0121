<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dreamy Wardrobe Intro</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body, html {
      height: 100%;
      overflow: hidden;
    }

    .bg {
      background: url('https://i.gifer.com/origin/3e/3e00bb53f158dc21fda8db30f7ab4ba1.gif') no-repeat center center/cover;
      height: 100vh;
      width: 100%;
      position: relative;
    }

    .overlay {
      background-color: rgba(0, 0, 0, 0.6);
      height: 100%;
      width: 100%;
      position: absolute;
      top: 0;
      left: 0;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      color: white;
      text-align: center;
      padding: 0 20px;
    }

    .line {
      opacity: 0;
      transform: translateY(20px);
      animation: fadeInUp 1s ease forwards;
    }

    .line:nth-child(1) {
      animation-delay: 0.5s;
    }

    .line:nth-child(2) {
      animation-delay: 1.5s;
    }

    .line:nth-child(3) {
      animation-delay: 2.5s;
    }

    @keyframes fadeInUp {
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .line h2 {
      font-size: 1.8rem;
      margin-bottom: 20px;
    }

    @media (min-width: 768px) {
      .line h2 {
        font-size: 2.5rem;
      }
    }
  </style>
</head>
<body>
  <div class="bg">
    <div class="overlay">
      <div class="line"><h2>Cyber Security Student | Ethical Hacking Enthusiast</h2></div>
      <div class="line"><h2>🌟 Dreaming Big | Learning Daily 🧚</h2></div>
      <div class="line"><h2>🚀 Welcome to my tech space! 🚀</h2></div>
    </div>
  </div>
</body>
</html>
