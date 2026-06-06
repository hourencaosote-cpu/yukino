[yukino.html](https://github.com/user-attachments/files/28668271/yukino.html)
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ゆきの｜沖縄・名護の定食居酒屋 — 郷土料理と豊富なメニューが揃う名護の名店</title>
  <meta name="description" content="沖縄県名護市宮里にある定食・居酒屋「ゆきの」。アグー豚や沖縄そば、新鮮な刺身など50種以上の定食と豊富な沖縄料理をリーズナブルにご提供。ホテルゆがふいん真裏・予約歓迎。">
  <meta name="keywords" content="ゆきの,名護,居酒屋,定食,沖縄料理,とんかつ,アグー,沖縄そば,名護市,沖縄">
  <meta property="og:title" content="ゆきの｜沖縄・名護の定食居酒屋">
  <meta property="og:description" content="50種以上の定食と豊富な沖縄料理。名護市の名店「ゆきの」へようこそ。">
  <meta property="og:type" content="website">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Shippori+Mincho:wght@400;500;600;700&family=Noto+Serif+JP:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --ink: #1a1209;
      --gold: #b8965a;
      --gold-light: #d4af72;
      --gold-pale: #f0e4c8;
      --cream: #faf6ef;
      --warm-white: #fffdf8;
      --stone: #8c7b6b;
      --stone-light: #c4b5a5;
      --deep: #0e0b07;
      --rust: #8b3a2a;
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'Noto Serif JP', 'Shippori Mincho', serif;
      background: var(--warm-white);
      color: var(--ink);
      overflow-x: hidden;
    }

    /* ── SCROLLBAR ── */
    ::-webkit-scrollbar { width: 4px; }
    ::-webkit-scrollbar-track { background: var(--cream); }
    ::-webkit-scrollbar-thumb { background: var(--gold); }

    /* ── NAV ── */
    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 100;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1.2rem 2.5rem;
      background: rgba(10, 8, 5, 0.88);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(184,150,90,0.2);
      transition: padding 0.3s;
    }

    .nav-logo {
      font-family: 'Shippori Mincho', serif;
      font-size: 1.5rem;
      font-weight: 700;
      color: var(--gold-light);
      letter-spacing: 0.15em;
      text-decoration: none;
    }

    .nav-logo span {
      display: block;
      font-size: 0.55rem;
      letter-spacing: 0.3em;
      color: var(--stone-light);
      font-weight: 400;
      margin-top: 2px;
    }

    .nav-links {
      display: flex;
      gap: 2rem;
      list-style: none;
    }

    .nav-links a {
      font-size: 0.75rem;
      letter-spacing: 0.25em;
      color: var(--stone-light);
      text-decoration: none;
      transition: color 0.3s;
    }

    .nav-links a:hover { color: var(--gold-light); }

    .nav-cta {
      background: transparent;
      border: 1px solid var(--gold);
      color: var(--gold-light);
      padding: 0.5rem 1.2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.75rem;
      letter-spacing: 0.2em;
      cursor: pointer;
      transition: all 0.3s;
      text-decoration: none;
    }

    .nav-cta:hover {
      background: var(--gold);
      color: var(--deep);
    }

    .hamburger {
      display: none;
      flex-direction: column;
      gap: 5px;
      cursor: pointer;
      background: none;
      border: none;
    }

    .hamburger span {
      display: block;
      width: 24px;
      height: 1px;
      background: var(--gold-light);
      transition: all 0.3s;
    }

    /* ── HERO ── */
    .hero {
      position: relative;
      height: 100vh;
      min-height: 600px;
      display: flex;
      align-items: center;
      justify-content: center;
      overflow: hidden;
      background: var(--deep);
    }

    .hero-bg {
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse at 30% 60%, rgba(139,58,42,0.18) 0%, transparent 60%),
        radial-gradient(ellipse at 75% 30%, rgba(184,150,90,0.12) 0%, transparent 55%),
        linear-gradient(160deg, #0e0b07 0%, #1a1209 40%, #0a0905 100%);
    }

    /* Japanese wave pattern overlay */
    .hero-pattern {
      position: absolute;
      inset: 0;
      opacity: 0.04;
      background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23d4af72' fill-opacity='1'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
    }

    .hero-vline {
      position: absolute;
      top: 0; bottom: 0;
      width: 1px;
      background: linear-gradient(to bottom, transparent, rgba(184,150,90,0.4) 30%, rgba(184,150,90,0.4) 70%, transparent);
    }
    .hero-vline:nth-child(1) { left: 15%; }
    .hero-vline:nth-child(2) { right: 15%; }

    .hero-content {
      position: relative;
      z-index: 2;
      text-align: center;
      padding: 2rem;
      animation: fadeUp 1.2s ease forwards;
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(30px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    .hero-eyebrow {
      font-size: 0.65rem;
      letter-spacing: 0.5em;
      color: var(--gold);
      text-transform: uppercase;
      margin-bottom: 1.8rem;
      opacity: 0;
      animation: fadeUp 1s 0.3s ease forwards;
    }

    .hero-title {
      font-family: 'Shippori Mincho', serif;
      font-size: clamp(3.5rem, 10vw, 7rem);
      font-weight: 700;
      color: var(--warm-white);
      line-height: 1;
      letter-spacing: 0.1em;
      margin-bottom: 0.5rem;
      opacity: 0;
      animation: fadeUp 1s 0.5s ease forwards;
    }

    .hero-title-en {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(1rem, 3vw, 1.6rem);
      font-style: italic;
      font-weight: 300;
      color: var(--gold-light);
      letter-spacing: 0.3em;
      margin-bottom: 2.5rem;
      opacity: 0;
      animation: fadeUp 1s 0.7s ease forwards;
    }

    .hero-desc {
      font-size: 0.82rem;
      line-height: 2;
      color: var(--stone-light);
      letter-spacing: 0.1em;
      max-width: 420px;
      margin: 0 auto 3rem;
      opacity: 0;
      animation: fadeUp 1s 0.9s ease forwards;
    }

    .hero-divider {
      width: 60px;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--gold), transparent);
      margin: 0 auto 3rem;
      opacity: 0;
      animation: fadeUp 1s 0.8s ease forwards;
    }

    .hero-btns {
      display: flex;
      gap: 1rem;
      justify-content: center;
      flex-wrap: wrap;
      opacity: 0;
      animation: fadeUp 1s 1.1s ease forwards;
    }

    .btn-primary {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      background: var(--gold);
      color: var(--deep);
      padding: 0.9rem 2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.8rem;
      letter-spacing: 0.2em;
      text-decoration: none;
      font-weight: 600;
      transition: all 0.3s;
    }

    .btn-primary:hover {
      background: var(--gold-light);
      transform: translateY(-2px);
    }

    .btn-outline {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      background: transparent;
      color: var(--gold-light);
      border: 1px solid var(--gold);
      padding: 0.9rem 2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.8rem;
      letter-spacing: 0.2em;
      text-decoration: none;
      transition: all 0.3s;
    }

    .btn-outline:hover {
      background: rgba(184,150,90,0.1);
      transform: translateY(-2px);
    }

    .hero-scroll {
      position: absolute;
      bottom: 2rem;
      left: 50%;
      transform: translateX(-50%);
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 0.5rem;
      font-size: 0.6rem;
      letter-spacing: 0.4em;
      color: var(--stone);
      animation: bounce 2s infinite;
    }

    .hero-scroll::after {
      content: '';
      display: block;
      width: 1px;
      height: 40px;
      background: linear-gradient(to bottom, var(--stone), transparent);
    }

    @keyframes bounce {
      0%, 100% { transform: translateX(-50%) translateY(0); }
      50% { transform: translateX(-50%) translateY(6px); }
    }

    /* ── SECTION COMMONS ── */
    section { padding: 6rem 1.5rem; }

    .section-label {
      font-size: 0.6rem;
      letter-spacing: 0.5em;
      color: var(--gold);
      text-transform: uppercase;
      display: block;
      margin-bottom: 0.8rem;
    }

    .section-title {
      font-family: 'Shippori Mincho', serif;
      font-size: clamp(1.8rem, 4vw, 2.8rem);
      font-weight: 700;
      line-height: 1.3;
      letter-spacing: 0.05em;
    }

    .section-title-en {
      font-family: 'Cormorant Garamond', serif;
      font-style: italic;
      font-size: clamp(0.9rem, 2vw, 1.1rem);
      font-weight: 300;
      color: var(--stone);
      letter-spacing: 0.2em;
      margin-top: 0.3rem;
    }

    .title-line {
      width: 40px;
      height: 1px;
      background: var(--gold);
      margin: 1.5rem 0;
    }

    /* ── ABOUT ── */
    .about {
      background: var(--cream);
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 5rem;
      align-items: center;
      max-width: 1100px;
      margin: 0 auto;
    }

    .about-text p {
      font-size: 0.88rem;
      line-height: 2.2;
      color: #3d3228;
      margin-bottom: 1.2rem;
    }

    .about-features {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1.5rem;
      margin-top: 2rem;
    }

    .feature-item {
      border-left: 2px solid var(--gold);
      padding-left: 1rem;
    }

    .feature-num {
      font-family: 'Cormorant Garamond', serif;
      font-size: 2rem;
      font-weight: 300;
      color: var(--gold);
      line-height: 1;
    }

    .feature-label {
      font-size: 0.75rem;
      letter-spacing: 0.1em;
      color: var(--stone);
      margin-top: 0.3rem;
    }

    .about-image-area {
      position: relative;
    }

    .about-img-box {
      background: linear-gradient(135deg, #1a1209, #2d2015);
      aspect-ratio: 3/4;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    .about-img-box::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(ellipse at 40% 40%, rgba(184,150,90,0.15), transparent 60%);
    }

    .about-img-kanji {
      font-family: 'Shippori Mincho', serif;
      font-size: 8rem;
      font-weight: 700;
      color: rgba(184,150,90,0.12);
      position: absolute;
      writing-mode: vertical-rl;
      letter-spacing: 0.1em;
      user-select: none;
    }

    .about-img-center {
      font-family: 'Shippori Mincho', serif;
      font-size: 1rem;
      color: var(--gold-light);
      letter-spacing: 0.3em;
      position: relative;
      z-index: 1;
      text-align: center;
    }

    .about-img-center::before {
      content: '雪乃';
      display: block;
      font-size: 4rem;
      font-weight: 700;
      color: rgba(184,150,90,0.6);
      margin-bottom: 1rem;
    }

    .about-badge {
      position: absolute;
      bottom: -1.5rem;
      right: -1.5rem;
      width: 120px;
      height: 120px;
      background: var(--gold);
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
    }

    .about-badge span {
      font-family: 'Shippori Mincho', serif;
      font-size: 0.65rem;
      font-weight: 700;
      color: var(--deep);
      letter-spacing: 0.05em;
      line-height: 1.5;
      text-align: center;
    }

    /* ── MENU ── */
    .menu-section {
      background: var(--deep);
      color: var(--warm-white);
    }

    .menu-inner {
      max-width: 1100px;
      margin: 0 auto;
    }

    .menu-header {
      text-align: center;
      margin-bottom: 4rem;
    }

    .menu-header .section-title { color: var(--warm-white); }
    .menu-header .title-line { margin: 1.5rem auto; }

    .menu-tabs {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      justify-content: center;
      margin-bottom: 3rem;
    }

    .menu-tab {
      background: transparent;
      border: 1px solid rgba(184,150,90,0.3);
      color: var(--stone-light);
      padding: 0.5rem 1.2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      cursor: pointer;
      transition: all 0.3s;
    }

    .menu-tab.active,
    .menu-tab:hover {
      background: var(--gold);
      color: var(--deep);
      border-color: var(--gold);
    }

    .menu-grid {
      display: none;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 1px;
      background: rgba(184,150,90,0.1);
    }

    .menu-grid.active { display: grid; }

    .menu-item {
      background: rgba(255,255,255,0.02);
      padding: 1.2rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 1rem;
      transition: background 0.3s;
    }

    .menu-item:hover { background: rgba(184,150,90,0.07); }

    .menu-item-name {
      font-size: 0.82rem;
      letter-spacing: 0.05em;
      color: var(--cream);
      line-height: 1.5;
    }

    .menu-item-price {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1rem;
      color: var(--gold);
      white-space: nowrap;
      font-weight: 300;
    }

    .menu-note {
      text-align: center;
      margin-top: 2rem;
      font-size: 0.75rem;
      color: var(--stone);
      letter-spacing: 0.1em;
    }

    /* ── HOURS ── */
    .hours-section {
      background: var(--cream);
    }

    .hours-inner {
      max-width: 900px;
      margin: 0 auto;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 4rem;
      align-items: start;
    }

    .hours-table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 1.5rem;
    }

    .hours-table tr {
      border-bottom: 1px solid rgba(184,150,90,0.15);
    }

    .hours-table td {
      padding: 0.9rem 0;
      font-size: 0.85rem;
    }

    .hours-table td:first-child {
      color: var(--stone);
      letter-spacing: 0.05em;
      width: 5rem;
    }

    .hours-table td:last-child {
      color: var(--ink);
      font-weight: 500;
    }

    .closed {
      color: var(--stone-light) !important;
    }

    .hours-note {
      margin-top: 1.2rem;
      font-size: 0.75rem;
      color: var(--stone);
      line-height: 1.8;
      letter-spacing: 0.05em;
    }

    .contact-info {
      margin-top: 1.5rem;
    }

    .contact-row {
      display: flex;
      align-items: flex-start;
      gap: 1rem;
      padding: 1rem 0;
      border-bottom: 1px solid rgba(184,150,90,0.15);
    }

    .contact-icon {
      width: 36px;
      height: 36px;
      background: var(--gold);
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
    }

    .contact-icon svg {
      width: 16px;
      height: 16px;
      fill: var(--deep);
    }

    .contact-label {
      font-size: 0.65rem;
      letter-spacing: 0.2em;
      color: var(--stone);
      margin-bottom: 0.3rem;
    }

    .contact-value {
      font-size: 0.88rem;
      color: var(--ink);
      letter-spacing: 0.05em;
    }

    .contact-value a {
      color: inherit;
      text-decoration: none;
    }

    /* ── PHONE CTA ── */
    .phone-cta {
      background: linear-gradient(135deg, #1a1209, #0e0b07);
      text-align: center;
      padding: 5rem 1.5rem;
      position: relative;
      overflow: hidden;
    }

    .phone-cta::before {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(ellipse at center, rgba(184,150,90,0.08), transparent 70%);
    }

    .phone-cta-inner {
      position: relative;
      z-index: 1;
    }

    .phone-cta p {
      font-size: 0.8rem;
      letter-spacing: 0.3em;
      color: var(--stone-light);
      margin-bottom: 1.5rem;
    }

    .phone-number {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(2rem, 6vw, 3.5rem);
      font-weight: 300;
      color: var(--gold-light);
      letter-spacing: 0.1em;
      margin-bottom: 1rem;
      display: block;
      text-decoration: none;
    }

    .phone-number:hover { color: var(--gold); }

    .phone-sub {
      font-size: 0.72rem;
      color: var(--stone);
      letter-spacing: 0.2em;
      margin-bottom: 2.5rem;
    }

    .btn-call {
      display: inline-flex;
      align-items: center;
      gap: 0.6rem;
      background: var(--gold);
      color: var(--deep);
      padding: 1rem 2.5rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.9rem;
      letter-spacing: 0.2em;
      text-decoration: none;
      font-weight: 700;
      transition: all 0.3s;
    }

    .btn-call:hover {
      background: var(--gold-light);
      transform: translateY(-3px);
      box-shadow: 0 8px 30px rgba(184,150,90,0.3);
    }

    .btn-call svg {
      width: 18px;
      height: 18px;
      fill: var(--deep);
    }

    /* ── ACCESS / MAP ── */
    .access-section {
      background: var(--warm-white);
    }

    .access-inner {
      max-width: 1000px;
      margin: 0 auto;
    }

    .access-grid {
      display: grid;
      grid-template-columns: 1fr 1.4fr;
      gap: 4rem;
      align-items: start;
      margin-top: 3rem;
    }

    .access-detail {
      font-size: 0.85rem;
      line-height: 2;
      color: #3d3228;
    }

    .access-detail strong {
      display: block;
      font-size: 0.65rem;
      letter-spacing: 0.3em;
      color: var(--gold);
      margin-top: 1.2rem;
      margin-bottom: 0.3rem;
    }

    .map-wrapper {
      position: relative;
    }

    .map-frame {
      width: 100%;
      height: 360px;
      border: none;
      display: block;
      filter: grayscale(30%) sepia(10%);
    }

    .map-link-overlay {
      position: absolute;
      bottom: 1rem;
      right: 1rem;
      background: var(--gold);
      color: var(--deep);
      padding: 0.6rem 1.2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.72rem;
      letter-spacing: 0.15em;
      text-decoration: none;
      font-weight: 700;
      display: flex;
      align-items: center;
      gap: 0.4rem;
      transition: all 0.3s;
    }

    .map-link-overlay:hover {
      background: var(--gold-light);
    }

    /* ── REVIEWS ── */
    .reviews-section {
      background: #f5efe6;
      padding: 5rem 1.5rem;
    }

    .reviews-inner {
      max-width: 1100px;
      margin: 0 auto;
    }

    .reviews-header { text-align: center; margin-bottom: 3rem; }
    .reviews-header .title-line { margin: 1.5rem auto; }

    .reviews-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 1.5rem;
    }

    .review-card {
      background: var(--warm-white);
      padding: 1.8rem;
      border-top: 2px solid var(--gold);
      transition: transform 0.3s;
    }

    .review-card:hover { transform: translateY(-4px); }

    .review-stars {
      color: var(--gold);
      font-size: 0.9rem;
      letter-spacing: 0.1em;
      margin-bottom: 0.8rem;
    }

    .review-text {
      font-size: 0.8rem;
      line-height: 1.9;
      color: #4a3d30;
      margin-bottom: 1rem;
    }

    .review-meta {
      font-size: 0.68rem;
      color: var(--stone);
      letter-spacing: 0.1em;
    }

    /* ── FOOTER ── */
    footer {
      background: var(--deep);
      padding: 3rem 1.5rem 2rem;
      color: var(--stone);
      text-align: center;
    }

    .footer-logo {
      font-family: 'Shippori Mincho', serif;
      font-size: 2rem;
      font-weight: 700;
      color: var(--gold-light);
      letter-spacing: 0.2em;
      margin-bottom: 1rem;
    }

    .footer-info {
      font-size: 0.75rem;
      line-height: 2;
      letter-spacing: 0.1em;
      margin-bottom: 2rem;
    }

    .footer-divider {
      width: 40px;
      height: 1px;
      background: rgba(184,150,90,0.3);
      margin: 1.5rem auto;
    }

    .footer-copy {
      font-size: 0.65rem;
      letter-spacing: 0.2em;
      color: rgba(140,123,107,0.5);
    }

    /* ── RESPONSIVE ── */
    @media (max-width: 768px) {
      nav { padding: 1rem 1.2rem; }

      .nav-links, .nav-cta { display: none; }

      .hamburger { display: flex; }

      .nav-links.open {
        display: flex;
        flex-direction: column;
        position: fixed;
        top: 60px; left: 0; right: 0;
        background: rgba(10,8,5,0.97);
        padding: 2rem;
        gap: 1.5rem;
        border-top: 1px solid rgba(184,150,90,0.2);
        backdrop-filter: blur(20px);
      }

      .nav-links.open a { font-size: 0.9rem; }

      .about {
        grid-template-columns: 1fr;
        gap: 2.5rem;
        padding: 4rem 1.5rem;
      }

      .about-image-area { order: -1; }

      .about-badge {
        right: 0;
        bottom: -1rem;
      }

      .hours-inner {
        grid-template-columns: 1fr;
        gap: 2.5rem;
      }

      .access-grid {
        grid-template-columns: 1fr;
        gap: 2rem;
      }

      .map-frame { height: 280px; }

      section { padding: 4rem 1.2rem; }

      .menu-grid { grid-template-columns: 1fr; }
    }

    /* ── ANIMATIONS ON SCROLL ── */
    .reveal {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }

    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>

