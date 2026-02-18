<svg width="1500" height="500" xmlns="http://www.w3.org/2000/svg">
  <!-- Definitions for gradients and styles -->
  <defs>
    <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#333333;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#4D4D4D;stop-opacity:1" />
    </linearGradient>
    <style>
      .text-main { font-family: 'Montserrat', sans-serif; font-weight: bold; font-size: 72px; fill: #FFFFFF; text-anchor: middle; }
      .text-sub { font-family: 'Montserrat', sans-serif; font-weight: normal; font-size: 36px; fill: #007BFF; text-anchor: middle; }
      .circuit-trace { stroke: #E0E0E0; stroke-width: 1; opacity: 0.2; fill: none; }
      .microcontroller { stroke: #333333; stroke-width: 2; fill: none; }
      .microcontroller-accent { fill: #007BFF; opacity: 0.3; }
      .robot-arm { fill: #333333; }
      .diagram-line { stroke: #E0E0E0; stroke-width: 2; stroke-dasharray: 5,5; fill: none; }
      .diagram-block { fill: #E0E0E0; stroke: #333333; stroke-width: 1; }
      .diagram-text { font-family: 'Montserrat', sans-serif; font-weight: 300; font-size: 12px; fill: #333333; text-anchor: middle; }
    </style>
  </defs>

  <!-- Background with gradient -->
  <rect width="1500" height="500" fill="url(#bgGradient)" />

  <!-- Subtle circuit traces (wavy lines) -->
  <path d="M0 100 Q 150 80 300 100 T 600 100 Q 750 120 900 100 T 1200 100 Q 1350 80 1500 100" class="circuit-trace" />
  <path d="M0 200 Q 150 180 300 200 T 600 200 Q 750 220 900 200 T 1200 200 Q 1350 180 1500 200" class="circuit-trace" />
  <path d="M0 300 Q 150 280 300 300 T 600 300 Q 750 320 900 300 T 1200 300 Q 1350 280 1500 300" class="circuit-trace" />
  <path d="M0 400 Q 150 380 300 400 T 600 400 Q 750 420 900 400 T 1200 400 Q 1350 380 1500 400" class="circuit-trace" />

  <!-- STM32-style microcontroller outline (left third, top) -->
  <g transform="translate(200, 150)">
    <!-- Chip body -->
    <rect x="0" y="0" width="150" height="100" class="microcontroller" />
    <rect x="10" y="10" width="130" height="80" class="microcontroller-accent" />
    <!-- Pins (simplified) -->
    <rect x="-10" y="20" width="10" height="5" class="microcontroller" />
    <rect x="-10" y="30" width="10" height="5" class="microcontroller" />
    <rect x="-10" y="40" width="10" height="5" class="microcontroller" />
    <rect x="-10" y="50" width="10" height="5" class="microcontroller" />
    <rect x="-10" y="60" width="10" height="5" class="microcontroller" />
    <rect x="150" y="20" width="10" height="5" class="microcontroller" />
    <rect x="150" y="30" width="10" height="5" class="microcontroller" />
    <rect x="150" y="40" width="10" height="5" class="microcontroller" />
    <rect x="150" y="50" width="10" height="5" class="microcontroller" />
    <rect x="150" y="60" width="10" height="5" class="microcontroller" />
  </g>

  <!-- Robotics arm silhouette (left third, below microcontroller) -->
  <g transform="translate(250, 300)">
    <!-- Base -->
    <rect x="0" y="80" width="20" height="40" class="robot-arm" />
    <!-- Arm segments -->
    <rect x="10" y="60" width="10" height="30" class="robot-arm" transform="rotate(-30 15 75)" />
    <rect x="15" y="40" width="10" height="30" class="robot-arm" transform="rotate(-60 20 55)" />
    <rect x="20" y="20" width="10" height="30" class="robot-arm" transform="rotate(-90 25 35)" />
    <!-- End effector -->
    <circle cx="25" cy="10" r="5" class="robot-arm" />
  </g>

  <!-- Control system block diagram (right third) -->
  <g transform="translate(1000, 200)">
    <!-- Blocks -->
    <rect x="0" y="0" width="50" height="30" class="diagram-block" />
    <text x="25" y="20" class="diagram-text">Sensor</text>
    <rect x="100" y="0" width="50" height="30" class="diagram-block" />
    <text x="125" y="20" class="diagram-text">Controller</text>
    <rect x="200" y="0" width="50" height="30" class="diagram-block" />
    <text x="225" y="20" class="diagram-text">Actuator</text>
    <!-- Lines (feedback loop) -->
    <line x1="50" y1="15" x2="100" y2="15" class="diagram-line" />
    <line x1="150" y1="15" x2="200" y2="15" class="diagram-line" />
    <line x1="250" y1="15" x2="300" y2="15" class="diagram-line" />
    <line x1="300" y1="15" x2="300" y2="100" class="diagram-line" />
    <line x1="300" y1="100" x2="0" y2="100" class="diagram-line" />
    <line x1="0" y1="100" x2="0" y2="15" class="diagram-line" />
  </g>

  <!-- Main text (centered) -->
  <text x="750" y="250" class="text-main">Farhan Ali</text>
  <text x="750" y="300" class="text-sub">Embedded Systems | Robotics | Intelligent Automation</text>

  <!-- Thin blue border -->
  <rect x="0" y="0" width="1500" height="500" fill="none" stroke="#007BFF" stroke-width="2" />
</svg>
