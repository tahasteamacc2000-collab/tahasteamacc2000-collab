<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 220" width="900" height="220" role="img" aria-label="Taha glitch banner">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#0b0b1a"/>
      <stop offset="1" stop-color="#1a0b2e"/>
    </linearGradient>
    <pattern id="scan" width="4" height="4" patternUnits="userSpaceOnUse">
      <rect width="4" height="1" fill="#000" opacity="0.35"/>
    </pattern>
    <filter id="warp" x="-5%" y="-5%" width="110%" height="110%">
      <feTurbulence type="fractalNoise" baseFrequency="0.001 0.4" numOctaves="1" seed="3" result="n">
        <animate attributeName="seed" values="1;5;2;9;4;7;3" dur="1.4s" repeatCount="indefinite" calcMode="discrete"/>
      </feTurbulence>
      <feDisplacementMap in="SourceGraphic" in2="n" scale="0">
        <animate attributeName="scale" values="0;0;0;0;28;0;0;12;0;0;0;40;0;0" dur="3s" repeatCount="indefinite" calcMode="discrete"/>
      </feDisplacementMap>
    </filter>
  </defs>

  <style>
    .t { font-family: 'Courier New', Consolas, monospace; font-weight: 900; font-size: 120px; letter-spacing: 14px; text-anchor: middle; }
    .cy { fill: #00fff0; mix-blend-mode: screen; animation: shiftA 2.6s steps(1) infinite; }
    .mg { fill: #ff2bd6; mix-blend-mode: screen; animation: shiftB 2.6s steps(1) infinite; }
    .wh { fill: #ffffff; }
    .sub { font-family: 'Courier New', Consolas, monospace; font-size: 22px; fill: #00ff9c; letter-spacing: 6px; text-anchor: middle; animation: flick 3.2s steps(1) infinite; }
    .bar { fill: #00fff0; opacity: 0; }
    .b1 { animation: bar1 2.6s steps(1) infinite; }
    .b2 { fill: #ff2bd6; animation: bar2 2.6s steps(1) infinite; }
    .b3 { fill: #ffffff; animation: bar3 2.6s steps(1) infinite; }
    .roll { animation: roll 5s linear infinite; }

    @keyframes shiftA {
      0%   { transform: translate(-4px, 0); }
      10%  { transform: translate(6px, -2px); }
      20%  { transform: translate(-2px, 1px); }
      30%  { transform: translate(-10px, 0); }
      40%  { transform: translate(3px, 2px); }
      55%  { transform: translate(-3px, 0); }
      70%  { transform: translate(12px, -1px); }
      85%  { transform: translate(-5px, 1px); }
      100% { transform: translate(-4px, 0); }
    }
    @keyframes shiftB {
      0%   { transform: translate(4px, 0); }
      10%  { transform: translate(-6px, 2px); }
      20%  { transform: translate(3px, -1px); }
      30%  { transform: translate(10px, 0); }
      40%  { transform: translate(-3px, -2px); }
      55%  { transform: translate(3px, 0); }
      70%  { transform: translate(-12px, 1px); }
      85%  { transform: translate(5px, -1px); }
      100% { transform: translate(4px, 0); }
    }
    @keyframes bar1 { 0%,28% { opacity: 0; } 30%,34% { opacity: .9; transform: translateX(-30px); } 36%,100% { opacity: 0; } }
    @keyframes bar2 { 0%,66% { opacity: 0; } 68%,73% { opacity: .9; transform: translateX(40px); } 75%,100% { opacity: 0; } }
    @keyframes bar3 { 0%,82% { opacity: 0; } 84%,87% { opacity: .8; transform: translateX(-20px); } 89%,100% { opacity: 0; } }
    @keyframes flick { 0%,88% { opacity: 1; } 90% { opacity: .2; } 92% { opacity: 1; } 94% { opacity: .1; } 96%,100% { opacity: 1; } }
    @keyframes roll { 0% { transform: translateY(-40px); } 100% { transform: translateY(260px); } }
  </style>

  <rect width="900" height="220" fill="url(#bg)"/>

  <g filter="url(#warp)">
    <text class="t cy" x="450" y="130">TAHA</text>
    <text class="t mg" x="450" y="130">TAHA</text>
    <text class="t wh" x="450" y="130">TAHA</text>

    <rect class="bar b1" x="250" y="62"  width="400" height="10"/>
    <rect class="bar b2" x="220" y="96"  width="460" height="8"/>
    <rect class="bar b3" x="270" y="118" width="360" height="6"/>
  </g>

  <text class="sub" x="450" y="185">GLITCH VIBES ONLY</text>

  <rect width="900" height="220" fill="url(#scan)"/>
  <rect class="roll" x="0" y="0" width="900" height="30" fill="#ffffff" opacity="0.05"/>
</svg>