<!-- NAV -->
<nav id="navbar">
  <a class="nav-logo" href="#">ゆきの<span>YUKINO / NAGO, OKINAWA</span></a>
  <ul class="nav-links" id="navLinks">
    <li><a href="#menu">メニュー</a></li>
    <li><a href="#hours">営業時間</a></li>
    <li><a href="#access">アクセス</a></li>
  </ul>
  <a href="tel:0980523486" class="nav-cta" style="display:none" id="navCtaDesktop">予約・お問い合わせ</a>
  <button class="hamburger" id="hamburger" aria-label="メニュー">
    <span></span><span></span><span></span>
  </button>
</nav>

<!-- HERO -->
<section class="hero" id="top">
  <div class="hero-bg"></div>
  <div class="hero-pattern"></div>
  <div class="hero-vline"></div>
  <div class="hero-vline"></div>
  <div class="hero-content">
    <p class="hero-eyebrow">Nago, Okinawa — Since Long Ago</p>
    <h1 class="hero-title">ゆきの</h1>
    <p class="hero-title-en">Yukino — Teishoku & Izakaya</p>
    <div class="hero-divider"></div>
    <p class="hero-desc">沖縄の恵みと島の食材を活かした<br>50種以上の定食と沖縄料理。<br>名護の地に根ざした、心温まる一皿を。</p>
    <div class="hero-btns">
      <a href="#menu" class="btn-primary">メニューを見る</a>
      <a href="tel:0980523486" class="btn-outline">
        <svg viewBox="0 0 24 24" width="14" height="14" fill="currentColor"><path d="M6.6 10.8c1.4 2.8 3.8 5.1 6.6 6.6l2.2-2.2c.3-.3.7-.4 1-.2 1.1.4 2.3.6 3.6.6.6 0 1 .4 1 1V20c0 .6-.4 1-1 1-9.4 0-17-7.6-17-17 0-.6.4-1 1-1h3.5c.6 0 1 .4 1 1 0 1.3.2 2.5.6 3.6.1.3 0 .7-.2 1L6.6 10.8z"/></svg>
        電話予約
      </a>
    </div>
  </div>
  <div class="hero-scroll">SCROLL</div>
