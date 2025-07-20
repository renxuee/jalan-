<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Mau Jalan Ga Sama Aku?</title>
  <style>
    body {
      font-family: sans-serif;
      text-align: center;
      padding-top: 100px;
      background-color: #fce4ec;
    }

    h1 {
      font-size: 2em;
      color: #ad1457;
    }

    .btn {
      padding: 15px 30px;
      font-size: 20px;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease-in-out;
    }

    #yesBtn {
      background-color: #43a047;
      color: white;
    }

    #noBtn {
      background-color: #e53935;
      color: white;
    }

    .hidden {
      opacity: 0;
      transform: scale(0);
      pointer-events: none;
    }
  </style>
</head>
<body>

  <h1>Mau jalan ga sama aku? 😳</h1>
  <button id="yesBtn" class="btn">Yes 🥰</button>
  <button id="noBtn" class="btn">No 😅</button>

  <script>
    const yesBtn = document.getElementById('yesBtn');
    const noBtn = document.getElementById('noBtn');

    let yesFontSize = 20;
    let noFontSize = 20;

    noBtn.addEventListener('click', function () {
      // Perbesar tombol Yes
      yesFontSize += 10;
      yesBtn.style.fontSize = yesFontSize + 'px';

      // Perkecil tombol No
      if (noFontSize > 5) {
        noFontSize -= 3;
        noBtn.style.fontSize = noFontSize + 'px';
        noBtn.style.padding = (noFontSize / 2) + 'px ' + (noFontSize) + 'px';
      }

      // Hilang

