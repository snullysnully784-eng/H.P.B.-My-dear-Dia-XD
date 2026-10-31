<!DOCTYPE html>  
<html lang="ckb" dir="rtl">  
<head>  
  <meta charset="UTF-8">  
  <meta name="viewport" content="width=device-width, initial-scale=1.0">  
  <title>یادی ١٨ ساڵیت پیرۆز دیە گیان 🎀</title>  
  <style>  
    :root {  
      --bg-color: #fff0f5;  
      --card-bg: #ffffff;  
      --primary: #ff69b4;  
      --primary-dark: #ff1493;  
      --accent: #ffb6c1;  
      --text: #4a4a4a;  
    }  
      
    body {  
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;  
      background-color: var(--bg-color);  
      color: var(--text);  
      margin: 0;  
      padding: 0;  
      display: flex;  
      flex-direction: column;  
      align-items: center;  
      min-height: 100vh;  
    }  
  
    /* Lock Screen */  
    #lock-screen {  
      position: fixed;  
      top: 0; left: 0; width: 100%; height: 100%;  
      background: linear-gradient(135deg, #ffb6c1, #ff69b4);  
      display: flex;  
      flex-direction: column;  
      justify-content: center;  
      align-items: center;  
      z-index: 999;  
      color: white;  
      text-align: center;  
      padding: 20px;  
      box-sizing: border-box;  
    }  
  
    .pass-input {  
      padding: 12px 20px;  
      border: 2px solid white;  
      border-radius: 25px;  
      outline: none;  
      font-size: 18px;  
      text-align: center;  
      margin-top: 15px;  
    }  
  
    .btn {  
      background: white;  
      color: var(--primary-dark);  
      border: none;  
      padding: 10px 25px;  
      border-radius: 25px;  
      font-size: 16px;  
      font-weight: bold;  
      cursor: pointer;  
      margin-top: 15px;  
      transition: transform 0.2s;  
    }  
  
    .btn:hover {  
      transform: scale(1.05);  
    }  
  
    /* Main Container */  
    .container {  
      max-width: 700px;  
      width: 90%;  
      margin: 30px auto;  
      display: none;  
    }  
  
    .card {  
      background: var(--card-bg);  
      border-radius: 20px;  
      padding: 25px;  
      margin-bottom: 25px;  
      box-shadow: 0 10px 25px rgba(255, 105, 180, 0.15);  
      border: 2px solid #ffe4e1;  
      text-align: center;  
    }  
  
    h1, h2 {  
      color: var(--primary-dark);  
    }  
  
    /* Gift Box & Video Section */  
    .gift-container {  
      cursor: pointer;  
      padding: 20px;  
      border: 2px dashed var(--primary);  
      border-radius: 15px;  
      background: #fff5f8;  
      transition: 0.3s;  
    }  
  
    .gift-icon {  
      font-size: 50px;  
      animation: bounce 1.5s infinite;  
    }  
  
    @keyframes bounce {  
      0%, 100% { transform: translateY(0); }  
      50% { transform: translateY(-10px); }  
    }  
  
    .video-grid {  
      display: none;  
      grid-template-columns: 1fr;  
      gap: 15px;  
      margin-top: 20px;  
    }  
  
    video {  
      width: 100%;  
      border-radius: 15px;  
      border: 3px solid var(--accent);  
    }  
  
    /* Music Player */  
    .music-btn {  
      background: var(--primary);  
      color: white;  
      font-size: 18px;  
    }  
  
    /* Quiz */  
    .quiz-option {  
      display: block;  
      width: 100%;  
      padding: 10px;  
      margin: 8px 0;  
      background: #fff0f5;  
      border: 1px solid var(--accent);  
      border-radius: 10px;  
      cursor: pointer;  
      font-size: 16px;  
    }  
  </style>  
