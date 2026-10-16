<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Dhanvishta | Custom Windows software, one-time fee from ₹1,999</title>
<meta name="description" content="Custom billing, CRM, inventory and automation software for Windows. One-time fee from ₹1,999. No subscriptions. You own your data.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#0b1220; --bg2:#0f1729; --card:#131d33; --line:#22304f;
  --text:#e6ecf7; --muted:#93a1bb; --blue:#3b82f6; --sky:#38bdf8; --green:#34d399; --red:#f87171;
  --max:1120px;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth;scroll-padding-top:76px}
body{font-family:'Inter',system-ui,-apple-system,'Segoe UI',Roboto,sans-serif;background:var(--bg);color:var(--text);line-height:1.6;-webkit-font-smoothing:antialiased}
a{color:inherit;text-decoration:none}
.wrap{max-width:var(--max);margin:0 auto;padding:0 20px}
:focus-visible{outline:2px solid var(--sky);outline-offset:3px;border-radius:6px}

/* header */
header{position:sticky;top:0;z-index:50;background:rgba(11,18,32,.85);backdrop-filter:blur(12px);border-bottom:1px solid var(--line)}
.nav{display:flex;align-items:center;justify-content:space-between;height:64px}
.logo{display:flex;align-items:center;gap:10px;font-weight:800;font-size:1.15rem;letter-spacing:-.01em}
.logo-mark{width:32px;height:32px;border-radius:9px;background:linear-gradient(135deg,var(--blue),var(--sky));display:grid;place-items:center;color:#06101f;font-weight:800}
.nav ul{display:flex;gap:28px;list-style:none}
.nav ul a{color:var(--muted);font-size:.93rem;font-weight:500;transition:color .2s}
.nav ul a:hover{color:var(--text)}
.btn{display:inline-flex;align-items:center;justify-content:center;gap:8px;padding:12px 22px;border-radius:10px;font-weight:600;font-size:.95rem;border:1px solid transparent;cursor:pointer;transition:transform .2s,box-shadow .2s,background .2s,border-color .2s}
.btn-primary{background:var(--blue);color:#fff;box-shadow:0 6px 24px rgba(59,130,246,.3)}
.btn-primary:hover{background:#2f73e6;transform:translateY(-2px);box-shadow:0 10px 30px rgba(59,130,246,.45)}
.btn-ghost{border-color:var(--line);color:var(--text);background:transparent}
.btn-ghost:hover{border-color:var(--sky);background:rgba(56,189,248,.07);transform:translateY(-2px)}
.btn-wa{background:#22c55e;color:#04210f}
.btn-wa:hover{background:#4ade80;transform:translateY(-2px)}
.nav .btn{padding:9px 16px;font-size:.88rem}

/* hero */
.hero{padding:72px 0 56px;background:radial-gradient(ellipse 70% 55% at 75% 0%,rgba(59,130,246,.18),transparent 70%)}
.hero-grid{display:grid;grid-template-columns:1.05fr 1fr;gap:48px;align-items:center}
.tagline{display:inline-block;padding:5px 12px;border:1px solid var(--line);border-radius:99px;color:var(--sky);font-size:.85rem;font-weight:500;margin-bottom:20px;background:rgba(56,189,248,.06)}
h1{font-size:clamp(2.1rem,4.6vw,3.4rem);line-height:1.1;letter-spacing:-.03em;font-weight:800}
.lead{color:var(--muted);font-size:1.08rem;margin:20px 0 28px;max-width:30em}
.cta-row{display:flex;flex-wrap:wrap;gap:12px}
.vs{margin-top:34px;display:grid;grid-template-columns:1fr 1fr;border:1px solid var(--line);border-radius:14px;overflow:hidden;font-size:.9rem}
.vs div{padding:16px 18px}
.vs .old{background:var(--bg2);color:var(--muted)}
.vs .new{background:rgba(59,130,246,.08);border-left:1px solid var(--line)}
.vs h3{font-size:.95rem;margin-bottom:8px;color:var(--text)}
.vs ul{list-style:none;display:grid;gap:5px}
.vs .old li::before{content:"✕  ";color:var(--red);font-weight:700}
.vs .new li::before{content:"✓  ";color:var(--green);font-weight:700}

/* dashboard mockup */
.mock{background:var(--card);border:1px solid var(--line);border-radius:16px;box-shadow:0 30px 80px rgba(0,0,0,.5),0 0 0 1px rgba(59,130,246,.08);overflow:hidden;font-size:.78rem}
.bar{display:flex;align-items:center;gap:6px;padding:10px 14px;background:var(--bg2);border-bottom:1px solid var(--line);color:var(--muted)}
.bar i{width:10px;height:10px;border-radius:50%;background:#2b3a5c;display:block}
.bar span{margin-left:10px;font-size:.75rem}
.app{display:grid;grid-template-columns:96px 1fr}
.side{background:var(--bg2);border-right:1px solid var(--line);padding:12px 8px;display:grid;gap:4px;align-content:start}
.side div{padding:7px 10px;border-radius:7px;color:var(--muted)}
.side .on{background:rgba(59,130,246,.18);color:var(--text);font-weight:600}
.main{padding:14px}
.stats{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
.stat{background:var(--bg2);border:1px solid var(--line);border-radius:9px;padding:9px 10px}
.stat small{color:var(--muted);display:block}
.stat b{font-size:1.05rem}
.chart{margin:10px 0;background:var(--bg2);border:1px solid var(--line);border-radius:9px;padding:10px 12px;height:96px;display:flex;align-items:flex-end;gap:7px}
.chart span{flex:1;background:linear-gradient(to top,var(--blue),var(--sky));border-radius:4px 4px 0 0;opacity:.9}
table{width:100%;border-collapse:collapse}
th,td{text-align:left;padding:6px 4px;border-bottom:1px solid var(--line)}
th{color:var(--muted);font-weight:500}
.paid{color:var(--green)} .due{color:#fbbf24}

/* sections */
section{padding:84px 0}
.head{max-width:620px;margin-bottom:44px}
h2{font-size:clamp(1.7rem,3.2vw,2.4rem);letter-spacing:-.025em;line-height:1.15;font-weight:800}
.head p{color:var(--muted);margin-top:12px}
.services{background:var(--bg2);border-block:1px solid var(--line)}
.grid4{display:grid;grid-template-columns:repeat(4,1fr);gap:18px}
.svc{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:26px 22px;transition:transform .25s,border-color .25s,box-shadow .25s}
.svc:hover{transform:translateY(-5px);border-color:var(--blue);box-shadow:0 14px 40px rgba(59,130,246,.15)}
.ico{width:44px;height:44px;border-radius:11px;background:rgba(59,130,246,.15);color:var(--sky);display:grid;place-items:center;margin-bottom:16px}
.ico svg{width:22px;height:22px;stroke:currentColor;fill:none;stroke-width:1.8;stroke-linecap:round;stroke-linejoin:round}
.svc h3{font-size:1.1rem;margin-bottom:8px}
.svc p{color:var(--muted);font-size:.92rem}

/* pricing */
.price-box{display:grid;grid-template-columns:1fr 1.1fr;gap:0;background:linear-gradient(135deg,#14213f,#0f1a33);border:1px solid #2a4276;border-radius:20px;overflow:hidden;box-shadow:0 30px 80px rgba(59,130,246,.15)}
.price-l{padding:44px 40px;border-right:1px solid #2a4276}
.price-l p{color:var(--muted)}
.amount{font-size:clamp(3rem,7vw,4.6rem);font-weight:800;letter-spacing:-.04em;line-height:1;margin:12px 0 6px}
.amount small{font-size:1.1rem;font-weight:600;color:var(--sky);letter-spacing:0;margin-left:6px}
.price-l .btn{margin-top:26px}
.price-r{padding:44px 40px}
.price-r h3{margin-bottom:16px;font-size:1.1rem}
.price-r ul{list-style:none;display:grid;gap:13px}
.price-r li{display:flex;gap:12px;color:#cdd7ea}
.price-r li::before{content:"✓";color:var(--green);font-weight:800}
.note{margin-top:20px;font-size:.85rem;color:var(--muted)}

/* final cta + footer */
.final{text-align:center;padding:84px 0;background:radial-gradient(ellipse 60% 80% at 50% 100%,rgba(59,130,246,.2),transparent 70%)}
.final p{color:var(--muted);margin:14px auto 28px;max-width:34em}
.final .cta-row{justify-content:center}
footer{border-top:1px solid var(--line);padding:32px 0;color:var(--muted);font-size:.9rem}
.foot{display:flex;flex-wrap:wrap;gap:16px;justify-content:space-between;align-items:center}
.foot a:hover{color:var(--text)}

@media (max-width:960px){
  .grid4{grid-template-columns:repeat(2,1fr)}
  .hero-grid,.price-box{grid-template-columns:1fr}
  .price-l{border-right:0;border-bottom:1px solid #2a4276}
}
@media (max-width:640px){
  .nav ul{display:none}
  .hero{padding-top:44px}
  .grid4{grid-template-columns:1fr}
  .vs{grid-template-columns:1fr}
  .vs .new{border-left:0;border-top:1px solid var(--line)}
  .price-l,.price-r{padding:30px 24px}
  .app{grid-template-columns:1fr}.side{display:none}
  section{padding:60px 0}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>

<header>
  <div class="wrap nav">
    <a href="#top" class="logo" aria-label="Dhanvishta home"><span class="logo-mark">D</span>Dhanvishta</a>
    <ul>
      <li><a href="#services">Services</a></li>
      <li><a href="#pricing">Pricing</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <a class="btn btn-wa" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20need%20custom%20software%20for%20my%20business." target="_blank" rel="noopener">WhatsApp us</a>
  </div>
</header>

<main id="top">
<div class="hero">
  <div class="wrap hero-grid">
    <div>
      <span class="tagline">Your Business Simplified</span>
      <h1>Stop renting generic software. Own software built for your business.</h1>
      <p class="lead">Dhanvishta builds custom Windows billing, CRM, inventory and automation tools around the way you already work. Pay once. Keep your data on your own computer.</p>
      <div class="cta-row">
        <a class="btn btn-primary" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20want%20a%20quote%20for%20custom%20software." target="_blank" rel="noopener">Get a free quote on WhatsApp</a>
        <a class="btn btn-ghost" href="#pricing">See pricing</a>
      </div>
      <div class="vs">
        <div class="old">
          <h3>Standard competitors</h3>
          <ul><li>Monthly or yearly fees</li><li>Fixed templates</li><li>Bloated, hard to learn</li></ul>
        </div>
        <div class="new">
          <h3>Bespoke Dhanvishta</h3>
          <ul><li>One-time fee</li><li>Built to your workflow</li><li>Light, fast, your data</li></ul>
        </div>
      </div>
    </div>

    <div class="mock" role="img" aria-label="Sample dashboard of a custom billing application">
      <div class="bar"><i></i><i></i><i></i><span>Your Business – Billing</span></div>
      <div class="app">
        <div class="side"><div class="on">Dashboard</div><div>Billing</div><div>Stock</div><div>Customers</div><div>Reports</div></div>
        <div class="main">
          <div class="stats">
            <div class="stat"><small>Today's sales</small><b>₹24,580</b></div>
            <div class="stat"><small>Pending</small><b>₹8,200</b></div>
            <div class="stat"><small>Low stock</small><b>6 items</b></div>
          </div>
          <div class="chart"><span style="height:35%"></span><span style="height:55%"></span><span style="height:42%"></span><span style="height:70%"></span><span style="height:60%"></span><span style="height:88%"></span><span style="height:74%"></span></div>
          <table>
            <tr><th>Invoice</th><th>Customer</th><th>Amount</th><th>Status</th></tr>
            <tr><td>#1042</td><td>Sharma Traders</td><td>₹4,200</td><td class="paid">Paid</td></tr>
            <tr><td>#1043</td><td>Gupta Stores</td><td>₹8,200</td><td class="due">Due</td></tr>
            <tr><td>#1044</td><td>Walk-in</td><td>₹1,150</td><td class="paid">Paid</td></tr>
          </table>
        </div>
      </div>
    </div>
  </div>
</div>

<section id="services" class="services">
  <div class="wrap">
    <div class="head">
      <h2>Software made for how you actually work</h2>
      <p>Tell us your process. We build only the screens and reports you need, nothing extra.</p>
    </div>
    <div class="grid4">
      <article class="svc">
        <div class="ico"><svg viewBox="0 0 24 24"><path d="M6 3h12v18l-3-2-3 2-3-2-3 2z"/><path d="M9 8h6M9 12h6"/></svg></div>
        <h3>Billing software</h3>
        <p>GST-ready invoices, quotations and payment tracking, printed in your own format.</p>
      </article>
      <article class="svc">
        <div class="ico"><svg viewBox="0 0 24 24"><circle cx="9" cy="8" r="3.2"/><path d="M3 20c0-3.3 2.7-6 6-6s6 2.7 6 6"/><path d="M16 5.5a3 3 0 0 1 0 5.5M18 14.5c1.8.8 3 2.6 3 5.5"/></svg></div>
        <h3>CRM systems</h3>
        <p>Keep customer details, follow-ups and history in one place, organised your way.</p>
      </article>
      <article class="svc">
        <div class="ico"><svg viewBox="0 0 24 24"><path d="M3 8l9-5 9 5v8l-9 5-9-5z"/><path d="M3 8l9 5 9-5M12 13v8"/></svg></div>
        <h3>Inventory management</h3>
        <p>Track stock, batches and low-stock alerts across products, brands and locations.</p>
      </article>
      <article class="svc">
        <div class="ico"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="3"/><path d="M12 2v3M12 19v3M2 12h3M19 12h3M4.9 4.9l2.1 2.1M17 17l2.1 2.1M19.1 4.9L17 7M7 17l-2.1 2.1"/></svg></div>
        <h3>Automation tools</h3>
        <p>Small utilities that replace repetitive work: Excel imports and exports, report generation, data cleanup.</p>
      </article>
    </div>
  </div>
</section>

<section id="pricing">
  <div class="wrap">
    <div class="head">
      <h2>Pay once. Own it for life.</h2>
      <p>No subscriptions, no renewal reminders, no surprise charges.</p>
    </div>
    <div class="price-box">
      <div class="price-l">
        <p>Custom software starting at</p>
        <div class="amount">₹1,999/-<small>one-time</small></div>
        <p>Final price depends on what you need built. Share your workflow and get a clear quote before we start.</p>
        <a class="btn btn-primary" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20please%20share%20a%20quote." target="_blank" rel="noopener">Ask for your quote</a>
      </div>
      <div class="price-r">
        <h3>What you get</h3>
        <ul>
          <li>A single one-time development fee, with no monthly or yearly charges</li>
          <li>Complete data ownership: your records stay with you</li>
          <li>Local control: runs on your Windows PC, without depending on someone else's servers</li>
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
    <p>Send a message describing your billing, stock or paperwork routine. We'll reply with how we'd build it and what it costs.</p>
    <div class="cta-row">
      <a class="btn btn-wa" href="https://wa.me/919555613854?text=Hi%20Dhanvishta%2C%20I%20need%20custom%20software%20for%20my%20business." target="_blank" rel="noopener">WhatsApp +91 95556 13854</a>
      <a class="btn btn-ghost" href="tel:+919555613854">Call now</a>
    </div>
  </div>
</div>
</main>

<footer>
  <div class="wrap foot">
    <div><strong style="color:var(--text)">Dhanvishta</strong> · Your Business Simplified</div>
    <div><a href="https://wa.me/919555613854" target="_blank" rel="noopener">WhatsApp: +91 95556 13854</a> · <a href="mailto:abhiks239@gmail.com">abhiks239@gmail.com</a></div>
    <div>© 2026 Dhanvishta</div>
  </div>
</footer>

</body>
</html>
