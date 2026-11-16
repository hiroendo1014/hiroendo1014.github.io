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
  .lucky-disclaimer {
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.72em;
    color: #8f88b8;
    margin-top: 0.5em;
  }
  .lucky-card { position: relative; }
  .lucky-card::before {
    content: "";
    position: absolute;
    inset: 7px;
    border: 1px solid rgba(245, 212, 138, 0.22);
    border-radius: 13px;
    pointer-events: none;
  }
  .lucky-flip {
    perspective: 1400px;
    cursor: pointer;
    -webkit-tap-highlight-color: transparent;
  }
  .lucky-flip-inner {
    display: grid;
    height: 100%;
    transition: transform 0.8s cubic-bezier(0.2, 0.7, 0.2, 1);
    transform-style: preserve-3d;
  }
  .lucky-flip.is-flipped .lucky-flip-inner { transform: rotateY(180deg); }
  .lucky-flip .lucky-card {
    grid-area: 1 / 1;
    backface-visibility: hidden;
    -webkit-backface-visibility: hidden;
    backdrop-filter: none;
    transition: border-color 0.3s, box-shadow 0.3s;
  }
  .lucky-flip .lucky-back { transform: rotateY(180deg); }
  .lucky-flip:not(.is-flipped) .lucky-back,
  .lucky-flip.is-flipped .lucky-front { pointer-events: none; }
  .lucky-flip:hover .lucky-card {
    border-color: rgba(245, 212, 138, 0.6);
    box-shadow: 0 0 60px rgba(137, 84, 255, 0.45), inset 0 0 30px rgba(245, 212, 138, 0.08);
  }
  .lucky-flip-btn {
    display: block;
    margin: 0.9em auto 0;
    padding: 0.2em 0.6em;
    background: none;
    border: 0;
    border-radius: 6px;
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.68em;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #e7a9ff;
    cursor: pointer;
  }
  .lucky-flip-btn:hover { color: #f5d48a; }
  .lucky-flip-btn:focus-visible { outline: 2px solid #f5d48a; outline-offset: 2px; }
  .lucky-glyph.is-text { font-family: "Cormorant Garamond", Georgia, serif; font-weight: 700; }
  .lucky-glyph.is-long { font-size: 3.2em; line-height: 1.55; }
  @media (prefers-reduced-motion: reduce) {
    .lucky-flip-inner { transition: none; }
  }
  .lucky-form {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: flex-end;
    gap: 0.9em 1.4em;
    margin: 0 0 1.6em;
    padding: 1em 1.2em;
    border: 1px solid rgba(245, 212, 138, 0.3);
    border-radius: 18px;
    background: rgba(255, 255, 255, 0.05);
  }
  .lucky-field { display: flex; flex-direction: column; gap: 0.35em; text-align: left; }
  #lucky-page .lucky-field label {
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.68em;
    letter-spacing: 0.18em;
    text-transform: uppercase;
    color: #f5d48a;
    margin: 0;
  }
  #lucky-page .lucky-field input,
  #lucky-page .lucky-field select {
    font-family: -apple-system, "Segoe UI", Roboto, sans-serif;
    font-size: 0.95em;
    color: #ece8ff;
    background: rgba(13, 10, 36, 0.7);
    border: 1px solid rgba(245, 212, 138, 0.45);
    border-radius: 10px;
    padding: 0.45em 0.7em;
    margin: 0;
    width: auto;
    min-width: 10em;
    color-scheme: dark;
    box-shadow: none;
  }
  #lucky-page .lucky-field input:focus,
  #lucky-page .lucky-field select:focus { outline: 2px solid #f5d48a; outline-offset: 1px; }
  #lucky-page .lucky-aura {
    font-size: 1.15em;
    font-style: italic;
    line-height: 1.4;
    color: #ece8ff;
    margin: 0.9em 0 0;
  }
</style>

<div class="lucky-sky" aria-hidden="true">
  <div class="lucky-stars"></div>
  <div class="lucky-stars layer2"></div>
  <svg class="lucky-wheel" id="lucky-wheel" viewBox="-100 -100 200 200"></svg>
</div>

