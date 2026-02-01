# Baby
Trying to create website for my girl
main
<!DOCTYPE html>
<html>
<head>
  <title>Lovepreet 💘</title>
  <style>
    body {
      text-align: center;
      font-family: "Poppins", sans-serif;
      margin-top: 80px;
      background: black;
      color: white;
      overflow: hidden;
    }

    h1 {
      font-size: 42px;
      color: #ff4d6d;
    }

    p {
      font-size: 20px;
      margin-bottom: 40px;
    }

    button {
      font-size: 20px;
      padding: 12px 28px;
      margin: 15px;
      border: none;
      border-radius: 12px;
      cursor: pointer;
      transition: 0.2s;
    }

    #yesBtn {
      background: linear-gradient(135deg, #00ff99, #00ccff);
      color: black;
      font-weight: bold;
    }

    #noBtn {
      background: red;
      color: white;
      position: absolute;
    }
  </style>
</head>
<body>

<h1>Lovepreet 💖</h1>
<p>Het has only one question for you 😏</p>
<h2>Will you be my Valentine? 💋</h2>

<button id="yesBtn" onclick="yesClicked()">YES 😍</button>
<button id="noBtn">NO 💀</button>

<script>
  const noBtn = document.getElementById("noBtn");
  const messages = [
    "Nice try 😏",
    "You really thought you could say no? 😂",
    "Not happening 💀",
    "Run faster baby 😈",
    "You belong to Het 💋",
    "Say YES already 😌"
  ];

  noBtn.addEventListener("mouseover", function () {
    const x = Math.random() * (window.innerWidth - 120);
    const y = Math.random() * (window.innerHeight - 60);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
    noBtn.innerText = messages[Math.floor(Math.random() * messages.length)];
  });

  function yesClicked() {
    document.body.innerHTML = `
      <h1>Too late 😈💍</h1>
      <h2>You are officially Het’s Valentine 💖</h2>
      <p>No refunds. No returns. Lifetime warranty 😌</p>
      <h3>I love you, Lovepreet 💋</h3>
    `;
  }
</script>

</body>
</html>
