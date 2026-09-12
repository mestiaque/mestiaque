<p align="center">
  <svg width="100%" height="180" viewBox="0 0 800 180" xmlns="http://w3.org">
    <style>
      .bg { fill: #0d1117; stroke: #00ffcc; stroke-width: 2; }
      .grid { stroke: #1f2937; stroke-width: 0.5; }
      .neon-text {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-weight: 900;
        font-size: 42px;
        fill: #00ffcc;
        letter-spacing: 5px;
        text-shadow: 0 0 10px #00ffcc, 0 0 20px #ff00ff;
        animation: glitch 1.5s infinite linear alternate-reverse;
      }
      .sub-text {
        font-family: 'Courier New', Courier, monospace;
        font-size: 14px;
        fill: #ff00ff;
        letter-spacing: 3px;
      }
      .scanline {
        stroke: #00ffcc;
        stroke-width: 1;
        opacity: 0.3;
        animation: moveScanline 6s linear infinite;
      }
      .glitch-line {
        stroke: #ff00ff;
        stroke-width: 2;
        animation: glitchL 2s infinite;
      }
      @keyframes glitch {
        0% { transform: translate(0) skew(0deg); text-shadow: 0 0 8px #00ffcc; }
        20% { transform: translate(-2px, 1px) skew(-1deg); }
        40% { transform: translate(1px, -1px) skew(1deg); text-shadow: 0 0 12px #ff00ff; }
        60% { transform: translate(-1px, 2px) skew(0deg); }
        80% { transform: translate(2px, -1px) skew(2deg); }
        100% { transform: translate(0) skew(0deg); text-shadow: 0 0 8px #00ffcc; }
      }
      @keyframes moveScanline {
        0% { y1: 10; y2: 10; }
        100% { y1: 170; y2: 170; }
      }
      @keyframes glitchL {
        0% { opacity: 0; y1: 50; y2: 50; }
        5% { opacity: 0.8; y1: 90; y2: 90; x1: 50; x2: 750; }
        7% { opacity: 0; }
        50% { opacity: 0; }
        52% { opacity: 0.5; y1: 40; y2: 40; x1: 200; x2: 600; }
        55% { opacity: 0; }
        100% { opacity: 0; }
      }
    </style>

    <!-- Background Matrix / Cyberpunk Grid -->
    <rect width="796" height="176" x="2" y="2" rx="8" class="bg" />
    <g class="grid">
      <line x1="0" y1="30" x2="800" y2="30" />
      <line x1="0" y1="60" x2="800" y2="60" />
      <line x1="0" y1="90" x2="800" y2="90" />
      <line x1="0" y1="120" x2="800" y2="120" />
      <line x1="0" y1="150" x2="800" y2="150" />
      <line x1="100" y1="0" x2="100" y2="180" />
      <line x1="200" y1="0" x2="200" y2="180" />
      <line x1="300" y1="0" x2="300" y2="180" />
      <line x1="400" y1="0" x2="400" y2="180" />
      <line x1="500" y1="0" x2="500" y2="180" />
      <line x1="600" y1="0" x2="600" y2="180" />
      <line x1="700" y1="0" x2="700" y2="180" />
    </g>

    <!-- Animated Scanline & Glitch Effect Elements -->
    <line x1="10" y1="10" x2="790" y2="10" class="scanline" />
    <line x1="0" y1="0" x2="0" y2="0" class="glitch-line" />

    <!-- Core Text -->
    <text x="50%" y="85" dominant-baseline="middle" text-anchor="middle" class="neon-text">MESTIAQUE</text>
    <text x="50%" y="130" dominant-baseline="middle" text-anchor="middle" class="sub-text">> FULL_STACK_MAGE_INITIALIZED_</text>
    
    <!-- UI Border Details -->
    <rect x="15" y="15" width="20" height="20" fill="none" stroke="#ff00ff" stroke-width="1.5"/>
    <rect x="765" y="15" width="20" height="20" fill="none" stroke="#ff00ff" stroke-width="1.5"/>
    <circle cx="25" cy="25" r="3" fill="#00ffcc" />
    <circle cx="775" cy="25" r="3" fill="#00ffcc" />
  </svg>
</p>
