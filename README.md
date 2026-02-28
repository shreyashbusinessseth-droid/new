<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Viva Beauty Salon Varanasi – Best Beauty Salon</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --rose: #c9736a;
    --rose-light: #e8a09a;
    --rose-dark: #9e4e47;
    --gold: #c9a96e;
    --gold-light: #e8d5b0;
    --cream: #fdf8f4;
    --cream-dark: #f5ede4;
    --text: #2a1f1c;
    --text-soft: #6b4f4a;
    --white: #ffffff;
    --shadow: 0 4px 24px rgba(201,115,106,0.13);
    --shadow-lg: 0 12px 40px rgba(201,115,106,0.2);
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--cream);
    color: var(--text);
    overflow-x: hidden;
  }

  /* ========== HEADER ========== */
  header {
    position: sticky; top: 0; z-index: 100;
    background: rgba(253,248,244,0.95);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--gold-light);
    padding: 0 1.2rem;
  }
  .header-inner {
    max-width: 1100px; margin: 0 auto;
    display: flex; align-items: center; justify-content: space-between;
    height: 64px;
  }
  .logo { display: flex; flex-direction: column; line-height: 1.1; }
  .logo-name {
    font-family: 'Playfair Display', serif;
    font-size: 1.25rem; font-weight: 700;
    color: var(--rose-dark);
    letter-spacing: 0.02em;
  }
  .logo-tag {
    font-size: 0.68rem; font-weight: 300;
    color: var(--gold); letter-spacing: 0.12em; text-transform: uppercase;
  }
  .header-right { display: flex; align-items: center; gap: 0.8rem; }
  .cart-btn {
    position: relative; background: var(--rose); color: #fff;
    border: none; border-radius: 50px; padding: 0.45rem 1rem;
    font-family: 'DM Sans', sans-serif; font-size: 0.85rem; font-weight: 500;
    cursor: pointer; display: flex; align-items: center; gap: 0.4rem;
    transition: background 0.2s, transform 0.15s;
    box-shadow: 0 2px 12px rgba(201,115,106,0.3);
  }
  .cart-btn:hover { background: var(--rose-dark); transform: translateY(-1px); }
  .cart-count {
    background: var(--gold); color: var(--text);
    border-radius: 50%; width: 18px; height: 18px;
    font-size: 0.7rem; font-weight: 700;
    display: none; align-items: center; justify-content: center;
  }
  .cart-count.show { display: flex; }

  /* ========== HERO ========== */
  .hero {
    position: relative; height: 88vw; max-height: 560px; min-height: 320px;
    overflow: hidden;
  }
  .hero img {
    width: 100%; height: 100%; object-fit: cover; object-position: center top;
    display: block;
  }
  .hero-overlay {
    position: absolute; inset: 0;
    background: linear-gradient(to bottom, rgba(42,31,28,0.1) 0%, rgba(42,31,28,0.55) 100%);
    display: flex; align-items: flex-end; padding: 2.5rem 1.5rem;
  }
  .hero-text { color: #fff; }
  .hero-text h1 {
    font-family: 'Playfair Display', serif;
    font-size: clamp(2rem, 7vw, 3.5rem);
    line-height: 1.1; margin-bottom: 0.4rem;
  }
  .hero-text p {
    font-size: 1rem; font-weight: 300; opacity: 0.9;
    letter-spacing: 0.04em;
  }
  .hero-text .hero-cta {
    margin-top: 1rem; display: inline-block;
    background: var(--gold); color: var(--text);
    padding: 0.6rem 1.6rem; border-radius: 50px;
    font-weight: 500; font-size: 0.9rem; text-decoration: none;
    transition: background 0.2s, transform 0.15s;
    box-shadow: 0 2px 12px rgba(201,169,110,0.4);
  }
  .hero-text .hero-cta:hover { background: var(--gold-light); transform: translateY(-1px); }

  /* ========== SECTION TITLE ========== */
  .section-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.6rem; color: var(--rose-dark);
    text-align: center; margin-bottom: 0.3rem;
  }
  .section-sub {
    text-align: center; color: var(--text-soft);
    font-size: 0.85rem; font-weight: 300; margin-bottom: 1.8rem;
    letter-spacing: 0.06em; text-transform: uppercase;
  }

  /* ========== CATEGORIES ========== */
  .categories-section { padding: 2.5rem 1.2rem 0; max-width: 1100px; margin: 0 auto; }
  .cat-scroll {
    display: flex; gap: 0.6rem; overflow-x: auto; padding-bottom: 0.5rem;
    scrollbar-width: none;
  }
  .cat-scroll::-webkit-scrollbar { display: none; }
  .cat-btn {
    flex-shrink: 0; padding: 0.45rem 1.2rem;
    border: 1.5px solid var(--rose-light); border-radius: 50px;
    background: transparent; color: var(--text-soft);
    font-family: 'DM Sans', sans-serif; font-size: 0.82rem; font-weight: 500;
    cursor: pointer; transition: all 0.2s; white-space: nowrap;
    letter-spacing: 0.03em;
  }
  .cat-btn:hover, .cat-btn.active {
    background: var(--rose); color: #fff; border-color: var(--rose);
    box-shadow: 0 2px 10px rgba(201,115,106,0.25);
  }

  /* ========== SERVICES GRID ========== */
  .services-section { padding: 2rem 1.2rem 3rem; max-width: 1100px; margin: 0 auto; }
  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
    gap: 1.3rem;
  }
  .service-card {
    background: var(--white); border-radius: 18px;
    overflow: hidden; box-shadow: var(--shadow);
    transition: transform 0.25s, box-shadow 0.25s;
    display: flex; flex-direction: column;
  }
  .service-card:hover { transform: translateY(-4px); box-shadow: var(--shadow-lg); }
  .card-img-wrap { position: relative; overflow: hidden; height: 200px; }
  .card-img-wrap img {
    width: 100%; height: 100%; object-fit: cover;
    transition: transform 0.4s ease;
  }
  .service-card:hover .card-img-wrap img { transform: scale(1.06); }
  .card-badge {
    position: absolute; top: 10px; left: 10px;
    background: rgba(253,248,244,0.92); color: var(--rose-dark);
    font-size: 0.65rem; font-weight: 600; padding: 0.25rem 0.7rem;
    border-radius: 50px; letter-spacing: 0.08em; text-transform: uppercase;
  }
  .card-body { padding: 1rem 1.1rem 1.2rem; flex: 1; display: flex; flex-direction: column; }
  .card-name {
    font-family: 'Playfair Display', serif;
    font-size: 1.05rem; font-weight: 700; color: var(--text);
    margin-bottom: 0.3rem;
  }
  .card-desc { font-size: 0.78rem; color: var(--text-soft); margin-bottom: 0.8rem; flex: 1; line-height: 1.5; }
  .card-footer { display: flex; align-items: center; justify-content: space-between; gap: 0.5rem; }
  .card-price {
    font-size: 1.15rem; font-weight: 700; color: var(--rose-dark);
    font-family: 'Playfair Display', serif;
  }
  .book-btn {
    background: linear-gradient(135deg, var(--rose), var(--rose-dark));
    color: #fff; border: none; border-radius: 50px;
    padding: 0.45rem 1.1rem; font-family: 'DM Sans', sans-serif;
    font-size: 0.82rem; font-weight: 500; cursor: pointer;
    transition: opacity 0.2s, transform 0.15s;
    box-shadow: 0 2px 10px rgba(201,115,106,0.3);
  }
  .book-btn:hover { opacity: 0.88; transform: translateY(-1px); }
  .book-btn.added { background: linear-gradient(135deg, var(--gold), #a07d3a); }

  /* ========== CART MODAL ========== */
  .modal-overlay {
    position: fixed; inset: 0; z-index: 200;
    background: rgba(42,31,28,0.55); backdrop-filter: blur(4px);
    display: none; align-items: flex-end; justify-content: center;
  }
  .modal-overlay.open { display: flex; }
  .cart-modal {
    background: var(--white); width: 100%; max-width: 520px;
    border-radius: 24px 24px 0 0; padding: 1.5rem 1.3rem 2rem;
    max-height: 90vh; overflow-y: auto;
    animation: slideUp 0.3s ease;
  }
  @keyframes slideUp { from { transform: translateY(100%); } to { transform: translateY(0); } }
  .modal-header {
    display: flex; align-items: center; justify-content: space-between;
    margin-bottom: 1.2rem;
  }
  .modal-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.3rem; color: var(--rose-dark);
  }
  .close-btn {
    background: var(--cream-dark); border: none; border-radius: 50%;
    width: 36px; height: 36px; cursor: pointer; font-size: 1.1rem;
    display: flex; align-items: center; justify-content: center;
    color: var(--text-soft); transition: background 0.2s;
  }
  .close-btn:hover { background: var(--rose-light); color: #fff; }
  .cart-items { display: flex; flex-direction: column; gap: 0.8rem; margin-bottom: 1.2rem; }
  .cart-item {
    display: flex; align-items: center; gap: 0.9rem;
    background: var(--cream); border-radius: 14px; padding: 0.8rem;
    animation: fadeIn 0.2s ease;
  }
  @keyframes fadeIn { from { opacity: 0; transform: translateY(8px); } to { opacity: 1; transform: none; } }
  .cart-item-name { flex: 1; font-size: 0.9rem; font-weight: 500; color: var(--text); }
  .cart-item-price { font-size: 0.82rem; color: var(--text-soft); margin-top: 0.1rem; }
  .qty-ctrl { display: flex; align-items: center; gap: 0.4rem; }
  .qty-btn {
    background: var(--white); border: 1.5px solid var(--rose-light);
    border-radius: 50%; width: 28px; height: 28px;
    cursor: pointer; font-size: 1rem; display: flex;
    align-items: center; justify-content: center; color: var(--rose-dark);
    transition: all 0.15s; font-weight: 700;
  }
  .qty-btn:hover { background: var(--rose); color: #fff; border-color: var(--rose); }
  .qty-num { font-weight: 700; font-size: 0.9rem; min-width: 20px; text-align: center; }
  .remove-btn {
    background: none; border: none; color: var(--rose-light);
    cursor: pointer; font-size: 1.1rem; padding: 0 0.2rem;
    transition: color 0.15s;
  }
  .remove-btn:hover { color: var(--rose-dark); }
  .cart-total-row {
    display: flex; justify-content: space-between; align-items: center;
    border-top: 1.5px solid var(--cream-dark); padding-top: 1rem; margin-top: 0.5rem;
  }
  .cart-total-label { font-size: 0.95rem; color: var(--text-soft); font-weight: 500; }
  .cart-total-val {
    font-family: 'Playfair Display', serif;
    font-size: 1.4rem; color: var(--rose-dark); font-weight: 700;
  }
  .checkout-btn {
    width: 100%; margin-top: 1rem;
    background: linear-gradient(135deg, var(--rose), var(--rose-dark));
    color: #fff; border: none; border-radius: 50px;
    padding: 0.85rem; font-family: 'DM Sans', sans-serif;
    font-size: 1rem; font-weight: 600; cursor: pointer;
    transition: opacity 0.2s, transform 0.15s;
    box-shadow: 0 4px 16px rgba(201,115,106,0.35);
    letter-spacing: 0.02em;
  }
  .checkout-btn:hover { opacity: 0.88; transform: translateY(-1px); }
  .empty-cart {
    text-align: center; padding: 2rem 1rem;
    color: var(--text-soft); font-size: 0.95rem;
  }
  .empty-cart .empty-icon { font-size: 2.5rem; margin-bottom: 0.5rem; }

  /* ========== CHECKOUT FORM MODAL ========== */
  .checkout-modal {
    background: var(--white); width: 100%; max-width: 520px;
    border-radius: 24px 24px 0 0; padding: 1.5rem 1.3rem 2rem;
    max-height: 95vh; overflow-y: auto;
    animation: slideUp 0.3s ease;
  }
  .form-group { margin-bottom: 1rem; }
  .form-group label {
    display: block; font-size: 0.8rem; font-weight: 600;
    color: var(--text-soft); margin-bottom: 0.35rem;
    letter-spacing: 0.05em; text-transform: uppercase;
  }
  .form-group input,
  .form-group textarea,
  .form-group select {
    width: 100%; padding: 0.7rem 1rem;
    border: 1.5px solid var(--cream-dark); border-radius: 12px;
    font-family: 'DM Sans', sans-serif; font-size: 0.9rem;
    color: var(--text); background: var(--cream);
    transition: border-color 0.2s, box-shadow 0.2s;
    outline: none;
  }
  .form-group input:focus,
  .form-group textarea:focus {
    border-color: var(--rose-light);
    box-shadow: 0 0 0 3px rgba(201,115,106,0.1);
  }
  .form-group textarea { resize: vertical; min-height: 80px; }
  .order-summary-box {
    background: var(--cream); border-radius: 14px;
    padding: 1rem; margin-bottom: 1rem;
    font-size: 0.85rem;
  }
  .order-summary-box h4 {
    font-family: 'Playfair Display', serif;
    font-size: 0.95rem; color: var(--rose-dark); margin-bottom: 0.6rem;
  }
  .order-summary-item {
    display: flex; justify-content: space-between;
    padding: 0.25rem 0; border-bottom: 1px solid var(--cream-dark);
    color: var(--text-soft);
  }
  .order-summary-item:last-child { border-bottom: none; }
  .order-total-row {
    display: flex; justify-content: space-between;
    padding-top: 0.5rem; font-weight: 700;
    color: var(--rose-dark); font-size: 0.95rem;
  }
  .submit-btn {
    width: 100%;
    background: linear-gradient(135deg, var(--gold), #a07d3a);
    color: var(--text); border: none; border-radius: 50px;
    padding: 0.85rem; font-family: 'DM Sans', sans-serif;
    font-size: 1rem; font-weight: 600; cursor: pointer;
    transition: opacity 0.2s, transform 0.15s;
    box-shadow: 0 4px 16px rgba(201,169,110,0.35);
    letter-spacing: 0.02em;
  }
  .submit-btn:hover { opacity: 0.88; transform: translateY(-1px); }
  .back-link {
    background: none; border: none; color: var(--rose);
    font-family: 'DM Sans', sans-serif; font-size: 0.85rem;
    cursor: pointer; text-decoration: underline; margin-bottom: 0.5rem;
    display: inline-block;
  }

  /* ========== SUCCESS MESSAGE ========== */
  .success-modal {
    background: var(--white); width: 100%; max-width: 520px;
    border-radius: 24px 24px 0 0; padding: 2.5rem 1.3rem 2.5rem;
    animation: slideUp 0.3s ease; text-align: center;
  }
  .success-icon { font-size: 3.5rem; margin-bottom: 1rem; }
  .success-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.5rem; color: var(--rose-dark); margin-bottom: 0.5rem;
  }
  .success-msg { color: var(--text-soft); font-size: 0.9rem; line-height: 1.6; margin-bottom: 1.5rem; }
  .wa-link {
    display: inline-flex; align-items: center; gap: 0.5rem;
    background: #25d366; color: #fff;
    padding: 0.7rem 1.8rem; border-radius: 50px;
    text-decoration: none; font-weight: 600; font-size: 0.95rem;
    box-shadow: 0 4px 16px rgba(37,211,102,0.3);
    transition: opacity 0.2s, transform 0.15s;
  }
  .wa-link:hover { opacity: 0.88; transform: translateY(-1px); }
  .done-btn {
    display: block; margin: 1rem auto 0; background: none;
    border: 1.5px solid var(--rose-light); border-radius: 50px;
    padding: 0.6rem 2rem; color: var(--text-soft);
    font-family: 'DM Sans', sans-serif; font-size: 0.85rem;
    cursor: pointer; transition: all 0.2s;
  }
  .done-btn:hover { background: var(--cream-dark); }

  /* ========== FLOATING BUTTONS ========== */
  .fab-group {
    position: fixed; bottom: 1.5rem; right: 1.2rem;
    display: flex; flex-direction: column; align-items: flex-end; gap: 0.7rem;
    z-index: 90;
  }
  .fab-wa {
    display: flex; align-items: center; justify-content: center;
    width: 52px; height: 52px; border-radius: 50%;
    background: #25d366; color: #fff;
    text-decoration: none; font-size: 1.5rem;
    box-shadow: 0 4px 18px rgba(37,211,102,0.4);
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .fab-wa:hover { transform: scale(1.08); box-shadow: 0 6px 24px rgba(37,211,102,0.5); }
  .fab-cart {
    display: none; align-items: center; justify-content: center;
    width: 52px; height: 52px; border-radius: 50%;
    background: var(--rose); color: #fff;
    border: none; font-size: 1.3rem; cursor: pointer;
    box-shadow: var(--shadow-lg);
    transition: transform 0.2s;
    position: relative;
  }
  .fab-cart:hover { transform: scale(1.08); }
  .fab-cart.show { display: flex; }
  .fab-badge {
    position: absolute; top: -4px; right: -4px;
    background: var(--gold); color: var(--text);
    border-radius: 50%; width: 20px; height: 20px;
    font-size: 0.65rem; font-weight: 700;
    display: flex; align-items: center; justify-content: center;
    border: 2px solid var(--white);
  }

  /* ========== INFO SECTION ========== */
  .info-section {
    background: var(--text); color: var(--cream);
    padding: 2.5rem 1.2rem;
    text-align: center;
  }
  .info-section h3 {
    font-family: 'Playfair Display', serif;
    font-size: 1.3rem; color: var(--gold-light); margin-bottom: 1rem;
  }
  .info-grid {
    max-width: 600px; margin: 0 auto;
    display: grid; grid-template-columns: 1fr 1fr; gap: 1rem;
    text-align: left;
  }
  .info-item { font-size: 0.85rem; line-height: 1.6; }
  .info-item span { color: var(--gold-light); font-size: 0.7rem; text-transform: uppercase; letter-spacing: 0.08em; display: block; margin-bottom: 0.1rem; }
  .info-item a { color: var(--rose-light); text-decoration: none; }
  footer {
    background: var(--text); border-top: 1px solid rgba(255,255,255,0.08);
    text-align: center; padding: 1rem;
    font-size: 0.75rem; color: rgba(253,248,244,0.4);
  }

  /* ========== RESPONSIVE ========== */
  @media (max-width: 480px) {
    .services-grid { grid-template-columns: repeat(2, 1fr); gap: 0.9rem; }
    .card-img-wrap { height: 150px; }
    .card-name { font-size: 0.9rem; }
    .card-desc { display: none; }
    .info-grid { grid-template-columns: 1fr; }
  }
  @media (min-width: 768px) {
    .cart-modal, .checkout-modal, .success-modal {
      border-radius: 24px;
      position: fixed; top: 50%; left: 50%;
      transform: translate(-50%, -50%);
      bottom: auto;
    }
    .modal-overlay.open { align-items: center; }
    @keyframes slideUp { from { opacity: 0; transform: translate(-50%, -40%); } to { opacity: 1; transform: translate(-50%, -50%); } }
  }

  /* hidden fields */
  .hidden { display: none !important; }
</style>
</head>
<body>

<!-- HEADER -->
<header>
  <div class="header-inner">
    <div class="logo">
      <span class="logo-name">✦ Viva Beauty Salon</span>
      <span class="logo-tag">Varanasi · Best Beauty Salon</span>
    </div>
    <div class="header-right">
      <button class="cart-btn" onclick="openCart()">
        🛒 Cart
        <span class="cart-count" id="cartCountHeader">0</span>
      </button>
    </div>
  </div>
</header>

<!-- HERO -->
<section class="hero">
  <img src="https://i.ibb.co/Kp8J11MS/close-up-portrait-young-beatufiul-woman-looking-mirror-fixing-her-makeup-touching-soft-clear-skin-st.jpg"
    alt="Viva Beauty Salon Varanasi – Luxury Beauty Treatments" loading="eager">
  <div class="hero-overlay">
    <div class="hero-text">
      <h1>Glow. Shine.<br><em>Transform.</em></h1>
      <p>Premium Beauty Services in Varanasi</p>
      <a href="#services" class="hero-cta">Explore Services ↓</a>
    </div>
  </div>
</section>

<!-- CATEGORIES -->
<section class="categories-section" id="services">
  <p class="section-sub">Our Services</p>
  <div class="cat-scroll" id="catFilters">
    <button class="cat-btn active" data-cat="all" onclick="filterCat(this,'all')">All Services</button>
    <button class="cat-btn" data-cat="skin care" onclick="filterCat(this,'skin care')">Skin Care</button>
    <button class="cat-btn" data-cat="hair care" onclick="filterCat(this,'hair care')">Hair Care</button>
    <button class="cat-btn" data-cat="nail care" onclick="filterCat(this,'nail care')">Nail Care</button>
    <button class="cat-btn" data-cat="eyelashes extension" onclick="filterCat(this,'eyelashes extension')">Eyelashes</button>
    <button class="cat-btn" data-cat="massage" onclick="filterCat(this,'massage')">Massage</button>
    <button class="cat-btn" data-cat="makeup" onclick="filterCat(this,'makeup')">Makeup</button>
  </div>
</section>

<!-- SERVICES GRID -->
<section class="services-section">
  <div class="services-grid" id="servicesGrid"></div>
</section>

<!-- INFO SECTION -->
<section class="info-section">
  <h3>✦ Viva Beauty Salon Varanasi</h3>
  <div class="info-grid">
    <div class="info-item"><span>Location</span>Varanasi, Uttar Pradesh</div>
    <div class="info-item"><span>Phone</span><a href="tel:8299856640">8299856640</a></div>
    <div class="info-item"><span>Email</span><a href="mailto:shreyashseth2007@gmail.com">shreyashseth2007@gmail.com</a></div>
    <div class="info-item"><span>WhatsApp</span><a href="https://wa.me/918299856640" target="_blank">Chat with us</a></div>
  </div>
</section>
<footer>© 2024 Viva Beauty Salon Varanasi. All rights reserved.</footer>

<!-- FLOATING BUTTONS -->
<div class="fab-group">
  <a class="fab-wa" href="https://wa.me/918299856640" target="_blank" title="Chat on WhatsApp">
    <svg width="26" height="26" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
  </a>
  <button class="fab-cart" id="fabCart" onclick="openCart()">
    🛒
    <span class="fab-badge" id="fabBadge">0</span>
  </button>
</div>

<!-- CART MODAL -->
<div class="modal-overlay" id="cartOverlay" onclick="closeCartIfOutside(event)">
  <div class="cart-modal" id="cartModal">
    <div class="modal-header">
      <span class="modal-title">Your Cart</span>
      <button class="close-btn" onclick="closeCart()">✕</button>
    </div>
    <div id="cartContent"></div>
  </div>
</div>

<!-- CHECKOUT MODAL -->
<div class="modal-overlay" id="checkoutOverlay" onclick="closeCheckoutIfOutside(event)">
  <div class="checkout-modal" id="checkoutModal">
    <div class="modal-header">
      <span class="modal-title">Book Your Service</span>
      <button class="close-btn" onclick="closeCheckout()">✕</button>
    </div>
    <button class="back-link" onclick="closeCheckout();openCart()">← Back to cart</button>

    <div class="order-summary-box" id="checkoutSummary"></div>

    <form id="bookingForm" action="https://formspree.io/f/xjgezdgb" method="POST">
      <!-- Hidden fields populated by JS -->
      <input type="hidden" name="_subject" id="fSubject">
      <input type="hidden" name="Order Summary" id="fOrderSummary">
      <input type="hidden" name="Grand Total" id="fGrandTotal">
      <input type="hidden" name="_replyto" value="shreyashseth2007@gmail.com">

      <div class="form-group">
        <label>Your Name *</label>
        <input type="text" name="Customer Name" required placeholder="Enter your full name">
      </div>
      <div class="form-group">
        <label>Phone Number *</label>
        <input type="tel" name="Phone Number" required placeholder="e.g. 9876543210">
      </div>
      <div class="form-group">
        <label>Address / Area *</label>
        <input type="text" name="Address" required placeholder="Your address or area in Varanasi">
      </div>
      <div class="form-group">
        <label>Preferred Date & Time (optional)</label>
        <input type="text" name="Preferred Date & Time" placeholder="e.g. Sunday, 11am">
      </div>
      <div class="form-group">
        <label>Special Instructions (optional)</label>
        <textarea name="Special Instructions" placeholder="Any requests or notes for the salon…"></textarea>
      </div>
      <button type="submit" class="submit-btn">✦ Confirm Booking</button>
    </form>
  </div>
</div>

<!-- SUCCESS MODAL -->
<div class="modal-overlay" id="successOverlay">
  <div class="success-modal">
    <div class="success-icon">🌸</div>
    <div class="success-title">Service Booked!</div>
    <div class="success-msg">
      Thank you! Viva Beauty Salon will contact you on WhatsApp to confirm your appointment. See you soon! ✨
    </div>
    <a class="wa-link" href="https://wa.me/918299856640" target="_blank">
      <svg width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z"/></svg>
      Chat on WhatsApp
    </a>
    <button class="done-btn" onclick="closeSuccess()">Done</button>
  </div>
</div>

<script>
// ===== DATA =====
const SERVICES = [
  { id: 1, name: 'Skin Care', cat: 'skin care', price: 2000, desc: 'Hydrating facials, deep cleansing & glow treatments for radiant skin.', img: 'https://i.ibb.co/gFLQq02L/skin-care-1.webp', alt: 'Skin care facial treatment' },
  { id: 2, name: 'Hair Care', cat: 'hair care', price: 2000, desc: 'Nourishing treatments, styling, cuts & colour for beautiful hair.', img: 'https://i.ibb.co/RkT74d1r/hair-care.webp', alt: 'Professional hair care treatment' },
  { id: 3, name: 'Nail Care', cat: 'nail care', price: 2000, desc: 'Manicures, pedicures & nail art for perfectly polished nails.', img: 'https://i.ibb.co/bgL3rY4K/viva-nail-transformed.webp', alt: 'Nail care and nail art' },
  { id: 4, name: 'Makeup', cat: 'makeup', price: 2000, desc: 'Bridal, party & everyday makeup by expert artists.', img: 'https://i.ibb.co/Mkw6BGc1/Capture-One-Catalog0829-scaled.webp', alt: 'Professional makeup service' },
  { id: 5, name: 'Eyelashes Extension', cat: 'eyelashes extension', price: 2000, desc: 'Luscious, long-lasting eyelash extensions for a dramatic look.', img: 'https://i.ibb.co/gFLQq02L/skin-care-1.webp', alt: 'Eyelashes extension service' },
  { id: 6, name: 'Relaxing Massage', cat: 'massage', price: 2000, desc: 'Full body & head massage to de-stress and rejuvenate.', img: 'https://i.ibb.co/RkT74d1r/hair-care.webp', alt: 'Relaxing massage therapy' },
];

// ===== CART =====
let cart = JSON.parse(localStorage.getItem('vivaCart') || '[]');
let currentCat = 'all';

function saveCart() { localStorage.setItem('vivaCart', JSON.stringify(cart)); }

function addToCart(id) {
  const svc = SERVICES.find(s => s.id === id);
  const existing = cart.find(i => i.id === id);
  if (existing) { existing.qty++; } else { cart.push({ ...svc, qty: 1 }); }
  saveCart(); updateCartUI();
  // Animate button
  const btn = document.querySelector(`.book-btn[data-id="${id}"]`);
  if (btn) {
    btn.textContent = '✓ Added';
    btn.classList.add('added');
    setTimeout(() => { btn.textContent = 'Book Service'; btn.classList.remove('added'); }, 1200);
  }
}

function removeFromCart(id) {
  cart = cart.filter(i => i.id !== id);
  saveCart(); updateCartUI(); renderCartContent();
}

function changeQty(id, delta) {
  const item = cart.find(i => i.id === id);
  if (!item) return;
  item.qty += delta;
  if (item.qty <= 0) { removeFromCart(id); return; }
  saveCart(); updateCartUI(); renderCartContent();
}

function getTotal() { return cart.reduce((s, i) => s + i.price * i.qty, 0); }
function getTotalItems() { return cart.reduce((s, i) => s + i.qty, 0); }

function updateCartUI() {
  const n = getTotalItems();
  const hdr = document.getElementById('cartCountHeader');
  const fab = document.getElementById('fabCart');
  const badge = document.getElementById('fabBadge');
  hdr.textContent = n;
  badge.textContent = n;
  if (n > 0) { hdr.classList.add('show'); fab.classList.add('show'); }
  else { hdr.classList.remove('show'); fab.classList.remove('show'); }
}

// ===== RENDER SERVICES =====
function renderServices(cat) {
  const grid = document.getElementById('servicesGrid');
  const filtered = cat === 'all' ? SERVICES : SERVICES.filter(s => s.cat === cat);
  grid.innerHTML = filtered.map(s => `
    <div class="service-card">
      <div class="card-img-wrap">
        <img src="${s.img}" alt="${s.alt}" loading="lazy">
        <span class="card-badge">${s.cat}</span>
      </div>
      <div class="card-body">
        <div class="card-name">${s.name}</div>
        <div class="card-desc">${s.desc}</div>
        <div class="card-footer">
          <span class="card-price">₹${s.price.toLocaleString('en-IN')}</span>
          <button class="book-btn" data-id="${s.id}" onclick="addToCart(${s.id})">Book Service</button>
        </div>
      </div>
    </div>
  `).join('');
}

function filterCat(btn, cat) {
  document.querySelectorAll('.cat-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  currentCat = cat;
  renderServices(cat);
}

// ===== CART MODAL =====
function openCart() {
  renderCartContent();
  document.getElementById('cartOverlay').classList.add('open');
  document.body.style.overflow = 'hidden';
}
function closeCart() {
  document.getElementById('cartOverlay').classList.remove('open');
  document.body.style.overflow = '';
}
function closeCartIfOutside(e) { if (e.target === document.getElementById('cartOverlay')) closeCart(); }

function renderCartContent() {
  const el = document.getElementById('cartContent');
  if (cart.length === 0) {
    el.innerHTML = `<div class="empty-cart"><div class="empty-icon">🛒</div>No services added yet.<br>Browse our services below!</div>`;
    return;
  }
  const itemsHTML = cart.map(i => `
    <div class="cart-item">
      <div style="flex:1">
        <div class="cart-item-name">${i.name}</div>
        <div class="cart-item-price">₹${(i.price * i.qty).toLocaleString('en-IN')} (₹${i.price.toLocaleString('en-IN')} × ${i.qty})</div>
      </div>
      <div class="qty-ctrl">
        <button class="qty-btn" onclick="changeQty(${i.id},-1)">−</button>
        <span class="qty-num">${i.qty}</span>
        <button class="qty-btn" onclick="changeQty(${i.id},1)">+</button>
      </div>
      <button class="remove-btn" onclick="removeFromCart(${i.id})" title="Remove">✕</button>
    </div>
  `).join('');
  el.innerHTML = `
    <div class="cart-items">${itemsHTML}</div>
    <div class="cart-total-row">
      <span class="cart-total-label">Grand Total</span>
      <span class="cart-total-val">₹${getTotal().toLocaleString('en-IN')}</span>
    </div>
    <button class="checkout-btn" onclick="closeCart();openCheckout()">Proceed to Book →</button>
  `;
}

// ===== CHECKOUT =====
function openCheckout() {
  if (cart.length === 0) { openCart(); return; }
  // Populate order summary box
  const box = document.getElementById('checkoutSummary');
  const itemRows = cart.map(i => `
    <div class="order-summary-item">
      <span>${i.name} × ${i.qty}</span>
      <span>₹${(i.price * i.qty).toLocaleString('en-IN')}</span>
    </div>`).join('');
  box.innerHTML = `<h4>📋 Order Summary</h4>${itemRows}
    <div class="order-total-row"><span>Grand Total</span><span>₹${getTotal().toLocaleString('en-IN')}</span></div>`;

  // Populate hidden fields
  document.getElementById('fSubject').value = `New Booking – Viva Beauty Salon (₹${getTotal().toLocaleString('en-IN')})`;
  const summary = cart.map(i => `${i.name} x${i.qty} = ₹${(i.price*i.qty).toLocaleString('en-IN')}`).join(' | ');
  document.getElementById('fOrderSummary').value = summary;
  document.getElementById('fGrandTotal').value = `₹${getTotal().toLocaleString('en-IN')}`;

  document.getElementById('checkoutOverlay').classList.add('open');
  document.body.style.overflow = 'hidden';
}
function closeCheckout() {
  document.getElementById('checkoutOverlay').classList.remove('open');
  document.body.style.overflow = '';
}
function closeCheckoutIfOutside(e) { if (e.target === document.getElementById('checkoutOverlay')) closeCheckout(); }

// ===== FORM SUBMIT =====
document.getElementById('bookingForm').addEventListener('submit', async function(e) {
  e.preventDefault();
  const btn = this.querySelector('.submit-btn');
  btn.textContent = 'Booking…'; btn.disabled = true;
  const data = new FormData(this);
  try {
    const res = await fetch(this.action, { method: 'POST', body: data, headers: { 'Accept': 'application/json' } });
    if (res.ok) {
      cart = []; saveCart(); updateCartUI();
      closeCheckout();
      document.getElementById('successOverlay').classList.add('open');
      this.reset();
    } else {
      alert('Submission failed. Please try again or contact us on WhatsApp.');
    }
  } catch(err) {
    alert('Network error. Please try again or contact us on WhatsApp.');
  }
  btn.textContent = '✦ Confirm Booking'; btn.disabled = false;
});

function closeSuccess() {
  document.getElementById('successOverlay').classList.remove('open');
  document.body.style.overflow = '';
}

// ===== INIT =====
renderServices('all');
updateCartUI();
</script>
</body>
</html>