<div id="lucky-page">
  <p class="lucky-intro">Tell the stars when you were born. Your lucky stock and currency are revealed anew every hour.</p>

  <form class="lucky-form" id="lucky-form" onsubmit="return false;">
    <div class="lucky-field">
      <label for="lucky-birth">Date of birth</label>
      <input type="date" id="lucky-birth" value="2001-10-14" min="1900-01-01" max="2100-12-31">
    </div>
    <div class="lucky-field">
      <label for="lucky-gender">Gender</label>
      <select id="lucky-gender">
        <option value="male" selected>Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option>
      </select>
    </div>
  </form>

  <div class="lucky-grid">
    <div class="lucky-card">
      <p class="lucky-label">Your birth sign</p>
      <div class="lucky-glyph" id="lucky-sign-glyph">✦</div>
      <p class="lucky-name" id="lucky-sign-name">…</p>
      <p class="lucky-sub" id="lucky-sign-dates"></p>
      <p class="lucky-aura" id="lucky-sign-aura"></p>
    </div>

    <div class="lucky-flip" id="lucky-flip">
      <div class="lucky-flip-inner">
        <div class="lucky-card lucky-front" id="lucky-front">
          <p class="lucky-label">Your lucky stock</p>
          <div class="lucky-glyph">🪄</div>
          <p class="lucky-name" id="lucky-stock-name">…</p>
          <span class="lucky-code" id="lucky-stock-code"></span><br>
          <a class="lucky-link" id="lucky-stock-link" href="https://www.bloomberg.com/" target="_blank" rel="noopener">View on Bloomberg ↗</a>
          <p class="lucky-fineprint">This is a <strong>Bloomstickberg</strong> pick: a real link to <span id="lucky-stock-url">bloomberg.com</span>, but the stock was chosen by a magic stick, not by Bloomberg.</p>
          <button type="button" class="lucky-flip-btn" id="lucky-flip-to-back">↻ Tap to flip the card</button>
        </div>
        <div class="lucky-card lucky-back" id="lucky-back" aria-hidden="true">
          <p class="lucky-label">Your lucky currency</p>
          <div class="lucky-glyph is-text" id="lucky-fx-glyph">¤</div>
          <p class="lucky-name" id="lucky-fx-name">…</p>
          <span class="lucky-code" id="lucky-fx-code"></span><br>
          <a class="lucky-link" id="lucky-fx-link" href="https://www.bloomberg.com/" target="_blank" rel="noopener" tabindex="-1">View on Bloomberg ↗</a>
          <p class="lucky-fineprint">Another <strong>Bloomstickberg</strong> pick: a real link to <span id="lucky-fx-url">bloomberg.com</span> for its exchange rate with the US dollar, chosen by the same magic stick.</p>
          <button type="button" class="lucky-flip-btn" id="lucky-flip-to-front" tabindex="-1">↻ Tap to flip back</button>
        </div>
      </div>
    </div>
  </div>

  <div class="lucky-footer">
    <div class="lucky-disclaimer">Not investment advice.</div>
  </div>
</div>