</section>

<!-- ABOUT -->
<section style="background: var(--cream); padding: 6rem 1.5rem;">
  <div class="about reveal">
    <div class="about-text">
      <span class="section-label">About Us</span>
      <h2 class="section-title">名護が愛する<br>味と賑わい</h2>
      <p class="section-title-en">A beloved gathering place in Nago</p>
      <div class="title-line"></div>
      <p>ホテルゆがふいんの真裏、名護市宮里に構える「ゆきの」は、地元の方々に愛され続ける定食・居酒屋です。</p>
      <p>アグー豚のやわらかステーキから新鮮な刺身盛合せ、沖縄そばやゴーヤチャンプルーまで、バラエティ豊かなメニューを良心的な価格でご提供しています。国内外の観光客にも人気の、名護を代表する一軒です。</p>
      <div class="about-features">
        <div class="feature-item">
          <div class="feature-num">50<span style="font-size:1rem">+</span></div>
          <div class="feature-label">定食の種類</div>
        </div>
        <div class="feature-item">
          <div class="feature-num">150<span style="font-size:1rem">+</span></div>
          <div class="feature-label">総メニュー数</div>
        </div>
        <div class="feature-item">
          <div class="feature-num">5</div>
          <div class="feature-label">営業日/週</div>
        </div>
        <div class="feature-item">
          <div class="feature-num">★5</div>
          <div class="feature-label">口コミ評価</div>
        </div>
      </div>
    </div>
    <div class="about-image-area">
      <div class="about-img-box">
        <div class="about-img-kanji">沖縄</div>
        <div class="about-img-center">名護・宮里の食卓</div>
      </div>
      <div class="about-badge">
        <span>地元の<br>名店<br>予約推奨</span>
      </div>
    </div>
  </div>
