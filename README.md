<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Tugas Profil</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;500&display=swap" rel="stylesheet">
<style>
  :root {
    --ink: #070A1A;
    --mist: #E4E9FF;
    --dim: #8B96C4;
    --edge: rgba(201, 211, 255, 0.2);
    --glass: rgba(9, 13, 34, 0.55);
    --card: rgba(9, 13, 34, 0.58);
    --chip-on: rgba(201, 211, 255, 0.16);
    --focus: #4DE1FF;
    color-scheme: dark;
    box-sizing: border-box;
    padding-top: env(safe-area-inset-top, 0px);
    padding-bottom: env(safe-area-inset-bottom, 0px);
  }
  html { scroll-padding-top: env(safe-area-inset-top, 0px); height: 100%; background: var(--ink); }
  *, *::before, *::after { box-sizing: inherit; }
  body {
    margin: 0;
    height: 100%;
    overflow: hidden;
    background: var(--ink);
    color: var(--mist);
    font-family: "Sora", system-ui, -apple-system, "Segoe UI", Roboto, sans-serif;
    touch-action: none;
    -webkit-user-select: none;
    user-select: none;
  }

  /* Lapisan 1: gambar ke-2 sebagai latar (digelapkan tipis agar cahaya menonjol) */
  .bg {
    position: fixed;
    inset: -24px;
    z-index: 0;
    background:
      linear-gradient(180deg, rgba(7, 10, 26, 0.5), rgba(7, 10, 26, 0.68)),
      url("data:image/jpeg;base64,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") center 40% / cover no-repeat;
    filter: blur(4px) saturate(1.1);
  }

  /* Lapisan 2: Cahaya Hidup, menambah cahaya di atas foto (hitam jadi transparan) */
  canvas {
    position: fixed;
    inset: 0;
    z-index: 1;
    width: 100%;
    height: 100%;
    display: block;
    mix-blend-mode: screen;
  }

  .ui {
    position: fixed;
    inset: 0;
    z-index: 2;
    display: flex;
    flex-direction: column;
    padding:
      calc(24px + env(safe-area-inset-top, 0px))
      24px
      calc(24px + env(safe-area-inset-bottom, 0px));
    pointer-events: none;
  }

  /* Kartu profil */
  .stage {
    flex: 1;
    display: grid;
    place-items: center;
    min-height: 0;
  }
  .profile {
    width: min(520px, 100%);
    padding: clamp(24px, 5vw, 40px);
    border: 1px solid var(--edge);
    border-radius: 24px;
    background: var(--card);
    -webkit-backdrop-filter: blur(16px);
    backdrop-filter: blur(16px);
    animation: arrive 1.1s cubic-bezier(.2, .7, .2, 1) both;
  }
  @keyframes arrive {
    from { opacity: 0; transform: translateY(14px); }
    to { opacity: 1; transform: none; }
  }
  .head {
    display: flex;
    align-items: flex-end;
    gap: clamp(16px, 4vw, 24px);
    margin-bottom: 24px;
  }
  .photo {
    flex: none;
    width: clamp(84px, 22vw, 104px);
    aspect-ratio: 96 / 119;
    border: 1px solid var(--edge);
    border-radius: 18px;
    object-fit: cover;
    object-position: center top;
    display: block;
  }
  h1 {
    margin: 0;
    font-weight: 300;
    font-size: clamp(2.4rem, 8vw, 3.8rem);
    letter-spacing: -0.035em;
    line-height: 1;
  }
  h2, h3, h4 {
    display: grid;
    grid-template-columns: 6.5rem 1fr;
    align-items: baseline;
    gap: 16px;
    margin: 0;
    padding: 14px 0;
    border-top: 1px solid var(--edge);
    font-size: 1rem;
    font-weight: 500;
    line-height: 1.4;
  }
  h2 .v { font-size: 1.2rem; }
  .k { color: var(--dim); font-weight: 300; }
  .v { color: var(--mist); overflow-wrap: anywhere; }

  /* Bawah: petunjuk + pilihan dunia partikel */
  .bottom { display: flex; flex-direction: column; align-items: flex-start; gap: 12px; }
  .hint {
    margin: 0;
    max-width: 36ch;
    font-size: 0.85rem;
    line-height: 1.6;
    color: var(--dim);
    transition: opacity 0.8s ease;
  }
  .hint.gone { opacity: 0; }

  .modes {
    display: inline-flex;
    gap: 4px;
    padding: 4px;
    border: 1px solid var(--edge);
    border-radius: 999px;
    background: var(--glass);
    -webkit-backdrop-filter: blur(14px);
    backdrop-filter: blur(14px);
    pointer-events: auto;
  }
  .modes button {
    min-height: 44px;
    padding: 0 20px;
    border: 0;
    border-radius: 999px;
    background: transparent;
    color: var(--dim);
    font: 500 0.9rem/1 "Sora", system-ui, sans-serif;
    cursor: pointer;
    transition: background 0.25s ease, color 0.25s ease;
  }
  .modes button:hover { color: var(--mist); }
  .modes button[aria-pressed="true"] { background: var(--chip-on); color: #fff; }
  .modes button:focus-visible { outline: 2px solid var(--focus); outline-offset: 2px; }

  @media (max-width: 380px) {
    .modes button { padding: 0 14px; }
    h2, h3, h4 { grid-template-columns: 5.5rem 1fr; }
  }
  @media (prefers-reduced-motion: reduce) {
    .profile { animation: none; }
    .hint, .modes button { transition: none; }
  }
</style>
</head>
<body>
<div class="bg" aria-hidden="true"></div>
<canvas id="c" role="img" aria-label="Latar seni cahaya interaktif yang bereaksi pada kursor atau sentuhan"></canvas>

<div class="ui">
  <main class="stage">
    <section class="profile">
      <div class="head">
        <img class="photo" alt="Foto profil Muhammad Fakhry Rayyan" width="96" height="119" src="data:image/jpeg;base64,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">
        <h1>Profil</h1>
      </div>
      <h2><span class="k">Nama</span><span class="v">Muhammad Fakhry Rayyan</span></h2>
      <h3><span class="k">Kelas</span><span class="v">10</span></h3>
      <h4><span class="k">No. induk</span><span class="v">42439</span></h4>
    </section>
  </main>

  <div class="bottom">
    <p class="hint" id="hint">Gerakkan kursor atau sentuh layar. Klik atau ketuk untuk melepas gelombang cahaya.</p>
    <div class="modes" role="group" aria-label="Pilih dunia partikel">
      <button type="button" data-mode="0" aria-pressed="true">Aurora</button>
      <button type="button" data-mode="1" aria-pressed="false">Galaksi</button>
      <button type="button" data-mode="2" aria-pressed="false">Magnet</button>
    </div>
  </div>
</div>

<script>
(() => {
  const cv = document.getElementById('c');
  const ctx = cv.getContext('2d');
  const hint = document.getElementById('hint');
  const buttons = Array.from(document.querySelectorAll('.modes button'));
  const reduce = window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  const speedK = reduce ? 0.4 : 1;

  // Palet: cyan -> violet -> rose -> amber, berputar kembali ke cyan
  const stops = [[77, 225, 255], [138, 107, 255], [255, 107, 181], [255, 196, 107]];
  const NB = 24;
  const styles = [];
  for (let i = 0; i < NB; i++) {
    const f = (i / NB) * stops.length;
    const i0 = Math.floor(f);
    const a = stops[i0 % stops.length];
    const b = stops[(i0 + 1) % stops.length];
    const k = f - i0;
    const c = a.map((v, j) => Math.round(v + (b[j] - v) * k));
    styles.push('rgba(' + c[0] + ',' + c[1] + ',' + c[2] + ',0.6)');
  }

  let W = 0, H = 0, DPR = 1, N = 0;
  let x, y, px, py, vx, vy, r, a0, w, ox, oy, bk;
  let mode = 0;
  let first = true;

  let tx = 0, ty = 0, mx = 0, my = 0, gx = 0, gy = 0;
  let lastInput = -1e9;
  let used = false;
  let T = 0;
  const bursts = [];

  function fillBg(alpha) {
    ctx.globalCompositeOperation = 'source-over';
    ctx.fillStyle = 'rgba(0,0,0,' + alpha + ')';
    ctx.fillRect(0, 0, W, H);
  }

  function resize() {
    DPR = Math.min(window.devicePixelRatio || 1, 2);
    W = window.innerWidth;
    H = window.innerHeight;
    cv.width = Math.round(W * DPR);
    cv.height = Math.round(H * DPR);
    ctx.setTransform(DPR, 0, 0, DPR, 0, 0);
    N = Math.max(1600, Math.min(4500, Math.floor((W * H) / 280)));
    x = new Float32Array(N); y = new Float32Array(N);
    px = new Float32Array(N); py = new Float32Array(N);
    vx = new Float32Array(N); vy = new Float32Array(N);
    r = new Float32Array(N); a0 = new Float32Array(N); w = new Float32Array(N);
    ox = new Float32Array(N); oy = new Float32Array(N);
    bk = new Uint8Array(N);
    if (!mx && !my) { mx = tx = gx = W / 2; my = ty = gy = H / 2; }
    init();
    fillBg(1);
  }

  function galaxyRadius() { return Math.min(W, H) * 0.5; }

  function init() {
    const Rmax = galaxyRadius();
    for (let i = 0; i < N; i++) {
      vx[i] = 0; vy[i] = 0; ox[i] = 0; oy[i] = 0;
      if (mode === 1) {
        const bulge = Math.random() < 0.16;
        const rr = bulge
          ? 8 + Math.pow(Math.random(), 2) * Rmax * 0.22
          : 24 + Math.pow(Math.random(), 1.5) * Rmax;
        r[i] = rr;
        const spread = Math.random() + Math.random() - 1;
        a0[i] = bulge
          ? Math.random() * 6.2832
          : (i % 3) * 2.0944 + rr * 0.013 + spread * (0.5 + (rr / Rmax) * 0.25);
        w[i] = 0.42 + 5 / (rr + 30);
      } else {
        x[i] = Math.random() * W;
        y[i] = Math.random() * H;
      }
      px[i] = x[i]; py[i] = y[i];
    }
    first = true;
  }

  function setMode(m) {
    mode = m;
    buttons.forEach((b, i) => b.setAttribute('aria-pressed', String(i === m)));
    init();
    fillBg(1);
  }

  function burst(bx, by) {
    bursts.push({ x: bx, y: by, t0: performance.now() });
    const R = 320;
    for (let i = 0; i < N; i++) {
      const dx = x[i] - bx, dy = y[i] - by;
      const d = Math.sqrt(dx * dx + dy * dy) + 0.001;
      if (d < R) {
        const f = Math.pow(1 - d / R, 2) * 16;
        vx[i] += (dx / d) * f;
        vy[i] += (dy / d) * f;
      }
    }
  }

  function markUsed() {
    if (!used) { used = true; hint.classList.add('gone'); }
  }

  window.addEventListener('pointermove', (e) => {
    tx = e.clientX; ty = e.clientY;
    lastInput = performance.now();
    markUsed();
  });
  window.addEventListener('pointerdown', (e) => {
    if (e.target.closest && e.target.closest('.modes')) return;
    tx = e.clientX; ty = e.clientY;
    lastInput = performance.now();
    markUsed();
    burst(e.clientX, e.clientY);
  });
  window.addEventListener('keydown', (e) => {
    if (e.key === '1' || e.key === '2' || e.key === '3') setMode(Number(e.key) - 1);
  });
  buttons.forEach((b, i) => b.addEventListener('click', () => setMode(i)));
  window.addEventListener('resize', resize);

  const AURORA_R = 240;

  let last = performance.now();

  function frame(now) {
    const dt = Math.min(50, now - last);
    last = now;
    const k = (dt / 16.667) * speedK;
    T += (dt / 1000) * speedK;

    // Jika tidak ada input, kursor bergerak sendiri supaya latar tetap hidup
    if (now - lastInput > 3500) {
      tx = W / 2 + Math.cos(T * 0.35) * W * 0.28 + Math.sin(T * 0.9) * W * 0.05;
      ty = H / 2 + Math.sin(T * 0.5) * H * 0.24;
    }
    const sm = 1 - Math.pow(mode === 2 ? 0.8 : 0.86, k);
    mx += (tx - mx) * sm;
    my += (ty - my) * sm;

    fillBg(1 - Math.pow(0.9, k));

    if (mode === 0) {
      const sw = 1 - Math.pow(0.93, k);
      const R2 = AURORA_R * AURORA_R;
      for (let i = 0; i < N; i++) {
        const xi = x[i], yi = y[i];
        const ang =
          Math.sin(xi * 0.0032 + T * 0.25) * Math.cos(yi * 0.0041 - T * 0.2) * 2.4 +
          Math.sin((xi * 0.6 + yi) * 0.0021 + T * 0.12) * 2.0;
        let tvx = Math.cos(ang) * 2.6;
        let tvy = Math.sin(ang) * 2.6;
        const dx = xi - mx, dy = yi - my;
        const d2 = dx * dx + dy * dy;
        if (d2 < R2) {
          const d = Math.sqrt(d2) + 0.001;
          const f = 1 - d / AURORA_R;
          tvx += (-dy / d) * f * 5.5 - (dx / d) * f * 1.5;
          tvy += (dx / d) * f * 5.5 - (dy / d) * f * 1.5;
        }
        vx[i] += (tvx - vx[i]) * sw;
        vy[i] += (tvy - vy[i]) * sw;
        px[i] = xi; py[i] = yi;
        let nx = xi + vx[i] * k;
        let ny = yi + vy[i] * k;
        if (nx < -20 || nx > W + 20 || ny < -20 || ny > H + 20 || Math.random() < 0.0012) {
          nx = Math.random() * W; ny = Math.random() * H;
          px[i] = nx; py[i] = ny;
        }
        x[i] = nx; y[i] = ny;
        const v = (nx / W) * 0.9 + (ny / H) * 0.5 + T * 0.03;
        bk[i] = ((Math.floor(v * NB) % NB) + NB) % NB;
      }
    } else if (mode === 1) {
      const Rmax = galaxyRadius();
      const gs = 1 - Math.pow(0.96, k);
      gx += (mx - gx) * gs;
      gy += (my - gy) * gs;
      const tilt = -0.45 + (mx / W - 0.5) * 0.7;
      const ct = Math.cos(tilt), st = Math.sin(tilt);
      const damp = Math.pow(0.93, k);
      for (let i = 0; i < N; i++) {
        const ang = a0[i] + w[i] * T;
        const lx = Math.cos(ang) * r[i];
        const ly = Math.sin(ang) * r[i] * 0.52;
        vx[i] = (vx[i] - ox[i] * 0.02 * k) * damp;
        vy[i] = (vy[i] - oy[i] * 0.02 * k) * damp;
        ox[i] += vx[i] * k;
        oy[i] += vy[i] * k;
        const nx = gx + lx * ct - ly * st + ox[i];
        const ny = gy + lx * st + ly * ct + oy[i];
        if (first) { px[i] = nx; py[i] = ny; } else { px[i] = x[i]; py[i] = y[i]; }
        x[i] = nx; y[i] = ny;
        const rn = Math.min(1, r[i] / Rmax);
        bk[i] = Math.floor((1 - rn) * (NB * 0.78));
      }
      first = false;
    } else {
      const damp = Math.pow(0.986, k);
      for (let i = 0; i < N; i++) {
        const dx = mx - x[i], dy = my - y[i];
        const d2 = dx * dx + dy * dy + 900;
        const d = Math.sqrt(d2);
        const inv = 1 / (d2 * d);
        const ax = 9000 * dx * inv + (-dy / d) * 0.07;
        const ay = 9000 * dy * inv + (dx / d) * 0.07;
        let nvx = (vx[i] + ax * k) * damp;
        let nvy = (vy[i] + ay * k) * damp;
        const sp2 = nvx * nvx + nvy * nvy;
        if (sp2 > 196) {
          const s = 14 / Math.sqrt(sp2);
          nvx *= s; nvy *= s;
        }
        vx[i] = nvx; vy[i] = nvy;
        px[i] = x[i]; py[i] = y[i];
        let nx = x[i] + nvx * k;
        let ny = y[i] + nvy * k;
        if (nx < -200 || nx > W + 200 || ny < -200 || ny > H + 200) {
          nx = Math.random() * W; ny = Math.random() * H;
          vx[i] = 0; vy[i] = 0;
          px[i] = nx; py[i] = ny;
        }
        x[i] = nx; y[i] = ny;
        const sp = Math.min(Math.sqrt(sp2) / 9, 1);
        bk[i] = Math.floor(sp * (NB * 0.86));
      }
    }

    // Gambar partikel per warna (satu stroke per keranjang warna)
    ctx.globalCompositeOperation = 'lighter';
    ctx.lineWidth = 1.3;
    ctx.lineCap = 'round';
    for (let b = 0; b < NB; b++) {
      ctx.beginPath();
      let any = false;
      for (let i = 0; i < N; i++) {
        if (bk[i] === b) {
          ctx.moveTo(px[i], py[i]);
          ctx.lineTo(x[i] + 0.01, y[i]);
          any = true;
        }
      }
      if (any) {
        ctx.strokeStyle = styles[b];
        ctx.stroke();
      }
    }

    // Riak gelombang dari klik / ketukan
    for (let i = bursts.length - 1; i >= 0; i--) {
      const age = (now - bursts[i].t0) / 1000;
      if (age > 1.1) { bursts.splice(i, 1); continue; }
      ctx.beginPath();
      ctx.arc(bursts[i].x, bursts[i].y, age * 520, 0, 6.2832);
      ctx.strokeStyle = 'rgba(201,211,255,' + (Math.max(0, 1 - age / 1.1) * 0.35).toFixed(3) + ')';
      ctx.lineWidth = 1.5;
      ctx.stroke();
    }

    requestAnimationFrame(frame);
  }

  resize();
  requestAnimationFrame(frame);
})();
</script>
</body>
</html>
