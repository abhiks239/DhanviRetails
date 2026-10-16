<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhanvishta - Custom Software & Windows Applications</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Inter', sans-serif; }
        body { background-color: #0f172a; color: #f8fafc; line-height: 1.6; }
        header { background: #1e293b; padding: 20px 50px; display: flex; justify-content: space-between; align-items: center; border-bottom: 1px solid #334155; position: sticky; top: 0; z-index: 1000; }
        .logo-area { display: flex; align-items: center; gap: 12px; }
        .logo-icon { width: 45px; height: 45px; background: linear-gradient(135deg, #3b82f6, #1d4ed8); border-radius: 10px; display: flex; align-items: center; justify-content: center; font-weight: bold; font-size: 22px; color: white; box-shadow: 0 4px 12px rgba(59, 130, 246, 0.4); }
        .logo-text h1 { font-size: 20px; font-weight: 700; color: #fff; letter-spacing: 0.5px; }
        .logo-text p { font-size: 11px; color: #94a3b8; }
        nav a { color: #cbd5e1; text-decoration: none; margin-left: 25px; font-weight: 500; transition: color 0.3s; }
        nav a:hover { color: #3b82f6; }
        .hero { padding: 60px 20px; text-align: center; max-width: 1000px; margin: 0 auto; }
        .hero h2 { font-size: 40px; font-weight: 700; margin-bottom: 15px; color: #fff; }
        .hero h2 span { color: #3b82f6; }
        .hero p { font-size: 18px; color: #94a3b8; margin-bottom: 30px; }
        .cta-btn { background: #3b82f6; color: white; padding: 14px 32px; border-radius: 8px; text-decoration: none; font-weight: 600; font-size: 16px; display: inline-block; transition: background 0.3s; box-shadow: 0 4px 14px rgba(59, 130, 246, 0.4); }
        .cta-btn:hover { background: #2563eb; }
        
        /* Dashboard Mockup Image Section */
        .hero-image-container { max-width: 900px; margin: 40px auto 0 auto; background: #1e293b; padding: 15px; border-radius: 14px; border: 1px solid #334155; box-shadow: 0 20px 40px rgba(0,0,0,0.5); }
        .hero-image-container img { width: 100%; border-radius: 8px; display: block; }

        .features { padding: 80px 20px; max-width: 1200px; margin: 0 auto; display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; }
        .feature-card { background: #1e293b; padding: 30px; border-radius: 12px; border: 1px solid #334155; transition: transform 0.3s; }
        .feature-card:hover { transform: translateY(-5px); border-color: #3b82f6; }
        .feature-icon { font-size: 36px; margin-bottom: 15px; }
        .feature-card h3 { font-size: 20px; margin-bottom: 12px; color: #f1f5f9; }
        .feature-card p { color: #94a3b8; font-size: 14px; }
        
        .pricing { background: linear-gradient(135deg, #1e293b, #0f172a); padding: 60px 20px; text-align: center; margin: 40px 20px; border-radius: 16px; border: 1px solid #334155; }
        .pricing h2 { font-size: 32px; margin-bottom: 15px; }
        .price { font-size: 48px; font-weight: 700; color: #3b82f6; margin: 20px 0; }
        
        footer { text-align: center; padding: 30px; background: #090d16; color: #64748b; font-size: 14px; border-top: 1px solid #1e293b; }
    </style>
</head>
<body>

    <header>
        <div class="logo-area">
            <div class="logo-icon">D</div>
            <div class="logo-text">
                <h1>DHANVISHTA</h1>
                <p>Your Business Simplified</p>
            </div>
        </div>
        <nav>
            <a href="#features">Services</a>
            <a href="#pricing">Pricing</a>
            <a href="tel:955613854" class="cta-btn" style="padding: 8px 18px; font-size: 14px;">Call Now</a>
        </nav>
    </header>

    <section class="hero">
        <h2>Build Your Dream Application: <span>Exactly How You Want It!</span>[cite: 8, 10, 13, 14, 15]</h2>
        <p>Custom Windows & Desktop Solutions, Billing Software, CRM, and Automation Tools. Zero monthly fees, full data ownership[cite: 5, 7, 8, 10, 13, 14, 15].</p>
        <a href="tel:955613854" class="cta-btn">Get Free Consultation: 955613854</a>[cite: 5, 7, 8, 10, 13, 14, 15]

        <!-- Real Software Dashboard Image Mockup -->
        <div class="hero-image-container">
            <img src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?auto=format&fit=crop&w=1200&q=80" alt="Dhanvishta Custom Software Dashboard">
        </div>
    </section>

    <section class="features" id="features">
        <div class="feature-card">
            <div class="feature-icon">💳</div>
            <h3>Billing & Invoicing</h3>
            <p>Custom-built GST billing software tailored precisely to your store or business workflow with zero recurring fee[cite: 5, 7, 8, 10, 13, 14, 15].</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">👥</div>
            <h3>CRM & Management</h3>
            <p>Track your customers, leads, and daily operations smoothly with dedicated desktop windows apps[cite: 5, 7, 8, 10, 13, 14, 15].</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">📦</div>
            <h3>Inventory Control</h3>
            <p>Manage stock levels effortlessly without heavy software bloatware or mandatory standard limits[cite: 8, 10, 13, 14, 15].</p>
        </div>
        <div class="feature-card">
            <div class="feature-icon">⚙️</div>
            <h3>Custom Automation</h3>
            <p>Automate repetitive tasks, data entry, and reports exactly per your custom requirements[cite: 8, 10, 13, 14, 15].</p>
        </div>
    </section>

    <section class="pricing" id="pricing">
        <h2>One-Time Investment. Lifetime Ownership.[cite: 5, 7, 8, 10, 13, 14, 15]</h2>
        <p>Say goodbye to monthly subscription traps and forced upgrades[cite: 5, 7, 8, 10, 13, 14, 15].</p>
        <div class="price">₹1,999/- onwards</div>[cite: 3, 8, 10, 13, 14, 15]
        <a href="tel:955613854" class="cta-btn">Book Your Custom App Now</a>[cite: 5, 7, 8, 10, 13, 14, 15]
    </section>

    <footer>
        <p>&copy; 2026 Dhanvishta Solutions. All rights reserved. | Contact & WhatsApp: 955613854</p>[cite: 5, 7, 8, 10, 13, 14, 15]
    </footer>

</body>
</html>
