<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Jayden's 21st 🎉</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Metal+Mania&family=Creepster&family=Nosifer&family=Butcherman&display=swap');
    
    * {
      box-sizing: border-box;
    }

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

    /* Metal/Rock background */
    body::before {
      content: '';
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: 
        radial-gradient(circle at 20% 30%, rgba(139, 0, 0, 0.6) 0%, transparent 40%),
        radial-gradient(circle at 80% 70%, rgba(220, 20, 60, 0.4) 0%, transparent 40%),
        radial-gradient(circle at 50% 50%, rgba(255, 0, 0, 0.2) 0%, transparent 60%),
        linear-gradient(135deg, #000 0%, #1a0000 25%, #330000 50%, #1a0000 75%, #000 100%);
      animation: hellfire 8s ease-in-out infinite;
      z-index: -2;
    }

    /* Lightning/sparks effect */
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

    @keyframes hellfire {
      0%, 100% { 
        background-position: 0% 0%, 100% 100%, 50% 50%;
        filter: brightness(1) contrast(1.2);
      }
      50% { 
        background-position: 100% 100%, 0% 0%, 25% 75%;
        filter: brightness(1.3) contrast(1.5);
      }
    }

    @keyframes sparkFall {
      0% {
        transform: translateY(-100vh) rotate(0deg);
        opacity: 0;
      }
      10% {
        opacity: 1;
      }
      90% {
        opacity: 1;
      }
      100% {
        transform: translateY(100vh) rotate(360deg);
        opacity: 0;
      }
    }

    /* Header */
    .header {
      text-align: center;
      padding: 2rem;
      position: relative;
      z-index: 10;
    }

    .title {
      font-family: 'Nosifer', cursive;
      font-size: clamp(2.5rem, 8vw, 5rem);
      font-weight: 900;
      background: linear-gradient(45deg, #8B4513, #A0522D, #654321, #8B4513);
      background-size: 400% 400%;
      background-clip: text;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: dirtFlow 2s ease-in-out infinite;
      text-shadow: 
        0 0 10px rgba(139, 69, 19, 0.8),
        0 0 20px rgba(139, 69, 19, 0.6),
        0 0 30px rgba(139, 69, 19, 0.4),
        2px 2px 0px rgba(101, 67, 33, 0.8),
        4px 4px 0px rgba(160, 82, 45, 0.6);
      letter-spacing: 3px;
      transform: perspective(500px) rotateX(15deg);
      position: relative;
    }

    .title::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: 
        radial-gradient(circle at 20% 20%, rgba(139, 69, 19, 0.3) 0%, transparent 30%),
        radial-gradient(circle at 80% 80%, rgba(160, 82, 45, 0.3) 0%, transparent 30%),
        radial-gradient(circle at 50% 50%, rgba(101, 67, 33, 0.2) 0%, transparent 40%);
      filter: blur(2px);
      z-index: -1;
    }

    @keyframes dirtFlow {
      0%, 100% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
    }

    .subtitle {
      font-family: 'Metal Mania', cursive;
      font-size: 1.5rem;
      margin-top: 1rem;
      color: #ff4444;
      text-shadow: 0 0 10px rgba(255, 68, 68, 0.8);
      letter-spacing: 2px;
      animation: pulse 2s infinite;
    }

    @keyframes pulse {
      0%, 100% { opacity: 1; }
      50% { opacity: 0.7; }
    }

    /* Video container */
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
      box-shadow: 
        0 0 50px rgba(255, 0, 0, 0.6),
        0 0 100px rgba(139, 0, 0, 0.4),
        inset 0 0 0 3px rgba(255, 0, 0, 0.3),
        inset 0 0 0 6px rgba(0, 0, 0, 0.8);
      background: 
        linear-gradient(45deg, transparent 30%, rgba(255, 0, 0, 0.1) 50%, transparent 70%),
        radial-gradient(circle at center, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.8));
      transition: all 0.3s ease;
      animation: metalGlow 4s ease-in-out infinite;
    }

    @keyframes metalGlow {
      0%, 100% {
        box-shadow: 
          0 0 50px rgba(255, 0, 0, 0.6),
          0 0 100px rgba(139, 0, 0, 0.4),
          inset 0 0 0 3px rgba(255, 0, 0, 0.3);
      }
      50% {
        box-shadow: 
          0 0 70px rgba(255, 0, 0, 0.8),
          0 0 140px rgba(139, 0, 0, 0.6),
          inset 0 0 0 3px rgba(255, 0, 0, 0.5);
      }
    }

    .video-wrapper:hover {
      transform: scale(1.03);
      box-shadow: 
        0 0 80px rgba(255, 0, 0, 0.8),
        0 0 160px rgba(139, 0, 0, 0.6),
        inset 0 0 0 3px rgba(255, 0, 0, 0.6);
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

    /* Controls */
    .controls {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 3rem;
      padding: 2rem;
      position: relative;
      z-index: 10;
    }

    .controls::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: 
        linear-gradient(135deg, rgba(0, 0, 0, 0.8), rgba(139, 0, 0, 0.3)),
        radial-gradient(circle at center, rgba(255, 0, 0, 0.1), transparent);
      border-top: 2px solid rgba(255, 0, 0, 0.4);
      z-index: -1;
    }

    .control-btn {
      background: 
        linear-gradient(145deg, rgba(255, 0, 0, 0.2), rgba(139, 0, 0, 0.4)),
        radial-gradient(circle at 30% 30%, rgba(255, 0, 0, 0.3), transparent);
      border: 2px solid rgba(255, 0, 0, 0.4);
      color: #fff;
      width: 70px;
      height: 70px;
      border-radius: 50%;
      cursor: pointer;
      transition: all 0.3s ease;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      position: relative;
      overflow: hidden;
      box-shadow: 
        0 0 20px rgba(255, 0, 0, 0.4),
        inset 0 0 20px rgba(0, 0, 0, 0.3);
    }

    .control-btn::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      width: 0;
      height: 0;
      background: radial-gradient(circle, rgba(255, 0, 0, 0.3), transparent);
      border-radius: 50%;
      transition: all 0.3s ease;
      transform: translate(-50%, -50%);
    }

    .control-btn:hover::before {
      width: 120%;
      height: 120%;
    }

    .control-btn:hover {
      transform: scale(1.15);
      box-shadow: 
        0 0 40px rgba(255, 0, 0, 0.8),
        0 0 80px rgba(255, 0, 0, 0.4),
        inset 0 0 20px rgba(255, 0, 0, 0.2);
      border-color: rgba(255, 0, 0, 0.8);
      text-shadow: 0 0 10px rgba(255, 0, 0, 0.8);
    }

    .control-btn:active {
      transform: scale(0.9);
      animation: metalClang 0.2s ease-out;
    }

    @keyframes metalClang {
      0% { filter: brightness(2); }
      100% { filter: brightness(1); }
    }

    .play-btn {
      width: 90px;
      height: 90px;
      font-size: 2rem;
      background: 
        linear-gradient(145deg, rgba(255, 0, 0, 0.4), rgba(139, 0, 0, 0.6)),
        radial-gradient(circle at 30% 30%, rgba(255, 0, 0, 0.5), transparent);
      border: 3px solid rgba(255, 0, 0, 0.6);
    }

    .play-btn:hover {
      background: 
        linear-gradient(145deg, rgba(255, 0, 0, 0.6), rgba(139, 0, 0, 0.8)),
        radial-gradient(circle at 30% 30%, rgba(255, 0, 0, 0.7), transparent);
      animation: rockPulse 0.5s ease-in-out;
    }

    @keyframes rockPulse {
      0%, 100% { transform: scale(1.15); }
      50% { transform: scale(1.25); }
    }

    /* Footer */
    .footer {
      text-align: center;
      padding: 2rem;
      font-size: 1.1rem;
      color: #cc4444;
      position: relative;
      z-index: 10;
      font-family: 'Metal Mania', cursive;
    }

    .footer-text {
      font-weight: 400;
      letter-spacing: 2px;
      text-shadow: 0 0 10px rgba(204, 68, 68, 0.6);
    }

    .emoji {
      font-size: 1.3em;
      animation: headbang 1s infinite;
      color: #ff0000;
      text-shadow: 0 0 10px rgba(255, 0, 0, 0.8);
    }

    @keyframes headbang {
      0%, 100% { transform: translateY(0) rotate(0deg); }
      25% { transform: translateY(-5px) rotate(-5deg); }
      75% { transform: translateY(-5px) rotate(5deg); }
    }

    /* Metal texture overlay */
    .metal-texture {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: 
        repeating-linear-gradient(
          45deg,
          transparent,
          transparent 2px,
          rgba(255, 0, 0, 0.05) 2px,
          rgba(255, 0, 0, 0.05) 4px
        );
      pointer-events: none;
      z-index: 1;
      opacity: 0.3;
    }

    /* Responsive design */
    @media (max-width: 768px) {
      .controls {
        gap: 2rem;
      }
      
      .control-btn {
        width: 60px;
        height: 60px;
        font-size: 1.2rem;
      }
      
      .play-btn {
        width: 75px;
        height: 75px;
        font-size: 1.8rem;
      }
      
      .video-container {
        padding: 1rem;
      }
      
      .title {
        font-size: clamp(2rem, 6vw, 3.5rem);
      }
    }

    /* Screen flash effect */
    .flash {
      animation: screenFlash 0.3s ease-out;
    }

    @keyframes screenFlash {
      0% { filter: brightness(1); }
      50% { filter: brightness(2) saturate(2); }
      100% { filter: brightness(1); }
    }
  </style>
