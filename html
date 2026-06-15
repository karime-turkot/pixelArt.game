<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>PixelForge — Editor de Pixel Art</title>
  <style>
    /* =========================================================
       PIXELFORGE — CSS
       Tudo quadrado. Sem border-radius. Pixel é pixel.
    ========================================================= */
 
    @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');
 
    :root {
      --bg:        #0d0d1a;
      --surface:   #13131f;
      --surface2:  #1a1a2e;
      --border:    #2a2a50;
 
      --purple:    #c000e0;
      --cyan:      #00d4ff;
      --yellow:    #ffe600;
      --green:     #00ff88;
      --red:       #ff2244;
      --white:     #f0f0ff;
      --muted:     #555580;
      --dim:       #2a2a4a;
 
      --font: 'Press Start 2P', monospace;
    }
 
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
 
    html { font-size: 16px; }
 
    body {
      background: var(--bg);
      color: var(--white);
      font-family: var(--font);
      font-size: 10px;
      line-height: 1.8;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      overflow-x: hidden;
    }
 
    /* ── SCANLINES overlay ── */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 999;
      background: repeating-linear-gradient(
        to bottom,
        transparent 0px,
        transparent 3px,
        rgba(0,0,0,0.18) 3px,
        rgba(0,0,0,0.18) 4px
      );
    }
 
    /* ── TOPBAR ── */
    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 12px 24px;
      background: var(--surface);
      border-bottom: 3px solid var(--purple);
      box-shadow: 0 0 20px rgba(192,0,224,0.4);
      gap: 16px;
      flex-wrap: wrap;
    }
 
    .topbar-logo {
      font-size: 13px;
      color: var(--purple);
      text-shadow: 0 0 10px var(--purple), 0 0 30px var(--purple);
      letter-spacing: 2px;
    }
 
    .topbar-status {
      display: flex;
      align-items: center;
      gap: 8px;
      color: var(--muted);
      font-size: 8px;
    }
 
    .status-dot {
      width: 8px;
      height: 8px;
      background: var(--green);
      box-shadow: 0 0 6px var(--green);
      animation: pulse 1.5s step-end infinite;
    }
 
    @keyframes pulse {
      0%, 100% { opacity: 1; }
      50%       { opacity: 0; }
    }
 
    .topbar-nav {
      display: flex;
      gap: 16px;
      list-style: none;
    }
 
    .topbar-nav a {
      color: var(--muted);
      text-decoration: none;
      font-size: 8px;
      letter-spacing: 1px;
      transition: color 0.1s, text-shadow 0.1s;
    }
 
    .topbar-nav a:hover, .topbar-nav a.active {
      color: var(--cyan);
      text-shadow: 0 0 8px var(--cyan);
    }
 
    /* ── HERO ── */
    .hero {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 48px 24px;
      gap: 32px;
      position: relative;
    }
 
    /* fundo de pixels aleatórios */
    #bgCanvas {
      position: fixed;
      inset: 0;
      z-index: 0;
      opacity: 0.06;
      pointer-events: none;
    }
 
    .hero > * { position: relative; z-index: 1; }
 
    /* título principal */
    .hero-title {
      font-size: clamp(20px, 5vw, 40px);
      color: var(--white);
      text-align: center;
      line-height: 1.6;
      text-shadow:
        4px 4px 0 var(--purple),
        8px 8px 0 rgba(192,0,224,0.3),
        0 0 40px rgba(192,0,224,0.6);
      letter-spacing: 3px;
    }
 
    .hero-title span {
      color: var(--cyan);
      text-shadow: 0 0 12px var(--cyan), 0 0 40px var(--cyan);
    }
 
    .hero-sub {
      font-size: 9px;
      color: var(--cyan);
      letter-spacing: 4px;
      text-align: center;
      text-shadow: 0 0 8px var(--cyan);
      text-transform: uppercase;
    }
 
    .hero-desc {
      font-size: 9px;
      color: var(--muted);
      text-align: center;
      max-width: 480px;
      line-height: 2.2;
      border-left: 3px solid var(--purple);
      border-right: 3px solid var(--cyan);
      padding: 16px 20px;
      background: var(--surface);
    }
 
    .hero-desc strong { color: var(--yellow); }
 
    /* ── GRADE DE PRÉVIA INTERATIVA ── */
    .canvas-wrap {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 12px;
    }
 
    .canvas-label {
      font-size: 8px;
      color: var(--muted);
      letter-spacing: 2px;
    }
 
    #previewCanvas {
      border: 3px solid var(--purple);
      box-shadow:
        0 0 0 1px var(--dim),
        0 0 20px rgba(192,0,224,0.5),
        0 0 60px rgba(192,0,224,0.2);
      cursor: crosshair;
      image-rendering: pixelated;
      display: block;
    }
 
    .canvas-hint {
      font-size: 7px;
      color: var(--dim);
      letter-spacing: 1px;
      animation: blink 1.2s step-end infinite;
    }
 
    @keyframes blink {
      0%, 100% { opacity: 1; }
      50%       { opacity: 0; }
    }
 
    /* ── TOOLBAR ── */
    .toolbar {
      display: flex;
      align-items: center;
      gap: 6px;
      background: var(--surface);
      border: 2px solid var(--border);
      padding: 10px 16px;
      box-shadow: 0 4px 0 var(--dim);
      flex-wrap: wrap;
      justify-content: center;
    }
 
    .tool-btn {
      width: 38px;
      height: 38px;
      background: var(--surface2);
      border: 2px solid var(--border);
      color: var(--white);
      font-size: 16px;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: border-color 0.1s, box-shadow 0.1s;
    }
 
    .tool-btn:hover { border-color: var(--cyan); box-shadow: 0 0 8px var(--cyan); }
    .tool-btn.active { border-color: var(--purple); box-shadow: 0 0 10px var(--purple); background: rgba(192,0,224,0.15); }
 
    .tool-sep { width: 2px; height: 32px; background: var(--border); margin: 0 4px; }
 
    .swatch {
      width: 28px;
      height: 28px;
      border: 2px solid var(--border);
      cursor: pointer;
      transition: transform 0.1s, box-shadow 0.1s;
    }
 
    .swatch:hover { transform: scale(1.25); }
    .swatch.active { outline: 2px solid var(--white); outline-offset: 2px; }
 
    .color-input-wrap {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2px;
      font-size: 7px;
      color: var(--muted);
    }
 
    #colorPicker {
      width: 38px;
      height: 28px;
      border: 2px solid var(--border);
      background: none;
      cursor: pointer;
      padding: 0;
    }
 
    .clear-btn {
      padding: 0 12px;
      height: 38px;
      background: var(--surface2);
      border: 2px solid var(--red);
      color: var(--red);
      font-family: var(--font);
      font-size: 7px;
      cursor: pointer;
      letter-spacing: 1px;
      transition: background 0.1s, box-shadow 0.1s;
    }
 
    .clear-btn:hover { background: rgba(255,34,68,0.15); box-shadow: 0 0 10px var(--red); }
 
    /* ── FEATURES / INFO ── */
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 2px;
      max-width: 720px;
      width: 100%;
    }
 
    .feature-card {
      background: var(--surface);
      border: 2px solid var(--border);
      padding: 20px 16px;
      display: flex;
      flex-direction: column;
      gap: 10px;
      transition: border-color 0.15s, box-shadow 0.15s;
    }
 
    .feature-card:hover { border-color: var(--purple); box-shadow: 0 0 12px rgba(192,0,224,0.3); }
 
    .feature-icon { font-size: 22px; }
 
    .feature-title {
      font-size: 8px;
      color: var(--cyan);
      letter-spacing: 1px;
    }
 
    .feature-desc {
      font-size: 7px;
      color: var(--muted);
      line-height: 2;
    }
 
    /* ── FOOTER ── */
    .footer {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 16px;
      padding: 12px 24px;
      background: var(--surface);
      border-top: 2px solid var(--border);
      font-size: 7px;
      color: var(--dim);
      flex-wrap: wrap;
      text-align: center;
    }
 
    .footer-cursor {
      color: var(--purple);
      text-shadow: 0 0 6px var(--purple);
      animation: blink 0.8s step-end infinite;
    }
 
    /* ── RESPONSIVO ── */
    @media (max-width: 500px) {
      .topbar-nav { display: none; }
      .hero { padding: 32px 16px; }
      .features { grid-template-columns: 1fr; }
    }
 
    @media (prefers-reduced-motion: reduce) {
      *, *::before, *::after { animation: none !important; transition: none !important; }
    }
  </style>
