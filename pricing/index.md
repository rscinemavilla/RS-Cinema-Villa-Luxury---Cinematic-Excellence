---
layout: default
title: Pricing
---
<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Jost:wght@300;400;500;600&display=swap');

*{box-sizing:border-box;margin:0;padding:0}
html,body{min-height:100%;background:#faf9f7;color:#1a1a1a}
body{font-family:'Jost',sans-serif;background:#faf9f7;color:#1a1a1a}

.site-header{position:sticky;top:0;z-index:1000;background:rgba(250,249,247,0.97);backdrop-filter:blur(12px);display:flex;align-items:center;justify-content:space-between;padding:0 40px;height:64px;border-bottom:1px solid rgba(0,0,0,0.08)}
.brand{color:#1a1a1a;font-family:'Cormorant Garamond',serif;font-size:20px;font-weight:600;letter-spacing:1px;text-decoration:none}
.site-nav{display:flex;gap:4px}
.site-nav a{color:#555;text-decoration:none;padding:0 14px;height:64px;line-height:64px;font-size:13px;font-weight:400;letter-spacing:0.5px;transition:color 0.2s}
.site-nav a:hover{color:#1a1a1a}
.site-nav a.active{color:#1a1a1a;font-weight:500;border-bottom:2px solid #c9a96e}
.nav-book-btn{background:#1a1a1a;color:#fff!important;padding:10px 22px!important;height:auto!important;line-height:normal!important;border-radius:3px;font-size:13px!important;letter-spacing:1px!important;transition:background 0.2s!important}
.nav-book-btn:hover{background:#333!important}

.hero{position:relative;width:100%;height:55vh;min-height:380px;background:url('/RSCinemaVilla/images/RScinemavilla5.JPG') center/cover no-repeat;display:flex;align-items:flex-end;justify-content:flex-start;overflow:hidden}
.hero::before{content:'';position:absolute;inset:0;background:linear-gradient(to top,rgba(0,0,0,0.75) 0%,rgba(0,0,0,0.15) 70%,transparent 100%)}
.hero-content{position:relative;padding:0 64px 56px;max-width:700px}
.hero-eyebrow{display:inline-block;color:#c9a96e;font-size:11px;font-weight:500;letter-spacing:3px;text-transform:uppercase;margin-bottom:16px}
.hero-content h1{font-family:'Cormorant Garamond',serif;font-size:clamp(2.2rem,4.5vw,4rem);font-weight:300;color:#fff;line-height:1.1;margin-bottom:14px}
.hero-content h1 em{font-style:italic;color:#e8d5b0}
.hero-content p{font-size:0.95rem;color:rgba(255,255,255,0.75);font-weight:300;line-height:1.7}

.section-eyebrow{font-size:11px;font-weight:500;letter-spacing:3px;text-transform:uppercase;color:#c9a96e;margin-bottom:14px}
.section-title{font-family:'Cormorant Garamond',serif;font-size:clamp(1.8rem,3.5vw,2.8rem);font-weight:300;color:#1a1a1a;line-height:1.2;margin-bottom:20px}
.section-title em{font-style:italic}
.divider{width:48px;height:1px;background:#c9a96e;margin:20px 0 24px}
.body-text{font-size:1rem;color:#555;line-height:1.85;font-weight:300}

/* PRICING INTRO */
.pricing-intro{background:#fff;padding:72px 64px;text-align:center;border-bottom:1px solid rgba(0,0,0,0.07)}
.pricing-intro-inner{max-width:800px;margin:0 auto}
.phone-cta{display:inline-flex;align-items:center;gap:14px;background:#1a1a1a;padding:18px 32px;border-radius:2px;margin-top:32px;text-decoration:none;transition:background 0.2s}
.phone-cta:hover{background:#333}
.phone-cta .label{font-size:11px;color:rgba(255,255,255,0.5);letter-spacing:1px;text-transform:uppercase;display:block;text-align:left}
.phone-cta .number{font-family:'Cormorant Garamond',serif;font-size:1.5rem;color:#c9a96e;font-weight:600}

/* PRICE HIGHLIGHT */
.price-highlight{background:#1a1a1a;padding:80px 64px;text-align:center}
.price-highlight .section-title{color:#fff}
.price-number{font-family:'Cormorant Garamond',serif;font-size:5rem;font-weight:300;color:#c9a96e;line-height:1;margin:16px 0 8px}
.price-unit{font-size:13px;color:rgba(255,255,255,0.4);letter-spacing:2px;text-transform:uppercase;margin-bottom:24px}
.price-note{font-size:0.9rem;color:rgba(255,255,255,0.45);font-weight:300;max-width:500px;margin:0 auto}

/* BOOKING OPTIONS */
.booking-section{background:#faf9f7;padding:96px 64px}
.booking-inner{max-width:1100px;margin:0 auto}
.booking-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:2px;margin-top:56px}
.booking-card{background:#fff;padding:40px 28px;text-align:center;border-top:3px solid transparent;transition:border-color 0.3s}
.booking-card:hover{border-top-color:#c9a96e}
.booking-icon{font-size:1.8rem;margin-bottom:16px;display:block}
.booking-title{font-family:'Cormorant Garamond',serif;font-size:1.25rem;color:#1a1a1a;margin-bottom:8px}
.booking-subtitle{font-size:0.85rem;font-weight:500;color:#c9a96e;margin-bottom:10px;letter-spacing:0.5px}
.booking-desc{font-size:0.85rem;color:#777;line-height:1.6;font-weight:300}

/* WHATS INCLUDED */
.included-section{background:#fff;padding:96px 64px;border-top:1px solid rgba(0,0,0,0.07)}
.included-inner{max-width:1100px;margin:0 auto}
.included-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:32px;margin-top:56px}
.included-item{display:flex;gap:16px;align-items:flex-start;padding:24px;background:#faf9f7;border-radius:2px}
.inc-icon{font-size:1.3rem;flex-shrink:0;margin-top:2px}
.inc-text strong{display:block;color:#1a1a1a;font-size:0.95rem;font-weight:500;margin-bottom:4px}
.inc-text span{color:#888;font-size:0.85rem;font-weight:300}

/* EVENTS WE HOST */
.events-section{background:#f0ebe1;padding:96px 64px}
.events-inner{max-width:1100px;margin:0 auto}
.events-list{display:grid;grid-template-columns:1fr 1fr;gap:2px;margin-top:56px}
.event-item{background:#fff;padding:32px 36px;display:flex;align-items:center;gap:20px;transition:background 0.2s}
.event-item:hover{background:#faf9f7}
.event-icon{font-size:1.5rem;flex-shrink:0}
.event-name{font-family:'Cormorant Garamond',serif;font-size:1.2rem;color:#1a1a1a}
.event-tag{font-size:0.8rem;color:#888;font-weight:300;margin-top:4px}

/* QUOTE SECTION */
.quote-section{background:#1a1a1a;padding:96px 64px}
.quote-inner{max-width:1100px;margin:0 auto;display:grid;grid-template-columns:1fr 1fr;gap:80px;align-items:center}
.quote-section .section-title{color:#fff}
.quote-section .divider{background:#c9a96e}
.quote-section .body-text{color:rgba(255,255,255,0.55)}
.quote-steps{margin-top:40px}
.quote-step{display:flex;gap:20px;align-items:flex-start;margin-bottom:28px}
.step-num{font-family:'Cormorant Garamond',serif;font-size:2.5rem;font-weight:300;color:rgba(201,169,110,0.3);line-height:1;flex-shrink:0;width:40px}
.step-text strong{display:block;color:#fff;font-size:0.95rem;font-weight:500;margin-bottom:4px}
.step-text span{color:rgba(255,255,255,0.45);font-size:0.85rem;font-weight:300}
.quote-cta-box{background:rgba(255,255,255,0.05);border:1px solid rgba(201,169,110,0.3);border-radius:2px;padding:48px 40px;text-align:center}
.quote-cta-phone{font-family:'Cormorant Garamond',serif;font-size:2.2rem;font-weight:400;color:#c9a96e;display:block;text-decoration:none;margin:20px 0 28px}
.cta-btns{display:flex;flex-direction:column;gap:12px}
.btn{display:inline-block;padding:14px 32px;font-size:13px;font-weight:500;letter-spacing:1px;text-decoration:none;border-radius:2px;transition:all 0.2s;text-align:center}
.btn-gold{background:#c9a96e;color:#fff}
.btn-gold:hover{background:#b8914f}
.btn-wa{background:#25D366;color:#fff}
.btn-wa:hover{background:#1ebe57}
.btn-airbnb{background:#FF5A5F;color:#fff}
.btn-airbnb:hover{background:#e04f54}
.btn-outline{border:1px solid rgba(255,255,255,0.3);color:#fff}
.btn-outline:hover{border-color:rgba(255,255,255,0.7)}

.site-footer{background:#111;padding:40px 64px;display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:16px}
.footer-brand{font-family:'Cormorant Garamond',serif;color:#c9a96e;font-size:18px;letter-spacing:1px}
.footer-tagline{color:rgba(255,255,255,0.35);font-size:12px;letter-spacing:1.5px;text-transform:uppercase;font-style:italic}
.footer-links a{color:rgba(255,255,255,0.4);font-size:12px;margin-left:20px;text-decoration:none;letter-spacing:0.5px;transition:color 0.2s}
.footer-links a:hover{color:#c9a96e}

@media(max-width:900px){
.site-header{padding:0 20px}
.hero-content{padding:0 24px 40px}
.pricing-intro,.price-highlight,.booking-section,.included-section,.events-section,.quote-section{padding:64px 24px}
.booking-grid{grid-template-columns:1fr 1fr}
.included-grid{grid-template-columns:1fr 1fr}
.events-list,.quote-inner{grid-template-columns:1fr}
.site-footer{padding:32px 24px;flex-direction:column;text-align:center}
.footer-links a{margin:0 10px}
.nav-book-btn{display:none}
}
@media(max-width:600px){
.booking-grid,.included-grid,.events-list{grid-template-columns:1fr}
.site-nav a{padding:0 8px;font-size:12px}
}
</style>

<header class="site-header">
  <a href="/RSCinemaVilla/" class="brand">RS Cinema Villa</a>
  <nav class="site-nav">
    <a href="/RSCinemaVilla/">Home</a>
    <a href="/RSCinemaVilla/gallery/">Gallery</a>
    <a href="/RSCinemaVilla/about-villa/">About Villa</a>
    <a href="/RSCinemaVilla/pricing/" class="active">Pricing</a>
    <a href="/RSCinemaVilla/reviews/">Reviews &amp; Testimonials</a>
    <a href="/RSCinemaVilla/contact/">Contact &amp; Book Now</a>
    <a href="https://wa.me/919206845678" class="nav-book-btn" target="_blank">Enquire Now</a>
  </nav>
</header>

<!-- HERO -->
<section class="hero">
  <div class="hero-content">
    <span class="hero-eyebrow">Transparent &middot; Flexible &middot; Tailored</span>
    <h1>Pricing that&rsquo;s made <em>just for you</em></h1>
    <p>Every celebration is unique. Our pricing is flexible &mdash; based on your event, guest count, and duration. Contact us for a personalised quote.</p>
  </div>
</section>

<!-- PRICING INTRO -->
<div class="pricing-intro">
  <div class="pricing-intro-inner">
    <p class="section-eyebrow">How Our Pricing Works</p>
    <h2 class="section-title">Transparent, flexible &amp; always <em>worth every rupee</em></h2>
    <div class="divider" style="margin:20px auto 24px"></div>
    <p class="body-text">RS Cinema Villa offers <strong>flexible pricing</strong> based on your event type, duration, and guest count. We don&rsquo;t believe in a one-size-fits-all approach &mdash; every celebration is unique, and your quote will be tailored to match exactly what you need.</p>
    <a href="tel:+919206845678" class="phone-cta">
      <div>
        <span class="label">Call / WhatsApp for instant pricing</span>
        <span class="number">+91 92068 45678</span>
      </div>
    </a>
  </div>
</div>

<!-- PRICE HIGHLIGHT -->
<section class="price-highlight">
  <p class="section-eyebrow">Investment Starting From</p>
  <h2 class="section-title" style="color:#fff">Your private luxury villa awaits</h2>
  <div class="price-number">&#8377;20,000</div>
  <div class="price-unit">per session</div>
  <p class="price-note">Pricing varies based on date, event type, guest count, and duration. Contact us for your personalised quote and the best available package.</p>
</section>

<!-- BOOKING OPTIONS -->
<section class="booking-section">
  <div class="booking-inner">
    <p class="section-eyebrow">Booking Options</p>
    <h2 class="section-title">Choose your <em>perfect stay</em></h2>
    <div class="divider"></div>
    <div class="booking-grid">
      <div class="booking-card">
        <span class="booking-icon">&#127751;</span>
        <div class="booking-title">Day Use</div>
        <div class="booking-subtitle">Morning to Evening</div>
        <p class="booking-desc">Perfect for events, parties, photo shoots, and daytime celebrations</p>
      </div>
      <div class="booking-card">
        <span class="booking-icon">&#127769;</span>
        <div class="booking-title">Night Use</div>
        <div class="booking-subtitle">Evening to Morning</div>
        <p class="booking-desc">Ideal for evening parties, overnight getaways, and celebrations</p>
      </div>
      <div class="booking-card">
        <span class="booking-icon">&#127968;</span>
        <div class="booking-title">Full Day &amp; Night</div>
        <div class="booking-subtitle">24-Hour Exclusive Access</div>
        <p class="booking-desc">Our most popular option &mdash; the entire villa is yours for a full day and night</p>
      </div>
      <div class="booking-card">
        <span class="booking-icon">&#128197;</span>
        <div class="booking-title">Multi-Day Stays</div>
        <div class="booking-subtitle">Extended Bookings</div>
        <p class="booking-desc">Available for extended family stays, film productions, and special occasions on request</p>
      </div>
    </div>
  </div>
</section>

<!-- WHATS INCLUDED -->
<section class="included-section">
  <div class="included-inner">
    <p class="section-eyebrow">What&rsquo;s Included</p>
    <h2 class="section-title">Everything included. <em>Nothing hidden.</em></h2>
    <div class="divider"></div>
    <p class="body-text">Every booking at RS Cinema Villa comes with full access to all our premium amenities. No hidden charges. No surprises.</p>
    <div class="included-grid">
      <div class="included-item"><span class="inc-icon">&#127946;</span><div class="inc-text"><strong>Private Swimming Pool</strong><span>Exclusive pool access throughout your stay</span></div></div>
      <div class="included-item"><span class="inc-icon">&#127968;</span><div class="inc-text"><strong>All 5 AC Bedrooms</strong><span>Spacious rooms with premium linens</span></div></div>
      <div class="included-item"><span class="inc-icon">&#127916;</span><div class="inc-text"><strong>Cinema &amp; Entertainment Room</strong><span>Projector, screen &amp; surround sound system</span></div></div>
      <div class="included-item"><span class="inc-icon">&#127807;</span><div class="inc-text"><strong>Manicured Lawn &amp; Outdoor Areas</strong><span>Perfect for events, walks &amp; photography</span></div></div>
      <div class="included-item"><span class="inc-icon">&#127859;</span><div class="inc-text"><strong>Fully-Equipped Kitchen</strong><span>Modern kitchen for self-catering</span></div></div>
      <div class="included-item"><span class="inc-icon">&#128225;</span><div class="inc-text"><strong>High-Speed Wi-Fi</strong><span>Seamless connectivity throughout the property</span></div></div>
      <div class="included-item"><span class="inc-icon">&#128274;</span><div class="inc-text"><strong>24-Hour Support &amp; Security</strong><span>Our team is always on-site during your stay</span></div></div>
      <div class="included-item"><span class="inc-icon">&#9832;</span><div class="inc-text"><strong>Hot Tub / Jacuzzi Access</strong><span>Unwind and relax in your private hot tub</span></div></div>
      <div class="included-item"><span class="inc-icon">&#128081;</span><div class="inc-text"><strong>Dedicated Hosting Team</strong><span>Personalized support throughout your booking</span></div></div>
    </div>
  </div>
</section>

<!-- EVENTS WE HOST -->
<section class="events-section">
  <div class="events-inner">
    <p class="section-eyebrow">Events We Host</p>
    <h2 class="section-title">Every event. <em>Done right.</em></h2>
    <div class="divider"></div>
    <div class="events-list">
      <div class="event-item"><span class="event-icon">&#127874;</span><div><div class="event-name">Birthday Parties &amp; Grand Celebrations</div><div class="event-tag">The most popular event at RS Cinema Villa</div></div></div>
      <div class="event-item"><span class="event-icon">&#128141;</span><div><div class="event-name">Anniversaries, Engagements &amp; Pre-Wedding Functions</div><div class="event-tag">Romantic escapes and milestone moments</div></div></div>
      <div class="event-item"><span class="event-icon">&#128106;</span><div><div class="event-name">Family Staycations &amp; Reunions</div><div class="event-tag">Space and privacy for the whole family</div></div></div>
      <div class="event-item"><span class="event-icon">&#127882;</span><div><div class="event-name">Private Parties &amp; Social Gatherings</div><div class="event-tag">Exclusive events in a stunning setting</div></div></div>
      <div class="event-item"><span class="event-icon">&#127916;</span><div><div class="event-name">Film Shoots, Music Videos &amp; Photo Sessions</div><div class="event-tag">A filmmaker&rsquo;s dream location near Hyderabad</div></div></div>
      <div class="event-item"><span class="event-icon">&#128188;</span><div><div class="event-name">Corporate Offsites &amp; Team Events</div><div class="event-tag">Productive retreats in a premium environment</div></div></div>
    </div>
  </div>
</section>

<!-- GET A QUOTE -->
<section class="quote-section">
  <div class="quote-inner">
    <div>
      <p class="section-eyebrow">Get a Custom Quote</p>
      <h2 class="section-title" style="color:#fff">Ready to know <em style="color:#e8d5b0">your price?</em></h2>
      <div class="divider"></div>
      <p class="body-text" style="color:rgba(255,255,255,0.55)">Getting a quote is quick and easy. Simply WhatsApp or call us, tell us your event date, number of guests, and what you have in mind &mdash; and we&rsquo;ll get back to you with the best package.</p>
      <div class="quote-steps">
        <div class="quote-step"><div class="step-num">01</div><div class="step-text"><strong>Contact Us</strong><span>WhatsApp or call +91 92068 45678 to get started</span></div></div>
        <div class="quote-step"><div class="step-num">02</div><div class="step-text"><strong>Share Your Event Details</strong><span>Tell us the date, guest count, and type of occasion</span></div></div>
        <div class="quote-step"><div class="step-num">03</div><div class="step-text"><strong>Receive Your Custom Quote</strong><span>We&rsquo;ll send you the best package for your needs</span></div></div>
        <div class="quote-step"><div class="step-num">04</div><div class="step-text"><strong>Confirm &amp; Celebrate</strong><span>Secure your dates with an advance payment and arrive</span></div></div>
      </div>
    </div>
    <div class="quote-cta-box">
      <p class="section-eyebrow" style="color:#c9a96e">Reach Us Anytime</p>
      <p style="color:rgba(255,255,255,0.5);font-size:0.9rem;margin-top:8px">We respond quickly &mdash; 7 days a week</p>
      <a href="tel:+919206845678" class="quote-cta-phone">+91 92068 45678</a>
      <div class="cta-btns">
        <a href="https://wa.me/919206845678?text=Hi%2C%20I%20would%20like%20to%20know%20the%20pricing%20for%20RS%20Cinema%20Villa" class="btn btn-wa" target="_blank">&#128172; WhatsApp Us for Pricing</a>
        <a href="https://calendly.com/rscinemavilla" class="btn btn-gold" target="_blank">&#128197; Book Now</a>
        <a href="https://www.airbnb.co.in/rooms/1506244066053865421" class="btn btn-airbnb" target="_blank">&#127968; View on Airbnb</a>
        <a href="https://www.instagram.com/rs_cinema_villa" class="btn btn-outline" target="_blank">&#128247; Follow @rs_cinema_villa</a>
      </div>
    </div>
  </div>
</section>

<footer class="site-footer">
  <div class="footer-brand">RS Cinema Villa</div>
  <div class="footer-tagline">The best moments in life are the ones worth planning for.</div>
  <div class="footer-links">
    <a href="https://www.instagram.com/rs_cinema_villa/" target="_blank">Instagram</a>
    <a href="mailto:rscinemavilla@gmail.com">Email</a>
    <a href="/RSCinemaVilla/contact/">Contact</a>
  </div>
</footer>
