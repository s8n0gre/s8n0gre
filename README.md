<!-- #################################################################### -->
<!--                   BOOT SEQUENCE — HEADER                           -->
<!-- #################################################################### -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0d1117,25:0a0a0a,50:001200,75:001a00,100:0d1117&height=220&section=header&text=s8n0gre&fontSize=68&fontColor=39FF14&animation=fadeIn&fontAlignY=58&desc=%5B%20SOFTWARE%20ENGINEERING%20STUDENT%20%5D&descSize=14&descAlignY=78&descAlign=50&stroke=39FF14&strokeWidth=2" />

</div>

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 860 520" width="860" height="520">
  <defs>
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Share+Tech+Mono&display=swap');
      text { font-family: 'Share Tech Mono', 'Courier New', monospace; }
    </style>
    <!-- Scanline pattern -->
    <pattern id="scan" x="0" y="0" width="860" height="4" patternUnits="userSpaceOnUse">
      <rect width="860" height="2" fill="#00ff41" opacity="0.03"/>
    </pattern>
    <!-- Glow filter -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="2.5" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glow2" x="-10%" y="-10%" width="120%" height="120%">
      <feGaussianBlur stdDeviation="1.2" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <!-- Matrix rain clip -->
    <clipPath id="rain-clip">
      <rect x="0" y="0" width="860" height="520"/>
    </clipPath>
  </defs>

  <!-- Background -->
  <rect width="860" height="520" fill="#050d05"/>
  <!-- Subtle grid -->
  <rect width="860" height="520" fill="url(#scan)"/>

  <!-- ─── MATRIX RAIN COLUMNS ─── -->
  <g clip-path="url(#rain-clip)" opacity="0.18" filter="url(#glow2)">
    <!-- col 1 -->
    <text x="12" y="0" font-size="11" fill="#00ff41">
      1<animate attributeName="y" from="-40" to="540" dur="3.1s" repeatCount="indefinite"/>
    </text>
    <text x="12" y="-80" font-size="11" fill="#00ff41">
      0<animate attributeName="y" from="-120" to="460" dur="3.1s" repeatCount="indefinite"/>
    </text>
    <!-- col 2 -->
    <text x="35" y="0" font-size="11" fill="#00ff41">
      A<animate attributeName="y" from="-20" to="540" dur="2.4s" begin="0.6s" repeatCount="indefinite"/>
    </text>
    <text x="35" y="-60" font-size="11" fill="#00ff41">
      F<animate attributeName="y" from="-100" to="460" dur="2.4s" begin="0.6s" repeatCount="indefinite"/>
    </text>
    <!-- col 3 -->
    <text x="58" y="0" font-size="11" fill="#00ff41">
      3<animate attributeName="y" from="-60" to="540" dur="3.8s" begin="1.2s" repeatCount="indefinite"/>
    </text>
    <!-- col 4 -->
    <text x="810" y="0" font-size="11" fill="#00ff41">
      9<animate attributeName="y" from="-30" to="540" dur="2.8s" begin="0.3s" repeatCount="indefinite"/>
    </text>
    <text x="810" y="-90" font-size="11" fill="#00ff41">
      B<animate attributeName="y" from="-130" to="460" dur="2.8s" begin="0.3s" repeatCount="indefinite"/>
    </text>
    <!-- col 5 -->
    <text x="835" y="0" font-size="11" fill="#00ff41">
      7<animate attributeName="y" from="-50" to="540" dur="3.4s" begin="1.8s" repeatCount="indefinite"/>
    </text>
    <!-- col 6 -->
    <text x="788" y="0" font-size="11" fill="#00ff41">
      E<animate attributeName="y" from="-10" to="540" dur="2.2s" begin="0.9s" repeatCount="indefinite"/>
    </text>
    <text x="788" y="-80" font-size="11" fill="#00ff41">
      2<animate attributeName="y" from="-120" to="460" dur="2.2s" begin="0.9s" repeatCount="indefinite"/>
    </text>
  </g>

  <!-- ─── OUTER BORDER BOX ─── -->
  <!-- Draw with animated stroke-dashoffset for "drawing in" effect -->
  <!-- Top line -->
  <line x1="20" y1="18" x2="840" y2="18" stroke="#00ff41" stroke-width="1.2" opacity="0.9">
    <animate attributeName="stroke-dasharray" from="0 1000" to="820 0" dur="0.6s" fill="freeze" begin="0.1s"/>
  </line>
  <!-- Bottom line -->
  <line x1="20" y1="502" x2="840" y2="502" stroke="#00ff41" stroke-width="1.2" opacity="0.9">
    <animate attributeName="stroke-dasharray" from="0 1000" to="820 0" dur="0.6s" fill="freeze" begin="0.3s"/>
  </line>
  <!-- Left line -->
  <line x1="20" y1="18" x2="20" y2="502" stroke="#00ff41" stroke-width="1.2" opacity="0.9">
    <animate attributeName="stroke-dasharray" from="0 600" to="484 0" dur="0.5s" fill="freeze" begin="0.5s"/>
  </line>
  <!-- Right line -->
  <line x1="840" y1="18" x2="840" y2="502" stroke="#00ff41" stroke-width="1.2" opacity="0.9">
    <animate attributeName="stroke-dasharray" from="0 600" to="484 0" dur="0.5s" fill="freeze" begin="0.5s"/>
  </line>
  <!-- Corner accents -->
  <g fill="none" stroke="#00ff41" stroke-width="1.5">
    <polyline points="20,18 20,18" opacity="0.9">
      <animate attributeName="points" from="20,18 20,18 20,18" to="20,38 20,18 40,18" dur="0.3s" fill="freeze" begin="0.9s"/>
    </polyline>
    <polyline points="840,18 840,18" opacity="0.9">
      <animate attributeName="points" from="840,18 840,18 840,18" to="820,18 840,18 840,38" dur="0.3s" fill="freeze" begin="0.9s"/>
    </polyline>
    <polyline points="20,502 20,502" opacity="0.9">
      <animate attributeName="points" from="20,502 20,502 20,502" to="20,482 20,502 40,502" dur="0.3s" fill="freeze" begin="0.9s"/>
    </polyline>
    <polyline points="840,502 840,502" opacity="0.9">
      <animate attributeName="points" from="840,502 840,502 840,502" to="820,502 840,502 840,482" dur="0.3s" fill="freeze" begin="0.9s"/>
    </polyline>
  </g>

  <!-- ─── DIVIDER LINES ─── -->
  <line x1="20" y1="162" x2="840" y2="162" stroke="#00ff41" stroke-width="0.8" opacity="0.5">
    <animate attributeName="opacity" from="0" to="0.5" dur="0.2s" fill="freeze" begin="1.0s"/>
  </line>
  <line x1="20" y1="270" x2="840" y2="270" stroke="#00ff41" stroke-width="0.8" opacity="0.5">
    <animate attributeName="opacity" from="0" to="0.5" dur="0.2s" fill="freeze" begin="1.6s"/>
  </line>
  <line x1="20" y1="390" x2="840" y2="390" stroke="#00ff41" stroke-width="0.8" opacity="0.5">
    <animate attributeName="opacity" from="0" to="0.5" dur="0.2s" fill="freeze" begin="2.4s"/>
  </line>

  <!-- ─── s8n0gre ASCII BANNER ─── -->
  <g filter="url(#glow)" fill="#00ff41" font-size="12.5" letter-spacing="0">
    <text x="80" y="58" opacity="0">
      ██████╗  █████╗ ███╗  ██╗ ██████╗  ██████╗ ██████╗ ███████╗
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.1s"/>
    </text>
    <text x="80" y="77" opacity="0">
      ██╔════╝ ██╔══██╗████╗ ██║██╔═══██╗██╔════╝ ██╔══██╗██╔════╝
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.22s"/>
    </text>
    <text x="80" y="96" opacity="0">
      ╚█████╗  ╚█████╔╝██╔██╗██║██║   ██║██║  ███╗██████╔╝█████╗
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.34s"/>
    </text>
    <text x="80" y="115" opacity="0">
       ╚═══██╗ ██╔══██╗██║╚████║██║   ██║██║   ██║██╔══██╗██╔══╝
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.46s"/>
    </text>
    <text x="80" y="134" opacity="0">
      ██████╔╝ ██║  ██║██║ ╚███║╚██████╔╝╚██████╔╝██║  ██║███████╗
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.58s"/>
    </text>
    <text x="80" y="153" opacity="0">
      ╚═════╝  ╚═╝  ╚═╝╚═╝  ╚══╝ ╚═════╝  ╚═════╝ ╚═╝  ╚═╝╚══════╝
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.70s"/>
    </text>
  </g>

  <!-- ─── DEDSEC ASCII BANNER ─── -->
  <g filter="url(#glow)" fill="#39ff14" font-size="12.5" letter-spacing="0">
    <text x="108" y="192" opacity="0">
      ██████╗ ███████╗██████╗ ███████╗███████╗ ██████╗
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.85s"/>
    </text>
    <text x="108" y="211" opacity="0">
      ██╔══██╗██╔════╝██╔══██╗██╔════╝██╔════╝██╔════╝
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="1.97s"/>
    </text>
    <text x="108" y="230" opacity="0">
      ██║  ██║█████╗  ██║  ██║███████╗█████╗  ██║
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="2.09s"/>
    </text>
    <text x="108" y="249" opacity="0">
      ██║  ██║██╔══╝  ██║  ██║╚════██║██╔══╝  ██║
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="2.21s"/>
    </text>
    <text x="108" y="268" opacity="0">
      ██████╔╝███████╗██████╔╝███████║███████╗╚██████╗
      <animate attributeName="opacity" from="0" to="1" dur="0.15s" fill="freeze" begin="2.33s"/>
    </text>
  </g>

  <!-- ─── BREACH SEQUENCE ─── -->
  <g font-size="12" fill="#00ff41" font-family="'Share Tech Mono','Courier New',monospace">

    <!-- Line 1 -->
    <text x="44" y="302" opacity="0">
      &gt;  BREACH INITIATED
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="2.6s"/>
    </text>
    <text x="380" y="302" opacity="0" fill="#00cc33">
      ........................................
      <animate attributeName="opacity" from="0" to="1" dur="0.3s" fill="freeze" begin="2.7s"/>
    </text>
    <text x="748" y="302" opacity="0" fill="#00ff41" filter="url(#glow2)">
      [OK]
      <animate attributeName="opacity" from="0" to="0.9" dur="0.1s" fill="freeze" begin="3.0s"/>
    </text>

    <!-- Line 2 -->
    <text x="44" y="322" opacity="0">
      &gt;  TARGET SYSTEM  ........ github.com/s8n0gre
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="3.1s"/>
    </text>
    <text x="672" y="322" opacity="0" fill="#00cc33">
      ............
      <animate attributeName="opacity" from="0" to="1" dur="0.2s" fill="freeze" begin="3.2s"/>
    </text>
    <text x="748" y="322" opacity="0" fill="#00ff41" filter="url(#glow2)">
      [OK]
      <animate attributeName="opacity" from="0" to="0.9" dur="0.1s" fill="freeze" begin="3.4s"/>
    </text>

    <!-- Line 3 -->
    <text x="44" y="342" opacity="0">
      &gt;  FIREWALL STATUS ........ BYPASSED
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="3.5s"/>
    </text>
    <text x="596" y="342" opacity="0" fill="#00cc33">
      ...........................
      <animate attributeName="opacity" from="0" to="1" dur="0.2s" fill="freeze" begin="3.6s"/>
    </text>
    <text x="748" y="342" opacity="0" fill="#00ff41" filter="url(#glow2)">
      [OK]
      <animate attributeName="opacity" from="0" to="0.9" dur="0.1s" fill="freeze" begin="3.8s"/>
    </text>

    <!-- Line 4 -->
    <text x="44" y="362" opacity="0">
      &gt;  IDENTITY MASK  ........ ACTIVE
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="3.9s"/>
    </text>
    <text x="568" y="362" opacity="0" fill="#00cc33">
      .....................................
      <animate attributeName="opacity" from="0" to="1" dur="0.2s" fill="freeze" begin="4.0s"/>
    </text>
    <text x="748" y="362" opacity="0" fill="#00ff41" filter="url(#glow2)">
      [OK]
      <animate attributeName="opacity" from="0" to="0.9" dur="0.1s" fill="freeze" begin="4.2s"/>
    </text>

    <!-- Line 5 -->
    <text x="44" y="382" opacity="0">
      &gt;  CTOS ACCESS    ........ ROOT GRANTED
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="4.3s"/>
    </text>
    <text x="610" y="382" opacity="0" fill="#00cc33">
      .................................
      <animate attributeName="opacity" from="0" to="1" dur="0.2s" fill="freeze" begin="4.4s"/>
    </text>
    <text x="748" y="382" opacity="0" fill="#00ff41" filter="url(#glow2)">
      [OK]
      <animate attributeName="opacity" from="0" to="0.9" dur="0.1s" fill="freeze" begin="4.6s"/>
    </text>
  </g>

  <!-- ─── OPERATOR TABLE ─── -->
  <g font-size="12" fill="#00ff41" font-family="'Share Tech Mono','Courier New',monospace">

    <!-- OPERATOR -->
    <text x="44" y="418" opacity="0">
      OPERATOR
      <animate attributeName="opacity" from="0" to="0.7" dur="0.1s" fill="freeze" begin="4.8s"/>
    </text>
    <text x="160" y="418" opacity="0" fill="#005500">
      ──────────────────────────────────────────────────
      <animate attributeName="opacity" from="0" to="1" dur="0.25s" fill="freeze" begin="4.85s"/>
    </text>
    <text x="720" y="418" opacity="0" filter="url(#glow2)">
      s8n0gre
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="5.1s"/>
    </text>

    <!-- FACTION -->
    <text x="44" y="436" opacity="0">
      FACTION
      <animate attributeName="opacity" from="0" to="0.7" dur="0.1s" fill="freeze" begin="5.1s"/>
    </text>
    <text x="160" y="436" opacity="0" fill="#005500">
      ──────────────────────────────────────────────────
      <animate attributeName="opacity" from="0" to="1" dur="0.25s" fill="freeze" begin="5.15s"/>
    </text>
    <text x="720" y="436" opacity="0">
      INDEPENDENT
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="5.4s"/>
    </text>

    <!-- MISSION -->
    <text x="44" y="454" opacity="0">
      MISSION
      <animate attributeName="opacity" from="0" to="0.7" dur="0.1s" fill="freeze" begin="5.4s"/>
    </text>
    <text x="160" y="454" opacity="0" fill="#005500">
      ──────────────────────────────────────────────────
      <animate attributeName="opacity" from="0" to="1" dur="0.25s" fill="freeze" begin="5.45s"/>
    </text>
    <text x="720" y="454" opacity="0">
      DSA x SYSTEMS
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="5.7s"/>
    </text>

    <!-- THREAT -->
    <text x="44" y="472" opacity="0">
      THREAT
      <animate attributeName="opacity" from="0" to="0.7" dur="0.1s" fill="freeze" begin="5.7s"/>
    </text>
    <text x="160" y="472" opacity="0" fill="#005500">
      ──────────────────────────────────────────────────
      <animate attributeName="opacity" from="0" to="1" dur="0.25s" fill="freeze" begin="5.75s"/>
    </text>
    <text x="720" y="472" opacity="0">
      TO BUGS ONLY
      <animate attributeName="opacity" from="0" to="1" dur="0.1s" fill="freeze" begin="6.0s"/>
    </text>
  </g>

  <!-- ─── WARNING LINES ─── -->
  <g font-size="11" font-family="'Share Tech Mono','Courier New',monospace">
    <text x="44" y="492" fill="#ff4444" opacity="0">
      [ WRN ]  Do not attempt to trace this connection. All activity is logged.
      <animate attributeName="opacity" from="0" to="0.85" dur="0.4s" fill="freeze" begin="6.1s"/>
      <!-- Pulse -->
      <animate attributeName="opacity" from="0.85" to="0.3" dur="1.4s" repeatCount="indefinite" begin="7s"/>
    </text>
  </g>

  <!-- ─── BLINKING CURSOR ─── -->
  <rect x="44" y="298" width="7" height="13" fill="#00ff41">
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite" begin="6.5s"/>
    <animate attributeName="x" from="44" to="750" dur="4s" fill="freeze" begin="2.6s"/>
    <!-- after typing done, park cursor at end -->
    <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite" begin="6.5s"/>
  </rect>

  <!-- ─── SCANLINE FLICKER OVERLAY ─── -->
  <rect width="860" height="520" fill="#00ff41" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0.04;0;0;0.02;0;0;0" dur="8s" repeatCount="indefinite" begin="0s"/>
  </rect>
