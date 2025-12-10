# CebuDropBox
curated monthly essentials box designed for families in Cebu.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Cebu Essentials Club | Filipino Pantry Subscription from the USA</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta
    name="description"
    content="Classy Filipino pantry subscription service. Order from the USA, we curate and deliver weekly or monthly essentials to your loved ones in Cebu City."
  />
  <style>
    :root {
      --bg: #f7f4f0;
      --card: #ffffff;
      --text: #1f2428;
      --muted: #6f7380;
      --primary: #b68b5a;   /* warm gold */
      --primary-soft: #f0e1cf;
      --accent: #364152;
      --radius-lg: 20px;
      --radius-md: 14px;
      --shadow-soft: 0 16px 40px rgba(15, 23, 42, 0.08);
      --max-width: 1080px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
        sans-serif;
      background: radial-gradient(circle at top left, #fdfaf6 0, #f7f4f0 42%, #f1ece6 100%);
      color: var(--text);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    img {
      max-width: 100%;
      display: block;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .page {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 50;
      backdrop-filter: blur(14px);
      background: rgba(247, 244, 240, 0.92);
      border-bottom: 1px solid rgba(15, 23, 42, 0.04);
    }

    .nav {
      max-width: var(--max-width);
      margin: 0 auto;
      padding: 0.65rem 1.1rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 1rem;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 0.7rem;
    }

    .brand-mark {
      width: 40px;
      height: 40px;
      border-radius: 999px;
      background: linear-gradient(135deg, #f0e1cf, #e0c39a);
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 700;
      font-size: 1.05rem;
      color: #3a2b1a;
      box-shadow: 0 12px 28px rgba(148, 120, 78, 0.4);
    }

    .brand-text {
      display: flex;
      flex-direction: column;
    }

    .brand-text span:first-child {
      font-size: 0.98rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      font-weight: 600;
    }

    .brand-text span:last-child {
      font-size: 0.75rem;
      color: var(--muted);
    }

    .nav-links {
      display: flex;
      gap: 1.4rem;
      font-size: 0.88rem;
    }

    .nav-links a {
      position: relative;
      padding-bottom: 2px;
      text-transform: uppercase;
      letter-spacing: 0.14em;
      font-size: 0.72rem;
      color: var(--muted);
    }

    .nav-links a::after {
      content: "";
      position: absolute;
      left: 0;
      bottom: -2px;
      width: 0;
      height: 1px;
      background: var(--primary);
      transition: width 0.2s ease-out;
    }

    .nav-links a:hover::after {
      width: 100%;
    }

    .nav-cta {
      border-radius: 999px;
      border: 1px solid rgba(182, 139, 90, 0.4);
      padding: 0.45rem 0.95rem;
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      background: #ffffff;
      color: var(--accent);
      cursor: pointer;
      font-weight: 600;
      transition: background 0.16s ease, transform 0.12s ease,
        box-shadow 0.16s ease;
      box-shadow: 0 10px 22px rgba(15, 23, 42, 0.07);
    }

    .nav-cta:hover {
      background: #f0e1cf;
      transform: translateY(-1px);
      box-shadow: 0 14px 30px rgba(15, 23, 42, 0.12);
    }

    main {
      flex: 1;
    }

    section {
      padding: 3.4rem 1.1rem;
    }

    .container {
      max-width: var(--max-width);
      margin: 0 auto;
    }

    /* HERO */

    .hero {
      padding-top: 2.7rem;
      padding-bottom: 3.2rem;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(0, 1fr);
      gap: 2.4rem;
      align-items: center;
    }

    .hero-tag {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.32rem 0.9rem;
      border-radius: 999px;
      background: rgba(240, 225, 207, 0.7);
      color: #7a5a31;
      font-size: 0.76rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      margin-bottom: 1rem;
    }

    .hero-tag span.dot {
      width: 7px;
      height: 7px;
      border-radius: 50%;
      background: #7a5a31;
    }

    .hero h1 {
      font-size: clamp(2rem, 3.4vw, 2.8rem);
      letter-spacing: 0.03em;
      text-transform: uppercase;
      margin-bottom: 0.8rem;
    }

    .hero h1 span.accent {
      color: var(--primary);
    }

    .hero-subtitle {
      font-size: 0.98rem;
      color: var(--muted);
      max-width: 32rem;
      margin-bottom: 1.5rem;
    }

    .hero-subtitle strong {
      color: var(--accent);
      font-weight: 600;
    }

    .hero-list {
      display: grid;
      gap: 0.35rem;
      font-size: 0.9rem;
      margin-bottom: 1.4rem;
    }

    .hero-list-item {
      display: flex;
      align-items: flex-start;
      gap: 0.4rem;
      color: var(--muted);
    }

    .hero-list-item span.bullet {
      margin-top: 0.22rem;
      width: 9px;
      height: 9px;
      border-radius: 999px;
      border: 1px solid rgba(182, 139, 90, 0.7);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.7rem;
      margin-bottom: 1rem;
      align-items: center;
    }

    .btn-primary {
      border-radius: 999px;
      border: none;
      outline: none;
      cursor: pointer;
      padding: 0.8rem 1.6rem;
      text-transform: uppercase;
      letter-spacing: 0.18em;
      font-size: 0.8rem;
      font-weight: 600;
      background: linear-gradient(135deg, #b68b5a, #8f6a3c);
      color: #fff;
      box-shadow: 0 18px 36px rgba(22, 28, 45, 0.24);
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      transition: transform 0.12s ease, box-shadow 0.12s ease,
        filter 0.16s ease;
    }

    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 22px 46px rgba(22, 28, 45, 0.3);
      filter: brightness(1.02);
    }

    .btn-ghost {
      border-radius: 999px;
      padding: 0.75rem 1.4rem;
      font-size: 0.82rem;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      background: transparent;
      border: 1px solid rgba(107, 114, 128, 0.28);
      color: var(--accent);
      cursor: pointer;
      font-weight: 500;
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      transition: background 0.14s ease, border-color 0.14s ease;
    }

    .btn-ghost:hover {
      background: rgba(255, 255, 255, 0.75);
      border-color: rgba(55, 65, 81, 0.6);
    }

    .hero-note {
      font-size: 0.76rem;
      color: var(--muted);
    }

    .hero-note span {
      font-weight: 600;
      color: var(--accent);
    }

    .hero-card {
      background: rgba(255, 255, 255, 0.92);
      border-radius: var(--radius-lg);
      padding: 1.3rem 1.4rem 1.2rem;
      box-shadow: var(--shadow-soft);
      border: 1px solid rgba(148, 120, 78, 0.22);
      position: relative;
      overflow: hidden;
    }

    .hero-card-label {
      text-transform: uppercase;
      font-size: 0.74rem;
      letter-spacing: 0.16em;
      color: var(--muted);
      margin-bottom: 0.5rem;
    }

    .hero-card-main {
      display: grid;
      grid-template-columns: auto minmax(0, 1fr);
      gap: 1rem;
      align-items: center;
      margin-bottom: 1rem;
    }

    .hero-illus {
      width: 60px;
      height: 60px;
      border-radius: 18px;
      background: radial-gradient(circle at 20% 0, #fff 0, #f0e1cf 45%, #d2b184 100%);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.6rem;
    }

    .hero-card h3 {
      font-size: 1rem;
      margin-bottom: 0.3rem;
    }

    .hero-card p {
      font-size: 0.86rem;
      color: var(--muted);
    }

    .hero-card-rows {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 0.7rem;
      font-size: 0.8rem;
      margin-top: 0.4rem;
    }

    .hero-card-row {
      background: #f9f4ec;
      border-radius: 10px;
      padding: 0.55rem 0.7rem;
    }

    .hero-card-row span.label {
      display: block;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.13em;
      color: #8b7354;
      margin-bottom: 0.18rem;
      font-weight: 600;
    }

    .hero-card-row span.value {
      font-weight: 500;
      color: var(--accent);
    }

    .hero-card-badge {
      position: absolute;
      right: 1rem;
      bottom: 0.9rem;
      font-size: 0.72rem;
      padding: 0.4rem 0.75rem;
      border-radius: 999px;
      background: rgba(22, 28, 45, 0.96);
      color: #fefaf3;
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
    }

    .hero-card-badge span.dot {
      width: 7px;
      height: 7px;
      border-radius: 50%;
      background: #34d399;
    }

    /* SECTION HEADINGS */

    .section-heading {
      text-align: center;
      margin-bottom: 2.1rem;
    }

    .section-heading h2 {
      font-size: 1.4rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      margin-bottom: 0.6rem;
    }

    .section-heading p {
      font-size: 0.9rem;
      color: var(--muted);
      max-width: 28rem;
      margin: 0.3rem auto 0;
    }

    /* HOW IT WORKS */

    .steps {
      display: grid;
      gap: 1rem;
      max-width: 680px;
      margin: 0 auto;
    }

    .step {
      display: grid;
      grid-template-columns: auto minmax(0, 1fr);
      gap: 0.8rem;
      align-items: flex-start;
    }

    .step-number {
      width: 26px;
      height: 26px;
      border-radius: 999px;
      border: 1px solid rgba(148, 120, 78, 0.5);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.8rem;
      font-weight: 600;
      background: #fdf7ef;
    }

    .step h3 {
      font-size: 0.96rem;
      margin-bottom: 0.2rem;
    }

    .step p {
      font-size: 0.86rem;
      color: var(--muted);
    }

    /* PLANS */

    .plans-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 1.2rem;
    }

    .plan {
      background: var(--card);
      border-radius: var(--radius-lg);
      padding: 1.4rem 1.5rem 1.3rem;
      box-shadow: var(--shadow-soft);
      border: 1px solid rgba(148, 120, 78, 0.18);
      display: flex;
      flex-direction: column;
      gap: 0.6rem;
    }

    .plan-label {
      text-transform: uppercase;
      letter-spacing: 0.14em;
      font-size: 0.74rem;
      color: var(--muted);
    }

    .plan-name {
      font-size: 1.05rem;
      font-weight: 600;
      color: var(--accent);
    }

    .plan-price {
      font-size: 1.1rem;
      font-weight: 600;
      margin-top: 0.3rem;
    }

    .plan-price span {
      font-size: 0.78rem;
      font-weight: 500;
      color: var(--muted);
      margin-left: 0.2rem;
    }

    .plan-list {
      margin-top: 0.4rem;
      display: grid;
      gap: 0.35rem;
      font-size: 0.85rem;
      color: var(--muted);
    }

    .plan-list-item {
      display: flex;
      gap: 0.4rem;
      align-items: flex-start;
    }

    .plan-list-item span.dot {
      margin-top: 0.32rem;
      width: 5px;
      height: 5px;
      border-radius: 50%;
      background: rgba(148, 120, 78, 0.9);
    }

    .plan-footer {
      margin-top: 0.8rem;
      font-size: 0.78rem;
      color: var(--muted);
    }

    .plan-cta {
      margin-top: 0.7rem;
      padding-top: 0.7rem;
      border-top: 1px dashed rgba(148, 120, 78, 0.35);
      font-size: 0.8rem;
      color: var(--accent);
    }

    .plan-cta strong {
      font-weight: 600;
    }

    /* FAQ & CONTACT */

    .faq-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(0, 1fr);
      gap: 1.8rem;
      align-items: flex-start;
    }

    .faq-list {
      display: grid;
      gap: 0.8rem;
    }

    .faq-item {
      background: rgba(255, 255, 255, 0.92);
      border-radius: var(--radius-md);
      padding: 0.9rem 1rem;
      border: 1px solid rgba(148, 120, 78, 0.16);
    }

    .faq-item h3 {
      font-size: 0.9rem;
      margin-bottom: 0.2rem;
    }

    .faq-item p {
      font-size: 0.84rem;
      color: var(--muted);
    }

    .contact-card {
      background: #151821;
      color: #f9f4eb;
      border-radius: var(--radius-lg);
      padding: 1.3rem 1.4rem;
      box-shadow: 0 18px 40px rgba(15, 23, 42, 0.66);
    }

    .contact-card h3 {
      font-size: 0.98rem;
      margin-bottom: 0.4rem;
    }

    .contact-card p {
      font-size: 0.86rem;
      margin-bottom: 0.9rem;
      color: #e5dfd5;
    }

    .contact-row {
      display: grid;
      gap: 0.45rem;
      font-size: 0.84rem;
    }

    .contact-row div span.label {
      display: block;
      font-size: 0.72rem;
      text-transform: uppercase;
      letter-spacing: 0.16em;
      color: #9ca3af;
      margin-bottom: 0.1rem;
    }

    .contact-row a {
      text-decoration: underline;
      text-underline-offset: 2px;
    }

    footer {
      padding: 1.8rem 1.1rem 2.2rem;
      font-size: 0.78rem;
      color: var(--muted);
    }

    footer .footer-inner {
      max-width: var(--max-width);
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      gap: 1rem;
      flex-wrap: wrap;
    }

    @media (max-width: 880px) {
      .nav-links {
        display: none;
      }

      .hero-grid {
        grid-template-columns: minmax(0, 1fr);
      }

      .hero-card {
        order: -1;
      }

      .plans-grid {
        grid-template-columns: minmax(0, 1fr);
      }

      .faq-grid {
        grid-template-columns: minmax(0, 1fr);
      }
    }

    @media (max-width: 520px) {
      header {
        position: static;
      }

      section {
        padding-inline: 1rem;
      }

      .hero {
        padding-top: 2rem;
      }

      .hero-card-rows {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }
  </style>
</head>
<body>
  <div class="page">
    <header>
      <nav class="nav">
        <div class="brand">
          <div class="brand-mark">CE</div>
          <div class="brand-text">
            <span>Cebu Essentials Club</span>
            <span>Filipino Pantry Subscription</span>
          </div>
        </div>
        <div class="nav-links">
          <a href="#how">How It Works</a>
          <a href="#plans">Plans</a>
          <a href="#faq">FAQ</a>
          <a href="#contact">Contact</a>
        </div>
        <button class="nav-cta" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">
          Join the Club
        </button>
      </nav>
    </header>

    <main>
      <!-- HERO -->
      <section class="hero">
        <div class="container hero-grid">
          <div>
            <div class="hero-tag">
              <span class="dot"></span>
              Cebu-based • Loved by families in the USA
            </div>
            <h1>
              Elegant <span class="accent">Filipino pantry</span><br />
              support for Cebu homes.
            </h1>
            <p class="hero-subtitle">
              <strong>Cebu Essentials Club</strong> is a weekly or monthly
              subscription of carefully selected <strong>Filipino household
              staples</strong> — ordered by clients in the USA, delivered with
              care to families in Cebu City.
            </p>

            <div class="hero-list">
              <div class="hero-list-item">
                <span class="bullet"></span>
                <span>Predictable support: choose weekly or monthly delivery.</span>
              </div>
              <div class="hero-list-item">
                <span class="bullet"></span>
                <span>Core staples only — rice, canned goods, condiments, coffee, and home essentials.</span>
              </div>
              <div class="hero-list-item">
                <span class="bullet"></span>
                <span>White-glove coordination from order to doorstep in Cebu.</span>
              </div>
            </div>

            <div class="hero-actions">
              <button class="btn-primary" onclick="document.getElementById('plans').scrollIntoView({behavior:'smooth'})">
                View Subscription Plans
              </button>
              <button class="btn-ghost" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">
                Arrange a Custom Box
              </button>
            </div>
            <p class="hero-note">
              Serving clients in the <span>United States</span> with deliveries
              to <span>Cebu City and nearby areas</span>.
            </p>
          </div>

          <div>
            <div class="hero-card">
              <div class="hero-card-label">A Glimpse Inside</div>
              <div class="hero-card-main">
                <div class="hero-illus">🥥</div>
                <div>
                  <h3>Curated Filipino Essentials</h3>
                  <p>
                    Every box is hand-assembled in Cebu — with quality staples
                    selected to support everyday Filipino home life.
                  </p>
                </div>
              </div>
              <div class="hero-card-rows">
                <div class="hero-card-row">
                  <span class="label">Core Staples</span>
                  <span class="value">Rice, canned goods, noodles, coffee</span>
                </div>
                <div class="hero-card-row">
                  <span class="label">Home Needs</span>
                  <span class="value">Soap, detergent & cleaning basics</span>
                </div>
                <div class="hero-card-row">
                  <span class="label">Optional Touches</span>
                  <span class="value">Cebu treats & kids’ snacks</span>
                </div>
              </div>
              <div class="hero-card-badge">
                <span class="dot"></span>
                Slots open for new members this month
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- HOW IT WORKS -->
      <section id="how">
        <div class="container">
          <div class="section-heading">
            <h2>How It Works</h2>
            <p>
              A calm, simple process — designed for clients abroad who want to
              quietly support loved ones in Cebu.
            </p>
          </div>
          <div class="steps">
            <div class="step">
              <div class="step-number">1</div>
              <div>
                <h3>Select a subscription plan</h3>
                <p>
                  Choose weekly or monthly deliveries and the type of box that
                  best fits your family’s needs in Cebu.
                </p>
              </div>
            </div>
            <div class="step">
              <div class="step-number">2</div>
              <div>
                <h3>Share your recipient details</h3>
                <p>
                  Send us your recipient’s full name, address in Cebu City
                  (or nearby), and preferred delivery days.
                </p>
              </div>
            </div>
            <div class="step">
              <div class="step-number">3</div>
              <div>
                <h3>We curate, purchase, and deliver</h3>
                <p>
                  We personally shop, assemble your box, and coordinate
                  delivery — with confirmation sent to you after each drop-off.
                </p>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- PLANS -->
      <section id="plans">
        <div class="container">
          <div class="section-heading">
            <h2>Subscription Plans</h2>
            <p>
              Sample structure only — final prices and contents can be adjusted
              to your budget and family size.
            </p>
          </div>

          <div class="plans-grid">
            <div class="plan">
              <div class="plan-label">Weekly</div>
              <div class="plan-name">Essentials Box</div>
              <div class="plan-price">
                ₱1,200–₱1,800
                <span>/ week (estimate)</span>
              </div>
              <div class="plan-list">
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Rice (1–2 kilos)</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Canned goods & instant noodles</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Eggs or bread (as available)</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Basic coffee & sugar</span>
                </div>
              </div>
              <p class="plan-footer">
                Ideal for light but consistent weekly support for a small
                household.
              </p>
              <p class="plan-cta">
                <strong>Note:</strong> Exact price and contents will be
                finalized with you before your first delivery.
              </p>
            </div>

            <div class="plan">
              <div class="plan-label">Monthly</div>
              <div class="plan-name">Home Staples Box</div>
              <div class="plan-price">
                ₱3,500–₱5,000
                <span>/ month (estimate)</span>
              </div>
              <div class="plan-list">
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Rice (5–10 kilos)</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Cooking oil, soy sauce, vinegar, basic condiments</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Canned goods & noodles for the month</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Laundry soap, dishwashing liquid, bathroom soap</span>
                </div>
              </div>
              <p class="plan-footer">
                A balanced monthly box focused on pantry and household needs.
              </p>
              <p class="plan-cta">
                <strong>Most popular.</strong> Perfect for families who want
                reliable, quiet support every month.
              </p>
            </div>

            <div class="plan">
              <div class="plan-label">Signature</div>
              <div class="plan-name">Pamilya Club Box</div>
              <div class="plan-price">
                ₱5,500+ 
                <span>/ month (custom)</span>
              </div>
              <div class="plan-list">
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>All Home Staples Box inclusions</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Extra snacks, kids’ baon items, Cebu delicacies</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Optional: hygiene items, vitamins, special requests</span>
                </div>
                <div class="plan-list-item">
                  <span class="dot"></span>
                  <span>Personal coordination for birthdays & occasions</span>
                </div>
              </div>
              <p class="plan-footer">
                A tailored experience for families who prefer a more generous,
                curated support box.
              </p>
              <p class="plan-cta">
                <strong>For this plan:</strong> we will schedule a short call
                or chat to understand your preferences.
              </p>
            </div>
          </div>
        </div>
      </section>

      <!-- FAQ + CONTACT -->
      <section id="faq">
        <div class="container faq-grid">
          <div>
            <div class="section-heading" style="text-align:left;margin-bottom:1.4rem;">
              <h2>Questions, Answered</h2>
              <p>
                Transparent, simple, and human — just as support for family
                should be.
              </p>
            </div>
            <div class="faq-list">
              <div class="faq-item">
                <h3>Are these prices final?</h3>
                <p>
                  No — all amounts shown here are estimates. We will confirm
                  your budget in pesos, create a sample contents list, and get
                  your approval before we begin your subscription.
                </p>
              </div>
              <div class="faq-item">
                <h3>Where do you deliver?</h3>
                <p>
                  We are based in Cebu City and can deliver within Cebu City
                  and selected nearby areas. For locations farther out, we
                  will discuss options with you first.
                </p>
              </div>
              <div class="faq-item">
                <h3>How do payments work from the USA?</h3>
                <p>
                  You may pay in USD through commonly used digital methods
                  (such as bank transfer or remittance). We’ll provide clear
                  instructions once you decide on a plan.
                </p>
              </div>
              <div class="faq-item">
                <h3>Can I pause or change my subscription?</h3>
                <p>
                  Yes. You can pause, skip, or adjust your box with prior
                  notice. We understand that life and budgets can change.
                </p>
              </div>
            </div>
          </div>

          <div id="contact">
            <div class="contact-card">
              <h3>Begin Your Subscription Conversation</h3>
              <p>
                Whether you already know your budget or you’re just exploring
                options, you’re welcome to reach out. We’ll respond with calm,
                clear details — no pressure.
              </p>
              <div class="contact-row">
                <div>
                  <span class="label">Email</span>
                  <a href="mailto:hello@cebuessentialsclub.com">
                    hello@cebuessentialsclub.com
                  </a>
                </div>
                <div>
                  <span class="label">WhatsApp / Viber</span>
                  <a href="https://wa.me/15551234567" target="_blank">
                    +1 (555) 123-4567
                  </a>
                </div>
                <div>
                  <span class="label">Cebu Time</span>
                  <span>We typically reply within the day during PH business hours.</span>
                </div>
              </div>
            </div>
          </div>

        </div>
      </section>
    </main>

    <footer>
      <div class="footer-inner">
        <div>© <span id="year"></span> Cebu Essentials Club. All rights reserved.</div>
        <div>Quiet, thoughtful support for families in Cebu.</div>
      </div>
    </footer>
  </div>

  <script>
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