</section>

<!-- MENU -->
<section class="menu-section" id="menu">
  <div class="menu-inner">
    <div class="menu-header reveal">
      <span class="section-label">Our Menu</span>
      <h2 class="section-title">メニュー</h2>
      <p class="section-title-en">From teishoku to Okinawan classics</p>
      <div class="title-line"></div>
    </div>

    <div class="menu-tabs reveal">
      <button class="menu-tab active" onclick="showTab('teishoku',this)">定食</button>
      <button class="menu-tab" onclick="showTab('curry',this)">カレー</button>
      <button class="menu-tab" onclick="showTab('donburi',this)">丼ぶり</button>
      <button class="menu-tab" onclick="showTab('okinawa',this)">沖縄料理</button>
      <button class="menu-tab" onclick="showTab('sashimi',this)">刺身</button>
      <button class="menu-tab" onclick="showTab('ippinryo',this)">一品料理</button>
      <button class="menu-tab" onclick="showTab('men',this)">麺類</button>
    </div>

    <div class="menu-grid active" id="tab-teishoku">
      <div class="menu-item"><span class="menu-item-name">アグーのやわらかステーキ定食</span><span class="menu-item-price">¥1,600</span></div>
      <div class="menu-item"><span class="menu-item-name">アグーのミルフィーユカツ定食</span><span class="menu-item-price">¥1,250</span></div>
      <div class="menu-item"><span class="menu-item-name">とんかつ定食</span><span class="menu-item-price">¥1,050</span></div>
      <div class="menu-item"><span class="menu-item-name">ヒレカツ定食</span><span class="menu-item-price">¥1,250</span></div>
      <div class="menu-item"><span class="menu-item-name">ささみのチーズカツ定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">海老フライ定食</span><span class="menu-item-price">¥1,350</span></div>
      <div class="menu-item"><span class="menu-item-name">魚フライ定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">カキフライ定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">魚バター焼定食</span><span class="menu-item-price">時価</span></div>
      <div class="menu-item"><span class="menu-item-name">魚煮付定食</span><span class="menu-item-price">時価</span></div>
      <div class="menu-item"><span class="menu-item-name">赤魚の切身バター焼定食</span><span class="menu-item-price">¥2,000</span></div>
      <div class="menu-item"><span class="menu-item-name">赤魚の切身煮付定食</span><span class="menu-item-price">¥2,000</span></div>
      <div class="menu-item"><span class="menu-item-name">刺身定食</span><span class="menu-item-price">¥1,800</span></div>
      <div class="menu-item"><span class="menu-item-name">天ぷら定食</span><span class="menu-item-price">¥1,800</span></div>
      <div class="menu-item"><span class="menu-item-name">うな重定食</span><span class="menu-item-price">¥1,700</span></div>
      <div class="menu-item"><span class="menu-item-name">カットステーキ定食</span><span class="menu-item-price">¥1,600</span></div>
      <div class="menu-item"><span class="menu-item-name">焼肉定食</span><span class="menu-item-price">¥1,300</span></div>
      <div class="menu-item"><span class="menu-item-name">しょうが焼定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">ゴーヤチャンプルー定食</span><span class="menu-item-price">¥1,150</span></div>
      <div class="menu-item"><span class="menu-item-name">沖縄そば定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">チキン唐揚げ定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">チーズハンバーグステーキ定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">エビチリ定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">牛みそ定食</span><span class="menu-item-price">¥1,200</span></div>
      <div class="menu-item"><span class="menu-item-name">豚肉キムチ炒め定食</span><span class="menu-item-price">¥1,200</span></div>
      <div class="menu-item"><span class="menu-item-name">マーボー豆腐定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">お子様ランチ</span><span class="menu-item-price">¥800</span></div>
    </div>

    <div class="menu-grid" id="tab-curry">
      <div class="menu-item"><span class="menu-item-name">カツカレー定食</span><span class="menu-item-price">¥1,200</span></div>
      <div class="menu-item"><span class="menu-item-name">チキン唐揚げカレー定食</span><span class="menu-item-price">¥1,200</span></div>
      <div class="menu-item"><span class="menu-item-name">コロッケカレー定食</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">エビフライカレー定食</span><span class="menu-item-price">¥1,450</span></div>
      <div class="menu-item"><span class="menu-item-name">カキフライカレー定食</span><span class="menu-item-price">¥1,200</span></div>
      <div class="menu-item"><span class="menu-item-name">魚フライカレー定食</span><span class="menu-item-price">¥1,200</span></div>
    </div>

    <div class="menu-grid" id="tab-donburi">
      <div class="menu-item"><span class="menu-item-name">カツ丼定食</span><span class="menu-item-price">¥1,300</span></div>
      <div class="menu-item"><span class="menu-item-name">親子丼定食</span><span class="menu-item-price">¥1,300</span></div>
      <div class="menu-item"><span class="menu-item-name">天丼定食</span><span class="menu-item-price">¥1,400</span></div>
      <div class="menu-item"><span class="menu-item-name">まぐろやまかけ丼定食</span><span class="menu-item-price">¥1,400</span></div>
      <div class="menu-item"><span class="menu-item-name">まぐろ丼定食</span><span class="menu-item-price">¥1,600</span></div>
      <div class="menu-item"><span class="menu-item-name">鉄火丼定食</span><span class="menu-item-price">¥1,600</span></div>
    </div>

    <div class="menu-grid" id="tab-okinawa">
      <div class="menu-item"><span class="menu-item-name">アグーの柔らかステーキ</span><span class="menu-item-price">¥1,300</span></div>
      <div class="menu-item"><span class="menu-item-name">やぎ刺</span><span class="menu-item-price">¥1,500</span></div>
      <div class="menu-item"><span class="menu-item-name">沖縄そば</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">ゴーヤチャンプルー</span><span class="menu-item-price">¥900</span></div>
      <div class="menu-item"><span class="menu-item-name">フーチャンプルー</span><span class="menu-item-price">¥800</span></div>
      <div class="menu-item"><span class="menu-item-name">野菜チャンプルー</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">ソーメンチャンプルー</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">ラフテー</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">海ぶどう</span><span class="menu-item-price">¥800</span></div>
      <div class="menu-item"><span class="menu-item-name">もずく酢</span><span class="menu-item-price">¥600</span></div>
      <div class="menu-item"><span class="menu-item-name">もずく天ぷら（大）</span><span class="menu-item-price">¥900</span></div>
      <div class="menu-item"><span class="menu-item-name">もずく天ぷら（小）</span><span class="menu-item-price">¥500</span></div>
      <div class="menu-item"><span class="menu-item-name">ぐるくん唐揚</span><span class="menu-item-price">¥750</span></div>
      <div class="menu-item"><span class="menu-item-name">ジーマーミ豆腐</span><span class="menu-item-price">¥500</span></div>
      <div class="menu-item"><span class="menu-item-name">スーチカー</span><span class="menu-item-price">¥650</span></div>
      <div class="menu-item"><span class="menu-item-name">アグーの焼き餃子</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">島唐辛子の揚げ餃子</span><span class="menu-item-price">¥650</span></div>
      <div class="menu-item"><span class="menu-item-name">タロイモの甘うまソースあえ</span><span class="menu-item-price">¥600</span></div>
    </div>

    <div class="menu-grid" id="tab-sashimi">
      <div class="menu-item"><span class="menu-item-name">マグロ刺身</span><span class="menu-item-price">¥1,050</span></div>
      <div class="menu-item"><span class="menu-item-name">さば刺身</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">白身刺身</span><span class="menu-item-price">¥1,050</span></div>
      <div class="menu-item"><span class="menu-item-name">タコ刺身</span><span class="menu-item-price">¥900</span></div>
      <div class="menu-item"><span class="menu-item-name">イラブチャー刺身</span><span class="menu-item-price">¥1,100</span></div>
      <div class="menu-item"><span class="menu-item-name">サーモン刺身</span><span class="menu-item-price">¥1,050</span></div>
      <div class="menu-item"><span class="menu-item-name">セイイカ刺身</span><span class="menu-item-price">¥800</span></div>
      <div class="menu-item"><span class="menu-item-name">刺身盛合せ（小）</span><span class="menu-item-price">¥1,500</span></div>
      <div class="menu-item"><span class="menu-item-name">刺身盛合せ（大）</span><span class="menu-item-price">¥3,000</span></div>
      <div class="menu-item"><span class="menu-item-name">海鮮みそあえ（小）</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">海鮮みそあえ（大）</span><span class="menu-item-price">¥1,400</span></div>
      <div class="menu-item"><span class="menu-item-name">海鮮キムチあえ（小）</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">海鮮キムチあえ（大）</span><span class="menu-item-price">¥1,400</span></div>
    </div>

    <div class="menu-grid" id="tab-ippinryo">
      <div class="menu-item"><span class="menu-item-name">チキン唐揚</span><span class="menu-item-price">¥750</span></div>
      <div class="menu-item"><span class="menu-item-name">チキン唐マヨ</span><span class="menu-item-price">¥800</span></div>
      <div class="menu-item"><span class="menu-item-name">手羽餃子</span><span class="menu-item-price">¥800</span></div>
      <div class="menu-item"><span class="menu-item-name">ホタテのウニソース焼</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">カマンベールチーズフライ</span><span class="menu-item-price">¥600</span></div>
      <div class="menu-item"><span class="menu-item-name">カットステーキ</span><span class="menu-item-price">¥1,300</span></div>
      <div class="menu-item"><span class="menu-item-name">赤魚の切身バター焼</span><span class="menu-item-price">¥1,700</span></div>
      <div class="menu-item"><span class="menu-item-name">赤魚の切身煮付</span><span class="menu-item-price">¥1,700</span></div>
      <div class="menu-item"><span class="menu-item-name">イカゲソ唐揚</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">タコ唐揚</span><span class="menu-item-price">¥750</span></div>
      <div class="menu-item"><span class="menu-item-name">エビチリ</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">揚げ出し豆腐</span><span class="menu-item-price">¥500</span></div>
      <div class="menu-item"><span class="menu-item-name">冷奴</span><span class="menu-item-price">¥400</span></div>
      <div class="menu-item"><span class="menu-item-name">枝豆</span><span class="menu-item-price">¥500</span></div>
      <div class="menu-item"><span class="menu-item-name">ポテトフライ</span><span class="menu-item-price">¥500</span></div>
      <div class="menu-item"><span class="menu-item-name">砂肝唐揚</span><span class="menu-item-price">¥700</span></div>
    </div>

    <div class="menu-grid" id="tab-men">
      <div class="menu-item"><span class="menu-item-name">沖縄そば</span><span class="menu-item-price">¥850</span></div>
      <div class="menu-item"><span class="menu-item-name">焼うどん（塩・ケチャップ）</span><span class="menu-item-price">¥900</span></div>
      <div class="menu-item"><span class="menu-item-name">焼きそば（塩・ケチャップ）</span><span class="menu-item-price">¥900</span></div>
      <div class="menu-item"><span class="menu-item-name">ピリうまキムチうどん</span><span class="menu-item-price">¥900</span></div>
      <div class="menu-item"><span class="menu-item-name">ソーメンチャンプルー</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">ピリ辛ソーメンチャンプルー</span><span class="menu-item-price">¥700</span></div>
      <div class="menu-item"><span class="menu-item-name">牛肉もやしそば</span><span class="menu-item-price">¥1,100</span></div>
    </div>

    <p class="menu-note reveal">※ 価格はすべて税込。仕入れ状況により変更となる場合があります。</p>
  </div>
