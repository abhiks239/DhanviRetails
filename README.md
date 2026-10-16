<html lang="en"> 
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Dhanvishta | Custom Windows Software — One-time fee from ₹1,999</title>
<meta name="description" content="Custom billing, accounting, inventory and CRM software for Windows. One-time fee from ₹1,999. No subscriptions. You own your data." />
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Sora:wght@600;700;800&display=swap" rel="stylesheet" />
<style>
  :root{
  --bg:#ffffff;--bg2:#f4f7fe;--bg3:#eaf1ff;
  --card:#ffffff;--line:#e2e8f0;--line2:#dbe4f5;
  --text:#0b1530;--muted:#5b6b8a;
  --blue:#2563eb;--blue2:#1d4ed8;--sky:#0ea5e9;
  --green:#10b981;--amber:#f59e0b;--red:#ef4444;
  --shadow:0 10px 30px rgba(37,99,235,.08);
  --shadow-lg:0 24px 60px rgba(15,23,42,.12);
  --h:'Sora','Inter',system-ui,sans-serif;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:80px}
body{font-family:'Inter',system-ui,-apple-system,'Segoe UI',sans-serif;background:var(--bg);color:var(--text);line-height:1.6;-webkit-font-smoothing:antialiased;overflow-x:hidden}
a{color:inherit;text-decoration:none}
img{max-width:100%;display:block}
.wrap{max-width:1160px;margin:0 auto;padding:0 20px}
:focus-visible{outline:2px solid var(--blue);outline-offset:3px;border-radius:6px}
h1,h2,h3,h4{font-family:var(--h);color:var(--text)}

