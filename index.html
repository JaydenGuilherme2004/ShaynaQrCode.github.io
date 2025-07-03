<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Jayden's 21st 🎉</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Metal+Mania&family=Creepster&family=Nosifer&family=Butcherman&display=swap');
    
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: 'Metal Mania', cursive;
      background: #000;
      color: #fff;
      display: flex;
      flex-direction: column;
      min-height: 100vh;
      overflow-x: hidden;
      position: relative;
    }

    body::before {
      content: '';
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: 
        radial-gradient(circle at 50% 50%, rgba(139, 0, 0, 0.4) 0%, transparent 50%),
        linear-gradient(135deg, #000, #1a0000, #330000);
      animation: hellfire 16s ease-in-out infinite alternate;
      z-index: -2;
    }

    @keyframes hellfire {
      0%, 100% { filter: brightness(1) contrast(1.2); }
      50% { filter: brightness(1.3) contrast(1.5); }
    }

    .sparks {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: -1;
    }

    .spark {
      position: absolute;
      width: 3px;
      height: 15px;
      background: linear-gradient(to bottom, #ff0000, #cc0000, transparent);
      border-radius: 50%;
      animation: sparkFall 3s infinite linear;
    }

    @keyframes sparkFall {
      0% { transform: translateY(-100vh); opacity: 0; }
      10%, 90% { opacity: 1; }
      100% { transform: translateY(100vh); opacity: 0; }
    }

    .header { text-align: center; padding: 2rem; position: relative; z-index: 10; }
    .title {
      font-family: 'Nosifer', cursive;
      font-size: clamp(2.5rem, 8vw, 5rem);
      background: linear-gradient(45deg, #8B4513, #A0522D);
      background-size: 200% 200%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: dirtFlow 3s ease-in-out infinite;
      text-shadow: 0 0 10px rgba(139, 69, 19, 0.8);
      letter-spacing: 3px;
    }

    @keyframes dirtFlow {
      0%, 100% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
    }

    .subtitle {
      font-size: 1.5rem;
      margin-top: 1rem;
      color: #ff4444;
      text-shadow: 0 0 10px rgba(255, 68, 68, 0.8);
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.7; }
    }

    .video-container {
      flex: 1;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 2rem;
      position: relative;
    }

    .video-wrapper {
      position: relative;
      width: 100%;
      max-width: 900px;
      padding-top: 50.625%;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 0 50px rgba(255, 0, 0, 0.6);
    }

    .video-wrapper iframe {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      border: none;
      border-radius: 15px;
    }

    .controls {
      display: flex;
      justify-content: center;
      gap: 2rem;
      padding: 2rem;
      position: relative;
      z-index: 10;
    }

    .control-btn {
      background: rgba(139, 0, 0, 0.4);
      border: 2px solid rgba(255, 0, 0, 0.4);
      color: #fff;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      cursor: pointer;
      font-size: 1.2rem;
    }

    .play-btn {
      width: 75px;
      height: 75px;
      font-size: 1.8rem;
    }

    .footer {
      text-align: center;
      padding: 2rem;
      font-size: 1.1rem;
      color: #cc4444;
    }

    .emoji {
      font-size: 1.3em;
      animation: headbang 1s infinite;
      color: #ff0000;
    }

    @keyframes headbang {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-5px); }
    }
  </style>
</head>
<body>
  <div class="sparks" id="sparks"></div>

  <div class="header">
    <div class="title">JAYDEN'S 21ST</div>
    <div class="subtitle">🤘 ROCK & ROLL FOREVER 🔥</div>
  </div>

  <div class="video-container">
    <div class="video-wrapper">
      <div id="player"></div>
    </div>
  </div>

  <div class="controls">
    <button class="control-btn" onclick="rewind()">⏮️</button>
    <button class="control-btn play-btn" onclick="togglePlay()">⏯️</button>
    <button class="control-btn" onclick="forward()">⏭️</button>
  </div>

  <div class="footer">
    <span class="emoji">🔥</span> TURN IT UP TO 11 AND ROCK ON <span class="emoji">🔥</span>
  </div>

  <script src="https://www.youtube.com/iframe_api"></script>
  <script>
    let player;

    function createSparks() {
      const sparksContainer = document.getElementById('sparks');
      sparksContainer.innerHTML = '';
      for (let i = 0; i < 15; i++) {
        const spark = document.createElement('div');
        spark.className = 'spark';
        spark.style.left = Math.random() * 100 + '%';
        spark.style.animationDelay = Math.random() * 3 + 's';
        spark.style.animationDuration = (Math.random() * 2 + 2) + 's';
        sparksContainer.appendChild(spark);
      }
    }

    function onYouTubeIframeAPIReady() {
      player = new YT.Player('player', {
        height: '100%',
        width: '100%',
        videoId: 'mj_dhImiej8',
        playerVars: { modestbranding: 1, rel: 0, showinfo: 0, controls: 1 },
        events: {
          onReady: () => createSparks(),
          onStateChange: (e) => {
            if (e.data === YT.PlayerState.PLAYING) {
              document.body.classList.add('flash');
              setTimeout(() => document.body.classList.remove('flash'), 300);
            }
          }
        }
      });
    }

    function togglePlay() {
      if (!player) return;
      const state = player.getPlayerState();
      if (state === YT.PlayerState.PLAYING) {
        player.pauseVideo();
      } else {
        player.playVideo();
        document.body.classList.add('flash');
        setTimeout(() => document.body.classList.remove('flash'), 300);
      }
    }

    function rewind() {
      if (player) {
        player.seekTo(Math.max(0, player.getCurrentTime() - 10));
      }
    }

    function forward() {
      if (player) {
        player.seekTo(Math.min(player.getDuration(), player.getCurrentTime() + 10));
      }
    }
  </script>
</body>
</html>
