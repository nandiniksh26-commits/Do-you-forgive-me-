<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Do You Forgive Me?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ffdde1, #ee9ca7);
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0;
    }

    .container {
      text-align: center;
      background: white;
      padding: 40px;
      border-radius: 16px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
      max-width: 400px;
      width: 90%;
    }

    h1 {
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      gap: 20px;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
    }

    button {
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    #yesBtn {
      background: #4CAF50;
      color: white;
      font-size: 18px;
      padding: 15px 30px;
    }

    #noBtn {
      background: #f44336;
      color: white;
      font-size: 18px;
      padding: 15px 30px;
    }

    .message {
      margin-top: 30px;
      font-size: 28px;
      display: none;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1 id="question">Will you forgive madmax?</h1>

    <div class="buttons" id="buttons">
      <button id="yesBtn">Yes 😊</button>
      <button id="noBtn">No 😢</button>
    </div>

    <div class="message" id="message">😊💖 Thank you! 💖😊</div>
  </div>

  <script>
    const yesBtn = document.getElementById('yesBtn');
    const noBtn = document.getElementById('noBtn');
    const message = document.getElementById('message');
    const buttons = document.getElementById('buttons');
    const question = document.getElementById('question');

    let yesSize = 1;

    yesBtn.addEventListener('click', () => {
      buttons.style.display = 'none';
      question.style.display = 'none';
      message.style.display = 'block';
    });

    noBtn.addEventListener('click', () => {
      yesSize += 0.3;
      yesBtn.style.transform = `scale(${yesSize})`;

      noBtn.textContent = 'Are you sure? 😬';

      // If yes button gets too big, hide the no button
      if (yesSize > 2.5) {
        noBtn.style.display = 'none';
      }
    });
  </script>
</body>
</html>