</section>

<!-- HOURS + CONTACT -->
<section class="hours-section" id="hours">
  <div class="hours-inner">
    <div class="reveal">
      <span class="section-label">Hours</span>
      <h2 class="section-title">営業時間</h2>
      <p class="section-title-en">Opening Hours</p>
      <div class="title-line"></div>
      <table class="hours-table">
        <tr><td>月曜日</td><td class="closed">定休日</td></tr>
        <tr><td>火曜日</td><td>17:00 〜 21:30</td></tr>
        <tr><td>水曜日</td><td class="closed">定休日</td></tr>
        <tr><td>木曜日</td><td>17:00 〜 21:30</td></tr>
        <tr><td>金曜日</td><td>17:00 〜 21:30</td></tr>
        <tr><td>土曜日</td><td>17:00 〜 21:30</td></tr>
        <tr><td>日曜日</td><td>17:00 〜 21:30</td></tr>
      </table>
      <p class="hours-note">
        ※ 混雑時はお断りする場合がございます。<br>
        ご予約はお電話にてお気軽にどうぞ。
      </p>
    </div>
    <div class="reveal">
      <span class="section-label">Contact</span>
      <h2 class="section-title">店舗情報</h2>
      <p class="section-title-en">Store Information</p>
      <div class="title-line"></div>
      <div class="contact-info">
        <div class="contact-row">
          <div class="contact-icon">
            <svg viewBox="0 0 24 24"><path d="M6.6 10.8c1.4 2.8 3.8 5.1 6.6 6.6l2.2-2.2c.3-.3.7-.4 1-.2 1.1.4 2.3.6 3.6.6.6 0 1 .4 1 1V20c0 .6-.4 1-1 1-9.4 0-17-7.6-17-17 0-.6.4-1 1-1h3.5c.6 0 1 .4 1 1 0 1.3.2 2.5.6 3.6.1.3 0 .7-.2 1L6.6 10.8z"/></svg>
          </div>
          <div>
            <div class="contact-label">PHONE</div>
            <div class="contact-value"><a href="tel:0980523486">0980-52-3486</a></div>
          </div>
        </div>
        <div class="contact-row">
          <div class="contact-icon">
            <svg viewBox="0 0 24 24"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/></svg>
          </div>
          <div>
            <div class="contact-label">ADDRESS</div>
            <div class="contact-value">〒905-0011<br>沖縄県名護市宮里450−8</div>
          </div>
        </div>
        <div class="contact-row">
          <div class="contact-icon">
            <svg viewBox="0 0 24 24"><path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm-5 14H7v-2h7v2zm3-4H7v-2h10v2zm0-4H7V7h10v2z"/></svg>
          </div>
          <div>
            <div class="contact-label">NOTE</div>
            <div class="contact-value">ホテルゆがふいん真裏<br>店内禁煙・泡盛ボトルキープ可</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- PHONE CTA -->
