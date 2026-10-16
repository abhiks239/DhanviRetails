<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Dhanvishta | Custom Windows software, one-time fee from ₹1,999</title>
<meta name="description" content="Custom billing, CRM, inventory and automation software for Windows. One-time fee from ₹1,999. No subscriptions. You own your data.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Sora:wght@600;700;800&display=swap" rel="stylesheet">
<style>
:root{--bg:#070d1a;--bg2:#0c1426;--card:#111b30;--line:#1f2d4a;--text:#e8eefb;--muted:#8fa0bf;--blue:#3b82f6;--sky:#38bdf8;--amber:#fbbf24;--green:#34d399;--red:#f87171;--h:'Sora','Inter',system-ui,sans-serif}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:76px}
body{font-family:'Inter',system-ui,-apple-system,'Segoe UI',sans-serif;background:var(--bg);color:var(--text);line-height:1.6;-webkit-font-smoothing:antialiased;overflow-x:hidden}
a{color:inherit;text-decoration:none}
.wrap{max-width:1140px;margin:0 auto;padding:0 20px}
:focus-visible{outline:2px solid var(--sky);outline-offset:3px;border-radius:6px}
h1,h2,h3{font-family:var(--h)}

/* header + logo */
header{position:sticky;top:0;z-index:50;background:rgba(7,13,26,.85);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
.nav{display:flex;align-items:center;justify-content:space-between;height:68px}
.logo{display:flex;align-items:center;gap:10px;font-family:var(--h);font-weight:800;font-size:1.2rem}
.logo img{height:38px;width:auto;display:block}
.mark{display:none;width:36px;height:36px;border-radius:10px;background:linear-gradient(135deg,var(--blue),var(--sky));place-items:center;color:#041020;font-weight:800}
.nav ul{display:flex;gap:28px;list-style:none}
.nav ul a{color:var(--muted);font-size:.93rem;font-weight:500;transition:color .2s}
.nav ul a:hover{color:var(--text)}
.btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;padding:13px 24px;border-radius:11px;font-weight:600;font-size:.95rem;border:1px solid transparent;cursor:pointer;transition:transform .2s,box-shadow .2s,background .2s,border-color .2s}
.btn-primary{background:var(--blue);color:#fff;box-shadow:0 8px 28px rgba(59,130,246,.35)}
.btn-primary:hover{background:#2f73e6;transform:translateY(-2px)}
.btn-ghost{border-color:var(--line);background:transparent}
.btn-ghost:hover{border-color:var(--sky);background:rgba(56,189,248,.07);transform:translateY(-2px)}
.btn-wa{background:#22c55e;color:#04210f}
.btn-wa:hover{background:#4ade80;transform:translateY(-2px)}
.nav .btn{padding:9px 16px;font-size:.88rem}

/* hero */
.hero{position:relative;padding:76px 0 90px;background:radial-gradient(ellipse 60% 60% at 85% 10%,rgba(59,130,246,.28),transparent 70%),radial-gradient(ellipse 40% 40% at 0% 100%,rgba(251,191,36,.08),transparent 70%)}
.hero::before{content:"";position:absolute;inset:0;background-image:linear-gradient(var(--line) 1px,transparent 1px),linear-gradient(90deg,var(--line) 1px,transparent 1px);background-size:56px 56px;opacity:.28;mask-image:radial-gradient(ellipse at 70% 30%,#000,transparent 70%);-webkit-mask-image:radial-gradient(ellipse at 70% 30%,#000,transparent 70%)}
.hero-grid{position:relative;display:grid;grid-template-columns:1fr 1.05fr;gap:40px;align-items:center}
.tag{display:inline-block;padding:6px 14px;border:1px solid #2a4276;border-radius:99px;color:var(--sky);font-size:.85rem;font-weight:500;margin-bottom:22px;background:rgba(56,189,248,.07)}
h1{font-size:clamp(2.2rem,5vw,3.7rem);line-height:1.08;letter-spacing:-.035em;font-weight:800}
.lead{color:var(--muted);font-size:1.1rem;margin:22px 0 30px;max-width:30em}
.cta-row{display:flex;flex-wrap:wrap;gap:12px}
.proof{display:flex;flex-wrap:wrap;gap:22px;margin-top:30px;color:var(--muted);font-size:.9rem}
.proof b{color:var(--text)}

/* app windows (used as images) */
.win{background:var(--card);border:1px solid #2a3b5f;border-radius:14px;overflow:hidden;font-size:.74rem;box-shadow:0 24px 60px rgba(0,0,0,.5)}
.win .bar{display:flex;align-items:center;gap:6px;padding:9px 12px;background:var(--bg2);border-bottom:1px solid var(--line);color:var(--muted)}
.win .bar i{width:9px;height:9px;border-radius:50%;background:#2b3a5c}
.win .bar span{margin-left:8px}
.win .body{padding:12px}
.row{display:flex;justify-content:space-between;align-items:center;gap:8px;padding:6px 0;border-bottom:1px solid var(--line)}
.row:last-child{border:0}
.muted{color:var(--muted)}
.ok{color:var(--green)}.warn{color:var(--amber)}.bad{color:var(--red)}
.pill{padding:2px 8px;border-radius:99px;font-size:.68rem;font-weight:600;background:rgba(52,211,153,.15);color:var(--green)}
.pill.r{background:rgba(248,113,113,.15);color:var(--red)}
.pill.a{background:rgba(251,191,36,.15);color:var(--amber)}
.total{display:flex;justify-content:space-between;margin-top:8px;padding:9px 10px;border-radius:8px;background:rgba(59,130,246,.15);font-weight:700;font-size:.85rem}
.stock{height:6px;border-radius:9px;background:var(--line);width:70px;overflow:hidden}
.stock span{display:block;height:100%;background:var(--sky)}
.av{width:24px;height:24px;border-radius:50%;display:grid;place-items:center;font-weight:700;font-size:.68rem;color:#041020}
.collage{position:relative;height:430px}
.collage .win{position:absolute}
.c1{width:78%;top:0;right:0;transform:rotate(2deg)}
.c2{width:66%;bottom:0;left:0;transform:rotate(-3deg)}
.badge{position:absolute;right:6%;bottom:14%;background:var(--amber);color:#1a1200;font-family:var(--h);font-weight:800;padding:12px 18px;border-radius:14px;transform:rotate(4deg);box-shadow:0 14px 34px rgba(251,191,36,.3);line-height:1.2;text-align:center}
.badge small{display:block;font-size:.72rem;font-weight:600}

/* sections */
section{padding:88px 0}
.head{max-width:640px;margin-bottom:44px}
h2{font-size:clamp(1.8rem,3.4vw,2.6rem);letter-spacing:-.03em;line-height:1.12;font-weight:800}
.head p{color:var(--muted);margin-top:12px}
.problem{background:var(--bg2);border-block:1px solid var(--line)}
.grid4{display:grid;grid-template-columns:repeat(4,1fr);gap:16px}
.pc{background:var(--card);border:1px solid var(--line);border-left:3px solid var(--red);border-radius:14px;padding:24px 20px}
.pc .big{font-family:var(--h);font-weight:800;font-size:1.5rem;color:var(--red);margin-bottom:8px}
.pc h3{font-size:1.02rem;margin-bottom:6px}
.pc p{color:var(--muted);font-size:.9rem}

/* solution */
.fix{display:grid;gap:14px}
.fixrow{display:grid;grid-template-columns:1fr 40px 1.3fr;align-items:center;gap:14px}
.fixrow>div{padding:18px 22px;border-radius:14px}
.f-prob{background:rgba(248,113,113,.07);border:1px solid rgba(248,113,113,.25);color:#f5b5b5;font-weight:500}
.f-sol{background:rgba(52,211,153,.07);border:1px solid rgba(52,211,153,.3)}
.f-sol b{display:block;font-family:var(--h);margin-bottom:2px}
.f-sol span{color:var(--muted);font-size:.9rem}
.fixrow .arr{padding:0;text-align:center;color:var(--sky);font-size:1.4rem;font-weight:700}

/* showcase */
.work{background:var(--bg2);border-block:1px solid var(--line)}
.grid2{display:grid;grid-template-columns:repeat(2,1fr);gap:28px}
.shot .win{margin-bottom:16px;transition:transform .3s,box-shadow .3s}
.shot:hover .win{transform:translateY(-6px);box-shadow:0 30px 70px rgba(59,130,246,.25)}
.shot h3{font-size:1.15rem;margin-bottom:4px}
.shot p{color:var(--muted);font-size:.93rem}
.flow{display:flex;align-items:center;gap:12px;justify-content:center;padding:14px 0}
.file{padding:14px 12px;border:1px dashed #3b5384;border-radius:10px;text-align:center;line-height:1.3}
.flow .go{color:var(--sky);font-size:1.3rem;font-weight:700}
.prog{height:6px;border-radius:9px;background:var(--line);margin-top:8px;overflow:hidden}
.prog span{display:block;height:100%;width:100%;background:var(--green)}

/* pricing */
.price-box{display:grid;grid-template-columns:1fr 1.1fr;background:linear-gradient(135deg,#15244a,#0d1730);border:1px solid #2f4a82;border-radius:22px;overflow:hidden;box-shadow:0 30px 90px rgba(59,130,246,.18)}
.price-l{padding:46px 40px;border-right:1px solid #2f4a82}
.price-l p{color:var(--muted)}
.amount{font-family:var(--h);font-size:clamp(3rem,7vw,4.6rem);font-weight:800;letter-spacing:-.04em;line-height:1;margin:12px 0 8px;color:var(--amber)}
.amount small{font-size:1.05rem;font-weight:600;color:var(--sky);letter-spacing:0;margin-left:6px}
.price-l .btn{margin-top:26px}
.price-r{padding:46px 40px}
.price-r h3{margin-bottom:16px}
.price-r ul{list-style:none;display:grid;gap:13px}
.price-r li{display:flex;gap:12px;color:#cdd8ee}
.price-r li::before{content:"✓";color:var(--green);font-weight:800}

.final{text-align:center;padding:90px 0;background:radial-gradient(ellipse 60% 80% at 50% 100%,rgba(59,130,246,.24),transparent 70%)}
.final p{color:var(--muted);margin:14px auto 28px;max-width:34em}
.final .cta-row{justify-content:center}
footer{border-top:1px solid var(--line);padding:32px 0;color:var(--muted);font-size:.9rem}
.foot{display:flex;flex-wrap:wrap;gap:16px;justify-content:space-between;align-items:center}
.foot a:hover{color:var(--text)}

@media (max-width:960px){
  .hero-grid,.price-box{grid-template-columns:1fr}
  .grid4{grid-template-columns:repeat(2,1fr)}
  .price-l{border-right:0;border-bottom:1px solid #2f4a82}
  .collage{height:400px;max-width:560px;margin:0 auto;width:100%}
}
@media (max-width:700px){
  .nav ul{display:none}
  .grid4,.grid2{grid-template-columns:1fr}
  .fixrow{grid-template-columns:1fr}.fixrow .arr{transform:rotate(90deg)}
  .collage{height:380px}.c1{width:88%}.c2{width:78%}
  section{padding:62px 0}.hero{padding-top:44px}
  .price-l,.price-r{padding:30px 24px}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>

<header>
  <div class="wrap nav">
    <a href="#top" class="logo" aria-label="Dhanvishta home">
      <img src="logo.png" alt="Dhanvishta logo" onerror="this.style.display='none';this.nextElementSibling.style.display='grid'">
      <span class="mark">D</span>Dhanvishta
    </a>
    <ul>
      <li><a href="#problem">Problem</a></li>
      <li><a href="#solution">Solution</a></li>
      <li><a href="#work">Our work</a></li>
      <li><a href="#pricing">Pricing</a></li>
    </ul>
    <a class="btn btn-wa" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20need%20custom%20software%20for%20my%20business." target="_blank" rel="noopener">WhatsApp us</a>
  </div>
</header>

<main id="top">
<div class="hero">
  <div class="wrap hero-grid">
    <div>
      <span class="tag">Your Business Simplified</span>
      <h1>Software made for your shop, not for everyone.</h1>
      <p class="lead">We build custom billing, inventory, CRM and automation software for Windows. Pay one time. Your data stays on your own computer.</p>
      <div class="cta-row">
        <a class="btn btn-primary" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20want%20a%20quote%20for%20custom%20software." target="_blank" rel="noopener">Get a free quote on WhatsApp</a>
        <a class="btn btn-ghost" href="#work">See what we build</a>
      </div>
      <div class="proof"><span><b>₹1,999</b> one-time start</span><span><b>0</b> monthly fees</span><span><b>100%</b> your data</span></div>
    </div>

    <div class="collage" role="img" aria-label="Sample billing and inventory software screens built by Dhanvishta">
      <div class="win c1">
        <div class="bar"><i></i><i></i><i></i><span>Billing – Invoice #1042</span></div>
        <div class="body">
          <div class="row"><span>Sharma Traders</span><span class="muted">16 Oct 2026</span></div>
          <div class="row"><span>Basmati Rice 25kg × 4</span><span>₹6,800</span></div>
          <div class="row"><span>Refined Oil 15L × 2</span><span>₹3,600</span></div>
          <div class="row"><span>GST 5%</span><span>₹520</span></div>
          <div class="total"><span>Total</span><span>₹10,920</span></div>
        </div>
      </div>
      <div class="win c2">
        <div class="bar"><i></i><i></i><i></i><span>Stock – Today</span></div>
        <div class="body">
          <div class="row"><span>Sugar 1kg</span><div class="stock"><span style="width:80%"></span></div><span class="pill">120</span></div>
          <div class="row"><span>Tea 250g</span><div class="stock"><span style="width:25%"></span></div><span class="pill a">18</span></div>
          <div class="row"><span>Soap Pack</span><div class="stock"><span style="width:8%"></span></div><span class="pill r">4</span></div>
        </div>
      </div>
      <div class="badge"><small>Starting at</small>₹1,999 one-time</div>
    </div>
  </div>
</div>

<section id="problem" class="problem">
  <div class="wrap">
    <div class="head">
      <h2>Does your software cause these problems?</h2>
      <p>Most small businesses are stuck with tools that were never made for them.</p>
    </div>
    <div class="grid4">
      <div class="pc"><div class="big">Every month</div><h3>Endless subscriptions</h3><p>You keep paying monthly or yearly. Stop paying and you lose access.</p></div>
      <div class="pc"><div class="big">Doesn't fit</div><h3>Rigid templates</h3><p>Your way of working is different, but the software forces its own way.</p></div>
      <div class="pc"><div class="big">Too heavy</div><h3>Bloated features</h3><p>Hundreds of buttons you never use make daily billing slow and confusing.</p></div>
      <div class="pc"><div class="big">Not yours</div><h3>Your data on their server</h3><p>Customer and sales records sit with a company you can't control.</p></div>
    </div>
  </div>
</section>

<section id="solution">
  <div class="wrap">
    <div class="head">
      <h2>What Dhanvishta does about it</h2>
      <p>For every problem, one clear fix.</p>
    </div>
    <div class="fix">
      <div class="fixrow"><div class="f-prob">Monthly and yearly subscriptions</div><div class="arr">→</div><div class="f-sol"><b>One-time fee, from ₹1,999</b><span>Pay once and the software is yours.</span></div></div>
      <div class="fixrow"><div class="f-prob">Rigid standard templates</div><div class="arr">→</div><div class="f-sol"><b>100% custom to your workflow</b><span>Your invoice format, your reports, your steps.</span></div></div>
      <div class="fixrow"><div class="f-prob">Bloated, confusing software</div><div class="arr">→</div><div class="f-sol"><b>Only what you need</b><span>A light Windows app that opens fast and is easy to learn.</span></div></div>
      <div class="fixrow"><div class="f-prob">Data locked on someone's server</div><div class="arr">→</div><div class="f-sol"><b>Data stays with you</b><span>Records are saved locally on your computer, under your control.</span></div></div>
    </div>
  </div>
</section>

<section id="work" class="work">
  <div class="wrap">
    <div class="head">
      <h2>This is the kind of software we build</h2>
      <p>Sample screens from our four main solutions. Each one is shaped around the client's own business.</p>
    </div>
    <div class="grid2">
      <div class="shot">
        <div class="win" role="img" aria-label="Billing software screen">
          <div class="bar"><i></i><i></i><i></i><span>Billing</span></div>
          <div class="body">
            <div class="row"><b>Invoice #1043</b><span class="pill a">Due</span></div>
            <div class="row"><span>Gupta Stores</span><span>₹8,200</span></div>
            <div class="row"><span>Sharma Traders</span><span>₹10,920</span></div>
            <div class="total"><span>Today's sales</span><span>₹24,580</span></div>
          </div>
        </div>
        <h3>Billing software</h3><p>Fast invoices in your own format, with payment tracking and daily sales totals.</p>
      </div>
      <div class="shot">
        <div class="win" role="img" aria-label="Inventory management screen">
          <div class="bar"><i></i><i></i><i></i><span>Inventory</span></div>
          <div class="body">
            <div class="row"><span>Brand A – Shirts</span><div class="stock"><span style="width:75%"></span></div><span class="pill">150</span></div>
            <div class="row"><span>Brand B – Jeans</span><div class="stock"><span style="width:30%"></span></div><span class="pill a">32</span></div>
            <div class="row"><span>Brand C – Jackets</span><div class="stock"><span style="width:6%"></span></div><span class="pill r">3</span></div>
          </div>
        </div>
        <h3>Inventory management</h3><p>See stock by brand and product, and get low-stock warnings before you run out.</p>
      </div>
      <div class="shot">
        <div class="win" role="img" aria-label="CRM customer list screen">
          <div class="bar"><i></i><i></i><i></i><span>Customers</span></div>
          <div class="body">
            <div class="row"><span style="display:flex;gap:8px;align-items:center"><span class="av" style="background:#38bdf8">R</span>Rajesh Kumar</span><span class="pill a">Call today</span></div>
            <div class="row"><span style="display:flex;gap:8px;align-items:center"><span class="av" style="background:#fbbf24">A</span>Anita Verma</span><span class="pill">Paid</span></div>
            <div class="row"><span style="display:flex;gap:8px;align-items:center"><span class="av" style="background:#34d399">M</span>Mehta &amp; Sons</span><span class="pill r">₹12,500 pending</span></div>
          </div>
        </div>
        <h3>CRM systems</h3><p>Customer details, follow-ups and pending payments organised in one place.</p>
      </div>
      <div class="shot">
        <div class="win" role="img" aria-label="Automation tool screen">
          <div class="bar"><i></i><i></i><i></i><span>Automation</span></div>
          <div class="body">
            <div class="flow">
              <div class="file">📄<br>sales.xlsx<br><span class="muted">2,400 rows</span></div>
              <span class="go">→</span>
              <div class="file" style="border-style:solid;border-color:var(--green)">✅<br>Report ready<br><span class="muted">in 3 seconds</span></div>
            </div>
            <div class="prog"><span></span></div>
          </div>
        </div>
        <h3>Automation tools</h3><p>Small utilities that replace hours of repeated work, like Excel import and export or report generation.</p>
      </div>
    </div>
  </div>
</section>

<section id="pricing">
  <div class="wrap">
    <div class="head">
      <h2>Pay once. Own it for life.</h2>
      <p>No subscriptions, no renewals, no surprise charges.</p>
    </div>
    <div class="price-box">
      <div class="price-l">
        <p>Custom software starting at</p>
        <div class="amount">₹1,999/-<small>one-time</small></div>
        <p>The final price depends on what you need built. Share your workflow and get a clear quote before we start.</p>
        <a class="btn btn-primary" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20please%20share%20a%20quote." target="_blank" rel="noopener">Ask for your quote</a>
      </div>
      <div class="price-r">
        <h3>What you get</h3>
        <ul>
          <li>A single one-time development fee, with no monthly or yearly charges</li>
          <li>Complete data ownership: your records stay with you</li>
          <li>Local control: runs on your Windows PC, not on someone else's servers</li>
          <li>Built around your workflow, with no rigid templates</li>
          <li>Lightweight software without bloat</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<div id="contact" class="final">
  <div class="wrap">
    <h2>Tell us what slows your business down</h2>
    <p>Send a message about your billing, stock or paperwork routine. We'll reply with how we'd build it and what it costs.</p>
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
      <img src="logo.png" alt="Dhanvishta logo" onerror="this.style.display='none';this.nextElementSibling.style.display='grid'">
      <span class="mark">D</span>Dhanvishta
    </a>
    <div><a href="https://wa.me/919555613854" target="_blank" rel="noopener">WhatsApp: +91 95556 13854</a> · <a href="mailto:abhiks239@gmail.com">abhiks239@gmail.com</a></div>
    <div>© 2026 Dhanvishta · Your Business Simplified</div>
  </div>
</footer>

</body>
</html>
