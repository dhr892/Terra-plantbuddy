# Terra-plantbuddy
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Terra's Plant Buddy Picker</title>
  <style>
    body {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      background-color: #fef8ec;
      color: #444;
      text-align: center;
      padding: 20px;
    }
    h1 {
      color: #3cba54;
    }
    .character {
      border: 2px dashed #ffcc00;
      border-radius: 20px;
      padding: 15px;
      margin: 15px;
      cursor: pointer;
      transition: transform 0.3s;
    }
    .character:hover {
      transform: scale(1.05);
      background-color: #fff9dc;
    }
    .message {
      margin-top: 30px;
      font-size: 1.2em;
    }
  </style>
</head>
<body>
  <h1>🌱 Welcome to Terra's Plant World! 🌱</h1>
  <p>Pick your plant buddy below:</p>

  <div class="character" onclick="showMessage('puffyleaf')">
    🚀 <strong>Captain PuffyLeaf</strong> – The brave space explorer
  </div>
  <div class="character" onclick="showMessage('cactusella')">
    👑 <strong>Princess Cactusella</strong> – The diva of desert royalty
  </div>
  <div class="character" onclick="showMessage('chonk')">
    ⚔️ <strong>Sir Chonk-a-Lot</strong> – The round knight of succulent kingdom
  </div>
  <div class="character" onclick="showMessage('dewdrop')">
    🔍 <strong>Detective Dewdrop</strong> – Solves the mystery of dry soil
  </div>

  <div class="message" id="message"></div>

  <script>
    const messages = {
      puffyleaf: `👨‍🚀 Hello, young explorer! I’m <strong>Captain PuffyLeaf</strong> from Planet Succulenton!<br><br>
      🚀 Mission: <em>Operation Plant Protector</em> has begun!<br>
      🌞 Put me near a bright window – I love sunlight!<br>
      💧 Every 3 days, check if the soil feels dry. Then spray me! But only a little – too much water makes my boots soggy!<br>
      ❗ Never pour water on my head – that's where my thinking cap is!<br><br>
      🌟 You’ve been trained by <strong>Terra</strong>, the coolest green team in the galaxy!`,

      cactusella: `👑 Greetings, darling! I’m <strong>Princess Cactusella</strong> of Succulent Palace!<br><br>
      💄 I love the spotlight – keep me in bright, sunny places.<br>
      💦 Spray me gently every few days, only when the soil feels dry. I’m delicate – no splashes on my face, please!<br>
      👗 Keep me in a dry pot with pretty soil that drains quickly.<br><br>
      💚 I only trust the fabulous team at <strong>Terra</strong> to care for me!`,

      chonk: `⚔️ Greetings, brave squire! I’m <strong>Sir Chonk-a-Lot</strong>, protector of the Green Realm!<br><br>
      🛡️ My round armor needs light! Keep me near the window of destiny!<br>
      💧 Spray me with your magic bottle when the soil is dry – not soggy!<br>
      🏰 My royal roots like cozy, dry soil. No floods in my kingdom!<br><br>
      🌟 You’ve joined the Knights of <strong>Terra</strong> – the guardians of green!`,

      dewdrop: `🔍 Hello detective! I’m <strong>Detective Dewdrop</strong>, solving the mystery of dry plants!<br><br>
      🕵️ Step 1: Observe! Is the soil dry? Yes? Time to spray – just a little!<br>
      🕯️ Step 2: Clues! My leaves must stay dry. Don’t water them directly!<br>
      🧠 Step 3: Place me where it’s bright – that’s where my best thinking happens!<br><br>
      🕵️‍♂️ You’re now a certified agent of <strong>Terra</strong> – Mission Plant Possible!`
    };

    function showMessage(character) {
      document.getElementById("message").innerHTML = messages[character];
    }
  </script>
</body>
</html>