<div class="phone-cta">
  <div class="phone-cta-inner reveal">
    <p>RESERVATION & INQUIRY</p>
    <a class="phone-number" href="tel:0980523486">0980-52-3486</a>
    <p class="phone-sub">営業時間内にお気軽にご連絡ください / 火・木〜日 17:00〜21:30</p>
    <a class="btn-call" href="tel:0980523486">
      <svg viewBox="0 0 24 24"><path d="M6.6 10.8c1.4 2.8 3.8 5.1 6.6 6.6l2.2-2.2c.3-.3.7-.4 1-.2 1.1.4 2.3.6 3.6.6.6 0 1 .4 1 1V20c0 .6-.4 1-1 1-9.4 0-17-7.6-17-17 0-.6.4-1 1-1h3.5c.6 0 1 .4 1 1 0 1.3.2 2.5.6 3.6.1.3 0 .7-.2 1L6.6 10.8z"/></svg>
      今すぐ電話する
    </a>
  </div>
</div>

<!-- REVIEWS -->
<section class="reviews-section">
  <div class="reviews-inner">
    <div class="reviews-header reveal">
      <span class="section-label">Reviews</span>
      <h2 class="section-title">お客様の声</h2>
      <p class="section-title-en">What our guests say</p>
      <div class="title-line"></div>
    </div>
    <div class="reviews-grid">
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">料理の味・量は大満足。沖縄の郷土料理を美味しく頂けます。地元の方も食べに来ていて、美味しい証拠。非常に満足でした。</p>
        <div class="review-meta">8か月前 ／ Google</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">店内禁煙で良かった。繁盛していて、夜も定食メニューをしているのでお手頃に沖縄料理が食べられる良心的なお店。座敷が多くて沖縄らしい雰囲気でした。</p>
        <div class="review-meta">8か月前 ／ Google</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">結構好きな店でたまに寄ります。メニューが豊富で地元料理も楽しめる。定食を頼むと小鉢も多いので定食で一杯やるのもあり。店内は広めで回転もしています。</p>
        <div class="review-meta">1年前 ／ Google</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★☆</div>
        <p class="review-text">噂に違わずの賑わい。メニューは定食だけで50種を超え、一品・沖縄料理・麺類・刺身など70種は有りそう。1人3,000円でお腹いっぱい。旅先のファミリー夕食にお安いですよ。</p>
        <div class="review-meta">7か月前 ／ Google</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">ラフテーは味がしみてて最高。グルクン唐揚げは魚嫌いな息子も絶賛。17:30予約なしでギリ入れました。行く予定があるなら予約したほうが安パイです。</p>
        <div class="review-meta">1年前 ／ Google</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">超昔からあるファミリー居酒屋。メニュー数はめちゃくちゃ多くて迷いました。牛もやし炒め定食をいただきました。どれも美味しそうで活気がすごくてとても良い雰囲気です。</p>
        <div class="review-meta">5か月前 ／ Google</div>
      </div>
    </div>
  </div>
