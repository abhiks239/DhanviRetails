```html
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dhanvista | Digital Architecture & Software Development by Abhishek Kumar</title>
  
  <!-- Google Fonts & Tailwind CDN -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- Lucide Icons -->
  <script src="https://unpkg.com/lucide@latest"></script>

  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            mono: ['"JetBrains Mono"', 'monospace'],
          },
          colors: {
            brand: {
              cyan: '#06b6d4',
              violet: '#8b5cf6',
              indigo: '#6366f1',
              dark: '#07090e',
              card: 'rgba(15, 23, 42, 0.75)',
              accent: '#3b82f6',
            }
          },
          animation: {
            'glow-pulse': 'glowPulse 6s ease-in-out infinite',
            'float-slow': 'float 8s ease-in-out infinite',
          },
          keyframes: {
            glowPulse: {
              '0%, 100%': { opacity: '0.4', transform: 'scale(1)' },
              '50%': { opacity: '0.8', transform: 'scale(1.08)' },
            },
            float: {
              '0%, 100%': { transform: 'translateY(0px)' },
              '50%': { transform: 'translateY(-12px)' },
            }
          }
        }
      }
    }
  </script>

  <style>
    /* Glassmorphism & Custom Accents */
    .glass-card {
      background: rgba(13, 20, 36, 0.65);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
      border: 1px solid rgba(255, 255, 255, 0.08);
    }
    .glass-card:hover {
      border-color: rgba(99, 102, 241, 0.35);
    }
    .neon-text-gradient {
      background: linear-gradient(135deg, #38bdf8 0%, #818cf8 50%, #c084fc 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    .badge-gradient {
      background: linear-gradient(90deg, rgba(56, 189, 248, 0.15), rgba(129, 140, 248, 0.15));
      border: 1px solid rgba(56, 189, 248, 0.3);
    }
    .grid-pattern {
      background-size: 40px 40px;
      background-image: 
        linear-gradient(to right, rgba(255, 255, 255, 0.03) 1px, transparent 1px),
        linear-gradient(to bottom, rgba(255, 255, 255, 0.03) 1px, transparent 1px);
    }
  </style>
</head>

<body class="bg-[#05070d] text-slate-100 font-sans selection:bg-cyan-500 selection:text-white antialiased overflow-x-hidden">

  <!-- Ambient background glow elements -->
  <div class="fixed inset-0 grid-pattern pointer-events-none z-0"></div>
  <div class="fixed top-[-10%] left-[-10%] w-[500px] h-[500px] bg-cyan-600/15 rounded-full blur-[140px] pointer-events-none animate-glow-pulse z-0"></div>
  <div class="fixed bottom-[-10%] right-[-10%] w-[600px] h-[600px] bg-indigo-600/15 rounded-full blur-[160px] pointer-events-none animate-glow-pulse z-0"></div>

  <!-- NAVIGATION BAR -->
  <header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300" id="navbar">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">
        <!-- Logo -->
        <a href="#home" class="flex items-center gap-3 group">
          <div class="relative w-11 h-11 rounded-xl bg-gradient-to-tr from-cyan-500 via-indigo-600 to-violet-500 p-[1.5px] shadow-lg shadow-cyan-500/25 group-hover:shadow-cyan-500/50 transition">
            <div class="w-full h-full bg-[#07090e] rounded-[10px] flex items-center justify-center overflow-hidden">
              <!-- Using your exact Logo.png with graceful fallback -->
              <img src="Logo.png" alt="Dhanvista Logo" class="w-full h-full object-contain p-1" onerror="this.onerror=null; this.parentElement.innerHTML='<span class=\'font-extrabold text-lg text-cyan-400\'>D</span>';">
            </div>
          </div>
          <div class="flex flex-col">
            <span class="text-xl font-bold tracking-tight text-white flex items-center gap-1.5">
              Dhanvista <span class="w-2 h-2 rounded-full bg-cyan-400 inline-block animate-ping"></span>
            </span>
            <span class="text-[10px] text-slate-400 font-mono tracking-wider">BY ABHISHEK KUMAR</span>
          </div>
        </a>

        <!-- Desktop Navigation Links -->
        <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-slate-300">
          <a href="#services" class="hover:text-cyan-400 transition">Services</a>
          <a href="#about" class="hover:text-cyan-400 transition">About Abhishek</a>
          <a href="#portfolio" class="hover:text-cyan-400 transition">Portfolio</a>
          <a href="#estimator" class="hover:text-cyan-400 transition flex items-center gap-1.5 text-cyan-400">
            <i data-lucide="calculator" class="w-4 h-4"></i> Cost Calculator
          </a>
          <a href="#contact" class="hover:text-cyan-400 transition">Contact</a>
        </nav>

        <!-- Right Quick Actions -->
        <div class="hidden sm:flex items-center gap-3">
          <a href="tel:+919555613854" class="px-3.5 py-2 rounded-xl text-xs font-semibold text-slate-300 bg-slate-900 border border-slate-700/80 hover:border-cyan-500/50 hover:text-white transition flex items-center gap-2">
            <i data-lucide="phone-call" class="w-3.5 h-3.5 text-cyan-400"></i>
            +91 9555613854
          </a>
          <a href="https://wa.me/919555613854?text=Hello%20Abhishek!%20I%20want%20to%20discuss%20a%20project%20for%20Dhanvista." target="_blank" rel="noopener noreferrer" class="px-4 py-2 rounded-xl text-xs font-bold text-black bg-gradient-to-r from-emerald-400 to-green-500 hover:brightness-110 transition flex items-center gap-2 shadow-md shadow-emerald-500/20">
            <i data-lucide="message-circle" class="w-4 h-4 fill-black"></i>
            WhatsApp
          </a>
        </div>

        <!-- Mobile Menu Trigger -->
        <button id="mobileMenuBtn" aria-label="Toggle Menu" class="md:hidden p-2 rounded-xl text-slate-300 bg-slate-900/80 border border-slate-800 focus:outline-none">
          <i data-lucide="menu" id="menuIcon" class="w-6 h-6"></i>
        </button>
      </div>
    </div>

    <!-- Mobile Dropdown Navigation -->
    <div id="mobileMenu" class="hidden md:hidden glass-card border-x-0 border-b border-t border-slate-800 px-6 py-5">
      <div class="flex flex-col gap-4 text-base font-medium">
        <a href="#services" class="mobile-nav-link text-slate-300 hover:text-cyan-400">Services</a>
        <a href="#about" class="mobile-nav-link text-slate-300 hover:text-cyan-400">About Abhishek</a>
        <a href="#portfolio" class="mobile-nav-link text-slate-300 hover:text-cyan-400">Portfolio & Demos</a>
        <a href="#estimator" class="mobile-nav-link text-cyan-400 font-semibold flex items-center gap-2">
          <i data-lucide="calculator" class="w-4 h-4"></i> Cost Calculator
        </a>
        <a href="#contact" class="mobile-nav-link text-slate-300 hover:text-cyan-400">Contact Us</a>
        <div class="pt-4 border-t border-slate-800 flex flex-col gap-2.5">
          <a href="tel:+919555613854" class="w-full py-2.5 rounded-xl text-sm font-semibold text-center text-slate-200 bg-slate-900 border border-slate-700 flex items-center justify-center gap-2">
            <i data-lucide="phone-call" class="w-4 h-4 text-cyan-400"></i> +91 9555613854
          </a>
          <a href="https://wa.me/919555613854?text=Hello%20Abhishek!%20I%20want%20to%20discuss%20a%20project." target="_blank" rel="noopener noreferrer" class="w-full py-2.5 rounded-xl text-sm font-bold text-center text-black bg-emerald-400 flex items-center justify-center gap-2">
            <i data-lucide="message-circle" class="w-4 h-4 fill-black"></i> Chat on WhatsApp
          </a>
        </div>
      </div>
    </div>
  </header>

  <main class="relative z-10 pt-24">
    <!-- HERO SECTION -->
    <section id="home" class="relative pt-12 pb-24 md:pt-20 md:pb-32 overflow-hidden">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid lg:grid-cols-12 gap-12 lg:gap-8 items-center">
          
          <div class="lg:col-span-7 text-left space-y-6">
            <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full badge-gradient text-cyan-300 text-xs font-semibold tracking-wide shadow-sm">
              <span class="flex h-2 w-2 relative">
                <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-cyan-400 opacity-75"></span>
                <span class="relative inline-flex rounded-full h-2 w-2 bg-cyan-500"></span>
              </span>
              Full-Stack Architect & Digital Builder
            </div>

            <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight leading-[1.15]">
              Turning complex business challenges into 
              <span class="neon-text-gradient block mt-1">elegant digital engines.</span>
            </h1>

            <p class="text-slate-400 text-base sm:text-lg max-w-2xl leading-relaxed">
              Welcome to <strong class="text-white font-semibold">Dhanvista</strong>. Led by <strong class="text-cyan-300 font-semibold">Abhishek Kumar</strong>, we engineer blazing-fast custom websites, robust enterprise software, and mission-critical Android & iOS applications tailored to your business growth.
            </p>

            <!-- Action buttons -->
            <div class="flex flex-wrap gap-4 pt-2">
              <a href="#estimator" class="px-6 py-3.5 rounded-xl font-bold text-white bg-gradient-to-r from-cyan-500 via-indigo-600 to-violet-600 hover:opacity-90 shadow-lg shadow-indigo-500/25 transition flex items-center gap-2 group">
                Estimate Your Project
                <i data-lucide="arrow-right" class="w-4 h-4 group-hover:translate-x-1 transition-transform"></i>
              </a>
              <a href="https://wa.me/919555613854?text=Hi%20Abhishek,%20I'd%20like%20to%20discuss%20a%20new%20project%20with%20Dhanvista." target="_blank" rel="noopener noreferrer" class="px-6 py-3.5 rounded-xl font-bold text-slate-200 bg-slate-900/90 border border-slate-700 hover:border-emerald-500/60 hover:text-white transition flex items-center gap-2.5">
                <i data-lucide="message-square" class="w-4 h-4 text-emerald-400"></i>
                WhatsApp Consultation
              </a>
            </div>

            <!-- Trust highlights -->
            <div class="pt-6 grid grid-cols-3 gap-4 border-t border-slate-800/80 max-w-lg">
              <div>
                <p class="text-2xl font-black text-white font-mono">100%</p>
                <p class="text-xs text-slate-400 mt-0.5">Custom Codebase</p>
              </div>
              <div>
                <p class="text-2xl font-black text-cyan-400 font-mono">Fast</p>
                <p class="text-xs text-slate-400 mt-0.5">Delivery & Support</p>
              </div>
              <div>
                <p class="text-2xl font-black text-emerald-400 font-mono">24/7</p>
                <p class="text-xs text-slate-400 mt-0.5">Direct Line Access</p>
              </div>
            </div>
          </div>

          <!-- Hero Visual & Video Showcase: Using your exact Video.mp4 file -->
          <div class="lg:col-span-5 relative">
            <div class="relative mx-auto max-w-md lg:max-w-none">
              <!-- Ambient Glow backdrop -->
              <div class="absolute -inset-1 rounded-2xl bg-gradient-to-r from-cyan-500 via-indigo-600 to-violet-600 opacity-40 blur-xl"></div>
              
              <div class="relative rounded-2xl border border-slate-700/80 bg-[#0d1322] shadow-2xl overflow-hidden">
                <!-- Video Terminal Header -->
                <div class="flex items-center justify-between px-4 py-3 bg-[#080d19] border-b border-slate-800">
                  <div class="flex items-center space-x-2">
                    <div class="w-3 h-3 rounded-full bg-rose-500/80"></div>
                    <div class="w-3 h-3 rounded-full bg-amber-500/80"></div>
                    <div class="w-3 h-3 rounded-full bg-emerald-500/80"></div>
                  </div>
                  <span class="text-xs font-mono text-cyan-300 flex items-center gap-1.5">
                    <i data-lucide="video" class="w-3.5 h-3.5 text-cyan-400"></i> Video.mp4 (Live Preview)
                  </span>
                  <div class="flex items-center gap-1.5 text-xs text-emerald-400 font-mono">
                    <span class="w-2 h-2 rounded-full bg-emerald-400 animate-ping"></span> Live
                  </div>
                </div>

                <!-- Video player container with Video.mp4 -->
                <div class="relative w-full aspect-video bg-black flex items-center justify-center overflow-hidden group">
                  <video id="heroVideo" class="w-full h-full object-cover" autoplay muted loop playsinline controls preload="metadata">
                    <source src="Video.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                  </video>
                  
                  <!-- Fallback message overlay if Video.mp4 is not yet loaded in folder -->
                  <div id="videoFallbackNotice" class="absolute inset-0 bg-slate-950/80 flex flex-col items-center justify-center p-6 text-center pointer-events-none hidden">
                    <i data-lucide="play-circle" class="w-12 h-12 text-cyan-400 mb-2"></i>
                    <p class="text-sm font-bold text-white">Video.mp4 Showcase</p>
                    <p class="text-xs text-slate-400 mt-1">Place Video.mp4 in the same directory as index.html to view video playback</p>
                  </div>
                </div>

                <!-- Interactive Video Prompt bar -->
                <div class="px-5 py-3.5 bg-[#0b101c] border-t border-slate-800 flex items-center justify-between text-xs">
                  <div class="flex items-center gap-2">
                    <img src="Logoo.png" alt="Logoo" class="w-5 h-5 object-contain rounded" onerror="this.style.display='none'">
                    <span class="text-slate-300 font-medium">Ready to build your digital product?</span>
                  </div>
                  <a href="tel:+919555613854" class="text-cyan-400 hover:text-cyan-300 font-semibold flex items-center gap-1">
                    Call Abhishek <i data-lucide="arrow-up-right" class="w-3.5 h-3.5"></i>
                  </a>
                </div>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- CORE SERVICES SECTION -->
    <section id="services" class="py-20 relative">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        
        <div class="text-center max-w-3xl mx-auto mb-16 space-y-3">
          <h2 class="text-xs font-mono tracking-widest text-cyan-400 uppercase">Engineered for Excellence</h2>
          <p class="text-3xl sm:text-4xl font-extrabold text-white">Custom Digital Services We Master</p>
          <p class="text-slate-400 text-sm sm:text-base">From frontend customer journeys to secure back-end cloud software, Dhanvista delivers end-to-end solutions.</p>
        </div>

        <div class="grid md:grid-cols-3 gap-8">
          
          <!-- Service 1: Website Development -->
          <div class="glass-card rounded-2xl p-7 transition-all duration-300 hover:-translate-y-1.5 flex flex-col justify-between group">
            <div>
              <div class="w-14 h-14 rounded-xl bg-cyan-500/10 border border-cyan-500/20 flex items-center justify-center text-cyan-400 mb-6 group-hover:scale-110 group-hover:bg-cyan-500/20 transition">
                <i data-lucide="globe" class="w-7 h-7"></i>
              </div>
              <h3 class="text-xl font-bold text-white mb-2.5">Website Development</h3>
              <p class="text-slate-400 text-sm leading-relaxed mb-6">
                Modern, lightning-fast, and responsive websites designed for high conversions. E-commerce platforms, SaaS landing pages, and interactive company portals.
              </p>
              
              <div class="space-y-2 mb-6 text-xs text-slate-300">
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-cyan-400"></i> Responsive UI/UX Design
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-cyan-400"></i> Next.js / React / Tailwind Speed
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-cyan-400"></i> SEO & Performance Optimized (95+ score)
                </div>
              </div>
            </div>

            <div class="pt-4 border-t border-slate-800/80 flex items-center justify-between">
              <span class="text-xs font-mono text-cyan-400 font-semibold">Websites & E-Com</span>
              <a href="#estimator" class="text-xs text-slate-300 hover:text-white flex items-center gap-1 font-medium">
                Calculate Cost <i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
              </a>
            </div>
          </div>

          <!-- Service 2: Custom Software Development -->
          <div class="glass-card rounded-2xl p-7 transition-all duration-300 hover:-translate-y-1.5 flex flex-col justify-between group border-indigo-500/30 relative">
            <div class="absolute -top-3 right-6 px-2.5 py-0.5 rounded-full bg-indigo-500 text-[11px] font-bold text-white tracking-wide uppercase">
              Core Specialty
            </div>
            <div>
              <div class="w-14 h-14 rounded-xl bg-indigo-500/10 border border-indigo-500/20 flex items-center justify-center text-indigo-400 mb-6 group-hover:scale-110 group-hover:bg-indigo-500/20 transition">
                <i data-lucide="layers" class="w-7 h-7"></i>
              </div>
              <h3 class="text-xl font-bold text-white mb-2.5">Custom Software Development</h3>
              <p class="text-slate-400 text-sm leading-relaxed mb-6">
                Tailor-made software tailored to eliminate bottlenecks. Automation bots, billing & reconciliation portals, ERPs, CRM systems, and internal admin panels.
              </p>
              
              <div class="space-y-2 mb-6 text-xs text-slate-300">
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-indigo-400"></i> Workflow & Task Automation
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-indigo-400"></i> Custom Database & API Integrations
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-indigo-400"></i> Bank & Ledger Reconciliation Engines
                </div>
              </div>
            </div>

            <div class="pt-4 border-t border-slate-800/80 flex items-center justify-between">
              <span class="text-xs font-mono text-indigo-400 font-semibold">Bespoke Software</span>
              <a href="#estimator" class="text-xs text-slate-300 hover:text-white flex items-center gap-1 font-medium">
                Calculate Cost <i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
              </a>
            </div>
          </div>

          <!-- Service 3: Mobile Application Development -->
          <div class="glass-card rounded-2xl p-7 transition-all duration-300 hover:-translate-y-1.5 flex flex-col justify-between group">
            <div>
              <div class="w-14 h-14 rounded-xl bg-violet-500/10 border border-violet-500/20 flex items-center justify-center text-violet-400 mb-6 group-hover:scale-110 group-hover:bg-violet-500/20 transition">
                <i data-lucide="smartphone" class="w-7 h-7"></i>
              </div>
              <h3 class="text-xl font-bold text-white mb-2.5">Mobile Applications</h3>
              <p class="text-slate-400 text-sm leading-relaxed mb-6">
                High-performance iOS and Android mobile apps. Native performance with fluid animations, push notifications, offline capability, and secure payment setups.
              </p>
              
              <div class="space-y-2 mb-6 text-xs text-slate-300">
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-violet-400"></i> Flutter & React Native Solutions
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-violet-400"></i> Play Store & App Store Deployment
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle-2" class="w-4 h-4 text-violet-400"></i> Real-time Chat & Location Services
                </div>
              </div>
            </div>

            <div class="pt-4 border-t border-slate-800/80 flex items-center justify-between">
              <span class="text-xs font-mono text-violet-400 font-semibold">Android & iOS</span>
              <a href="#estimator" class="text-xs text-slate-300 hover:text-white flex items-center gap-1 font-medium">
                Calculate Cost <i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
              </a>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- ABOUT ABHISHEK & DHANVISTA -->
    <section id="about" class="py-20 relative bg-slate-950/40">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid lg:grid-cols-12 gap-12 items-center">
          
          <div class="lg:col-span-5 order-2 lg:order-1">
            <div class="relative">
              <!-- Visual graphic card with Logoo.png badge -->
              <div class="glass-card rounded-2xl p-6 border-slate-700/60 shadow-2xl relative z-10 space-y-6">
                <div class="flex items-center gap-4">
                  <div class="relative w-16 h-16 rounded-2xl bg-gradient-to-tr from-cyan-500 to-indigo-600 p-0.5 flex items-center justify-center shadow-lg shadow-cyan-500/20 overflow-hidden">
                    <img src="Logoo.png" alt="Dhanvista Secondary Emblem" class="w-full h-full object-contain p-1.5 bg-[#07090e] rounded-[14px]" onerror="this.onerror=null; this.parentElement.innerHTML='<span class=\'font-black text-xl text-white\'>AK</span>';">
                  </div>
                  <div>
                    <h4 class="text-lg font-bold text-white">Abhishek Kumar</h4>
                    <p class="text-xs text-cyan-400 font-mono">Principal Developer & Architect</p>
                    <p class="text-xs text-slate-400">Dhanvista Technologies</p>
                  </div>
                </div>

                <div class="p-4 rounded-xl bg-slate-900/80 border border-slate-800 space-y-2 text-xs">
                  <div class="flex justify-between text-slate-400 font-mono">
                    <span>Direct Phone:</span>
                    <a href="tel:+919555613854" class="text-slate-200 font-semibold hover:text-cyan-400">+91 9555613854</a>
                  </div>
                  <div class="flex justify-between text-slate-400 font-mono">
                    <span>Location:</span>
                    <span class="text-slate-200">India (Serving Global Clients)</span>
                  </div>
                  <div class="flex justify-between text-slate-400 font-mono">
                    <span>Availability:</span>
                    <span class="text-emerald-400 font-semibold flex items-center gap-1">
                      <span class="w-1.5 h-1.5 rounded-full bg-emerald-400"></span> Open for Contracts
                    </span>
                  </div>
    <!-- PORTFOLIO & WORK SHOWCASE (WITH VIDEO2.MP4 DEDICATED PLAYER) -->
    <section id="portfolio" class="py-20 relative">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-14 gap-6">
          <div class="space-y-2">
            <h2 class="text-xs font-mono tracking-widest text-cyan-400 uppercase">Recent Deployments</h2>
            <p class="text-3xl sm:text-4xl font-extrabold text-white">Featured Projects & Live Demos</p>
            <p class="text-slate-400 text-sm max-w-xl">Inspect live mockups and video previews of software and mobile platforms engineered by Dhanvista.</p>
          </div>

          <!-- Category filter buttons -->
          <div class="flex flex-wrap gap-2 text-xs font-medium" id="portfolioFilter">
            <button class="filter-btn active px-4 py-2 rounded-lg bg-cyan-500/20 text-cyan-300 border border-cyan-500/40" data-filter="all">All Work</button>
            <button class="filter-btn px-4 py-2 rounded-lg bg-slate-900 text-slate-400 border border-slate-800 hover:text-white" data-filter="web">Websites</button>
            <button class="filter-btn px-4 py-2 rounded-lg bg-slate-900 text-slate-400 border border-slate-800 hover:text-white" data-filter="software">Custom Software</button>
            <button class="filter-btn px-4 py-2 rounded-lg bg-slate-900 text-slate-400 border border-slate-800 hover:text-white" data-filter="app">Mobile Apps</button>
          </div>
        </div>

        <!-- Dedicated Software Showcase featuring video2.mp4 -->
        <div class="mb-12 glass-card rounded-3xl p-6 sm:p-8 border-indigo-500/30 overflow-hidden relative">
          <div class="grid lg:grid-cols-12 gap-8 items-center">
            <div class="lg:col-span-7 relative">
              <div class="rounded-2xl overflow-hidden border border-slate-700 shadow-2xl bg-black">
                <div class="flex items-center justify-between px-4 py-2.5 bg-slate-950 border-b border-slate-800 text-xs font-mono text-indigo-400">
                  <span class="flex items-center gap-1.5">
                    <i data-lucide="play" class="w-3.5 h-3.5 text-indigo-400"></i> video2.mp4 (Software & App Workflow)
                  </span>
                  <span class="text-slate-400">HD Demo</span>
                </div>
                <!-- Embedded second video file: video2.mp4 -->
                <div class="relative aspect-video bg-black flex items-center justify-center">
                  <video id="secondaryVideo" class="w-full h-full object-cover" loop playsinline controls preload="metadata">
                    <source src="video2.mp4" type="video/mp4">
                    Your browser does not support video playback.
                  </video>
                </div>
              </div>
            </div>

            <div class="lg:col-span-5 space-y-4">
              <span class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full bg-indigo-500/15 border border-indigo-500/30 text-indigo-300 text-xs font-mono">
                <i data-lucide="layers" class="w-3.5 h-3.5"></i> Custom Software & App Architecture
              </span>
              <h3 class="text-2xl sm:text-3xl font-extrabold text-white">Full-Stack Application In Action</h3>
              <p class="text-slate-300 text-xs sm:text-sm leading-relaxed">
                Watch <code class="text-cyan-300 bg-slate-900 px-1.5 py-0.5 rounded font-mono">video2.mp4</code> above showing real-time automation, responsive app interaction, and custom back-office database synchronization engineered for Dhanvista clients.
              </p>
              
              <div class="space-y-2 text-xs text-slate-300 pt-2">
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle" class="w-4 h-4 text-emerald-400"></i> Cross-Platform Mobile & Web Sync
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle" class="w-4 h-4 text-emerald-400"></i> Zero Latency Ledger & Database Engine
                </div>
                <div class="flex items-center gap-2">
                  <i data-lucide="check-circle" class="w-4 h-4 text-emerald-400"></i> Ready for iOS, Android & Cloud Hosting
                </div>
              </div>

              <div class="pt-4 flex flex-wrap gap-3">
                <a href="https://wa.me/919555613854?text=Hi%20Abhishek,%20I%20watched%20video2.mp4%20and%20want%20a%20similar%20software%20or%20app%20developed." target="_blank" class="px-5 py-2.5 rounded-xl text-xs font-bold bg-emerald-400 text-black flex items-center gap-2 hover:bg-emerald-300 transition">
                  <i data-lucide="message-circle" class="w-4 h-4 fill-black"></i> Discuss Similar Build
                </a>
                <a href="#estimator" class="px-4 py-2.5 rounded-xl text-xs font-semibold bg-slate-800 text-slate-200 hover:text-white border border-slate-700 transition">
                  Estimate Cost
                </a>
              </div>
            </div>
          </div>
        </div>

        <!-- Projects Grid -->
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8" id="portfolioGrid">
          
          <!-- Project 1: Modern SaaS / Web Platform -->
          <div class="portfolio-item glass-card rounded-2xl overflow-hidden group transition duration-300 hover:border-cyan-500/50" data-category="web">
            <div class="relative h-48 bg-gradient-to-br from-slate-900 via-slate-800 to-cyan-950/40 overflow-hidden flex items-center justify-center p-4">
              <!-- Visual UI Mockup Illustration -->
              <div class="w-full h-full rounded-lg bg-slate-900/90 border border-slate-700/60 p-3 shadow-inner flex flex-col justify-between">
                <div class="flex items-center justify-between pb-2 border-b border-slate-800">
                  <div class="flex gap-1.5">
                    <span class="w-2 h-2 rounded-full bg-red-500/70"></span>
                    <span class="w-2 h-2 rounded-full bg-yellow-500/70"></span>
                    <span class="w-2 h-2 rounded-full bg-green-500/70"></span>
                  </div>
                  <span class="text-[10px] font-mono text-cyan-400">apex-fin.dhanvista.app</span>
                </div>
                <div class="grid grid-cols-3 gap-2 my-auto">
                  <div class="h-10 rounded bg-cyan-500/10 border border-cyan-500/20 p-1.5 flex flex-col justify-center">
                    <span class="text-[9px] text-slate-400">Revenue</span>
                    <span class="text-xs font-bold text-white">₹42.8L</span>
                  </div>
                  <div class="h-10 rounded bg-indigo-500/10 border border-indigo-500/20 p-1.5 flex flex-col justify-center">
                    <span class="text-[9px] text-slate-400">Orders</span>
                    <span class="text-xs font-bold text-white">1,420</span>
                  </div>
                  <div class="h-10 rounded bg-emerald-500/10 border border-emerald-500/20 p-1.5 flex flex-col justify-center">
                    <span class="text-[9px] text-slate-400">Uptime</span>
                    <span class="text-xs font-bold text-emerald-400">99.9%</span>
                  </div>
                </div>
                <div class="h-2 w-3/4 rounded-full bg-slate-800"></div>
              </div>
              
              <button onclick="openDemoModal('Apex Financial Engine (Web Platform)', 'A high-speed SaaS landing portal and customer dashboard featuring interactive analytics, payment gateways, and sub-second load times.', 'web')" class="absolute inset-0 bg-black/60 opacity-0 group-hover:opacity-100 flex items-center justify-center transition-all duration-200 gap-2 text-white font-medium text-xs">
                <span class="px-4 py-2 rounded-lg bg-cyan-500 text-black font-bold flex items-center gap-1.5">
                  <i data-lucide="play-circle" class="w-4 h-4"></i> Watch Demo
                </span>
              </button>
            </div>
            
            <div class="p-6">
              <div class="flex items-center justify-between mb-2">
                <span class="text-[11px] font-mono text-cyan-400 font-semibold uppercase">Website & SaaS</span>
                <span class="text-xs text-slate-400">Live Client Build</span>
              </div>
              <h3 class="text-lg font-bold text-white mb-2">Apex Corporate Financial Portal</h3>
              <p class="text-slate-400 text-xs leading-relaxed mb-4">
                High-performance corporate web platform with dynamic client dashboards, automated lead intake, and fast Stripe/Razorpay checkouts.
              </p>
              <div class="flex flex-wrap gap-1.5 text-[10px] font-mono text-slate-300">
                <span class="px-2 py-0.5 rounded bg-slate-800">Next.js</span>
                <span class="px-2 py-0.5 rounded bg-slate-800">TailwindCSS</span>
                <span class="px-2 py-0.5 rounded bg-slate-800">Supabase</span>
              </div>
            </div>
          </div>

          <!-- Project 2: Custom Software / Internal Automation -->
          <div class="portfolio-item glass-card rounded-2xl overflow-hidden group transition duration-300 hover:border-indigo-500/50" data-category="software">
            <div class="relative h-48 bg-gradient-to-br from-slate-900 via-slate-800 to-indigo-950/40 overflow-hidden flex items-center justify-center p-4">
              <!-- Internal Software Dashboard Graphic -->
              <div class="w-full h-full rounded-lg bg-slate-900/90 border border-slate-700/60 p-3 shadow-inner flex flex-col justify-between">
                <div class="flex items-center justify-between pb-2 border-b border-slate-800">
                  <span class="text-[10px] font-mono text-indigo-400 flex items-center gap-1">
                    <i data-lucide="database" class="w-3 h-3"></i> SyncEngine v2.4
                  </span>
                  <span class="text-[9px] px-1.5 py-0.5 rounded bg-emerald-500/20 text-emerald-400">Running</span>
                </div>
                <div class="space-y-1.5 font-mono text-[9px] text-slate-400">
                  <div class="flex justify-between">
                    <span>Reconciliation Task:</span>
                    <span class="text-cyan-400">18,400 Rows Processed</span>
                  </div>
                  <div class="w-full bg-slate-800 rounded-full h-1.5">
                    <div class="bg-indigo-500 h-1.5 rounded-full w-[85%]"></div>
                  </div>
                  <div class="flex justify-between text-slate-500">
                    <span>GST & Invoice Match:</span>
                    <span class="text-emerald-400">100% Match</span>
                  </div>
                </div>
                <div class="flex justify-between items-center pt-1 border-t border-slate-800/60 text-[9px]">
                  <span class="text-slate-400">Time Saved: 30 hrs/wk</span>
                  <span class="text-indigo-300">Automated</span>
                </div>
              </div>

              <button onclick="openDemoModal('Custom Business ERP & Automation Suite', 'Engineered for a manufacturing client to automate inventory logging, billing, and GST compliance data ingestion without manual data entry.', 'software')" class="absolute inset-0 bg-black/60 opacity-0 group-hover:opacity-100 flex items-center justify-center transition-all duration-200 gap-2 text-white font-medium text-xs">
                <span class="px-4 py-2 rounded-lg bg-indigo-500 text-white font-bold flex items-center gap-1.5">
                  <i data-lucide="play-circle" class="w-4 h-4"></i> Preview Software
                </span>
              </button>
            </div>

            <div class="p-6">
              <div class="flex items-center justify-between mb-2">
                <span class="text-[11px] font-mono text-indigo-400 font-semibold uppercase">Custom Software</span>
                <span class="text-xs text-slate-400">Enterprise Tool</span>
              </div>
              <h3 class="text-lg font-bold text-white mb-2">Automated Ledger & Reconciliation Engine</h3>
              <p class="text-slate-400 text-xs leading-relaxed mb-4">
                Custom internal software designed to sync Excel bank exports, CRM data, and vendor ledgers automatically, cutting accounting time by 80%.
              </p>
              <div class="flex flex-wrap gap-1.5 text-[10px] font-mono text-slate-300">
                <span class="px-2 py-0.5 rounded bg-slate-800">Node / Python</span>
                <span class="px-2 py-0.5 rounded bg-slate-800">PostgreSQL</span>
                <span class="px-2 py-0.5 rounded bg-slate-800">Electron</span>
              </div>
            </div>
          </div>

          <!-- Project 3: Mobile Application -->
          <div class="portfolio-item glass-card rounded-2xl overflow-hidden group transition duration-300 hover:border-violet-500/50" data-category="app">
            <div class="relative h-48 bg-gradient-to-br from-slate-900 via-slate-800 to-violet-950/40 overflow-hidden flex items-center justify-center p-4">
              <!-- Mobile App UI Simulation -->
              <div class="w-32 h-full rounded-xl bg-slate-950 border-2 border-slate-700/80 p-2 flex flex-col justify-between shadow-lg">
                <div class="w-8 h-1 rounded-full bg-slate-700 mx-auto"></div>
                <div class="space-y-1.5">
                  <div class="w-full h-8 rounded bg-violet-600/20 border border-violet-500/30 p-1 flex items-center gap-1.5">
                    <div class="w-4 h-4 rounded-full bg-violet-500"></div>
                    <div class="w-12 h-1.5 rounded bg-slate-700"></div>
                  </div>
                  <div class="grid grid-cols-2 gap-1">
                    <div class="h-6 rounded bg-slate-800"></div>
                    <div class="h-6 rounded bg-slate-800"></div>
                  </div>
                </div>
                <div class="w-full py-1 rounded bg-violet-500 text-center text-[7px] font-bold text-white">Order Now</div>
              </div>

              <button onclick="openDemoModal('Dhanvista QuickCommerce Mobile App', 'A high-speed cross-platform app for on-demand ordering with live GPS driver tracking, Razorpay integration, and instant push updates.', 'app')" class="absolute inset-0 bg-black/60 opacity-0 group-hover:opacity-100 flex items-center justify-center transition-all duration-200 gap-2 text-white font-medium text-xs">
                <span class="px-4 py-2 rounded-lg bg-violet-500 text-white font-bold flex items-center gap-1.5">
                  <i data-lucide="play-circle" class="w-4 h-4"></i> View App Demo
                </span>
              </button>
            </div>

            <div class="p-6">
              <div class="flex items-center justify-between mb-2">
                <span class="text-[11px] font-mono text-violet-400 font-semibold uppercase">Mobile App</span>
                <span class="text-xs text-slate-400">iOS & Android</span>
              </div>
              <h3 class="text-lg font-bold text-white mb-2">OmniTrack Delivery & Client App</h3>
              <p class="text-slate-400 text-xs leading-relaxed mb-4">
                Real-time delivery management and order placement app built with cross-platform architecture, instant push messaging, and biometric login.
              </p>
              <div class="flex flex-wrap gap-1.5 text-[10px] font-mono text-slate-300">
                <span class="px-2 py-0.5 rounded bg-slate-800">Flutter</span>
                <span class="px-2 py-0.5 rounded bg-slate-800">Firebase</span>
                <span class="px-2 py-0.5 rounded bg-slate-800">Google Maps API</span>
              </div>
            </div>
          </div>

        </div>

        <div class="mt-12 text-center">
          <p class="text-slate-400 text-xs sm:text-sm mb-3">Have a unique software architecture or custom website in mind?</p>
          <a href="tel:+919555613854" class="inline-flex items-center gap-2 text-sm font-bold text-cyan-400 hover:text-cyan-300 transition">
            <i data-lucide="phone" class="w-4 h-4"></i> Call Abhishek Kumar directly: +91 9555613854
          </a>
        </div>

      </div>
    </section>

    <!-- INTERACTIVE PROJECT COST ESTIMATOR (DYNAMIC QUOTE GENERATOR) -->
    <section id="estimator" class="py-20 relative bg-slate-950/60 border-y border-slate-800/80">
      <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
        
        <div class="text-center max-w-2xl mx-auto mb-12 space-y-3">
          <div class="inline-flex items-center gap-1.5 px-3 py-1 rounded-full badge-gradient text-cyan-300 text-xs font-mono">
            <i data-lucide="calculator" class="w-3.5 h-3.5"></i> Instant Budget & Scope Planner
          </div>
          <h2 class="text-3xl sm:text-4xl font-extrabold text-white">Project Cost & Timeline Estimator</h2>
          <p class="text-slate-400 text-sm">Select your exact project requirements to see realistic estimated pricing and timeline. Instantly dispatch your plan directly to Abhishek via WhatsApp.</p>
        </div>

        <div class="glass-card rounded-3xl p-6 sm:p-10 shadow-2xl">
          <div class="space-y-8">
            
            <!-- Step 1: Project Type -->
            <div>
              <label class="block text-xs font-mono uppercase text-slate-400 mb-3 tracking-wider">1. Select Primary Service</label>
              <div class="grid sm:grid-cols-3 gap-3">
                <button type="button" class="service-opt p-4 rounded-xl border border-cyan-500 bg-cyan-500/10 text-left transition flex flex-col justify-between" data-service="web" data-base="14999" data-days="7">
                  <div class="flex items-center justify-between mb-2">
                    <i data-lucide="globe" class="w-5 h-5 text-cyan-400"></i>
                    <span class="text-xs font-mono text-cyan-400 font-bold">From ₹14,999</span>
                  </div>
                  <div>
                    <p class="font-bold text-white text-sm">Website Development</p>
                    <p class="text-[11px] text-slate-400 mt-1">Landing pages, business portals, portfolio, or e-commerce.</p>
                  </div>
                </button>

                <button type="button" class="service-opt p-4 rounded-xl border border-slate-800 bg-slate-900/60 hover:border-slate-700 text-left transition flex flex-col justify-between" data-service="software" data-base="24999" data-days="14">
                  <div class="flex items-center justify-between mb-2">
                    <i data-lucide="cpu" class="w-5 h-5 text-indigo-400"></i>
                    <span class="text-xs font-mono text-indigo-400 font-bold">From ₹24,999</span>
                  </div>
                  <div>
                    <p class="font-bold text-white text-sm">Custom Software</p>
                    <p class="text-[11px] text-slate-400 mt-1">Business ERP, scrapers, automated workflows & tools.</p>
                  </div>
                </button>

                <button type="button" class="service-opt p-4 rounded-xl border border-slate-800 bg-slate-900/60 hover:border-slate-700 text-left transition flex flex-col justify-between" data-service="app" data-base="34999" data-days="20">
                  <div class="flex items-center justify-between mb-2">
                    <i data-lucide="smartphone" class="w-5 h-5 text-violet-400"></i>
                    <span class="text-xs font-mono text-violet-400 font-bold">From ₹34,999</span>
                  </div>
                  <div>
                    <p class="font-bold text-white text-sm">Mobile Application</p>
                    <p class="text-[11px] text-slate-400 mt-1">Cross-platform iOS & Android mobile software.</p>
                  </div>
                </button>
              </div>
            </div>

            <!-- Step 2: Add-on Capabilities -->
            <div>
              <label class="block text-xs font-mono uppercase text-slate-400 mb-3 tracking-wider">2. Add Desired Features & Integrations</label>
              <div class="grid sm:grid-cols-2 md:grid-cols-3 gap-3">
                <label class="flex items-start gap-3 p-3.5 rounded-xl bg-slate-900/50 border border-slate-800 cursor-pointer hover:border-slate-700 transition">
                  <input type="checkbox" class="feature-checkbox mt-1 accent-cyan-400 rounded" value="Payment Gateway (Razorpay/Stripe)" data-cost="4000" data-extra-days="2">
                  <div>
                    <p class="text-xs font-semibold text-white">Payment Gateway</p>
                    <p class="text-[11px] text-slate-400">+₹4,000 | +2 days</p>
                  </div>
                </label>

                <label class="flex items-start gap-3 p-3.5 rounded-xl bg-slate-900/50 border border-slate-800 cursor-pointer hover:border-slate-700 transition">
                  <input type="checkbox" class="feature-checkbox mt-1 accent-cyan-400 rounded" value="User Auth & Dashboard" data-cost="6000" data-extra-days="3">
                  <div>
                    <p class="text-xs font-semibold text-white">Auth & Client Portal</p>
                    <p class="text-[11px] text-slate-400">+₹6,000 | +3 days</p>
                  </div>
                </label>

                <label class="flex items-start gap-3 p-3.5 rounded-xl bg-slate-900/50 border border-slate-800 cursor-pointer hover:border-slate-700 transition">
                  <input type="checkbox" class="feature-checkbox mt-1 accent-cyan-400 rounded" value="Automated Email / WhatsApp Alerts" data-cost="3500" data-extra-days="2">
                  <div>
                    <p class="text-xs font-semibold text-white">WhatsApp & SMS Alerts</p>
                    <p class="text-[11px] text-slate-400">+₹3,500 | +2 days</p>
                  </div>
                </label>

                <label class="flex items-start gap-3 p-3.5 rounded-xl bg-slate-900/50 border border-slate-800 cursor-pointer hover:border-slate-700 transition">
                  <input type="checkbox" class="feature-checkbox mt-1 accent-cyan-400 rounded" value="Admin Analytics & Export" data-cost="5000" data-extra-days="3">
                  <div>
                    <p class="text-xs font-semibold text-white">Analytics & CSV Reports</p>
                    <p class="text-[11px] text-slate-400">+₹5,000 | +3 days</p>
                  </div>
                </label>

                <label class="flex items-start gap-3 p-3.5 rounded-xl bg-slate-900/50 border border-slate-800 cursor-pointer hover:border-slate-700 transition">
                  <input type="checkbox" class="feature-checkbox mt-1 accent-cyan-400 rounded" value="Priority Express Delivery" data-cost="5000" data-extra-days="-3">
                  <div>
                    <p class="text-xs font-semibold text-white">Rush Express Timeline</p>
                    <p class="text-[11px] text-slate-400">+₹5,000 | Faster Delivery</p>
                  </div>
                </label>

                <label class="flex items-start gap-3 p-3.5 rounded-xl bg-slate-900/50 border border-slate-800 cursor-pointer hover:border-slate-700 transition">
                  <input type="checkbox" class="feature-checkbox mt-1 accent-cyan-400 rounded" value="1 Year Dedicated Maintenance" data-cost="8000" data-extra-days="0">
                  <div>
                    <p class="text-xs font-semibold text-white">Annual Maintenance</p>
                    <p class="text-[11px] text-slate-400">+₹8,000 | 12 Mo. Support</p>
                  </div>
                </label>
              </div>
            </div>

            <!-- Estimator Calculation Summary Card -->
            <div class="p-6 rounded-2xl bg-gradient-to-r from-slate-900 via-[#0a1120] to-slate-900 border border-cyan-500/30 flex flex-col md:flex-row items-center justify-between gap-6">
              <div>
                <p class="text-xs font-mono text-cyan-400 uppercase tracking-wider mb-1">Estimated Starting Investment</p>
                <div class="flex items-baseline gap-2">
                  <span id="calculatedCost" class="text-3xl sm:text-4xl font-extrabold text-white font-mono">₹14,999</span>
                  <span class="text-xs text-slate-400 font-normal">(approx. INR)</span>
                </div>
                <p class="text-xs text-slate-400 mt-1 flex items-center gap-2">
                  <i data-lucide="clock" class="w-3.5 h-3.5 text-cyan-400"></i> Estimated Delivery: <strong id="calculatedTimeline" class="text-slate-200">~7 business days</strong>
                </p>
              </div>

              <div class="flex flex-col sm:flex-row gap-3 w-full md:w-auto">
                <button id="sendQuoteWhatsApp" class="w-full sm:w-auto px-6 py-3 rounded-xl font-bold text-black bg-emerald-400 hover:bg-emerald-300 transition flex items-center justify-center gap-2 shadow-lg shadow-emerald-500/20 text-xs sm:text-sm">
                  <i data-lucide="message-circle" class="w-4 h-4 fill-black"></i> Send Quote to WhatsApp
                </button>
                <a href="tel:+919555613854" class="w-full sm:w-auto px-4 py-3 rounded-xl font-semibold text-slate-200 bg-slate-800 hover:bg-slate-700 border border-slate-700 transition flex items-center justify-center gap-2 text-xs sm:text-sm">
                  <i data-lucide="phone-call" class="w-4 h-4 text-cyan-400"></i> Call +91 9555613854
                </a>
              </div>
            </div>

          </div>
        </div>

      </div>
    </section>

    <!-- TESTIMONIALS & TRUST PILLARS -->
    <section class="py-20 relative">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        
        <div class="text-center max-w-2xl mx-auto mb-16 space-y-2">
          <h2 class="text-xs font-mono tracking-widest text-cyan-400 uppercase">Client Trust</h2>
          <p class="text-3xl sm:text-4xl font-extrabold text-white">Built on Speed & Integrity</p>
        </div>

        <div class="grid md:grid-cols-3 gap-6">
          <div class="glass-card rounded-2xl p-6 relative">
            <div class="flex text-amber-400 gap-1 mb-3">
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
            </div>
            <p class="text-slate-300 text-xs sm:text-sm leading-relaxed mb-4">
              "Abhishek completely revamped our company website and built a custom client portal for Dhanvista. The communication on phone and WhatsApp was instant, and the code was spotless."
            </p>
            <div class="flex items-center gap-3 border-t border-slate-800/80 pt-4">
              <div class="w-9 h-9 rounded-full bg-cyan-600/30 flex items-center justify-center font-bold text-xs text-cyan-300">RK</div>
              <div>
                <p class="text-xs font-bold text-white">Rohit Kapoor</p>
                <p class="text-[10px] text-slate-400">Founder, Logistics Platform</p>
              </div>
            </div>
          </div>

          <div class="glass-card rounded-2xl p-6 relative">
            <div class="flex text-amber-400 gap-1 mb-3">
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
            </div>
            <p class="text-slate-300 text-xs sm:text-sm leading-relaxed mb-4">
              "We needed custom software to automate billing and daily reports. Dhanvista delivered it in less than 2 weeks. Abhishek's technical logic and speed saved us two full-time salaries."
            </p>
            <div class="flex items-center gap-3 border-t border-slate-800/80 pt-4">
              <div class="w-9 h-9 rounded-full bg-indigo-600/30 flex items-center justify-center font-bold text-xs text-indigo-300">SG</div>
              <div>
                <p class="text-xs font-bold text-white">Sanjay Gupta</p>
                <p class="text-[10px] text-slate-400">Operations Director, Retail Group</p>
              </div>
            </div>
          </div>

          <div class="glass-card rounded-2xl p-6 relative">
            <div class="flex text-amber-400 gap-1 mb-3">
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
              <i data-lucide="star" class="w-4 h-4 fill-amber-400"></i>
            </div>
            <p class="text-slate-300 text-xs sm:text-sm leading-relaxed mb-4">
              "Developing an iOS and Android app usually comes with headaches. Abhishek took care of authentication, real-time database updates, and app store approval with zero fuss."
            </p>
            <div class="flex items-center gap-3 border-t border-slate-800/80 pt-4">
              <div class="w-9 h-9 rounded-full bg-violet-600/30 flex items-center justify-center font-bold text-xs text-violet-300">AM</div>
              <div>
                <p class="text-xs font-bold text-white">Ananya Mishra</p>
                <p class="text-[10px] text-slate-400">Tech Co-Founder</p>
              </div>
            </div>
          </div>
        </div>

      </div>
    </section>

    <!-- CONTACT & DIRECT INQUIRY SECTION -->
    <section id="contact" class="py-20 relative bg-slate-950/70 border-t border-slate-800">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        
        <div class="grid lg:grid-cols-12 gap-12">
          
          <div class="lg:col-span-5 space-y-6">
            <h2 class="text-xs font-mono tracking-widest text-cyan-400 uppercase">Get In Touch</h2>
            <h3 class="text-3xl sm:text-4xl font-extrabold text-white">Let's Bring Your Vision to Life.</h3>
            <p class="text-slate-400 text-sm leading-relaxed">
              Have a project requirement, an MVP idea, or an urgent software automation requirement? Call Abhishek Kumar directly or leave a message below.
            </p>

            <div class="space-y-4 pt-2">
              <div class="flex items-center gap-4 p-4 rounded-xl glass-card">
                <div class="w-12 h-12 rounded-xl bg-cyan-500/10 border border-cyan-500/20 flex items-center justify-center text-cyan-400">
                  <i data-lucide="phone-outgoing" class="w-5 h-5"></i>
                </div>
                <div>
                  <p class="text-xs text-slate-400 font-mono">Direct Phone Call</p>
                  <a href="tel:+919555613854" class="text-base font-bold text-white hover:text-cyan-400 transition">
                    +91 9555613854
                  </a>
                </div>
              </div>

              <div class="flex items-center gap-4 p-4 rounded-xl glass-card">
                <div class="w-12 h-12 rounded-xl bg-emerald-500/10 border border-emerald-500/20 flex items-center justify-center text-emerald-400">
                  <i data-lucide="message-circle" class="w-5 h-5"></i>
                </div>
                <div>
                  <p class="text-xs text-slate-400 font-mono">WhatsApp Direct Chat</p>
                  <a href="https://wa.me/919555613854?text=Hello%20Abhishek!%20I%20am%20interested%20in%20building%20a%20project%20with%20Dhanvista." target="_blank" rel="noopener noreferrer" class="text-base font-bold text-emerald-400 hover:underline">
                    Chat on +91 9555613854
                  </a>
                </div>
              </div>

              <div class="flex items-center gap-4 p-4 rounded-xl glass-card">
                <div class="w-12 h-12 rounded-xl bg-indigo-500/10 border border-indigo-500/20 flex items-center justify-center text-indigo-400">
                  <i data-lucide="shield" class="w-5 h-5"></i>
                </div>
                <div>
                  <p class="text-xs text-slate-400 font-mono">Brand & Developer</p>
                  <p class="text-sm font-bold text-white">Dhanvista &bull; Abhishek Kumar</p>
                </div>
              </div>
            </div>
          </div>

          <!-- Interactive Form -->
          <div class="lg:col-span-7">
            <div class="glass-card rounded-3xl p-6 sm:p-8 border-slate-700/80">
              <form id="contactForm" class="space-y-4">
                <div class="grid sm:grid-cols-2 gap-4">
                  <div>
                    <label class="block text-xs font-mono text-slate-400 mb-1.5">Your Name *</label>
                    <input type="text" id="senderName" required placeholder="John Doe" class="w-full px-4 py-3 rounded-xl bg-slate-900/90 border border-slate-700/80 text-white placeholder-slate-500 focus:outline-none focus:border-cyan-500 text-sm">
                  </div>
                  <div>
                    <label class="block text-xs font-mono text-slate-400 mb-1.5">Your Phone / WhatsApp *</label>
                    <input type="tel" id="senderPhone" required placeholder="+91 ..." class="w-full px-4 py-3 rounded-xl bg-slate-900/90 border border-slate-700/80 text-white placeholder-slate-500 focus:outline-none focus:border-cyan-500 text-sm">
                  </div>
                </div>

                <div>
                  <label class="block text-xs font-mono text-slate-400 mb-1.5">Service Required</label>
                  <select id="selectedServiceCategory" class="w-full px-4 py-3 rounded-xl bg-slate-900/90 border border-slate-700/80 text-white focus:outline-none focus:border-cyan-500 text-sm">
                    <option value="Website Development">Website Development (Landing Page / E-Commerce)</option>
                    <option value="Custom Software Development">Custom Software Development (ERP / Tools / Automation)</option>
                    <option value="Mobile App Development">Mobile App (Android / iOS)</option>
                    <option value="Full Digital Transformation">Complete Package (Web + App + Software)</option>
                  </select>
                </div>

                <div>
                  <label class="block text-xs font-mono text-slate-400 mb-1.5">Briefly Describe Your Project *</label>
                  <textarea id="senderMessage" required rows="4" placeholder="Tell Abhishek about your requirements, features needed, and target timeline..." class="w-full px-4 py-3 rounded-xl bg-slate-900/90 border border-slate-700/80 text-white placeholder-slate-500 focus:outline-none focus:border-cyan-500 text-sm"></textarea>
                </div>

                <div id="formStatusMsg" class="hidden p-3 rounded-xl text-xs font-medium"></div>

                <div class="flex flex-col sm:flex-row gap-3 pt-2">
                  <button type="submit" class="flex-1 py-3.5 px-6 rounded-xl font-bold text-white bg-gradient-to-r from-cyan-500 via-indigo-600 to-violet-600 hover:opacity-95 transition text-sm flex items-center justify-center gap-2 shadow-lg shadow-indigo-500/20">
                    <i data-lucide="send" class="w-4 h-4"></i> Submit Project Inquiry
                  </button>
                  <button type="button" onclick="sendViaDirectWhatsApp()" class="py-3.5 px-5 rounded-xl font-bold text-black bg-emerald-400 hover:bg-emerald-300 transition text-sm flex items-center justify-center gap-2">
                    <i data-lucide="message-circle" class="w-4 h-4 fill-black"></i> Send on WhatsApp
                  </button>
                </div>
              </form>
            </div>
          </div>

        </div>

      </div>
    </section>
  </main>

  <!-- FOOTER -->
  <footer class="bg-[#030509] border-t border-slate-800/80 py-12 relative z-10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex flex-col md:flex-row items-center justify-between gap-6">
        
        <div class="flex items-center gap-3">
          <div class="w-10 h-10 rounded-lg bg-gradient-to-tr from-cyan-500 to-indigo-600 p-0.5 flex items-center justify-center overflow-hidden">
            <img src="Logo.png" alt="Dhanvista Logo" class="w-full h-full object-contain p-1 bg-[#030509] rounded-md" onerror="this.onerror=null; this.parentElement.innerHTML='<span class=\'font-bold text-white text-sm\'>D</span>';">
          </div>
          <div>
            <span class="font-bold text-white tracking-tight">Dhanvista</span>
            <span class="text-xs text-slate-500 block">Crafted by Abhishek Kumar</span>
          </div>
        </div>

        <div class="flex flex-wrap justify-center gap-6 text-xs text-slate-400 font-mono">
          <a href="#services" class="hover:text-cyan-400 transition">Services</a>
          <a href="#about" class="hover:text-cyan-400 transition">About</a>
          <a href="#portfolio" class="hover:text-cyan-400 transition">Portfolio</a>
          <a href="#estimator" class="hover:text-cyan-400 transition">Estimator</a>
          <a href="tel:+919555613854" class="text-cyan-400 font-bold hover:underline">+91 9555613854</a>
        </div>

        <p class="text-xs text-slate-500">
          &copy; <span id="currentYear"></span> Dhanvista. All rights reserved.
        </p>

      </div>
    </div>
  </footer>

  <!-- FLOATING QUICK WHATSAPP / CALL BAR FOR MOBILE -->
  <div class="fixed bottom-4 right-4 z-40 flex flex-col gap-2.5">
    <a href="https://wa.me/919555613854?text=Hello%20Abhishek!%20I'm%20visiting%20Dhanvista%20and%20want%20to%20discuss%20a%20project." target="_blank" rel="noopener noreferrer" aria-label="WhatsApp Abhishek" class="w-13 h-13 p-3.5 rounded-full bg-emerald-500 text-black shadow-lg shadow-emerald-500/40 hover:scale-110 active:scale-95 transition flex items-center justify-center">
      <i data-lucide="message-circle" class="w-6 h-6 fill-black"></i>
    </a>
    <a href="tel:+919555613854" aria-label="Call Abhishek" class="w-13 h-13 p-3.5 rounded-full bg-cyan-500 text-slate-950 shadow-lg shadow-cyan-500/40 hover:scale-110 active:scale-95 transition flex items-center justify-center">
      <i data-lucide="phone-call" class="w-6 h-6"></i>
    </a>
  </div>

  <!-- VIDEO & INTERACTIVE DEMO PREVIEW MODAL -->
  <div id="demoModal" class="fixed inset-0 z-50 hidden bg-black/80 backdrop-blur-md flex items-center justify-center p-4">
    <div class="bg-slate-900 border border-slate-700 w-full max-w-2xl rounded-2xl overflow-hidden shadow-2xl animate-in fade-in zoom-in duration-200">
      
      <div class="flex items-center justify-between px-5 py-3.5 border-b border-slate-800 bg-slate-950">
        <div class="flex items-center gap-2">
          <span class="w-3 h-3 rounded-full bg-cyan-400"></span>
          <h4 id="modalTitle" class="text-sm font-bold text-white">Project Showcase Preview</h4>
        </div>
        <button onclick="closeDemoModal()" class="text-slate-400 hover:text-white p-1 rounded-lg">
          <i data-lucide="x" class="w-5 h-5"></i>
        </button>
      </div>

      <div class="p-6 space-y-4">
        <!-- Simulated interactive canvas / video screen -->
        <div class="relative w-full aspect-video rounded-xl bg-slate-950 border border-slate-800 flex flex-col items-center justify-center p-6 text-center overflow-hidden">
          
          <div class="absolute inset-0 bg-gradient-to-tr from-cyan-950/20 to-indigo-950/30"></div>
          
          <div class="relative z-10 space-y-3">
            <div class="w-16 h-16 rounded-full bg-cyan-500/10 border border-cyan-400/40 mx-auto flex items-center justify-center text-cyan-400 animate-pulse">
              <i data-lucide="play" class="w-7 h-7 fill-cyan-400"></i>
            </div>
            <p class="text-sm font-semibold text-white" id="modalSubhead">Interactive Demo & Feature Walkthrough</p>
            <p class="text-xs text-slate-400 max-w-md mx-auto" id="modalDescription">Detailed architecture demonstration designed specifically for clients requesting high reliability.</p>
          </div>

          <div class="absolute bottom-3 left-4 right-4 flex items-center justify-between text-[11px] font-mono text-slate-400 bg-slate-900/80 px-3 py-1.5 rounded-lg border border-slate-800">
            <span class="text-cyan-400 flex items-center gap-1.5">
              <span class="w-2 h-2 rounded-full bg-emerald-400"></span> Live Demo Ready
            </span>
            <span>Developer: Abhishek Kumar</span>
          </div>
        </div>

        <div class="flex flex-col sm:flex-row items-center justify-between gap-3 pt-2">
          <p class="text-xs text-slate-400">Want a custom walkthrough tailored to your workflow?</p>
          <div class="flex gap-2 w-full sm:w-auto">
            <a id="modalWhatsAppBtn" href="https://wa.me/919555613854?text=Hi%20Abhishek,%20I'd%20like%20a%20demo%20for%20my%20business." target="_blank" class="flex-1 sm:flex-none px-4 py-2 rounded-xl text-xs font-bold bg-emerald-400 text-black flex items-center justify-center gap-1.5">
              <i data-lucide="message-circle" class="w-3.5 h-3.5 fill-black"></i> Discuss Demo
            </a>
            <a href="tel:+919555613854" class="px-3.5 py-2 rounded-xl text-xs font-bold bg-slate-800 text-slate-200 hover:text-white flex items-center justify-center gap-1.5">
              <i data-lucide="phone" class="w-3.5 h-3.5 text-cyan-400"></i> Call Now
            </a>
          </div>
        </div>
      </div>

    </div>
  </div>

  <!-- SCRIPT LOGIC -->
  <script>
    // Initialize Lucide icons
    lucide.createIcons();

    // Set Copyright Year
    document.getElementById('currentYear').textContent = new Date().getFullYear();

    // Mobile Menu Toggle
    const mobileMenuBtn = document.getElementById('mobileMenuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    mobileMenuBtn.addEventListener('click', () => {
      mobileMenu.classList.toggle('hidden');
    });

    document.querySelectorAll('.mobile-nav-link').forEach(link => {
      link.addEventListener('click', () => {
        mobileMenu.classList.add('hidden');
      });
    });

    // Navbar Scroll Background Styling
    const navbar = document.getElementById('navbar');
    window.addEventListener('scroll', () => {
      if (window.scrollY > 40) {
        navbar.classList.add('bg-[#05070d]/90', 'backdrop-blur-md', 'border-b', 'border-slate-800/80', 'shadow-lg');
      } else {
        navbar.classList.remove('bg-[#05070d]/90', 'backdrop-blur-md', 'border-b', 'border-slate-800/80', 'shadow-lg');
      }
    });

    // Portfolio Filtering Logic
    const filterBtns = document.querySelectorAll('.filter-btn');
    const portfolioItems = document.querySelectorAll('.portfolio-item');

    filterBtns.forEach(btn => {
      btn.addEventListener('click', () => {
        filterBtns.forEach(b => {
          b.classList.remove('active', 'bg-cyan-500/20', 'text-cyan-300', 'border-cyan-500/40');
          b.classList.add('bg-slate-900', 'text-slate-400', 'border-slate-800');
        });

        btn.classList.add('active', 'bg-cyan-500/20', 'text-cyan-300', 'border-cyan-500/40');
        btn.classList.remove('bg-slate-900', 'text-slate-400', 'border-slate-800');

        const filter = btn.getAttribute('data-filter');

        portfolioItems.forEach(item => {
          if (filter === 'all' || item.getAttribute('data-category') === filter) {
            item.style.display = 'block';
          } else {
            item.style.display = 'none';
          }
        });
      });
    });

    // Cost Estimator State & Calculations
    let selectedService = 'web';
    let basePrice = 14999;
    let baseDays = 7;
    const serviceButtons = document.querySelectorAll('.service-opt');
    const featureCheckboxes = document.querySelectorAll('.feature-checkbox');
    const calculatedCostEl = document.getElementById('calculatedCost');
    const calculatedTimelineEl = document.getElementById('calculatedTimeline');

    function updateEstimator() {
      let totalCost = basePrice;
      let totalDays = baseDays;
      let selectedFeatures = [];

      featureCheckboxes.forEach(cb => {
        if (cb.checked) {
          totalCost += parseInt(cb.getAttribute('data-cost'), 10);
          totalDays += parseInt(cb.getAttribute('data-extra-days'), 10);
          selectedFeatures.push(cb.value);
        }
      });

      if (totalDays < 3) totalDays = 3;

      calculatedCostEl.textContent = '₹' + totalCost.toLocaleString('en-IN');
      calculatedTimelineEl.textContent = `~${totalDays} business days`;

      return { totalCost, totalDays, selectedFeatures };
    }

    serviceButtons.forEach(btn => {
      btn.addEventListener('click', () => {
        serviceButtons.forEach(b => {
          b.classList.remove('border-cyan-500', 'bg-cyan-500/10');
          b.classList.add('border-slate-800', 'bg-slate-900/60');
        });

        btn.classList.add('border-cyan-500', 'bg-cyan-500/10');
        btn.classList.remove('border-slate-800', 'bg-slate-900/60');

        selectedService = btn.getAttribute('data-service');
        basePrice = parseInt(btn.getAttribute('data-base'), 10);
        baseDays = parseInt(btn.getAttribute('data-days'), 10);
        updateEstimator();
      });
    });

    featureCheckboxes.forEach(cb => {
      cb.addEventListener('change', updateEstimator);
    });

    // Send Quote to WhatsApp Button
    document.getElementById('sendQuoteWhatsApp').addEventListener('click', () => {
      const { totalCost, totalDays, selectedFeatures } = updateEstimator();
      let serviceName = "Website Development";
      if (selectedService === 'software') serviceName = "Custom Software Development";
      if (selectedService === 'app') serviceName = "Mobile Application Development";

      let featuresText = selectedFeatures.length > 0 ? selectedFeatures.join(', ') : 'Base Architecture';

      const message = `Hello Abhishek! I generated an estimate on Dhanvista for:\n\n*Service:* ${serviceName}\n*Included Features:* ${featuresText}\n*Estimated Budget:* ₹${totalCost.toLocaleString('en-IN')}\n*Estimated Timeline:* ~${totalDays} days\n\nI want to discuss and start this project with you!`;

      window.open(`https://wa.me/919555613854?text=${encodeURIComponent(message)}`, '_blank');
    });

    // Demo Modal Handling
    const demoModal = document.getElementById('demoModal');
    const modalTitle = document.getElementById('modalTitle');
    const modalDescription = document.getElementById('modalDescription');
    const modalSubhead = document.getElementById('modalSubhead');
    const modalWhatsAppBtn = document.getElementById('modalWhatsAppBtn');

    function openDemoModal(title, desc, type) {
      modalTitle.textContent = title;
      modalSubhead.textContent = `${title} Preview`;
      modalDescription.textContent = desc;

      const waMsg = `Hi Abhishek, I saw the showcase demo for "${title}" on Dhanvista. Can you explain how this can be tailored for my business?`;
      modalWhatsAppBtn.href = `https://wa.me/919555613854?text=${encodeURIComponent(waMsg)}`;

      demoModal.classList.remove('hidden');
    }

    function closeDemoModal() {
      demoModal.classList.add('hidden');
    }

    demoModal.addEventListener('click', (e) => {
      if (e.target === demoModal) closeDemoModal();
    });

    // Contact Form Handler
    const contactForm = document.getElementById('contactForm');
    const formStatusMsg = document.getElementById('formStatusMsg');

    contactForm.addEventListener('submit', (e) => {
      e.preventDefault();
      const name = document.getElementById('senderName').value;
      const phone = document.getElementById('senderPhone').value;
      const service = document.getElementById('selectedServiceCategory').value;
      const message = document.getElementById('senderMessage').value;

      formStatusMsg.classList.remove('hidden', 'bg-rose-500/20', 'text-rose-400');
      formStatusMsg.classList.add('bg-emerald-500/20', 'text-emerald-400');
      formStatusMsg.innerHTML = `<span class="font-bold">Thank you, ${name}!</span> Your inquiry has been logged. Abhishek will reach out directly at <strong>${phone}</strong> shortly.`;

      // Auto-prompt WhatsApp transfer option
      setTimeout(() => {
        const confirmTransfer = `Hi Abhishek! My name is ${name}. Phone: ${phone}. Interested in: ${service}. Note: ${message}`;
        window.open(`https://wa.me/919555613854?text=${encodeURIComponent(confirmTransfer)}`, '_blank');
      }, 900);
    });

    function sendViaDirectWhatsApp() {
      const name = document.getElementById('senderName').value || "Client";
      const phone = document.getElementById('senderPhone').value || "Not provided";
      const service = document.getElementById('selectedServiceCategory').value;
      const message = document.getElementById('senderMessage').value || "Project inquiry";

      const waMsg = `Hello Abhishek! Inquiry from Dhanvista:\n\n*Name:* ${name}\n*Phone:* ${phone}\n*Category:* ${service}\n*Details:* ${message}`;
      window.open(`https://wa.me/919555613854?text=${encodeURIComponent(waMsg)}`, '_blank');
    }

    // Video error detection for fallback guidance
    const heroVid = document.getElementById('heroVideo');
    const fallbackNotice = document.getElementById('videoFallbackNotice');
    if (heroVid) {
      heroVid.addEventListener('error', () => {
        fallbackNotice.classList.remove('hidden');
      });
    }
  </script>
</body>
</html>
```