</svg>

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=16&duration=2500&pause=900&color=39FF14&center=true&vCenter=true&width=560&height=38&lines=%24+whoami+--+s8n0gre;%24+status+--+always+learning;%24+mission+--+300%2B+DSA+problems+in+2026;%24+engine+--+chess-driven+thinking;%24+uptime+--+counting..." />

</div>

<br/>

<div align="center">

[![Profile Views](https://komarev.com/ghpvc/?username=s8n0gre&style=for-the-badge&color=39FF14&labelColor=0d1117&label=VISITORS)](https://github.com/s8n0gre)
&nbsp;
[![GitHub followers](https://img.shields.io/github/followers/s8n0gre?style=for-the-badge&color=39FF14&labelColor=0d1117&label=FOLLOWERS&logo=github)](https://github.com/s8n0gre)
&nbsp;
[![GitHub stars](https://img.shields.io/github/stars/s8n0gre?style=for-the-badge&color=39FF14&labelColor=0d1117&label=STARS&logo=github)](https://github.com/s8n0gre)

</div>

<br/>

---

<!-- #################################################################### -->
<!--                        SYSTEM INFO                                  -->
<!-- #################################################################### -->

<div align="center">

```
┌─────────────────────────────────────────────────────────────────┐
│                     [ SYSTEM PROFILE ]                          │
├──────────────────────┬──────────────────────────────────────────┤
│  PROCESS             │  SOFTWARE_ENGINEERING_STUDENT.exe        │
│  ARCHITECTURE        │  PROBLEM_SOLVER × CHESS_THINKER          │
│  KERNEL              │  ALGORITHMS v∞                           │
│  MEMORY              │  Loaded with DSA patterns                │
│  SCHEDULER           │  Daily grind — no zero days              │
│  LANGUAGE_RUNTIME    │  C++ · Java · Python · JS                │
│  UPTIME              │  Still counting...                       │
│  THREAT_LEVEL        │  MAXIMUM (to bugs)                       │
└──────────────────────┴──────────────────────────────────────────┘
```

</div>

<br/>

---

<!-- #################################################################### -->
<!--                    INIT SEQUENCE — ABOUT                            -->
<!-- #################################################################### -->

<div align="center">

```
╭───────────────────────────────────────────────────────────────╮
│  >_ INIT: loading developer instance...                       │
╰───────────────────────────────────────────────────────────────╯
```

</div>

```python
#!/usr/bin/env python3
# ┌─────────────────────────────────────────────────┐
# │         s8n0gre.py  —  instance config          │
# └─────────────────────────────────────────────────┘

class Developer:
    def __init__(self):
        self.alias        = "s8n0gre"
        self.role         = "Software Engineering Student"
        self.os           = "Arch Linux (btw)"
        self.editor       = "VS Code  [ vim mode ON ]"
        self.languages    = ["C++", "Java", "Python", "JavaScript"]
        self.stack        = ["HTML", "CSS", "Git", "GitHub"]
        self.focus        = ["Data Structures", "Algorithms", "System Design"]
        self.mindset      = "Chess-driven · Analytical · Relentless"
        self.current_run  = "300+ DSA problems — 2026"
        self.philosophy   = "Think in trees. Code in branches. Win on roots."
        self.weakness     = "Starting is the hardest part"  # working on it

    def status(self) -> str:
        return "[  ONLINE  ] — always building, always learning"

    def contact(self) -> dict:
        return { "github": "github.com/s8n0gre" }

if __name__ == "__main__":
    dev = Developer()
    print(dev.status())
```

<br/>

---

<!-- #################################################################### -->
<!--                  RAINBOW REPTILE CONTRIBUTION                       -->
<!-- #################################################################### -->

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)"
    srcset="https://raw.githubusercontent.com/s8n0gre/s8n0gre/output/pacman-contribution-graph-dark.svg" />
  <source media="(prefers-color-scheme: light)"
    srcset="https://raw.githubusercontent.com/s8n0gre/s8n0gre/output/pacman-contribution-graph.svg" />
  <img
    alt="pacman devouring contributions"
    src="https://raw.githubusercontent.com/s8n0gre/s8n0gre/output/pacman-contribution-graph.svg"
    width="100%" />
</picture>

</div>

<br/>

---

<!-- #################################################################### -->
<!--                         TECH STACK                                  -->
<!-- #################################################################### -->

<div align="center">

```
╔═══════════════════════════════════════════════════════════════════╗
║                >_ TECH ARSENAL — MODULES LOADED                  ║
╠════════════════╦═══════════════════════╦══════════════════════════╣
║  LANGUAGES     ║  WEB                  ║  TOOLCHAIN               ║
╠════════════════╬═══════════════════════╬══════════════════════════╣
║  ► C++         ║  ► JavaScript         ║  ► Git                   ║
║  ► Java        ║  ► HTML5              ║  ► GitHub                ║
║  ► Python      ║  ► CSS3               ║  ► VS Code               ║
╚════════════════╩═══════════════════════╩══════════════════════════╝
```
<br/><br/>

<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub-161B22?style=for-the-badge&logo=github&logoColor=white" />

</div>

<br/>

---

<!-- #################################################################### -->
<!--                       GITHUB METRICS                                -->
<!-- #################################################################### -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║            >_ DIAGNOSTIC REPORT — github.com/s8n0gre            ║
╚══════════════════════════════════════════════════════════════════╝
```

<img src="https://github-readme-stats.vercel.app/api?username=s8n0gre&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=39FF14&icon_color=39FF14&text_color=C9D1D9&border_radius=6&ring_color=39FF14" height="170" />
&nbsp;
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=s8n0gre&layout=compact&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=39FF14&text_color=C9D1D9&border_radius=6" height="170" />

<br/><br/>

<img src="https://streak-stats.demolab.com?user=s8n0gre&theme=github-dark-blue&hide_border=true&background=0D1117&ring=39FF14&fire=39FF14&currStreakLabel=39FF14&sideLabels=9FB3C8&dates=C9D1D9&border_radius=6" width="65%" />

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=s8n0gre&theme=matrix&no-frame=true&no-bg=true&margin-w=6&column=7" width="100%" />

</div>

<br/>

---

<!-- #################################################################### -->
<!--                      ACTIVITY GRAPH                                 -->
<!-- #################################################################### -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║            >_ COMMIT HEATMAP — activity.log                      ║
╚══════════════════════════════════════════════════════════════════╝
```

<img src="https://github-readme-activity-graph.vercel.app/graph?username=s8n0gre&theme=github-dark&bg_color=0d1117&color=39FF14&line=39FF14&point=ffffff&area=true&area_color=003300&hide_border=true&radius=4" width="100%" />

</div>

<br/>

---

<!-- #################################################################### -->
<!--                      DSA PROGRESS TERMINAL                          -->
<!-- #################################################################### -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║               >_ DSA PROGRESS REPORT — 2026.log                 ║
╠══════════════════════════════════════════════════════════════════╣
║                                                                  ║
║  Arrays        ████████████████░░░░░░░░░░░░  [ACTIVE]           ║
║  Linked Lists  ██████████████░░░░░░░░░░░░░░  [ACTIVE]           ║
║  Trees         ████████████░░░░░░░░░░░░░░░░  [IN PROGRESS]      ║
║  Graphs        ████████░░░░░░░░░░░░░░░░░░░░  [LOADING...]       ║
║  Dynamic Prog  ██████░░░░░░░░░░░░░░░░░░░░░░  [UNLOCKING...]     ║
║  Backtracking  █████░░░░░░░░░░░░░░░░░░░░░░░  [QUEUED]           ║
║                                                                  ║
║  TARGET: 300 problems  ░░░░░░░░░░░░░░░░░░░░  [GRINDING]         ║
╚══════════════════════════════════════════════════════════════════╝
```

</div>

<br/>

---

<!-- #################################################################### -->
<!--                       2026 OBJECTIVES                               -->
<!-- #################################################################### -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║                  >_ MISSION BRIEF — 2026                         ║
╚══════════════════════════════════════════════════════════════════╝
```

</div>

```yaml
# ┌──────────────────────────────────────────────────────────┐
# │            OBJECTIVES.yml  —  FY 2026                    │
# └──────────────────────────────────────────────────────────┘

DSA:
  target:    "300+ problems solved"
  domains:   [arrays, linked-lists, trees, graphs, dp, backtracking]
  platforms: [LeetCode, Codeforces, HackerRank]
  strategy:  "pattern recognition over brute force memorization"

Development:
  goal:      "ship projects, not just ideas"
  stack:     "frontend foundations → backend logic → APIs"
  rule:      "build → break → learn → repeat"

Mindset:
  mode:      "chess player — always 3 moves ahead"
  practice:  "no zero days"
  mantra:    "every bug is a feature not yet understood"

System:
  uptime:    "365/365"
  logging:   "git commit -m 'consistent'"
  exit_code: 0  # always finish what you start
```

<br/>

---

<!-- #################################################################### -->
<!--                          FOCUS MATRIX                               -->
<!-- #################################################################### -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║                    >_ FOCUS MATRIX                               ║
╠══════════════════╦══════════════════╦════════════════════════════╣
║  CATEGORY        ║  STATUS          ║  PRIORITY                  ║
╠══════════════════╬══════════════════╬════════════════════════════╣
║  DSA             ║  [##########]    ║  CRITICAL                  ║
║  Problem Solving ║  [#########·]    ║  CRITICAL                  ║
║  Projects        ║  [######····]    ║  HIGH                      ║
║  Backend         ║  [####······]    ║  MEDIUM                    ║
║  Chess           ║  [##########]    ║  ALWAYS                    ║
╚══════════════════╩══════════════════╩════════════════════════════╝
```

<br/>

<img src="https://img.shields.io/badge/DSA-CRITICAL-39FF14?style=for-the-badge&labelColor=0d1117&logo=leetcode&logoColor=39FF14" />
<img src="https://img.shields.io/badge/Projects-HIGH-58A6FF?style=for-the-badge&labelColor=0d1117&logo=github&logoColor=58A6FF" />
<img src="https://img.shields.io/badge/Backend-MEDIUM-ffaa00?style=for-the-badge&labelColor=0d1117&logo=node.js&logoColor=ffaa00" />
<img src="https://img.shields.io/badge/Chess-ALWAYS-ff4444?style=for-the-badge&labelColor=0d1117&logo=lichess&logoColor=ff4444" />

</div>

<br/>

---

<!-- #################################################################### -->
<!--                           FOOTER                                    -->
<!-- #################################################################### -->

<div align="center">

```
╔══════════════════════════════════════════════════════════════════╗
║                                                                  ║
║   "The only way to get better is to never stop being worse."     ║
║                                                                  ║
║   [ github.com/s8n0gre ]  ·  [ ALWAYS BUILDING ]  ·  [ 2026 ]  ║
║                                                                  ║
╚══════════════════════════════════════════════════════════════════╝
```

<img src="https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&size=13&duration=3000&pause=1200&color=39FF14&center=true&vCenter=true&width=480&lines=%24+shutdown+--graceful+--save+progress;Saving+state...+%5B+OK+%5D;Committing+to+main...+%5B+OK+%5D;Session+logged.+See+you+tomorrow." />

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:001200,80:001a00,100:0d1117&height=110&section=footer&fontColor=39FF14" />

</div>
