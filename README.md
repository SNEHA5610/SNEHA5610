<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Happy New Year Wishes</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #ffefd5;
      padding: 50px;
    }
    .gift-container {
      margin-top: 50px;
      cursor: pointer;
    }
    .gift-box {
      width: 150px;
      height: 150px;
      background-color: #ff6347;
      position: relative;
      margin: 0 auto;
      border-radius: 10px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
    }
    .gift-box::before,
    .gift-box::after {
      content: '';
      position: absolute;
      background-color: #fff;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    .gift-box::before {
      width: 100%;
      height: 20px;
    }
    .gift-box::after {
      width: 20px;
      height: 100%;
    }
    .message {
      display: none;
      margin-top: 20px;
      font-size: 1.5rem;
      color: #333;
    }
    .reveal .message {
      display: block;
    }
  </style>
</head>
<body>
  <h1>🎉 Happy New Year 2025! 🎉</h1>
  <p>Click on the gift below to reveal your New Year wish!</p>
  <div class="gift-container" onclick="showMessage()">
    <div class="gift-box"></div>
  </div>
  <div class="message" id="message">✨ Wishing you a year full of joy, success, and prosperity! ✨</div>

  <script>
    function showMessage() {
      document.querySelector('.gift-container').classList.add('reveal');
    }
  </script>
</body>
</html>
