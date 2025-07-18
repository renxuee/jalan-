<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Gombalan Buat Kamu</title>
  <style>
    body {
      background-color: #ffe6f0;
      font-family: 'Comic Sans MS', cursive;
      text-align: center;
      margin-top: 100px;
    }
    .gombal {
      font-size: 24px;
      color: #d63384;
      margin-bottom: 20px;
    }
    button {
      padding: 10px 20px;
      background-color: #ff69b4;
      border: none;
      border-radius: 10px;
      font-size: 18px;
      color: white;
      cursor: pointer;
    }
    button:hover {
      background-color: #ff1493;
    }
  </style>
</head>
<body>

  <div class="gombal" id="gombalan">Klik tombol di bawah untuk dapetin gombalan spesial ❤️</div>
  <button onclick="gombalin()">Gombalin Aku!</button>

  <script>
    const gombalanList = [
      "Kamu tahu nggak bedanya kamu sama bintang? Bintang cuma ada di langit, tapi kamu ada di hatiku ⭐❤️",
      "Aku gak butuh matahari lagi... soalnya senyum kamu udah cukup nerangin hariku ☀️😊",
      "Kalau kamu jadi angka, kamu pasti angka 1. Soalnya kamu yang pertama di hatiku 💘",
      "Kamu tahu gak kenapa aku nggak bisa tidur? Soalnya kamu terus ada di pikiranku 😴💕",
      "Kalau kamu jadi huruf, kamu pasti huruf U... karena kamu selalu ada di U-bun pikiranku! 😄"
    ];

    function gombalin() {
      const randomIndex = Math.floor(Math.random() * gombalanList.length);
      document.getElementById("gombalan").innerText = gombalanList[randomIndex];
    }
  </script>

</body>
</html>

