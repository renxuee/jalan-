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
      padding: 15px 30px;
    }

    #noBtn {
      background-color: #e53935;
      color: white;
      padding: 15px 30px;
    }

    .hidden {
      display: none;
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

    let yesSize = 20; // ukuran awal font Yes
    let noSize = 20;  // ukuran awal font No

    noBtn.addEventListener('click', function () {
      // Perbesar tombol Yes
      yesSize += 10;
      yesBtn.style.fontSize = yesSize + 'px';
      yesBtn.style.padding = (yesSize / 2) + 'px ' + (yesSize) + 'px';

      // Perkecil tombol No
      if (noSize > 5) {
        noSize -= 3;
        noBtn.style.fontSize = noSize + 'px';
        noBtn.style.padding = (noSize / 2) + 'px ' + (noSize) + 'px';
      }

      // Hilangkan tombol No jika sudah terlalu kecil
      if (noSize <= 5) {
        noBtn.classList.add('hidden');
      }
    });

    yesBtn.addEventListener('click', function () {
      alert("Yayyy! Kita jalan bareng 🥳💖");
    });
  </script>

</body>
</html>