</head>
<body>
 
  <!-- FUNDO ANIMADO -->
  <canvas id="bgCanvas"></canvas>
 
  <!-- TOPBAR -->
  <nav class="topbar">
    <div class="topbar-logo">&#x2588; PIXELFORGE</div>
    <div class="topbar-status">
      <div class="status-dot"></div>
      EDITOR ONLINE
    </div>
    <ul class="topbar-nav">
      <li><a href="#" class="active">[ INICIO ]</a></li>
      <li><a href="#">[ GALERIA ]</a></li>
      <li><a href="#">[ AJUDA ]</a></li>
    </ul>
  </nav>
 
  <!-- HERO -->
  <main class="hero">
 
    <p class="hero-sub">&#x25BA; editor de pixel art no navegador</p>
 
    <h1 class="hero-title">PIXEL<span>FORGE</span></h1>
 
    <p class="hero-desc">
      Escolha uma cor, clique ou arraste sobre a grade e<br>
      dê vida à sua arte — <strong>pixel por pixel</strong>.<br>
      Ferramentas simples. Possibilidades infinitas.
    </p>
 
    <!-- GRADE INTERATIVA -->
    <div class="canvas-wrap">
      <div class="canvas-label">&#x25BA; GRADE DE PIXELS — TENTE PINTAR!</div>
      <canvas id="previewCanvas" width="480" height="300"></canvas>
      <div class="canvas-hint">&#x2588; CLIQUE E ARRASTE PARA PINTAR &#x2588;</div>
    </div>
 
    <!-- TOOLBAR -->
    <div class="toolbar">
 
      <!-- Ferramentas -->
      <button class="tool-btn active" id="btnBrush" title="Pincel">&#x270F;</button>
      <button class="tool-btn" id="btnEraser" title="Borracha">&#x25A1;</button>
      <button class="tool-btn" id="btnFill" title="Balde de tinta">&#x25CF;</button>
 
      <div class="tool-sep"></div>
 
      <!-- Swatches de cor -->
      <div class="swatch active" style="background:#c000e0" data-color="#c000e0"></div>
      <div class="swatch" style="background:#00d4ff" data-color="#00d4ff"></div>
      <div class="swatch" style="background:#ffe600" data-color="#ffe600"></div>
      <div class="swatch" style="background:#00ff88" data-color="#00ff88"></div>
      <div class="swatch" style="background:#ff2244" data-color="#ff2244"></div>
      <div class="swatch" style="background:#f0f0ff" data-color="#f0f0ff"></div>
      <div class="swatch" style="background:#0d0d1a; border-color:#555" data-color="#0d0d1a"></div>
 
      <div class="tool-sep"></div>
 
      <!-- Seletor de cor livre -->
      <div class="color-input-wrap">
        <span>COR</span>
        <input type="color" id="colorPicker" value="#c000e0" />
      </div>
 
      <div class="tool-sep"></div>
 
      <!-- Limpar -->
      <button class="clear-btn" id="btnClear">&#x2715; LIMPAR</button>
 
    </div>
 
    <!-- CARDS DE FEATURES -->
    <div class="features">
      <div class="feature-card">
        <div class="feature-icon">&#x270F;</div>
        <div class="feature-title">PINCEL</div>
        <div class="feature-desc">Clique ou arraste para pintar célula a célula com a cor escolhida.</div>
      </div>
      <div class="feature-card">
        <div class="feature-icon">&#x1F5D1;</div>
        <div class="feature-title">BORRACHA</div>
        <div class="feature-desc">Apague pixels específicos sem precisar limpar toda a grade.</div>
      </div>
      <div class="feature-card">
        <div class="feature-icon">&#x1FA63;</div>
        <div class="feature-title">BALDE</div>
        <div class="feature-desc">Preencha uma área inteira com a cor selecionada em um clique.</div>
      </div>
      <div class="feature-card">
        <div class="feature-icon">&#x1F3A8;</div>
        <div class="feature-title">PALETA LIVRE</div>
        <div class="feature-desc">Escolha qualquer cor do espectro com o seletor de cor customizado.</div>
      </div>
    </div>
 
  </main>
 
  <!-- FOOTER -->
  <footer class="footer">
    <span>PIXELFORGE &copy; 2025</span>
    <span class="footer-cursor">&#x2588;</span>
    <span>PARTE 4 — ESQUELETO DO SITE</span>
    <span class="footer-cursor">&#x2588;</span>
    <span>FEITO COM &#x1F3AE; E MUITO CSS</span>
  </footer>
 
  <script>
    /* ==========================================================
       PIXELFORGE — JAVASCRIPT
    ========================================================== */
 
    'use strict';
 
    // ── BOAS VINDAS ──────────────────────────────────────────
    window.addEventListener('load', () => {
      setTimeout(() => {
        alert(
          '╔══════════════════════════════════╗\n' +
          '║                                  ║\n' +
          '║   🎨  BEM-VINDO AO               ║\n' +
          '║       PIXELFORGE!                ║\n' +
          '║                                  ║\n' +
          '╠══════════════════════════════════╣\n' +
          '║                                  ║\n' +
          '║  Seu editor de Pixel Art está    ║\n' +
          '║  pronto para uso!                ║\n' +
          '║                                  ║\n' +
          '║  ✏️  Clique na grade para pintar  ║\n' +
          '║  🧹  Use a borracha para apagar  ║\n' +
          '║  🪣  Balde preenche áreas        ║\n' +
          '║  🎨  Escolha qualquer cor        ║\n' +
          '║                                  ║\n' +
          '║  A arte começa agora!  🕹️        ║\n' +
          '║                                  ║\n' +
          '╚══════════════════════════════════╝'
        );
      }, 300);
    });
 
    // ── FUNDO ANIMADO ────────────────────────────────────────
    (function initBg() {
      const cv = document.getElementById('bgCanvas');
      const cx = cv.getContext('2d');
      const COLS = 50, ROWS = 30, CELL = 20;
      const COLORS = ['#c000e0','#00d4ff','#ffe600','#00ff88','#ff2244'];
      const cells = [];
 
      function resize() {
        cv.width  = window.innerWidth;
        cv.height = window.innerHeight;
      }
      resize();
      window.addEventListener('resize', resize);
 
      // Popula células esparsas
      for (let i = 0; i < 60; i++) {
        cells.push({
          x: Math.floor(Math.random() * (window.innerWidth  / CELL)) * CELL,
          y: Math.floor(Math.random() * (window.innerHeight / CELL)) * CELL,
          color: COLORS[Math.floor(Math.random() * COLORS.length)],
          life: Math.random(),
          speed: 0.004 + Math.random() * 0.008
        });
      }
 
      function draw() {
        cx.clearRect(0, 0, cv.width, cv.height);
        cells.forEach(c => {
          c.life += c.speed;
          if (c.life > 1) {
            c.life = 0;
            c.x = Math.floor(Math.random() * (cv.width  / CELL)) * CELL;
            c.y = Math.floor(Math.random() * (cv.height / CELL)) * CELL;
            c.color = COLORS[Math.floor(Math.random() * COLORS.length)];
          }
          const alpha = Math.sin(c.life * Math.PI);
          cx.fillStyle = c.color;
          cx.globalAlpha = alpha;
          cx.fillRect(c.x, c.y, CELL - 1, CELL - 1);
        });
        cx.globalAlpha = 1;
        requestAnimationFrame(draw);
      }
      draw();
    })();
 
    // ── GRADE DE PREVIEW INTERATIVA ─────────────────────────
    (function initGrid() {
      const cv   = document.getElementById('previewCanvas');
      const ctx  = cv.getContext('2d');
      const COLS = 24, ROWS = 15;
      const CW   = cv.width  / COLS;
      const CH   = cv.height / ROWS;
 
      // Responsivo
      function resizeCanvas() {
        const maxW = Math.min(window.innerWidth - 48, 480);
        cv.style.width  = maxW + 'px';
        cv.style.height = (maxW * (ROWS / COLS)) + 'px';
      }
      resizeCanvas();
      window.addEventListener('resize', resizeCanvas);
 
      // Estado da grade: null = vazio
      const grid = Array.from({ length: ROWS }, () => Array(COLS).fill(null));
 
      let currentColor = '#c000e0';
      let currentTool  = 'brush'; // 'brush' | 'eraser' | 'fill'
      let isPainting   = false;
 
      // ─ Render ─
      function render() {
        ctx.clearRect(0, 0, cv.width, cv.height);
 
        // Fundo xadrez (indica transparência)
        for (let r = 0; r < ROWS; r++) {
          for (let c = 0; c < COLS; c++) {
            const isLight = (r + c) % 2 === 0;
            ctx.fillStyle = isLight ? '#1a1a2e' : '#13131f';
            ctx.fillRect(c * CW, r * CH, CW, CH);
          }
        }
 
        // Pixels pintados
        for (let r = 0; r < ROWS; r++) {
          for (let c = 0; c < COLS; c++) {
            if (grid[r][c]) {
              ctx.fillStyle = grid[r][c];
              ctx.fillRect(c * CW, r * CH, CW, CH);
            }
          }
        }
 
        // Grade de linhas
        ctx.strokeStyle = 'rgba(42,42,80,0.7)';
        ctx.lineWidth   = 0.5;
        for (let c = 0; c <= COLS; c++) {
          ctx.beginPath();
          ctx.moveTo(c * CW, 0);
          ctx.lineTo(c * CW, cv.height);
          ctx.stroke();
        }
        for (let r = 0; r <= ROWS; r++) {
          ctx.beginPath();
          ctx.moveTo(0, r * CH);
          ctx.lineTo(cv.width, r * CH);
          ctx.stroke();
        }
      }
 
      // ─ Ferramentas ─
      function getCell(e) {
        const rect = cv.getBoundingClientRect();
        const scaleX = cv.width  / rect.width;
        const scaleY = cv.height / rect.height;
        const touch  = e.touches ? e.touches[0] : e;
        const x = (touch.clientX - rect.left)  * scaleX;
        const y = (touch.clientY - rect.top)   * scaleY;
        return {
          col: Math.floor(x / CW),
          row: Math.floor(y / CH)
        };
      }
 
      function paint(e) {
        const { col, row } = getCell(e);
        if (col < 0 || col >= COLS || row < 0 || row >= ROWS) return;
 
        if (currentTool === 'brush') {
          grid[row][col] = currentColor;
        } else if (currentTool === 'eraser') {
          grid[row][col] = null;
        }
        render();
      }
 
      function floodFill(startRow, startCol, targetColor, fillColor) {
        if (targetColor === fillColor) return;
        const stack = [[startRow, startCol]];
        while (stack.length) {
          const [r, c] = stack.pop();
          if (r < 0 || r >= ROWS || c < 0 || c >= COLS) continue;
          if (grid[r][c] !== targetColor) continue;
          grid[r][c] = fillColor;
          stack.push([r+1,c],[r-1,c],[r,c+1],[r,c-1]);
        }
        render();
      }
 
      // ─ Eventos do canvas ─
      cv.addEventListener('mousedown', e => {
        isPainting = true;
        if (currentTool === 'fill') {
          const { col, row } = getCell(e);
          floodFill(row, col, grid[row][col], currentColor);
        } else {
          paint(e);
        }
      });
      cv.addEventListener('mousemove', e => { if (isPainting) paint(e); });
      cv.addEventListener('mouseup',   () => { isPainting = false; });
      cv.addEventListener('mouseleave',() => { isPainting = false; });
 
      // touch
      cv.addEventListener('touchstart', e => { e.preventDefault(); isPainting = true; paint(e); }, { passive: false });
      cv.addEventListener('touchmove',  e => { e.preventDefault(); if (isPainting) paint(e); }, { passive: false });
      cv.addEventListener('touchend',   () => { isPainting = false; });
 
      // ─ Toolbar: ferramentas ─
      const btnBrush  = document.getElementById('btnBrush');
      const btnEraser = document.getElementById('btnEraser');
      const btnFill   = document.getElementById('btnFill');
      const btnClear  = document.getElementById('btnClear');
 
      function setTool(tool) {
        currentTool = tool;
        [btnBrush, btnEraser, btnFill].forEach(b => b.classList.remove('active'));
        if (tool === 'brush')  btnBrush.classList.add('active');
        if (tool === 'eraser') btnEraser.classList.add('active');
        if (tool === 'fill')   btnFill.classList.add('active');
      }
 
      btnBrush.addEventListener('click',  () => setTool('brush'));
      btnEraser.addEventListener('click', () => setTool('eraser'));
      btnFill.addEventListener('click',   () => setTool('fill'));
 
      btnClear.addEventListener('click', () => {
        for (let r = 0; r < ROWS; r++)
          for (let c = 0; c < COLS; c++)
            grid[r][c] = null;
        render();
      });
 
      // ─ Toolbar: cores ─
      const swatches     = document.querySelectorAll('.swatch');
      const colorPicker  = document.getElementById('colorPicker');
 
      function setColor(color) {
        currentColor = color;
        colorPicker.value = color;
        swatches.forEach(s => s.classList.remove('active'));
        const match = [...swatches].find(s => s.dataset.color === color);
        if (match) match.classList.add('active');
      }
 
      swatches.forEach(s => {
        s.addEventListener('click', () => setColor(s.dataset.color));
      });
 
      colorPicker.addEventListener('input', e => {
        setColor(e.target.value);
        swatches.forEach(s => s.classList.remove('active'));
      });
 
      render();
    })();
 
    console.log('%c[PixelForge] Pronto para pintar! 🎨', 'color:#c000e0; font-weight:bold; font-size:14px;');
  </script>
</body>
</html>