/* ---------- buttons ---------- */
.btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;padding:13px 24px;border-radius:12px;font-weight:600;font-size:.95rem;border:1px solid transparent;cursor:pointer;transition:transform .2s,box-shadow .2s,background .2s,border-color .2s;font-family:inherit}
.btn-primary{background:var(--blue);color:#fff;box-shadow:0 10px 24px rgba(37,99,235,.32)}
.btn-primary:hover{background:var(--blue2);transform:translateY(-2px);box-shadow:0 14px 30px rgba(37,99,235,.38)}
.btn-ghost{border-color:var(--line2);background:#fff;color:var(--text)}
.btn-ghost:hover{border-color:var(--blue);color:var(--blue);background:#f2f6ff;transform:translateY(-2px)}
.btn-wa{background:#16a34a;color:#fff;box-shadow:0 10px 24px rgba(22,163,74,.3)}
.btn-wa:hover{background:#15803d;transform:translateY(-2px)}

/* ---------- header ---------- */
header{position:sticky;top:0;z-index:50;background:rgba(255,255,255,.88);backdrop-filter:blur(14px);border-bottom:1px solid var(--line)}
.nav{display:flex;align-items:center;justify-content:space-between;height:72px}
.logo{display:flex;align-items:center;gap:10px;font-family:var(--h);font-weight:800;font-size:1.25rem;color:var(--text);flex:0 0 auto}
.logo-mark{display:inline-flex;align-items:center;justify-content:center;flex:0 0 auto;line-height:0}
.logo-img{display:block;height:42px;width:auto;max-width:170px;object-fit:contain}
.logo .mark{display:none;width:38px;height:38px;border-radius:11px;background:linear-gradient(135deg,var(--blue),var(--sky));place-items:center;color:#fff;font-weight:800;font-size:1.05rem;box-shadow:0 6px 16px rgba(37,99,235,.35)}
.logo-mark.no-img .mark{display:grid}
.nav ul{display:flex;gap:30px;list-style:none}
.nav ul a{color:var(--muted);font-size:.94rem;font-weight:500;transition:color .2s}
.nav ul a:hover{color:var(--blue)}
.nav .btn{padding:10px 18px;font-size:.88rem}

/* ---------- hero ---------- */
.hero{position:relative;padding:80px 0 90px;background:linear-gradient(180deg,#f4f7fe 0%,#ffffff 100%);overflow:hidden}
.hero::before{content:"";position:absolute;top:-200px;right:-180px;width:640px;height:640px;background:radial-gradient(circle,rgba(37,99,235,.14),transparent 65%);border-radius:50%}
.hero::after{content:"";position:absolute;bottom:-240px;left:-180px;width:560px;height:560px;background:radial-gradient(circle,rgba(14,165,233,.12),transparent 65%);border-radius:50%}
.hero-grid{position:relative;display:grid;grid-template-columns:1.05fr 1fr;gap:56px;align-items:center}
.tag{display:inline-flex;align-items:center;gap:8px;padding:7px 14px;border:1px solid #c7d9ff;border-radius:99px;color:var(--blue);font-size:.85rem;font-weight:600;margin-bottom:22px;background:#eaf1ff}
.tag::before{content:"";width:7px;height:7px;border-radius:50%;background:var(--green);box-shadow:0 0 0 3px rgba(16,185,129,.25)}
h1{font-size:clamp(2.1rem,4.6vw,3.5rem);line-height:1.08;letter-spacing:-.035em;font-weight:800}
h1 .accent{background:linear-gradient(120deg,var(--blue),var(--sky));-webkit-background-clip:text;background-clip:text;color:transparent}
.lead{color:var(--muted);font-size:1.1rem;margin:22px 0 30px;max-width:31em}
.cta-row{display:flex;flex-wrap:wrap;gap:12px}
.proof{display:flex;flex-wrap:wrap;gap:26px;margin-top:34px;color:var(--muted);font-size:.9rem}
.proof span{display:flex;align-items:center;gap:8px}
.proof b{color:var(--text);font-family:var(--h);font-size:1.05rem}
.proof i{font-style:normal;color:var(--green);font-weight:800}

/* hero visual: photo + floating cards */
.hero-visual{position:relative;height:520px}
.hero-photo{position:absolute;inset:0;border-radius:22px;overflow:hidden;box-shadow:var(--shadow-lg);border:6px solid #fff}
.hero-photo img{width:100%;height:100%;object-fit:cover}
.float-card{position:absolute;background:#fff;border:1px solid var(--line);border-radius:14px;padding:14px 16px;box-shadow:var(--shadow-lg);font-size:.82rem;min-width:200px}
.float-card .ttl{font-family:var(--h);font-weight:700;font-size:.78rem;color:var(--muted);text-transform:uppercase;letter-spacing:.05em;margin-bottom:8px}
.fc1{top:22px;left:-26px;animation:float 5s ease-in-out infinite}
.fc2{bottom:26px;right:-22px;animation:float 6s ease-in-out infinite reverse}
@keyframes float{0%,100%{transform:translateY(0)}50%{transform:translateY(-10px)}}
.mini-row{display:flex;justify-content:space-between;gap:14px;padding:4px 0;color:var(--muted)}
.mini-row b{color:var(--text)}
.bar-line{height:6px;border-radius:9px;background:var(--bg3);width:70px;overflow:hidden}
.bar-line span{display:block;height:100%;background:var(--blue)}

/* ---------- sections ---------- */
section{padding:92px 0}
.head{max-width:680px;margin-bottom:48px}
.eyebrow{display:inline-block;font-family:var(--h);font-weight:700;font-size:.8rem;letter-spacing:.12em;text-transform:uppercase;color:var(--blue);margin-bottom:14px}
h2{font-size:clamp(1.8rem,3.4vw,2.6rem);letter-spacing:-.03em;line-height:1.15;font-weight:800}
.head p{color:var(--muted);margin-top:14px;font-size:1.05rem}

/* ---------- problem ---------- */
.problem{background:var(--bg2)}
.grid4{display:grid;grid-template-columns:repeat(4,1fr);gap:18px}
.pc{background:#fff;border:1px solid var(--line);border-radius:16px;padding:26px 22px;transition:transform .25s,box-shadow .25s,border-color .25s}
.pc:hover{transform:translateY(-4px);box-shadow:var(--shadow);border-color:#c7d9ff}
.pc .icn{width:44px;height:44px;border-radius:12px;display:grid;place-items:center;background:#fee2e2;color:var(--red);font-size:1.2rem;margin-bottom:14px}
.pc .big{font-family:var(--h);font-weight:800;font-size:.78rem;color:var(--red);letter-spacing:.06em;text-transform:uppercase;margin-bottom:6px}
.pc h3{font-size:1.05rem;margin-bottom:6px}
.pc p{color:var(--muted);font-size:.92rem}

/* ---------- with / without ---------- */
.compare{background:#fff}
.compare-wrap{display:grid;grid-template-columns:1fr 1fr;gap:24px;border-radius:24px;overflow:hidden;border:1px solid var(--line);box-shadow:var(--shadow-lg)}
.col{padding:36px 32px}
.col-bad{background:linear-gradient(180deg,#fff5f5,#ffffff)}
.col-good{background:linear-gradient(180deg,#eff9ff,#ffffff)}
.col h3{display:flex;align-items:center;gap:12px;font-size:1.25rem;margin-bottom:22px}
.col h3 .pill-i{width:38px;height:38px;border-radius:11px;display:grid;place-items:center;color:#fff;font-size:1rem;font-weight:800}
.col-bad .pill-i{background:var(--red)}
.col-good .pill-i{background:var(--green)}
.col ul{list-style:none;display:grid;gap:14px}
.col li{display:flex;gap:12px;align-items:flex-start;font-size:.96rem;color:#2b3550;padding-bottom:14px;border-bottom:1px dashed var(--line)}
.col li:last-child{border-bottom:0;padding-bottom:0}
.col li .tick{flex:0 0 22px;width:22px;height:22px;border-radius:50%;display:grid;place-items:center;font-size:.72rem;font-weight:800;color:#fff;margin-top:2px}
.col-bad .tick{background:var(--red)}
.col-good .tick{background:var(--green)}
.col-bad li b{color:var(--red)}
.col-good li b{color:var(--green)}

/* ---------- examples ---------- */
.work{background:var(--bg2)}
.grid2{display:grid;grid-template-columns:repeat(2,1fr);gap:30px}
.shot{background:#fff;border:1px solid var(--line);border-radius:20px;overflow:hidden;transition:transform .3s,box-shadow .3s}
.shot:hover{transform:translateY(-6px);box-shadow:var(--shadow-lg)}
.shot-img{position:relative;height:230px;overflow:hidden;border-bottom:1px solid var(--line)}
.shot-img img{width:100%;height:100%;object-fit:cover;transition:transform .5s}
.shot:hover .shot-img img{transform:scale(1.05)}
.shot-img::after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,rgba(255,255,255,0) 40%,rgba(255,255,255,.85))}
.shot-body{padding:24px 26px 28px}
.shot-body h3{font-size:1.2rem;margin-bottom:8px;display:flex;align-items:center;gap:10px}
.shot-body h3 .badge-n{font-size:.7rem;background:#eaf1ff;color:var(--blue);padding:3px 9px;border-radius:99px;font-weight:700;letter-spacing:.05em}
.shot-body p{color:var(--muted);font-size:.94rem;margin-bottom:18px}

/* mini app mockup inside shot */
.mockup{background:#f7f9ff;border:1px solid var(--line);border-radius:12px;padding:14px;font-size:.78rem;font-family:'Inter',sans-serif}
.mockup .row{display:flex;justify-content:space-between;align-items:center;gap:8px;padding:6px 0;border-bottom:1px solid #eaf0fb;color:#2b3550}
.mockup .row:last-child{border:0}
.mockup .row .muted{color:var(--muted)}
.mockup .total{display:flex;justify-content:space-between;margin-top:8px;padding:8px 10px;border-radius:8px;background:#eaf1ff;font-weight:700;font-size:.84rem;color:var(--blue)}
.pill{padding:2px 9px;border-radius:99px;font-size:.68rem;font-weight:700;background:rgba(16,185,129,.14);color:var(--green)}
.pill.r{background:rgba(239,68,68,.14);color:var(--red)}
.pill.a{background:rgba(245,158,11,.16);color:#b45309}
.pill.b{background:rgba(37,99,235,.12);color:var(--blue)}
.stock{height:6px;border-radius:9px;background:#e2e8f0;width:64px;overflow:hidden}
.stock span{display:block;height:100%;background:var(--blue)}
.av{width:24px;height:24px;border-radius:50%;display:grid;place-items:center;font-weight:700;font-size:.68rem;color:#fff}
.flow{display:flex;align-items:center;gap:10px;justify-content:center;padding:6px 0}
.file{padding:10px 10px;border:1px dashed #b8c8ea;border-radius:10px;text-align:center;line-height:1.3;background:#fff;flex:1}
.file b{display:block;font-size:.74rem;color:#0b1530}
.file small{color:var(--muted);font-size:.68rem}
.flow .go{color:var(--blue);font-size:1.1rem;font-weight:800}
.prog{height:6px;border-radius:9px;background:#e2e8f0;margin-top:10px;overflow:hidden}
.prog span{display:block;height:100%;width:100%;background:var(--green)}

/* ---------- pricing ---------- */
.price-box{display:grid;grid-template-columns:1fr 1.1fr;background:linear-gradient(135deg,#eef4ff,#ffffff);border:1px solid #c7d9ff;border-radius:24px;overflow:hidden;box-shadow:var(--shadow-lg)}
.price-l{padding:48px 42px;border-right:1px solid #dbe4f5;background:linear-gradient(160deg,#ffffff,#f4f7fe)}
.price-l p{color:var(--muted)}
.amount{font-family:var(--h);font-size:clamp(3rem,7vw,4.6rem);font-weight:800;letter-spacing:-.04em;line-height:1;margin:12px 0 8px;color:var(--blue)}
.amount small{font-size:1.05rem;font-weight:600;color:var(--muted);letter-spacing:0;margin-left:6px}
.price-l .btn{margin-top:26px;width:100%}
.price-r{padding:48px 42px}
.price-r h3{margin-bottom:18px;font-size:1.15rem}
.price-r ul{list-style:none;display:grid;gap:14px}
.price-r li{display:flex;gap:12px;color:#2b3550;font-size:.95rem}
.price-r li::before{content:"✓";color:var(--green);font-weight:800;flex:0 0 auto}

/* ---------- final ---------- */
.final{text-align:center;padding:96px 0;background:linear-gradient(180deg,#f4f7fe,#eaf1ff)}
.final p{color:var(--muted);margin:16px auto 30px;max-width:34em;font-size:1.05rem}
.final .cta-row{justify-content:center}

/* ---------- footer ---------- */
footer{border-top:1px solid var(--line);padding:34px 0;color:var(--muted);font-size:.9rem;background:#fff}
.foot{display:flex;flex-wrap:wrap;gap:16px;justify-content:space-between;align-items:center}
.foot a:hover{color:var(--blue)}
.foot .logo{font-size:1rem}
.foot .logo-img{height:34px;max-width:140px}
.foot .mark{width:32px;height:32px;border-radius:9px;font-size:.9rem}

/* ---------- responsive ---------- */
@media (max-width:960px){
  .hero-grid{grid-template-columns:1fr;gap:40px}
  .hero-visual{height:420px;max-width:560px;margin:0 auto;width:100%}
  .grid4{grid-template-columns:repeat(2,1fr)}
  .compare-wrap{grid-template-columns:1fr}
  .price-box{grid-template-columns:1fr}
  .price-l{border-right:0;border-bottom:1px solid #dbe4f5}
  .fc1{left:8px}.fc2{right:8px}
}
@media (max-width:700px){
  .nav ul{display:none}
  .grid4,.grid2{grid-template-columns:1fr}
  section{padding:64px 0}
  .hero{padding:48px 0 64px}
  .price-l,.price-r{padding:32px 24px}
  .col{padding:28px 22px}
  .hero-visual{height:360px}
  .float-card{font-size:.76rem;min-width:170px;padding:11px 13px}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important;animation:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>

<header>
  <div class="wrap nav">
   <a href="#top" class="logo" aria-label="Dhanvishta — Home">
  <span class="logo-mark">
    <img src="Logo.png" alt="Dhanvishta" class="logo-img"
         onerror="this.style.display='none';this.parentElement.classList.add('no-img')" />
    <span class="mark" aria-hidden="true">D</span>
  </span>
  <span class="logo-text">Dhanvishta</span>
</a>
    <ul>
      <li><a href="#problem">Problem</a></li>
      <li><a href="#compare">With vs Without</a></li>
      <li><a href="#work">Examples</a></li>
      <li><a href="#pricing">Pricing</a></li>
    </ul>
    <a class="btn btn-wa" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20need%20custom%20software%20for%20my%20business." target="_blank" rel="noopener">WhatsApp us</a>
  </div>
</header>

<main id="top">

<!-- ============ HERO ============ -->
<div class="hero">
  <div class="wrap hero-grid">
    <div>
      <span class="tag">Your Business Simplified</span>
      <h1>Software made for <span class="accent">your shop</span>, not for everyone.</h1>
      <p class="lead">We build custom billing, accounting, inventory and CRM software for Windows. Pay one time. Your data stays on your own computer.</p>
      <div class="cta-row">
        <a class="btn btn-primary" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20want%20a%20quote%20for%20custom%20software." target="_blank" rel="noopener">Get a free quote on WhatsApp</a>
        <a class="btn btn-ghost" href="#work">See real examples</a>
      </div>
      <div class="proof">
        <span><b>₹1,999</b> one-time start</span>
        <span><i>●</i> <b>0</b> monthly fees</span>
        <span><i>●</i> <b>100%</b> your data</span>
      </div>
    </div>

    <div class="hero-visual">
      <div class="hero-photo">
        <img src="https://images.unsplash.com/photo-1556742049-0cfed4f6a45d?auto=format&fit=crop&w=1000&q=80" alt="Shop owner using billing software on a Windows computer" loading="lazy" />
      </div>

      <div class="float-card fc1">
        <div class="ttl">Today's Sales</div>
        <div class="mini-row"><span>Invoices</span><b>42</b></div>
        <div class="mini-row"><span>Collected</span><b style="color:var(--green)">₹1,24,580</b></div>
        <div class="mini-row"><span>Pending</span><b style="color:var(--amber)">₹18,200</b></div>
      </div>

      <div class="float-card fc2">
        <div class="ttl">Stock Alert</div>
        <div class="mini-row"><span>Sugar 1kg</span><div class="bar-line"><span style="width:80%"></span></div><b>120</b></div>
        <div class="mini-row"><span>Tea 250g</span><div class="bar-line"><span style="width:25%;background:var(--amber)"></span></div><b>18</b></div>
        <div class="mini-row"><span>Soap Pack</span><div class="bar-line"><span style="width:8%;background:var(--red)"></span></div><b>4</b></div>
      </div>
    </div>
  </div>
</div>

<!-- ============ PROBLEM ============ -->
<section id="problem" class="problem">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow">The Problem</span>
      <h2>Does your current software cause these problems?</h2>
      <p>Most small businesses are stuck with tools that were never made for them.</p>
    </div>
    <div class="grid4">
      <div class="pc">
        <div class="icn">₹</div>
        <div class="big">Every month</div>
          <h3>Endless subscriptions</h3>
        <p>You keep paying monthly or yearly. Stop paying and you lose access to your own records.</p>
      </div>
      <div class="pc">
        <div class="icn">⚙</div>
        <div class="big">Doesn't fit</div>
        <h3>Rigid templates</h3>
        <p>Your way of working is different, but the software forces its own steps on you.</p>
      </div>
      <div class="pc">
        <div class="icn">☰</div>
        <div class="big">Too heavy</div>
        <h3>Bloated features</h3>
        <p>Hundreds of buttons you never use make daily billing slow and confusing.</p>
      </div>
      <div class="pc">
        <div class="icn">🔒</div>
        <div class="big">Not yours</div>
        <h3>Data on their servers</h3>
        <p>Customer and sales records sit with a company you can't control or reach.</p>
      </div>
    </div>
  </div>
</section>

<!-- ============ WITH US / WITHOUT US ============ -->
<section id="compare" class="compare">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow">Side by Side</span>
      <h2>With Dhanvishta vs without us</h2>
      <p>Same business. Same day. Very different experience.</p>
    </div>

    <div class="compare-wrap">
      <div class="col col-bad">
        <h3><span class="pill-i">✕</span> Without Us</h3>
        <ul>
          <li><span class="tick">✕</span><span>You pay <b>₹500–₹3,000 every month</b> for software you don't own.</span></li>
          <li><span class="tick">✕</span><span>Your invoices don't match your shop's format — you adjust your work to the software.</span></li>
          <li><span class="tick">✕</span><span>Your sales and customer data live on <b>someone else's server</b>.</span></li>
          <li><span class="tick">✕</span><span>Simple tasks take 5–10 clicks because of unnecessary features.</span></li>
          <li><span class="tick">✕</span><span>If you stop paying, your software stops working — <b>instantly</b>.</span></li>
          <li><span class="tick">✕</span><span>Support is slow, generic and scripted. Nobody knows your business.</span></li>
        </ul>
      </div>
      <div class="col col-good">
        <h3><span class="pill-i">✓</span> With Us</h3>
        <ul>
          <li><span class="tick">✓</span><span>You pay <b>one time from ₹1,999</b> and the software is yours for life.</span></li>
          <li><span class="tick">✓</span><span>Built around <b>your invoice format</b>, your reports, your exact workflow.</span></li>
          <li><span class="tick">✓</span><span>Your data is stored <b>locally on your Windows PC</b>, fully under your control.</span></li>
          <li><span class="tick">✓</span><span>Only the features you need — daily billing done in <b>2–3 clicks</b>.</span></li>
          <li><span class="tick">✓</span><span>It runs offline. No renewals, no expiry, no surprise lockouts.</span></li>
          <li><span class="tick">✓</span><span>Direct WhatsApp support from the person who built it.</span></li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ============ EXAMPLES ============ -->
<section id="work" class="work">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow">Real Examples</span>
      <h2>Four types of software we build for shops like yours</h2>
      <p>Real screens. Real data. Each one is shaped around the client's own business.</p>
    </div>

    <div class="grid2">

      <!-- 1. BILLING -->
      <div class="shot">
        <div class="shot-img">
          <img src="https://images.unsplash.com/photo-1556740738-b6a63e27c4df?auto=format&fit=crop&w=1000&q=80" alt="Billing and invoicing software for shops" loading="lazy" />
        </div>
        <div class="shot-body">
          <h3>Billing &amp; Invoicing <span class="badge-n">01</span></h3>
          <p>Fast GST invoices in your own format, with payment tracking and daily sales totals.</p>
          <div class="mockup">
            <div class="row"><b>Invoice #INV-1042</b><span class="pill a">Due</span></div>
            <div class="row"><span>Sharma Traders</span><span class="muted">16 Oct 2026</span></div>
            <div class="row"><span>Basmati Rice 25kg × 4</span><span>₹6,800</span></div>
            <div class="row"><span>Refined Oil 15L × 2</span><span>₹3,600</span></div>
            <div class="row"><span>GST 5%</span><span>₹520</span></div>
            <div class="total"><span>Total</span><span>₹10,920</span></div>
          </div>
        </div>
      </div>

      <!-- 2. ACCOUNTING -->
      <div class="shot">
        <div class="shot-img">
          <img src="https://images.unsplash.com/photo-1554224155-6726b3ff858f?auto=format&fit=crop&w=1000&q=80" alt="Accounting and bookkeeping software for small business" loading="lazy" />
        </div>
        <div class="shot-body">
          <h3>Accounting &amp; Books <span class="badge-n">02</span></h3>
          <p>Ledgers, Profit &amp; Loss, GST summaries and receivables — all in plain language you understand.</p>
          <div class="mockup">
            <div class="row"><b>Profit &amp; Loss — Oct 2026</b><span class="pill b">Auto</span></div>
            <div class="row"><span>Sales revenue</span><span style="color:var(--green)">+ ₹4,82,000</span></div>
            <div class="row"><span>Purchase cost</span><span style="color:var(--red)">− ₹3,10,400</span></div>
            <div class="row"><span>Expenses</span><span style="color:var(--red)">− ₹48,200</span></div>
            <div class="row"><span>GST payable</span><span class="muted">₹18,640</span></div>
            <div class="total"><span>Net profit</span><span>₹1,23,400</span></div>
          </div>
        </div>
      </div>

      <!-- 3. INVENTORY -->
      <div class="shot">
        <div class="shot-img">
          <img src="https://images.unsplash.com/photo-1553413077-190dd305871c?auto=format&fit=crop&w=1000&q=80" alt="Inventory management software with stock tracking" loading="lazy" />
        </div>
        <div class="shot-body">
          <h3>Inventory &amp; Stock <span class="badge-n">03</span></h3>
          <p>Track stock by brand and product. Get low-stock alerts before you run out of bestsellers.</p>
          <div class="mockup">
            <div class="row"><span>Brand A – Shirts</span><div class="stock"><span style="width:75%"></span></div><span class="pill">150</span></div>
            <div class="row"><span>Brand B – Jeans</span><div class="stock"><span style="width:30%;background:var(--amber)"></span></div><span class="pill a">32</span></div>
            <div class="row"><span>Brand C – Jackets</span><div class="stock"><span style="width:6%;background:var(--red)"></span></div><span class="pill r">3</span></div>
            <div class="row"><span>Reorder suggestion</span><b style="color:var(--blue)">4 items</b></div>
          </div>
        </div>
      </div>

      <!-- 4. CRM -->
      <div class="shot">
        <div class="shot-img">
          <img src="https://images.unsplash.com/photo-1521737604893-d14cc237f11d?auto=format&fit=crop&w=1000&q=80" alt="CRM software for customer follow-ups and payments" loading="lazy" />
        </div>
        <div class="shot-body">
          <h3>CRM &amp; Follow-ups <span class="badge-n">04</span></h3>
          <p>Customer details, follow-up reminders and pending payments organised in one screen.</p>
          <div class="mockup">
            <div class="row"><span style="display:flex;gap:8px;align-items:center"><span class="av" style="background:#0ea5e9">R</span>Rajesh Kumar</span><span class="pill a">Call today</span></div>
            <div class="row"><span style="display:flex;gap:8px;align-items:center"><span class="av" style="background:#f59e0b">A</span>Anita Verma</span><span class="pill">Paid</span></div>
            <div class="row"><span style="display:flex;gap:8px;align-items:center"><span class="av" style="background:#10b981">M</span>Mehta &amp; Sons</span><span class="pill r">₹12,500 pending</span></div>
            <div class="row"><span>Follow-ups due today</span><b style="color:var(--blue)">7</b></div>
          </div>
        </div>
      </div>

      <!-- 5. AUTOMATION -->
      <div class="shot">
        <div class="shot-img">
          <img src="https://images.unsplash.com/photo-1551434678-e076c223a692?auto=format&fit=crop&w=1000&q=80" alt="Automation tools replacing repeated manual work" loading="lazy" />
        </div>
        <div class="shot-body">
          <h3>Automation Tools <span class="badge-n">05</span></h3>
          <p>Small utilities that replace hours of repeated work — Excel import, report generation, backups.</p>
          <div class="mockup">
            <div class="flow">
              <div class="file">📄<b>sales.xlsx</b><small>2,400 rows</small></div>
              <span class="go">→</span>
              <div class="file" style="border-color:var(--green);border-style:solid">✅<b>Report ready</b><small>in 3 seconds</small></div>
            </div>
            <div class="prog"><span></span></div>
          </div>
        </div>
      </div>

      <!-- 6. ANYTHING CUSTOM -->
      <div class="shot">
        <div class="shot-img">
          <img src="https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?auto=format&fit=crop&w=1000&q=80" alt="Custom Windows software built to match a business workflow" loading="lazy" />
        </div>
        <div class="shot-body">
          <h3>Or anything you need <span class="badge-n">06</span></h3>
          <p>If your business has a repeated routine that wastes hours, we can build a small tool for it.</p>
          <div class="mockup">
            <div class="row"><span>Tell us your daily task</span><span class="pill b">Reply in 1 hr</span></div>
            <div class="row"><span>Get a fixed quote</span><span class="pill">Clear pricing</span></div>
            <div class="row"><span>Delivered on your Windows PC</span><span class="pill">One-time fee</span></div>
            <div class="total"><span>Lifetime ownership</span><span>✓ Yours</span></div>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- ============ PRICING ============ -->
<section id="pricing">
  <div class="wrap">
    <div class="head">
      <span class="eyebrow">Pricing</span>
      <h2>Pay once. Own it for life.</h2>
      <p>No subscriptions, no renewals, no surprise charges.</p>
    </div>
    <div class="price-box">
      <div class="price-l">
        <p>Custom software starting at</p>
        <div class="amount">₹1,999<small>one-time</small></div>
        <p>The final price depends on what you need built. Share your workflow and get a clear quote before we start.</p>
        <a class="btn btn-primary" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20please%20share%20a%20quote." target="_blank" rel="noopener">Ask for your quote</a>
      </div>
      <div class="price-r">
        <h3>What you get</h3>
        <ul>
          <li>One-time development fee — no monthly or yearly charges, ever</li>
          <li>Complete data ownership: your records stay with you</li>
          <li>Runs locally on your Windows PC, not on someone else's servers</li>
          <li>Built around your workflow, with no rigid templates</li>
          <li>Lightweight software without bloat — opens fast, easy to learn</li>
          <li>Direct WhatsApp support from the developer who built it</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- ============ FINAL CTA ============ -->
<div id="contact" class="final">
  <div class="wrap">
    <h2>Tell us what slows your business down</h2>
    <p>Send a message about your billing, stock, accounting or paperwork routine. We'll reply with how we'd build it and what it costs.</p>
    <div class="cta-row">
      <a class="btn btn-wa" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20need%20custom%20software%20for%20my%20business." target="_blank" rel="noopener">WhatsApp +91 95556 13854</a>
      <a class="btn btn-ghost" href="tel:+919555613854">Call now</a>
    </div>
  </div>
</div>

</main>

<footer>
  <div class="wrap foot">
    <a href="#top" class="logo">
  <span class="logo-mark">
    <img src="Logo.png" alt="Dhanvishta" class="logo-img"
         onerror="this.style.display='none';this.parentElement.classList.add('no-img')" />
    <span class="mark" aria-hidden="true">D</span>
  </span>
  <span class="logo-text">Dhanvishta</span>
</a>
    <div>
      <a href="https://wa.me/919555613854" target="_blank" rel="noopener">WhatsApp: +91 95556 13854</a> ·
      <a href="mailto:abhiks239@gmail.com">abhiks239@gmail.com</a>
    </div>
    <div>© 2026 Dhanvishta · Your Business Simplified</div>
  </div>
</footer>

</body>
</html>
