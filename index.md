---
layout: default
title: RS Cinema Villa
---

<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
      font-family: 'Google Sans', Arial, sans-serif;
      background: #fff;
      color: #333;
  }

  /* ── NAVBAR ── */
  .site-header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: #202124;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 24px;
      height: 56px;
  }
  .site-header .brand {
      color: #fff;
      font-size: 18px;
      font-weight: 600;
      text-decoration: none;
  }
  .site-nav {
      display: flex;
      gap: 0;
  }
  .site-nav a {
      color: #e8eaed;
      text-decoration: none;
      padding: 0 16px;
      height: 56px;
      line-height: 56px;
      font-size: 14px;
      font-weight: 500;
      transition: background 0.2s;
  }
  .site-nav a:hover { background: rgba(255,255,255,0.1); }
  .site-nav a.active { border-bottom: 3px solid #fff; font-weight: 700; }

  /* ── HERO ── */
  .hero {
      position: relative;
      width: 100%;
      min-height: 400px;
      background: url('/RS-Cinema-Villa-Luxury---Cinematic-Excellence/images/RScinemavilla1.jpg') center/cover no-repeat;
      display: flex;
      align-items: center;
      justify-content: center;
  }
  .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: rgba(0,0,0,0.45);
  }
  .hero-box {
      position: relative;
      border: 2px solid rgba(255,255,255,0.7);
      padding: 40px 60px;
      text-align: center;
      color: #fff;
  }
  .hero-box h1 {
      font-size: 52px;
      font-weight: 700;
      margin-bottom: 12px;
      letter-spacing: 1px;
  }
  .hero-box h2 {
      font-size: 26px;
      font-weight: 400;
  }

  /* ── INTRO SECTION ── */
  .intro-section {
      display: flex;
      align-items: flex-start;
      gap: 40px;
      max-width: 1100px;
      margin: 48px auto;
      padding: 0 32px;
  }
  .intro-img {
      width: 42%;
      flex-shrink: 0;
      border-radius: 4px;
      overflow: hidden;
  }
  .intro-img img {
      width: 100%;
      height: auto;
      display: block;
      border-radius: 4px;
  }
  .intro-text {
      flex: 1;
      padding-top: 4px;
  }
  .intro-text .welcome-line {
      font-size: 15px;
      line-height: 1.65;
      margin-bottom: 12px;
  }
  .intro-text .phone-line {
      font-size: 15px;
      font-weight: 600;
      margin-bottom: 20px;
  }
  .intro-text .phone-line a {
      color: #1a73e8;
      text-decoration: underline;
  }
  .intro-text .perfect-for-title {
      font-size: 15px;
      font-weight: 700;
      margin-bottom: 12px;
  }
  .intro-text ul {
      list-style: none;
      padding: 0;
      margin-bottom: 20px;
  }
  .intro-text ul li {
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 15px;
      margin-bottom: 10px;
      padding-left: 4px;
  }
  .intro-text ul li::before {
      content: '▪';
      color: #555;
      font-size: 10px;
      flex-shrink: 0;
  }
  .cta-row {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 8px;
      font-size: 15px;
      margin-bottom: 16px;
  }
  .cta-row a {
      color: #1a73e8;
      text-decoration: underline;
      font-weight: 500;
  }
  .cta-row .sep {
      color: #555;
  }
  .follow-row {
      font-size: 15px;
  }
  .follow-row a {
      color: #1a73e8;
      text-decoration: underline;
  }

  /* ── FOOTER TAGLINE ── */
  .footer-tagline {
      text-align: center;
      padding: 32px 24px 48px;
      font-style: italic;
      color: #555;
      font-size: 15px;
  }

  @media (max-width: 700px) {
      .intro-section { flex-direction: column; }
      .intro-img { width: 100%; }
      .hero-box h1 { font-size: 32px; }
      .hero-box h2 { font-size: 18px; }
      .site-nav a { padding: 0 8px; font-size: 12px; }
  }
  </style>

  <!-- NAVBAR -->
  <header class="site-header">
      <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/" class="brand">RS Cinema Villa</a>a>
      <nav class="site-nav">
            <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/" class="active">Home</a>a>
            <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/gallery/">Gallery</a>a>
            <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/about-villa/">About Villa</a>a>
            <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/pricing/">Pricing</a>a>
            <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/reviews/">Reviews &amp; Testimonials</a>a>
            <a href="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/contact/">Contact &amp; Book Now</a>a>
      </nav>nav>
  </header>header>

  <!-- HERO BANNER -->
  <section class="hero">
      <div class="hero-box">
            <h1>RS Cinema Villa</h1>h1>
          <h2>Luxury Private Villa for Celebrations &amp; Events</h2>h2>
      </div>div>
  </section>section>
  
  <!-- INTRO SECTION -->
  <section class="intro-section">
      <div class="intro-img">
            <img src="/RS-Cinema-Villa-Luxury---Cinematic-Excellence/images/RScinemavilla1.jpg" alt="RS Cinema Villa exterior view">
      </div>div>
      <div class="intro-text">
            <p class="welcome-line"><strong>Welcome to RS Cinema Villa 🎬✨</strong>strong> A luxury private villa in the peaceful heart of Moinabad, Hyderabad — designed for privacy, celebration, and premium experiences.</p>p>
            <p class="phone-line">Phone / WhatsApp: <a href="https://wa.me/919206845678">+91 92068 45678</a>a></p>p>

            <p class="perfect-for-title">🎉 <strong>Perfect For:</strong></p>
                <ul>
                      <li>🎂 Birthdays &amp; Celebrations</li>
                            <li>💍 Engagements &amp; Pre-wedding Functions</li>
                                  <li>👨‍👩‍👧 Family Get-togethers &amp; Reunions</li>
                                        <li>🎊 Private Parties &amp; Social Events</li>
                                              <li>🎬 Movie &amp; Photo Shoots</li>
                                                    <li>💼 Corporate Offsites</li>
                                                          <li>🎨 Customizable Décor &amp; Music</li>
                                                              </ul>

                                                                  <div class="cta-row">
                                                                        <span>📅</span> <a href="https://calendly.com/rscinemavilla/booking">Book Now</a>
                                                                              <span class="sep">|</span>
                                                                                    <span>💬</span> <a href="https://wa.me/919206845678">WhatsApp Us</a>
                                                                                          <span class="sep">|</span>
                                                                                                <span>🏠</span> <a href="https://www.airbnb.co.in/rooms/1506244066053865421">View on Airbnb</a>
                                                                                                    </div>
                                                                                                    
                                                                                                        <div class="follow-row">
                                                                                                              📸 Follow us: <a href="https://www.instagram.com/rs_cinema_villa/">@rs_cinema_villa</a>
                                                                                                                  </div>
                                                                                                                    </div>
                                                                                                                    </section>
                                                                                                                    
                                                                                                                    <!-- FOOTER TAGLINE -->
                                                                                                                    <div class="footer-tagline">
                                                                                                                      Where every moment becomes a memory worth keeping.
                                                                                                                      </div>
  </h1>
</style>