</head>
<body>
  <!-- Metal texture overlay -->
  <div class="metal-texture"></div>
  
  <!-- Sparks effect -->
  <div class="sparks" id="sparks"></div>

  <!-- Header -->
  <div class="header">
    <div class="title">JAYDEN'S 21ST</div>
    <div class="subtitle">🤘 ROCK & ROLL FOREVER 🔥</div>
  </div>

  <!-- Video Section -->
  <div class="video-container">
    <div class="video-wrapper">
      <div id="player"></div>
    </div>
  </div>

  <!-- Controls -->
  <div class="controls">
    <button class="control-btn" onclick="rewind()">⏮️</button>
    <button class="control-btn play-btn" onclick="togglePlay()">⏯️</button>
    <button class="control-btn" onclick="forward()">⏭️</button>
  </div>

  <!-- Footer -->
  <div class="footer">
    <div class="footer-text">
      <span class="emoji">🔥</span> 
      TURN IT UP TO 11 AND ROCK ON 
      <span class="emoji">🔥</span>
    </div>
  </div>

  <!-- YouTube Player API -->
  <script src="https://www.youtube.com/iframe_api"></script>
  <script>
    function onYouTubeIframeAPIReady() {
      player = new YT.Player('player', {
        height: '100%',
        width: '100%',
        videoId: 'mj_dhImiej8',
        playerVars: {
          modestbranding: 1,
          rel: 0,
          showinfo: 0,
          controls: 1,
          autoplay: 0,
          fs: 1,
          cc_load_policy: 0,
          iv_load_policy: 3,
          autohide: 0
        },
        events: {
          onReady: (event) => {
            console.log('Player ready!');
            createSparks();
          },
          onStateChange: (event) => {
            if (event.data === YT.PlayerState.PLAYING) {
              document.body.classList.add('playing');
              // Screen flash effect when playing
              document.body.classList.add('flash');
              setTimeout(() => {
                document.body.classList.remove('flash');
              }, 300);
            } else {
              document.body.classList.remove('playing');
            }
          },
          onError: (event) => {
            console.log('YouTube player error:', event.data);
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
        // Add screen flash effect
        document.body.classList.add('flash');
        setTimeout(() => {
          document.body.classList.remove('flash');
        }, 300);
      }
    }

    function rewind() {
      if (player) {
        const currentTime = player.getCurrentTime();
        player.seekTo(Math.max(0, currentTime - 10));
        // Add flash effect for feedback
        document.querySelector('.video-wrapper').classList.add('flash');
        setTimeout(() => {
          document.querySelector('.video-wrapper').classList.remove('flash');
        }, 300);
      }
    }

    function forward() {
      if (player) {
        const currentTime = player.getCurrentTime();
        const duration = player.getDuration();
        player.seekTo(Math.min(duration, currentTime + 10));
        // Add flash effect for feedback
        document.querySelector('.video-wrapper').classList.add('flash');
        setTimeout(() => {
          document.querySelector('.video-wrapper').classList.remove('flash');
        }, 300);
      }
    }

  </script>
</body>
</html>
