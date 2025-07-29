<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Typing Animation</title>
  <style>
    body {
      background-color: #0f0f0f;
      color: #fff;
      font-family: 'Courier New', monospace;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
    }
    .typing-container {
      text-align: center;
      white-space: nowrap;
      overflow: hidden;
      border-right: 2px solid #fff;
      font-size: 1.5rem;
      width: 0;
      animation: typing 3s steps(40, end) forwards, blink 0.75s step-end infinite;
    }

    @keyframes typing {
      from { width: 0 }
      to { width: 100% }
    }

    @keyframes blink {
      50% { border-color: transparent }
    }

    .line {
      display: none;
    }

    .line.show {
      display: block;
      animation: typing 3s steps(40, end) forwards, blink 0.75s step-end infinite;
    }
  </style>
</head>
<body>

  <div class="typing-container line" id="line1">
    Cyber Security Student | Ethical Hacking Enthusiast
  </div>
  <div class="typing-container line" id="line2">
    🌟 Dreaming Big | Learning Daily 🧚
  </div>
  <div class="typing-container line" id="line3">
    🚀 Welcome to my tech space! 🚀
  </div>

  <script>
    const lines = document.querySelectorAll('.line');

    function showLine(index) {
      if (index < lines.length) {
        lines[index].classList.add('show');
        setTimeout(() => {
          showLine(index + 1);
        }, 4000); // Wait before showing next line
      }
    }

    showLine(0);
  </script>

</body>
</html>