</section>

<!-- ACCESS -->
<section class="access-section" id="access">
  <div class="access-inner">
    <div class="reveal">
      <span class="section-label">Access</span>
      <h2 class="section-title">アクセス</h2>
      <p class="section-title-en">How to find us</p>
      <div class="title-line"></div>
    </div>
    <div class="access-grid reveal">
      <div>
        <div class="access-detail">
          <strong>住所</strong>
          〒905-0011<br>
          沖縄県名護市宮里450−8
          <strong>最寄り</strong>
          ホテルゆがふいん名護 真裏<br>
          喜瀬・名護周辺リゾートホテルから好アクセス
          <strong>駐車場</strong>
          あり（お問い合わせください）
          <strong>営業時間</strong>
          火・木・金・土・日<br>
          17:00〜21:30<br>
          ※月・水 定休日
          <strong>お問い合わせ</strong>
          <a href="tel:0980523486" style="color:var(--gold); font-weight:600; font-size:1.1rem;">0980-52-3486</a>
        </div>
        <br>
        <a href="https://maps.app.goo.gl/eURE5MPN7vzDD2gp8" target="_blank" rel="noopener" class="btn-primary" style="display:inline-flex; margin-top:1rem;">
          <svg viewBox="0 0 24 24" width="14" height="14" fill="currentColor"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/></svg>
          Google マップで開く
        </a>
      </div>
      <div class="map-wrapper">
        <iframe
          class="map-frame"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3568.123456789!2d127.9799!3d26.5912!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x34e42e1234567890%3A0xabcdef1234567890!2z5oKT56ysMDAwNeOBjuaFi-WFrA!5e0!3m2!1sja!2sjp!4v1234567890"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
          title="ゆきの 地図">
        </iframe>
        <a href="https://maps.app.goo.gl/eURE5MPN7vzDD2gp8" target="_blank" rel="noopener" class="map-link-overlay">
          <svg viewBox="0 0 24 24" width="12" height="12" fill="currentColor"><path d="M19 19H5V5h7V3H5c-1.11 0-2 .9-2 2v14c0 1.1.89 2 2 2h14c1.1 0 2-.9 2-2v-7h-2v7zM14 3v2h3.59l-9.83 9.83 1.41 1.41L19 6.41V10h2V3h-7z"/></svg>
          大きな地図で見る
        </a>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-logo">ゆきの</div>
  <div class="footer-info">
    〒905-0011 沖縄県名護市宮里450−8<br>
    TEL: 0980-52-3486<br>
    営業時間: 17:00〜21:30（火・木〜日）　定休日: 月・水
  </div>
  <div class="footer-divider"></div>
  <p class="footer-copy">© 2025 ゆきの All Rights Reserved.</p>
</footer>

<script>
  // Hamburger menu
  const hamburger = document.getElementById('hamburger');
  const navLinks = document.getElementById('navLinks');
  hamburger.addEventListener('click', () => {
    navLinks.classList.toggle('open');
  });

  // Menu tabs
  function showTab(id, btn) {
    document.querySelectorAll('.menu-grid').forEach(g => g.classList.remove('active'));
    document.querySelectorAll('.menu-tab').forEach(t => t.classList.remove('active'));
    document.getElementById('tab-' + id).classList.add('active');
    btn.classList.add('active');
  }

  // Scroll reveal
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry, i) => {
      if (entry.isIntersecting) {
        setTimeout(() => {
          entry.target.classList.add('visible');
        }, 80 * i);
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.1 });
  reveals.forEach(el => observer.observe(el));

  // Nav desktop CTA visibility
  const navCtaDesktop = document.getElementById('navCtaDesktop');
  function updateNavCta() {
    if (window.innerWidth > 768) {
      navCtaDesktop.style.display = 'inline-flex';
    } else {
      navCtaDesktop.style.display = 'none';
    }
  }
  updateNavCta();
  window.addEventListener('resize', updateNavCta);
</script>
</body>
</html>
