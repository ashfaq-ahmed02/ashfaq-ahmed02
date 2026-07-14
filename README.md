<svg width="1180" height="610" viewBox="0 0 1180 610" xmlns="http://www.w3.org/2000/svg">
<defs>
  <clipPath id="canvasClip"><rect x="0" y="0" width="1180" height="610" rx="24"/></clipPath>
  <clipPath id="leftClip"><rect x="24" y="24" width="420" height="562" rx="20"/></clipPath>
  <clipPath id="rightClip"><rect x="470" y="24" width="686" height="562" rx="20"/></clipPath>

  <linearGradient id="accentGrad" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#7C3AED"/>
    <stop offset="50%" stop-color="#22D3EE"/>
    <stop offset="100%" stop-color="#10B981"/>
    <animateTransform attributeName="gradientTransform" type="translate" values="-1 0;1 0;-1 0" dur="6s" repeatCount="indefinite"/>
  </linearGradient>

  <linearGradient id="borderShimmer" x1="0%" y1="0%" x2="100%" y2="100%">
    <stop offset="0%" stop-color="#7C3AED" stop-opacity="0"/>
    <stop offset="50%" stop-color="#22D3EE" stop-opacity="0.9"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
    <animateTransform attributeName="gradientTransform" type="rotate" values="0 590 305;360 590 305" dur="8s" repeatCount="indefinite"/>
  </linearGradient>

  <radialGradient id="blob1" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#7C3AED" stop-opacity="0.35"/>
    <stop offset="100%" stop-color="#7C3AED" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="blob2" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity="0.3"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </radialGradient>
  <radialGradient id="blob3" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#10B981" stop-opacity="0.25"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
  </radialGradient>

  <linearGradient id="scanGrad" x1="0%" y1="0%" x2="0%" y2="100%">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity="0"/>
    <stop offset="50%" stop-color="#22D3EE" stop-opacity="0.35"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </linearGradient>

  <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
    <feGaussianBlur stdDeviation="4" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>
  <filter id="softGlow" x="-50%" y="-50%" width="200%" height="200%">
    <feGaussianBlur stdDeviation="2.2" result="b"/>
    <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
  </filter>
  <filter id="noiseF" x="0" y="0" width="100%" height="100%">
    <feTurbulence type="fractalNoise" baseFrequency="0.85" numOctaves="2" stitchTiles="stitch" result="n"/>
    <feColorMatrix in="n" type="matrix" values="0 0 0 0 1  0 0 0 0 1  0 0 0 0 1  0 0 0 0.025 0"/>
  </filter>

  <clipPath id="typeClip0"><rect x="0" y="0" width="0" height="30"><animate attributeName="width" values="0;226;226;0" keyTimes="0;0.02;0.23;0.25" dur="20s" begin="0s" repeatCount="indefinite"/></rect></clipPath>
  <clipPath id="typeClip1"><rect x="0" y="0" width="0" height="30"><animate attributeName="width" values="0;250;250;0" keyTimes="0;0.02;0.23;0.25" dur="20s" begin="4s" repeatCount="indefinite"/></rect></clipPath>
  <clipPath id="typeClip2"><rect x="0" y="0" width="0" height="30"><animate attributeName="width" values="0;300;300;0" keyTimes="0;0.02;0.23;0.25" dur="20s" begin="8s" repeatCount="indefinite"/></rect></clipPath>
  <clipPath id="typeClip3"><rect x="0" y="0" width="0" height="30"><animate attributeName="width" values="0;180;180;0" keyTimes="0;0.02;0.23;0.25" dur="20s" begin="12s" repeatCount="indefinite"/></rect></clipPath>
  <clipPath id="typeClip4"><rect x="0" y="0" width="0" height="30"><animate attributeName="width" values="0;190;190;0" keyTimes="0;0.02;0.23;0.25" dur="20s" begin="16s" repeatCount="indefinite"/></rect></clipPath>
</defs>