<script>
(function () {
  var SIGNS = [
    ["♈", "Aries", "Mar 21 – Apr 19", 3, 21, "A blazing red aura of courage that charges in before the doubts arrive."],
    ["♉", "Taurus", "Apr 20 – May 20", 4, 20, "A deep emerald aura of calm, steady as fertile earth."],
    ["♊", "Gemini", "May 21 – Jun 20", 5, 21, "A flickering yellow aura of curiosity, always mid-conversation."],
    ["♋", "Cancer", "Jun 21 – Jul 22", 6, 21, "A silvery moonlit aura that shelters everyone it touches."],
    ["♌", "Leo", "Jul 23 – Aug 22", 7, 23, "A radiant golden aura that fills the room like sunlight."],
    ["♍", "Virgo", "Aug 23 – Sep 22", 8, 23, "A clear sage-green aura of quiet precision and care."],
    ["♎", "Libra", "Sep 23 – Oct 22", 9, 23, "A soft rose-pink aura of harmony, balancing every scale it meets."],
    ["♏", "Scorpio", "Oct 23 – Nov 21", 10, 23, "A smoldering crimson aura of depth, intensity and secrets kept."],
    ["♐", "Sagittarius", "Nov 22 – Dec 21", 11, 22, "A bright violet aura of adventure, aimed at the far horizon."],
    ["♑", "Capricorn", "Dec 22 – Jan 19", 12, 22, "A dark garnet aura of ambition, climbing patiently toward the summit."],
    ["♒", "Aquarius", "Jan 20 – Feb 18", 1, 20, "An electric turquoise aura of originality, a few years ahead of its time."],
    ["♓", "Pisces", "Feb 19 – Mar 20", 2, 19, "A shimmering sea-blue aura of dreams and intuition."]
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
  var CURRENCIES = [
    ["EUR", "€", "Euro", "EURUSD"], ["GBP", "£", "British Pound", "GBPUSD"],
    ["JPY", "¥", "Japanese Yen", "USDJPY"], ["CHF", "Fr", "Swiss Franc", "USDCHF"],
    ["CAD", "C$", "Canadian Dollar", "USDCAD"], ["AUD", "A$", "Australian Dollar", "AUDUSD"],
    ["NZD", "NZ$", "New Zealand Dollar", "NZDUSD"], ["CNY", "元", "Chinese Yuan", "USDCNY"],
    ["HKD", "HK$", "Hong Kong Dollar", "USDHKD"], ["SGD", "S$", "Singapore Dollar", "USDSGD"],
    ["KRW", "₩", "South Korean Won", "USDKRW"], ["INR", "₹", "Indian Rupee", "USDINR"],
    ["TWD", "NT$", "New Taiwan Dollar", "USDTWD"], ["THB", "฿", "Thai Baht", "USDTHB"],
    ["IDR", "Rp", "Indonesian Rupiah", "USDIDR"], ["PHP", "₱", "Philippine Peso", "USDPHP"],
    ["MXN", "Mex$", "Mexican Peso", "USDMXN"], ["BRL", "R$", "Brazilian Real", "USDBRL"],
    ["ZAR", "R", "South African Rand", "USDZAR"], ["TRY", "₺", "Turkish Lira", "USDTRY"],
    ["SEK", "kr", "Swedish Krona", "USDSEK"], ["NOK", "kr", "Norwegian Krone", "USDNOK"],
    ["DKK", "kr", "Danish Krone", "USDDKK"], ["PLN", "zł", "Polish Złoty", "USDPLN"],
    ["ILS", "₪", "Israeli New Shekel", "USDILS"], ["CZK", "Kč", "Czech Koruna", "USDCZK"],
    ["HUF", "Ft", "Hungarian Forint", "USDHUF"], ["RON", "lei", "Romanian Leu", "USDRON"],
    ["ISK", "kr", "Icelandic Króna", "USDISK"], ["RSD", "din", "Serbian Dinar", "USDRSD"],
    ["UAH", "₴", "Ukrainian Hryvnia", "USDUAH"], ["GEL", "₾", "Georgian Lari", "USDGEL"],
    ["KZT", "₸", "Kazakhstani Tenge", "USDKZT"], ["MNT", "₮", "Mongolian Tögrög", "USDMNT"],
    ["MYR", "RM", "Malaysian Ringgit", "USDMYR"], ["VND", "₫", "Vietnamese Đồng", "USDVND"],
    ["MOP", "MOP$", "Macanese Pataca", "USDMOP"], ["PKR", "₨", "Pakistani Rupee", "USDPKR"],
    ["BDT", "৳", "Bangladeshi Taka", "USDBDT"], ["LKR", "Rs", "Sri Lankan Rupee", "USDLKR"],
    ["NPR", "रू", "Nepalese Rupee", "USDNPR"], ["SAR", "SR", "Saudi Riyal", "USDSAR"],
    ["AED", "د.إ", "UAE Dirham", "USDAED"], ["QAR", "QR", "Qatari Riyal", "USDQAR"],
    ["KWD", "KD", "Kuwaiti Dinar", "USDKWD"], ["BHD", "BD", "Bahraini Dinar", "USDBHD"],
    ["OMR", "RO", "Omani Rial", "USDOMR"], ["JOD", "JD", "Jordanian Dinar", "USDJOD"],
    ["EGP", "E£", "Egyptian Pound", "USDEGP"], ["MAD", "DH", "Moroccan Dirham", "USDMAD"],
    ["NGN", "₦", "Nigerian Naira", "USDNGN"], ["KES", "KSh", "Kenyan Shilling", "USDKES"],
    ["GHS", "₵", "Ghanaian Cedi", "USDGHS"], ["CLP", "CLP$", "Chilean Peso", "USDCLP"],
    ["COP", "COL$", "Colombian Peso", "USDCOP"], ["PEN", "S/", "Peruvian Sol", "USDPEN"],
    ["ARS", "AR$", "Argentine Peso", "USDARS"], ["UYU", "$U", "Uruguayan Peso", "USDUYU"]
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
  var DEFAULT_BIRTH = "2001-10-14";
  var DEFAULT_GENDER = "male";
  var STORE_KEY = "lucky-profile";

  function hashString(str) {
    var h = 2166136261;
    for (var i = 0; i < str.length; i++) {
      h ^= str.charCodeAt(i);
      h = Math.imul(h, 16777619);
    }
    return h >>> 0;
  }

  function readBirth() {
    var v = $("lucky-birth").value;
    var m = /^(\d{4})-(\d{2})-(\d{2})$/.exec(v);
    if (!m) { v = DEFAULT_BIRTH; m = /^(\d{4})-(\d{2})-(\d{2})$/.exec(v); }
    return { iso: v, month: +m[2], day: +m[3] };
  }

  function birthSign(month, day) {
    var idx = -1;
    SIGNS.forEach(function (s, i) { if (s[3] === month) { idx = day >= s[4] ? i : (i + 11) % 12; } });
    return SIGNS[idx < 0 ? 6 : idx];
  }

  function render() {
    var hour = Math.floor(Date.now() / HOUR);
    shownHour = hour;
    var birth = readBirth();
    var gender = $("lucky-gender").value || DEFAULT_GENDER;
    var sign = birthSign(birth.month, birth.day);
    $("lucky-sign-aura").textContent = sign[5];
    var r = rng(hashString(birth.iso + "|" + gender + "|" + hour));
    var stock = STOCKS[Math.floor(r() * STOCKS.length)];
    var url = "https://www.bloomberg.com/quote/" + stock[0] + ":JP";

    $("lucky-sign-glyph").textContent = sign[0] + "︎";
    $("lucky-sign-name").textContent = sign[1];
    $("lucky-sign-dates").textContent = sign[2];
    $("lucky-stock-name").textContent = stock[1];
    $("lucky-stock-code").textContent = stock[0] + ":JP · Nikkei 225";
    $("lucky-stock-link").href = url;
    $("lucky-stock-url").textContent = url.replace("https://www.", "");

    var fx = CURRENCIES[Math.floor(r() * CURRENCIES.length)];
    var pair = fx[3].slice(0, 3) + "/" + fx[3].slice(3);
    var fxUrl = "https://www.bloomberg.com/quote/" + fx[3] + ":CUR";
    var glyph = $("lucky-fx-glyph");
    glyph.textContent = fx[1];
    glyph.classList.toggle("is-long", fx[1].length > 2);
    $("lucky-fx-name").textContent = fx[2];
    $("lucky-fx-code").textContent = fx[0] + " · " + pair;
    $("lucky-fx-link").href = fxUrl;
    $("lucky-fx-url").textContent = fxUrl.replace("https://www.", "");
  }

  function setupFlip() {
    var flip = $("lucky-flip");
    var faces = { front: $("lucky-front"), back: $("lucky-back") };
    var buttons = { front: $("lucky-flip-to-back"), back: $("lucky-flip-to-front") };

    function show(side) {
      var hidden = side === "front" ? "back" : "front";
      flip.classList.toggle("is-flipped", side === "back");
      faces[side].removeAttribute("aria-hidden");
      faces[hidden].setAttribute("aria-hidden", "true");
      faces[side].querySelectorAll("a, button").forEach(function (el) { el.removeAttribute("tabindex"); });
      faces[hidden].querySelectorAll("a, button").forEach(function (el) { el.setAttribute("tabindex", "-1"); });
    }

    flip.addEventListener("click", function (e) {
      if (e.target.closest("a")) { return; }
      var side = flip.classList.contains("is-flipped") ? "front" : "back";
      show(side);
      if (e.target.closest("button")) { buttons[side].focus({ preventScroll: true }); }
    });

    show("front");
  }

  function setupForm() {
    var birthEl = $("lucky-birth");
    var genderEl = $("lucky-gender");
    try {
      var saved = JSON.parse(localStorage.getItem(STORE_KEY) || "null");
      if (saved && /^\d{4}-\d{2}-\d{2}$/.test(saved.birth)) { birthEl.value = saved.birth; }
      if (saved && ["male", "female", "other"].indexOf(saved.gender) >= 0) { genderEl.value = saved.gender; }
    } catch (e) {}
    function update() {
      try { localStorage.setItem(STORE_KEY, JSON.stringify({ birth: birthEl.value, gender: genderEl.value })); } catch (e) {}
      render();
    }
    birthEl.addEventListener("change", update);
    birthEl.addEventListener("input", update);
    genderEl.addEventListener("change", update);
  }

  function tick() {
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
  setupForm();
  render();
  setupFlip();
  setInterval(tick, 1000);
})();
</script>
{:/nomarkdown}