</head>  
<body>  
  
  <!-- Lock Screen -->  
  <div id="lock-screen">  
    <h1>💖 بەخێربیی دیە گیان 💖</h1>  
    <p>تکایە کۆدی نهێنی بنووسە بۆ بەردەوامبوون:</p>  
    <input type="password" id="passcode" class="pass-input" placeholder="کۆدی نهێنی...">  
    <button onclick="checkPass()" class="btn">بچۆ ژوورەوە ✨</button>  
    <p id="error-msg" style="color: yellow; display: none; margin-top: 10px;">کۆدەکە هەڵەیە!</p>  
  </div>  
  
  <!-- Main Content -->  
  <div class="container" id="main-content">  
      
    <!-- Header -->  
    <div class="card">  
      <h1>🎉 یادی 18 ساڵیت پیرۆز بێت دیە گیان 🎀</h1>  
      <p>1ی مانگی 12 - یادگارییەکی تایبەت و پڕ لە خۆشەویستی</p>  
    </div>  
  
    <!-- Music Player Card -->  
    <div class="card">  
      <h2>🎶 بەشی گۆرانی دڵخواز</h2>  
      <p>🌸 "وەرە کوردبە و مەکە پەیمان شکێنی..." - مەرزیە فەریقی 🌸</p>  
      <button onclick="toggleMusic()" class="btn music-btn" id="music-control">▶ لێدانی گۆرانی</button>  
    </div>  
  
    <!-- Surprise Videos Card -->  
    <div class="card">  
      <h2>🎁 دیارییە سوپڕایزەکە 🎁</h2>  
      <div class="gift-container" id="gift-box" onclick="openGift()">  
        <div class="gift-icon">🎁</div>  
        <p><b>کلیک لەسەر دیارییەکە بکە بۆ کردنی!</b></p>  
      </div>  
  
      <div class="video-grid" id="video-content">  
        <h3>✨ یادگارییە ڤیدیۆییەکانی ئێمە ✨</h3>  
        <video controls src="video1.mp4"></video>  
        <video controls src="video2.mp4"></video>  
        <video controls src="video3.mp4"></video>  
      </div>  
    </div>  
  
    <!-- Memory Quiz Card -->  
    <div class="card">  
      <h2>🧠 کویزی یادگارییەکانمان</h2>  
      <p><b>پرسیار: ئێمە یەکەمجار لە کوێ یەکترمان ناسی؟</b></p>  
      <button class="quiz-option" onclick="answerQuiz(false)">لە مەکتەب 🏫</button>  
      <button class="quiz-option" onclick="answerQuiz(true)">لە پەیمانگا 🎓</button>  
      <button class="quiz-option" onclick="answerQuiz(false)">لە پارک 🌸</button>  
      <p id="quiz-result" style="font-weight: bold; margin-top: 10px;"></p>  
    </div>  
  
  </div>  
  
  <script>  
    // Passcode Check  
    function checkPass() {  
      const code = document.getElementById('passcode').value;  
      if (code === 'دەتجێم') {  
        document.getElementById('lock-screen').style.display = 'none';  
        document.getElementById('main-content').style.display = 'block';  
      } else {  
        document.getElementById('error-msg').style.display = 'block';  
      }  
    }  
  
    // Open Gift Videos  
    function openGift() {  
      document.getElementById('gift-box').style.display = 'none';  
      document.getElementById('video-content').style.display = 'grid';  
    }  
  
    // Quiz Check  
    function answerQuiz(isCorrect) {  
      const res = document.getElementById('quiz-result');  
      if (isCorrect) {  
        res.style.color = 'green';  
        res.innerText = 'ئافەرین! درستە، ئێمە لە پەیمانگا یەکتریمان ناسی ❤️';  
      } else {  
        res.style.color = 'red';  
        res.innerText = 'نەخێر! دروست نییە، دووبارە تاقی بکەرەوە 😜';  
      }  
    }  
  
    // Web Audio Synthesizer for Song Melody Demo  
    let audioCtx = null;  
    let isPlaying = false;  
    let timerId = null;  
  
    function toggleMusic() {  
      const btn = document.getElementById('music-control');  
      if (!isPlaying) {  
        if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();  
        isPlaying = true;  
        btn.innerText = "⏸ ڕاگرتنی گۆرانی";  
        playMelody();  
      } else {  
        isPlaying = false;  
        btn.innerText = "▶ لێدانی گۆرانی";  
        if (timerId) clearTimeout(timerId);  
      }  
    }  
  
    function playNote(freq, duration) {  
      if (!isPlaying) return;  
      const osc = audioCtx.createOscillator();  
      const gain = audioCtx.createGain();  
      osc.type = 'sine';  
      osc.frequency.value = freq;  
      gain.gain.setValueAtTime(0.1, audioCtx.currentTime);  
      gain.gain.exponentialRampToValueAtTime(0.001, audioCtx.currentTime + duration);  
      osc.connect(gain);  
      gain.connect(audioCtx.destination);  
      osc.start();  
      osc.stop(audioCtx.currentTime + duration);  
    }  
  
    function playMelody() {  
      const notes = [261, 293, 329, 349, 392, 440, 493, 523];  
      let step = 0;  
      function loop() {  
        if (!isPlaying) return;  
        playNote(notes[step % notes.length], 0.4);  
        step++;  
        timerId = setTimeout(loop, 400);  
      }  
      loop();  
    }  
  </script>  
</body>  
</html>  