<style>
  .mono { font-family: 'Consolas','Monaco','Courier New',monospace; }
  .pill:hover rect { filter: url(#glow); }
</style>

<g clip-path="url(#canvasClip)">
  <rect x="0" y="0" width="1180" height="610" fill="#030712"/>

  <circle cx="140" cy="120" r="220" fill="url(#blob1)">
    <animateTransform attributeName="transform" type="translate" values="0 0;30 20;0 0" dur="9s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1000" cy="150" r="260" fill="url(#blob2)">
    <animateTransform attributeName="transform" type="translate" values="0 0;-25 25;0 0" dur="11s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="560" r="240" fill="url(#blob3)">
    <animateTransform attributeName="transform" type="translate" values="0 0;20 -20;0 0" dur="10s" repeatCount="indefinite"/>
  </circle>

  <rect x="0" y="0" width="1180" height="610" filter="url(#noiseF)"/>

  <g opacity="0.7">
    <circle cx="90" cy="90" r="1.6" fill="#22D3EE"><animateMotion path="M0,0 C40,-30 80,30 20,80" dur="12s" repeatCount="indefinite"/></circle>
    <circle cx="1080" cy="500" r="1.8" fill="#7C3AED"><animateMotion path="M0,0 C-50,20 -20,-40 -70,-10" dur="14s" repeatCount="indefinite"/></circle>
    <circle cx="600" cy="60" r="1.4" fill="#10B981"><animateMotion path="M0,0 C30,40 -30,60 10,90" dur="10s" repeatCount="indefinite"/></circle>
    <circle cx="900" cy="300" r="1.5" fill="#22D3EE"><animateMotion path="M0,0 C-40,-20 40,-40 0,-70" dur="13s" repeatCount="indefinite"/></circle>
    <circle cx="300" cy="550" r="1.6" fill="#7C3AED"><animateMotion path="M0,0 C25,-25 55,10 15,45" dur="9s" repeatCount="indefinite"/></circle>
  </g>

  <rect x="24" y="24" width="420" height="562" rx="20" fill="#0F172A" fill-opacity="0.55"/>
  <rect x="470" y="24" width="686" height="562" rx="20" fill="#0F172A" fill-opacity="0.55"/>
  <rect x="24" y="24" width="420" height="562" rx="20" fill="none" stroke="rgba(255,255,255,.08)" stroke-width="1"/>
  <rect x="470" y="24" width="686" height="562" rx="20" fill="none" stroke="rgba(255,255,255,.08)" stroke-width="1"/>
  <rect x="1" y="1" width="1178" height="608" rx="23" fill="none" stroke="url(#borderShimmer)" stroke-width="1.5"/>

  <!-- LEFT: ASCII portrait -->
  <g clip-path="url(#leftClip)">
    <g class="mono" font-size="15" fill="url(#accentGrad)">
      <animateTransform attributeName="transform" type="translate" values="0 0;0 -6;0 0" dur="5s" repeatCount="indefinite"/>
      <text x="55" y="90" opacity="0" xml:space="preserve">   ┌─────────────┐<animate attributeName="opacity" values="0;1" begin="0.2s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="112" opacity="0" xml:space="preserve">   │   ◕     ◕   │<animate attributeName="opacity" values="0;1" begin="0.5s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="134" opacity="0" xml:space="preserve">   │      ▽      │<animate attributeName="opacity" values="0;1" begin="0.8s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="156" opacity="0" xml:space="preserve">   │   ‾‾‾‾‾‾‾   │<animate attributeName="opacity" values="0;1" begin="1.1s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="178" opacity="0" xml:space="preserve">   └───┬─────┬───┘<animate attributeName="opacity" values="0;1" begin="1.4s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="200" opacity="0" xml:space="preserve">       │     │</text>
      <text x="55" y="200" opacity="0"><animate attributeName="opacity" values="0;1" begin="1.7s" dur="0.4s" fill="freeze"/>       │     │</text>
      <text x="55" y="222" opacity="0" xml:space="preserve">  ┌────┴─────┴────┐<animate attributeName="opacity" values="0;1" begin="2.0s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="244" opacity="0" xml:space="preserve">  │   &lt; / &gt;  DEV   │<animate attributeName="opacity" values="0;1" begin="2.3s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="266" opacity="0" xml:space="preserve">  └────────────────┘<animate attributeName="opacity" values="0;1" begin="2.6s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="288" opacity="0" xml:space="preserve">        ║      ║<animate attributeName="opacity" values="0;1" begin="2.9s" dur="0.4s" fill="freeze"/></text>
      <text x="55" y="310" opacity="0" xml:space="preserve">       ═╩═    ═╩═<animate attributeName="opacity" values="0;1" begin="3.2s" dur="0.4s" fill="freeze"/></text>
    </g>
    <rect x="24" y="90" width="420" height="14" fill="url(#scanGrad)">
      <animate attributeName="y" values="80;560;80" dur="6s" repeatCount="indefinite"/>
    </rect>
    <rect x="60" y="330" width="9" height="16" fill="#22D3EE">
      <animate attributeName="opacity" values="1;1;0;0" keyTimes="0;0.5;0.51;1" dur="1s" repeatCount="indefinite"/>
    </rect>
    <text x="44" y="430" class="mono" font-size="12" fill="#94A3B8" opacity="0">
      root@dev:~$ whoami
      <animate attributeName="opacity" values="0;1" begin="3.6s" dur="0.5s" fill="freeze"/>
    </text>
  </g>

  <!-- RIGHT: terminal -->
  <g clip-path="url(#rightClip)">
    <rect x="470" y="24" width="686" height="36" fill="#0F172A"/>
    <circle cx="496" cy="42" r="6" fill="#EF4444"/>
    <circle cx="518" cy="42" r="6" fill="#F59E0B"/>
    <circle cx="540" cy="42" r="6" fill="#10B981"/>
    <text x="1100" y="47" text-anchor="end" class="mono" font-size="12" fill="#94A3B8">bash — profile</text>

    <text x="510" y="105" class="mono" font-size="26" fill="#F8FAFC" opacity="0">Hi 👋
      <animate attributeName="opacity" values="0;1" begin="0.3s" dur="0.6s" fill="freeze"/>
    </text>
    <text x="510" y="140" class="mono" font-size="22" fill="url(#accentGrad)" opacity="0">I'm &#123;NAME&#125;
      <animate attributeName="opacity" values="0;1" begin="0.9s" dur="0.6s" fill="freeze"/>
    </text>

    <g class="mono" font-size="19" fill="#22D3EE">
      <text x="510" y="180" clip-path="url(#typeClip0)">Frontend Engineer</text>
      <text x="510" y="180" clip-path="url(#typeClip1)">Full Stack Developer</text>
      <text x="510" y="180" clip-path="url(#typeClip2)">Open Source Contributor</text>
      <text x="510" y="180" clip-path="url(#typeClip3)">UI Engineer</text>
      <text x="510" y="180" clip-path="url(#typeClip4)">AI Enthusiast</text>
      <rect x="510" y="164" width="9" height="20" fill="#22D3EE">
        <animate attributeName="opacity" values="1;1;0;0" keyTimes="0;0.5;0.51;1" dur="1s" repeatCount="indefinite"/>
      </rect>
    </g>

    <g class="mono" font-size="14" fill="#94A3B8">
      <g opacity="0"><animate attributeName="opacity" values="0;1" begin="1.6s" dur="0.5s" fill="freeze"/>
        <text x="510" y="222">🌍  Location: Your City, Country</text></g>
      <g opacity="0"><animate attributeName="opacity" values="0;1" begin="1.9s" dur="0.5s" fill="freeze"/>
        <text x="510" y="248">🎓  Education: Your Degree, University</text></g>
      <g opacity="0"><animate attributeName="opacity" values="0;1" begin="2.2s" dur="0.5s" fill="freeze"/>
        <text x="510" y="274">🚀  Current Focus: What you're building</text></g>
      <g opacity="0"><animate attributeName="opacity" values="0;1" begin="2.5s" dur="0.5s" fill="freeze"/>
        <text x="510" y="300">🔗  Portfolio: yourportfolio.dev</text></g>
      <g opacity="0"><animate attributeName="opacity" values="0;1" begin="2.8s" dur="0.5s" fill="freeze"/>
        <text x="510" y="326">✉️  Email: you@example.com</text></g>
    </g>

    <text x="510" y="365" class="mono" font-size="13" fill="#F8FAFC" opacity="0.85">Skills</text>
    <g class="mono" font-size="12" font-weight="bold">
      <!-- row 1 -->
      <g class="pill"><rect x="510" y="378" width="66" height="26" rx="13" fill="#0F172A" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)"/><text x="543" y="395" text-anchor="middle" fill="#F8FAFC">React</text></g>
      <g class="pill"><rect x="584" y="378" width="70" height="26" rx="13" fill="#0F172A" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)"/><text x="619" y="395" text-anchor="middle" fill="#F8FAFC">Next.js</text></g>
      <g class="pill"><rect x="662" y="378" width="76" height="26" rx="13" fill="#0F172A" stroke="#10B981" stroke-width="1" filter="url(#softGlow)"/><text x="700" y="395" text-anchor="middle" fill="#F8FAFC">Node.js</text></g>
      <g class="pill"><rect x="746" y="378" width="90" height="26" rx="13" fill="#0F172A" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)"/><text x="791" y="395" text-anchor="middle" fill="#F8FAFC">TypeScript</text></g>
      <g class="pill"><rect x="844" y="378" width="80" height="26" rx="13" fill="#0F172A" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)"/><text x="884" y="395" text-anchor="middle" fill="#F8FAFC">Tailwind</text></g>
      <!-- row 2 -->
      <g class="pill"><rect x="510" y="412" width="72" height="26" rx="13" fill="#0F172A" stroke="#10B981" stroke-width="1" filter="url(#softGlow)"/><text x="546" y="429" text-anchor="middle" fill="#F8FAFC">Python</text></g>
      <g class="pill"><rect x="590" y="412" width="72" height="26" rx="13" fill="#0F172A" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)"/><text x="626" y="429" text-anchor="middle" fill="#F8FAFC">Docker</text></g>
      <g class="pill"><rect x="670" y="412" width="82" height="26" rx="13" fill="#0F172A" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)"/><text x="711" y="429" text-anchor="middle" fill="#F8FAFC">Postgres</text></g>
      <g class="pill"><rect x="760" y="412" width="60" height="26" rx="13" fill="#0F172A" stroke="#10B981" stroke-width="1" filter="url(#softGlow)"/><text x="790" y="429" text-anchor="middle" fill="#F8FAFC">AWS</text></g>
      <g class="pill"><rect x="828" y="412" width="52" height="26" rx="13" fill="#0F172A" stroke="#7C3AED" stroke-width="1" filter="url(#softGlow)"/><text x="854" y="429" text-anchor="middle" fill="#F8FAFC">Git</text></g>
      <g class="pill"><rect x="888" y="412" width="66" height="26" rx="13" fill="#0F172A" stroke="#22D3EE" stroke-width="1" filter="url(#softGlow)"/><text x="921" y="429" text-anchor="middle" fill="#F8FAFC">Figma</text></g>
    </g>

    <line x1="510" y1="465" x2="1122" y2="465" stroke="rgba(255,255,255,.08)" stroke-width="1"/>

    <g class="mono" font-size="13" font-weight="bold">
      <circle cx="530" cy="500" r="18" fill="#0F172A" stroke="#7C3AED" stroke-width="1.2" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" repeatCount="indefinite"/>
      </circle>
      <text x="530" y="504" text-anchor="middle" fill="#F8FAFC" font-size="11">GH</text>

      <circle cx="590" cy="500" r="18" fill="#0F172A" stroke="#22D3EE" stroke-width="1.2" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="0.4s" repeatCount="indefinite"/>
      </circle>
      <text x="590" y="504" text-anchor="middle" fill="#F8FAFC" font-size="11">in</text>

      <circle cx="650" cy="500" r="18" fill="#0F172A" stroke="#10B981" stroke-width="1.2" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="0.8s" repeatCount="indefinite"/>
      </circle>
      <text x="650" y="504" text-anchor="middle" fill="#F8FAFC" font-size="11">X</text>

      <circle cx="710" cy="500" r="18" fill="#0F172A" stroke="#7C3AED" stroke-width="1.2" filter="url(#softGlow)">
        <animate attributeName="stroke-opacity" values="0.5;1;0.5" dur="3s" begin="1.2s" repeatCount="indefinite"/>
      </circle>
      <text x="710" y="504" text-anchor="middle" fill="#F8FAFC" font-size="13">🔗</text>
    </g>
  </g>
</g>
</svg>
