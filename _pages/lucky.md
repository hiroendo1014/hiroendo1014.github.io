---
permalink: /lucky/
title: "Lucky⭐️"
author_profile: true
---

{::nomarkdown}
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,700;1,500&display=swap" rel="stylesheet">

<style>
  html:has(#lucky-page),
  html[data-theme="dark"]:has(#lucky-page) {
    --global-bg-color: #0d0a24 !important;
    --global-footer-bg-color: transparent !important;
    --global-border-color: rgba(245, 212, 138, 0.35) !important;
    --global-text-color: #ece8ff !important;
    --global-text-color-light: #c9c2ef !important;
    --global-link-color: #f5d48a !important;
    --global-link-color-hover: #ffe9b8 !important;
    --global-link-color-visited: #f5d48a !important;
    --global-masthead-link-color: #ece8ff !important;
    --global-masthead-link-color-hover: #f5d48a !important;
  }
  body:has(#lucky-page) {
    background-color: #0d0a24;
    background-image:
      radial-gradient(ellipse at 18% 12%, rgba(137, 84, 255, 0.35), transparent 55%),
      radial-gradient(ellipse at 85% 30%, rgba(255, 120, 200, 0.22), transparent 50%),
      radial-gradient(ellipse at 50% 100%, rgba(60, 190, 255, 0.20), transparent 60%),
      linear-gradient(180deg, #0d0a24 0%, #1a1145 55%, #0b0720 100%);
    background-attachment: fixed;
  }
  body:has(#lucky-page) .masthead {
    background: rgba(13, 10, 36, 0.75);
    backdrop-filter: blur(6px);
    border-bottom-color: rgba(245, 212, 138, 0.2);
  }

  .lucky-sky {
    position: fixed;
    inset: 0;
    z-index: -1;
    pointer-events: none;
    overflow: hidden;
  }
  .lucky-stars {
    position: absolute;
    inset: -50%;
    background-image:
      radial-gradient(1.5px 1.5px at 20px 30px, #fff, transparent),
      radial-gradient(1px 1px at 90px 120px, #fff, transparent),
      radial-gradient(1.5px 1.5px at 160px 60px, #ffe9b8, transparent),
      radial-gradient(1px 1px at 210px 170px, #fff, transparent),
      radial-gradient(2px 2px at 50px 200px, #d9ccff, transparent),
      radial-gradient(1px 1px at 130px 230px, #fff, transparent);
    background-size: 250px 250px;
    opacity: 0.7;
    animation: lucky-twinkle 6s ease-in-out infinite alternate;
  }
  .lucky-stars.layer2 {
    background-size: 380px 380px;
    opacity: 0.45;
    animation-duration: 9s;
    animation-delay: -3s;
  }
  .lucky-wheel {
    position: absolute;
    top: 50%;
    left: 50%;
    width: min(120vmin, 1100px);
    height: min(120vmin, 1100px);
    transform: translate(-50%, -50%);
    opacity: 0.16;
    animation: lucky-spin 240s linear infinite;
  }
  @keyframes lucky-twinkle { from { opacity: 0.35; } to { opacity: 0.85; } }
  @keyframes lucky-spin {
    from { transform: translate(-50%, -50%) rotate(0deg); }
    to   { transform: translate(-50%, -50%) rotate(360deg); }
  }
  @media (prefers-reduced-motion: reduce) {
    .lucky-stars, .lucky-wheel { animation: none; }
  }

  #lucky-page {
    font-family: "Cormorant Garamond", Georgia, serif;
    color: #ece8ff;
  }
  #lucky-page .lucky-intro {
    font-size: 1.25em;
    font-style: italic;
    color: #c9c2ef;
    margin-bottom: 1.5em;
  }
  .lucky-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.25em;
  }
  .lucky-card {
    background: rgba(255, 255, 255, 0.06);
    border: 1px solid rgba(245, 212, 138, 0.3);
    border-radius: 18px;
    padding: 1.4em 1.1em 1.2em;
    text-align: center;
    box-shadow: 0 0 40px rgba(137, 84, 255, 0.25), inset 0 0 30px rgba(245, 212, 138, 0.05);
    backdrop-filter: blur(4px);
  }
  #lucky-page .lucky-label {
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.72em;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #f5d48a;
    margin: 0 0 0.75em;
  }
  .lucky-glyph {
    font-size: 4.5em;
    line-height: 1.1;
    color: #f5d48a;
    text-shadow: 0 0 24px rgba(245, 212, 138, 0.7);
  }
  #lucky-page .lucky-name {
    font-size: 2em;
    font-weight: 700;
    margin: 0.15em 0 0;
    line-height: 1.15;
  }
  #lucky-page .lucky-sub {
    font-size: 1.1em;
    color: #c9c2ef;
    margin: 0.25em 0 0;
  }
  .lucky-code {
    display: inline-block;
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.8em;
    letter-spacing: 0.08em;
    padding: 0.2em 0.7em;
    margin-top: 0.6em;
    border: 1px solid rgba(245, 212, 138, 0.45);
    border-radius: 999px;
    color: #f5d48a;
  }
  .lucky-link {
    display: inline-block;
    margin-top: 1em;
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.9em;
    font-weight: 600;
    padding: 0.55em 1.1em;
    border-radius: 999px;
    background: linear-gradient(135deg, #f5d48a, #e7a9ff);
    color: #1a1145 !important;
    text-decoration: none !important;
    white-space: nowrap;
  }
  .lucky-link:hover { filter: brightness(1.08); }
  #lucky-page .lucky-fineprint {
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.72em;
    line-height: 1.5;
    color: #b3abd9;
    margin: 0.9em 0 0;
  }
  .lucky-footer {
    margin-top: 1.75em;
    text-align: center;
    font-size: 1.1em;
    color: #c9c2ef;
  }
  .lucky-footer strong { color: #f5d48a; font-variant-numeric: tabular-nums; }
  .lucky-disclaimer {
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.72em;
    color: #8f88b8;
    margin-top: 0.5em;
  }
</style>

<div class="lucky-sky" aria-hidden="true">
  <div class="lucky-stars"></div>
  <div class="lucky-stars layer2"></div>
  <svg class="lucky-wheel" id="lucky-wheel" viewBox="-100 -100 200 200"></svg>
</div>

<div id="lucky-page">
  <p class="lucky-intro">The stars have been consulted. A new reading is revealed every hour.</p>

  <div class="lucky-grid">
    <div class="lucky-card">
      <p class="lucky-label">This hour's lucky sign</p>
      <div class="lucky-glyph" id="lucky-sign-glyph">✦</div>
      <p class="lucky-name" id="lucky-sign-name">…</p>
      <p class="lucky-sub" id="lucky-sign-dates"></p>
    </div>

    <div class="lucky-card">
      <p class="lucky-label">This hour's lucky stock</p>
      <div class="lucky-glyph">🪄</div>
      <p class="lucky-name" id="lucky-stock-name">…</p>
      <span class="lucky-code" id="lucky-stock-code"></span><br>
      <a class="lucky-link" id="lucky-stock-link" href="https://www.bloomberg.com/" target="_blank" rel="noopener">View on Bloomberg ↗</a>
      <p class="lucky-fineprint">This is a <strong>Bloomstickberg</strong> pick: a real link to <span id="lucky-stock-url">bloomberg.com</span>, but the stock was chosen by a magic stick, not by Bloomberg.</p>
    </div>
  </div>

  <div class="lucky-footer">
    Next reading in <strong id="lucky-countdown">--:--</strong>
    <div class="lucky-disclaimer">Picked at random for fun. Not investment advice.</div>
  </div>
</div>

<script>
(function () {
  var SIGNS = [
    ["♈", "Aries", "Mar 21 – Apr 19"],
    ["♉", "Taurus", "Apr 20 – May 20"],
    ["♊", "Gemini", "May 21 – Jun 20"],
    ["♋", "Cancer", "Jun 21 – Jul 22"],
    ["♌", "Leo", "Jul 23 – Aug 22"],
    ["♍", "Virgo", "Aug 23 – Sep 22"],
    ["♎", "Libra", "Sep 23 – Oct 22"],
    ["♏", "Scorpio", "Oct 23 – Nov 21"],
    ["♐", "Sagittarius", "Nov 22 – Dec 21"],
    ["♑", "Capricorn", "Dec 22 – Jan 19"],
    ["♒", "Aquarius", "Jan 20 – Feb 18"],
    ["♓", "Pisces", "Feb 19 – Mar 20"]
  ];
  var STOCKS = [
    ["7203", "Toyota Motor"], ["6758", "Sony Group"], ["9984", "SoftBank Group"],
    ["6861", "Keyence"], ["8035", "Tokyo Electron"], ["9983", "Fast Retailing"],
    ["6098", "Recruit Holdings"], ["8306", "Mitsubishi UFJ Financial Group"],
    ["7974", "Nintendo"], ["4063", "Shin-Etsu Chemical"], ["6501", "Hitachi"],
    ["9432", "NTT"], ["9433", "KDDI"], ["8058", "Mitsubishi Corporation"],
    ["8001", "ITOCHU"], ["8031", "Mitsui & Co."], ["6367", "Daikin Industries"],
    ["4519", "Chugai Pharmaceutical"], ["4568", "Daiichi Sankyo"],
    ["4502", "Takeda Pharmaceutical"], ["6954", "FANUC"], ["6902", "DENSO"],
    ["7267", "Honda Motor"], ["6981", "Murata Manufacturing"], ["6273", "SMC"],
    ["8316", "Sumitomo Mitsui Financial Group"], ["8411", "Mizuho Financial Group"],
    ["8766", "Tokio Marine Holdings"], ["9020", "East Japan Railway"],
    ["9022", "Central Japan Railway"], ["2914", "Japan Tobacco"],
    ["4661", "Oriental Land"], ["6146", "DISCO"], ["6857", "Advantest"],
    ["6762", "TDK"], ["7741", "HOYA"], ["7751", "Canon"], ["4543", "Terumo"],
    ["2802", "Ajinomoto"], ["4452", "Kao"], ["7832", "Bandai Namco Holdings"],
    ["9766", "Konami Group"], ["5108", "Bridgestone"], ["6702", "Fujitsu"],
    ["6752", "Panasonic Holdings"], ["8801", "Mitsui Fudosan"],
    ["8802", "Mitsubishi Estate"], ["9101", "Nippon Yusen"], ["9735", "SECOM"],
    ["4901", "FUJIFILM Holdings"], ["6503", "Mitsubishi Electric"],
    ["7011", "Mitsubishi Heavy Industries"]
  ];
  var HOUR = 3600000;

  function rng(seed) {
    return function () {
      seed = (seed + 0x6D2B79F5) | 0;
      var t = Math.imul(seed ^ (seed >>> 15), 1 | seed);
      t = (t + Math.imul(t ^ (t >>> 7), 61 | t)) ^ t;
      return ((t ^ (t >>> 14)) >>> 0) / 4294967296;
    };
  }

  function $(id) { return document.getElementById(id); }

  var shownHour = -1;

  function render() {
    var hour = Math.floor(Date.now() / HOUR);
    shownHour = hour;
    var r = rng(hour * 2654435761);
    var sign = SIGNS[Math.floor(r() * SIGNS.length)];
    var stock = STOCKS[Math.floor(r() * STOCKS.length)];
    var url = "https://www.bloomberg.com/quote/" + stock[0] + ":JP";

    $("lucky-sign-glyph").textContent = sign[0] + "︎";
    $("lucky-sign-name").textContent = sign[1];
    $("lucky-sign-dates").textContent = sign[2];
    $("lucky-stock-name").textContent = stock[1];
    $("lucky-stock-code").textContent = stock[0] + ":JP · Nikkei 225";
    $("lucky-stock-link").href = url;
    $("lucky-stock-url").textContent = url.replace("https://www.", "");
  }

  function tick() {
    var left = HOUR - (Date.now() % HOUR);
    var m = Math.floor(left / 60000);
    var s = Math.floor((left % 60000) / 1000);
    $("lucky-countdown").textContent = m + ":" + (s < 10 ? "0" : "") + s;
    if (Math.floor(Date.now() / HOUR) !== shownHour) { render(); }
  }

  function drawWheel() {
    var svg = $("lucky-wheel");
    var ns = "http://www.w3.org/2000/svg";
    var gold = "#f5d48a";
    [94, 78, 60, 30].forEach(function (rad, i) {
      var c = document.createElementNS(ns, "circle");
      c.setAttribute("r", rad);
      c.setAttribute("fill", "none");
      c.setAttribute("stroke", gold);
      c.setAttribute("stroke-width", i === 0 ? 0.8 : 0.4);
      svg.appendChild(c);
    });
    for (var i = 0; i < 12; i++) {
      var a = (i * 30 - 90) * Math.PI / 180;
      var line = document.createElementNS(ns, "line");
      line.setAttribute("x1", 60 * Math.cos(a));
      line.setAttribute("y1", 60 * Math.sin(a));
      line.setAttribute("x2", 94 * Math.cos(a));
      line.setAttribute("y2", 94 * Math.sin(a));
      line.setAttribute("stroke", gold);
      line.setAttribute("stroke-width", 0.4);
      svg.appendChild(line);
      var g = (i * 30 + 15 - 90) * Math.PI / 180;
      var t = document.createElementNS(ns, "text");
      t.setAttribute("x", 86 * Math.cos(g));
      t.setAttribute("y", 86 * Math.sin(g));
      t.setAttribute("fill", gold);
      t.setAttribute("font-size", 9);
      t.setAttribute("text-anchor", "middle");
      t.setAttribute("dominant-baseline", "central");
      t.textContent = SIGNS[i][0] + "︎";
      svg.appendChild(t);
    }
    var star = document.createElementNS(ns, "polygon");
    var pts = [];
    for (var k = 0; k < 16; k++) {
      var rr = k % 2 === 0 ? 28 : 11;
      var b = (k * 22.5 - 90) * Math.PI / 180;
      pts.push((rr * Math.cos(b)).toFixed(2) + "," + (rr * Math.sin(b)).toFixed(2));
    }
    star.setAttribute("points", pts.join(" "));
    star.setAttribute("fill", "none");
    star.setAttribute("stroke", gold);
    star.setAttribute("stroke-width", 0.5);
    svg.appendChild(star);
  }

  drawWheel();
  render();
  tick();
  setInterval(tick, 1000);
})();
</script>
{:/nomarkdown}
