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
      background-color: #f3e5f5;
    }

    h1 {
      font-size: 2em;
      color: #6a1b9a;
    }

    .btn {
      padding: 15px 30px;
      font-size: 20px;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: 0.2s ease-in-out;
    }

    #yesBtn {
      background-color: #66bb6a;
      color: white;
    }

    #noBtn {
      background-color: #ef5350;
      color: white;
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

    noBtn.addEventListener('click', function() {
      yesFontSize += 10;
      yesBtn.style.fontSize = yesFontSize + 'px';

      if (yesFontSize >= 60) {
        alert("Udah deh, bilang 'iya' aja 😆");
      }
    });

    yesBtn.addEventListener('click', function() {
      alert("Awww, Oke Gas! ");
    });
  </script>

</body>
</html>
