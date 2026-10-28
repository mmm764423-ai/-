<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>عربان</title>
<meta name="description" content="عربان: لاعب رول بلاي، حساباتي في مكان واحد">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans+Arabic:wght@400;500;600&family=Reem+Kufi:wght@500;700&display=swap" rel="stylesheet">
<style>
  :root {
    --field: #262b1d;
    --field-deep: #1c2015;
    --khaki: #d4cba3;
    --khaki-dim: #9a9577;
    --brass: #c2a25a;
    --steel: #8d9a8b;
    --display: "Reem Kufi", "Noto Kufi Arabic", "Segoe UI", Tahoma, sans-serif;
    --body: "IBM Plex Sans Arabic", "Segoe UI", Tahoma, Arial, sans-serif;
  }
  * { box-sizing: border-box; margin: 0; }
  html, body { min-height: 100%; }
  body {
    background:
      radial-gradient(ellipse at 50% 0%, #343a27 0%, var(--field) 55%, var(--field-deep) 100%);
    background-attachment: fixed;
    color: var(--khaki);
    font-family: var(--body);
    line-height: 1.7;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 0 20px 56px;
    overflow-x: hidden;
  }

  /* ---------- dog tag ---------- */
  .chain {
    width: 2px;
    height: 72px;
    background: repeating-linear-gradient(to bottom, var(--steel) 0 6px, transparent 6px 9px);
    opacity: .8;
  }
  .swing {
    transform-origin: 50% 0;
    animation: swing 2.4s ease-out 1 both;
  }
  @keyframes swing {
    0%   { transform: rotate(7deg); }
    22%  { transform: rotate(-4.5deg); }
    44%  { transform: rotate(2.6deg); }
    66%  { transform: rotate(-1.3deg); }
    100% { transform: rotate(0); }
  }
  .tag {
    position: relative;
    width: min(320px, 84vw);
    padding: 56px 28px 34px;
    text-align: center;
    border-radius: 34px;
    color: #2a2d1f;
    background: linear-gradient(145deg, #e3dcc0 0%, #b9b18c 48%, #d6cea9 100%);
    box-shadow:
      inset 0 0 0 3px rgba(255,255,255,.35),
      inset 0 0 0 7px rgba(60,58,40,.35),
      0 22px 40px rgba(0,0,0,.45);
  }
  .tag::before {
    content: "";
    position: absolute;
    top: 18px;
    left: 50%;
    width: 22px;
    height: 22px;
    margin-left: -11px;
    border-radius: 50%;
    background: var(--field-deep);
    box-shadow: inset 0 2px 4px rgba(0,0,0,.7), 0 1px 0 rgba(255,255,255,.4);
  }
  .tag h1 {
    font-family: var(--display);
    font-weight: 700;
    font-size: clamp(64px, 20vw, 92px);
    line-height: 1.05;
    letter-spacing: 0;
    text-shadow: 0 1px 0 rgba(255,255,255,.55), 0 -1px 0 rgba(0,0,0,.25);
  }
  .tag .rule {
    height: 0;
    border-top: 2px solid rgba(42,45,31,.55);
    margin: 14px 18px 14px;
  }
  .tag p {
    font-weight: 600;
    font-size: 17px;
    line-height: 1.8;
    text-shadow: 0 1px 0 rgba(255,255,255,.45);
  }

  /* ---------- links ---------- */
  main {
    width: min(480px, 100%);
    margin-top: 44px;
    display: grid;
    gap: 14px;
  }
  .plate {
    display: flex;
    align-items: center;
    gap: 16px;
    width: 100%;
    padding: 16px 18px;
    text-align: right;
    text-decoration: none;
    color: var(--khaki);
    font: inherit;
    background: rgba(212,203,163,.07);
    border: 1.5px solid rgba(212,203,163,.35);
    border-radius: 10px;
    cursor: pointer;
    transition: background .15s, border-color .15s;
  }
  .plate:hover { background: rgba(212,203,163,.14); border-color: var(--brass); }
  .plate:focus-visible { outline: 3px solid var(--brass); outline-offset: 3px; }
  .plate svg { width: 30px; height: 30px; flex: none; fill: var(--brass); }
  .plate .what { display: grid; line-height: 1.5; flex: 1; min-width: 0; }
  .plate .name { font-weight: 600; font-size: 19px; }
  .plate .handle {
    font-size: 15px;
    color: var(--khaki-dim);
    direction: ltr;
    text-align: right;
    unicode-bidi: plaintext;
  }
  .plate .act {
    font-size: 14px;
    font-weight: 500;
    color: var(--brass);
    white-space: nowrap;
  }

  footer {
    margin-top: 40px;
    font-size: 14px;
    color: var(--khaki-dim);
  }

  @media (prefers-reduced-motion: reduce) {
    .swing { animation: none; }
    .plate { transition: none; }
  }
</style>
</head>
<body>

  <div class="chain" aria-hidden="true"></div>
  <div class="swing">
    <div class="tag">
      <h1>عربان</h1>
      <div class="rule" aria-hidden="true"></div>
      <p>لاعب رول بلاي من خمس سنين<br>خبرة عسكرية كويسة</p>
    </div>
  </div>

  <main>
    <a class="plate" href="https://www.tiktok.com/@4_0_4_a_b_s" target="_blank" rel="noopener">
      <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M19.6 6.7a5.2 5.2 0 0 1-3.2-1.1A5.2 5.2 0 0 1 14.5 2h-3.3v12.6a2.7 2.7 0 1 1-2.7-2.7c.3 0 .5 0 .8.1V8.6a6 6 0 0 0-.8-.1 6 6 0 1 0 6 6V9a8.4 8.4 0 0 0 4.9 1.6V6.7z"/></svg>
      <span class="what">
        <span class="name">تيك توك</span>
        <span class="handle">@4_0_4_a_b_s</span>
      </span>
      <span class="act">افتح</span>
    </a>

    <button class="plate" type="button" id="discord" data-copy="7.8.9.10" aria-live="polite">
      <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M20.317 4.3698a19.7913 19.7913 0 00-4.8851-1.5152.0741.0741 0 00-.0785.0371c-.211.3753-.4447.8648-.6083 1.2495-1.8447-.2762-3.68-.2762-5.4868 0-.1636-.3933-.4058-.8742-.6177-1.2495a.077.077 0 00-.0785-.037 19.7363 19.7363 0 00-4.8852 1.515.0699.0699 0 00-.0321.0277C.5334 9.0458-.319 13.5799.0992 18.0578a.0824.0824 0 00.0312.0561c2.0528 1.5076 4.0413 2.4228 5.9929 3.0294a.0777.0777 0 00.0842-.0276c.4616-.6304.8731-1.2952 1.226-1.9942a.076.076 0 00-.0416-.1057c-.6528-.2476-1.2743-.5495-1.8722-.8923a.077.077 0 01-.0076-.1277c.1258-.0943.2517-.1923.3718-.2914a.0743.0743 0 01.0776-.0105c3.9278 1.7933 8.18 1.7933 12.0614 0a.0739.0739 0 01.0785.0095c.1202.099.246.1981.3728.2924a.077.077 0 01-.0066.1276 12.2986 12.2986 0 01-1.873.8914.0766.0766 0 00-.0407.1067c.3604.698.7719 1.3628 1.225 1.9932a.076.076 0 00.0842.0286c1.961-.6067 3.9495-1.5219 6.0023-3.0294a.077.077 0 00.0313-.0552c.5004-5.177-.8382-9.6739-3.5485-13.6604a.061.061 0 00-.0312-.0286zM8.02 15.3312c-1.1825 0-2.1569-1.0857-2.1569-2.419 0-1.3332.9555-2.4189 2.157-2.4189 1.2108 0 2.1757 1.0952 2.1568 2.419 0 1.3332-.9555 2.4189-2.1569 2.4189zm7.9748 0c-1.1825 0-2.1569-1.0857-2.1569-2.419 0-1.3332.9554-2.4189 2.1569-2.4189 1.2108 0 2.1757 1.0952 2.1568 2.419 0 1.3332-.946 2.4189-2.1568 2.4189Z"/></svg>
      <span class="what">
        <span class="name">ديسكورد</span>
        <span class="handle">7.8.9.10</span>
      </span>
      <span class="act" id="discord-act">انسخ اليوزر</span>
    </button>
  </main>

  <footer>عربان</footer>

<script>
  (function () {
    var btn = document.getElementById("discord");
    var act = document.getElementById("discord-act");
    var timer;
    function done(ok) {
      act.textContent = ok ? "تم النسخ" : "اليوزر: 7.8.9.10";
      clearTimeout(timer);
      timer = setTimeout(function () { act.textContent = "انسخ اليوزر"; }, 2000);
    }
    btn.addEventListener("click", function () {
      var text = btn.getAttribute("data-copy");
      if (navigator.clipboard && navigator.clipboard.writeText) {
        navigator.clipboard.writeText(text).then(function () { done(true); }, function () { done(false); });
      } else {
        done(false);
      }
    });
  })();
</script>
</body>
</html>
