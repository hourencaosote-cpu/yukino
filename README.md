<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ゆきの｜名護の定食・居酒屋 — 沖縄県名護市宮里の老舗食堂</title>
  <meta name="description" content="沖縄県名護市宮里にある昔ながらの定食居酒屋「ゆきの」。アグー豚・沖縄そば・新鮮刺身など50種以上の定食と豊富な沖縄料理。地元の方から観光客まで長く愛されるお店です。">
  <meta name="keywords" content="ゆきの,名護,居酒屋,定食,沖縄料理,沖縄そば,アグー,とんかつ,名護市,老舗,食堂">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Zen+Kurenaido&family=Kaisei+Tokumin:wght@400;500;700&family=Shippori+Mincho:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --noren-red:   #c0392b;
      --noren-dark:  #8b1a1a;
      --ink:         #2c1a0e;
      --warm-bg:     #fdf6e8;
      --paper:       #faf0d7;
      --aged:        #f0e0b8;
      --matcha:      #5a7a4a;
      --wood:        #8b5e3c;
      --wood-light:  #c49a6c;
      --text:        #3a2412;
      --muted:       #8c7055;
      --line:        rgba(139,94,60,0.25);
    }

    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }

    body {
      font-family: 'Shippori Mincho', 'Kaisei Tokumin', serif;
      background: var(--warm-bg);
      color: var(--text);
      overflow-x: hidden;
      /* subtle paper grain */
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='300' height='300'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3CfeColorMatrix type='saturate' values='0'/%3E%3C/filter%3E%3Crect width='300' height='300' filter='url(%23n)' opacity='0.035'/%3E%3C/svg%3E");
    }

    ::-webkit-scrollbar { width: 6px; }
    ::-webkit-scrollbar-track { background: var(--aged); }
    ::-webkit-scrollbar-thumb { background: var(--wood-light); border-radius: 3px; }

    /* ━━━━━━━━━━━━ NAV ━━━━━━━━━━━━ */
    nav {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 200;
      background: var(--noren-dark);
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 1.5rem;
      height: 58px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.25);
    }

    /* noren stripe detail */
    nav::after {
      content: '';
      position: absolute;
      bottom: -6px; left: 0; right: 0;
      height: 6px;
      background: repeating-linear-gradient(
        90deg,
        var(--noren-red) 0, var(--noren-red) 18px,
        var(--noren-dark) 18px, var(--noren-dark) 36px
      );
    }

    .nav-logo {
      font-family: 'Zen Kurenaido', serif;
      font-size: 1.6rem;
      color: #fff;
      text-decoration: none;
      letter-spacing: 0.12em;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }

    .nav-logo-mark {
      width: 32px; height: 32px;
      background: #fff;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1rem;
      color: var(--noren-dark);
      font-weight: 700;
      flex-shrink: 0;
    }

    .nav-links {
      display: flex;
      gap: 1.8rem;
      list-style: none;
    }

    .nav-links a {
      color: rgba(255,255,255,0.85);
      text-decoration: none;
      font-size: 0.82rem;
      letter-spacing: 0.12em;
      transition: color 0.2s;
    }

    .nav-links a:hover { color: #ffd080; }

    .nav-tel {
      display: flex;
      align-items: center;
      gap: 0.4rem;
      background: var(--noren-red);
      color: #fff;
      text-decoration: none;
      padding: 0.4rem 1rem;
      font-size: 0.8rem;
      letter-spacing: 0.1em;
      border-radius: 2px;
      transition: background 0.2s;
    }

    .nav-tel:hover { background: #e74c3c; }

    .hamburger {
      display: none;
      flex-direction: column;
      gap: 5px;
      background: none;
      border: none;
      cursor: pointer;
      padding: 4px;
    }

    .hamburger span {
      display: block;
      width: 22px;
      height: 2px;
      background: #fff;
      border-radius: 2px;
      transition: all 0.3s;
    }

    /* ━━━━━━━━━━━━ HERO ━━━━━━━━━━━━ */
    .hero {
      margin-top: 64px;
      background: var(--noren-dark);
      min-height: 92vh;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    /* traditional seigaiha (青海波) wave pattern */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      opacity: 0.07;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='56' height='28'%3E%3Cellipse cx='28' cy='28' rx='28' ry='28' fill='none' stroke='%23fff' stroke-width='1.5'/%3E%3Cellipse cx='0' cy='28' rx='28' ry='28' fill='none' stroke='%23fff' stroke-width='1.5'/%3E%3Cellipse cx='56' cy='28' rx='28' ry='28' fill='none' stroke='%23fff' stroke-width='1.5'/%3E%3C/svg%3E");
      background-size: 56px 28px;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: 0; left: 0; right: 0;
      height: 80px;
      background: linear-gradient(to top, var(--warm-bg), transparent);
    }

    /* big decorative kanji in background */
    .hero-kanji-bg {
      position: absolute;
      right: -2rem;
      top: 50%;
      transform: translateY(-50%);
      font-family: 'Zen Kurenaido', serif;
      font-size: clamp(16rem, 30vw, 28rem);
      color: rgba(255,255,255,0.035);
      writing-mode: vertical-rl;
      line-height: 1;
      user-select: none;
      pointer-events: none;
      letter-spacing: -0.05em;
    }

    .hero-inner {
      position: relative;
      z-index: 2;
      text-align: center;
      padding: 2rem 1.5rem;
    }

    .hero-noren {
      display: inline-block;
      background: var(--noren-red);
      color: #fff;
      font-family: 'Zen Kurenaido', serif;
      font-size: 0.7rem;
      letter-spacing: 0.4em;
      padding: 0.35rem 1.2rem;
      margin-bottom: 2rem;
      position: relative;
      animation: fadeDown 0.8s ease both;
    }

    /* noren hanging strings */
    .hero-noren::before,
    .hero-noren::after {
      content: '';
      position: absolute;
      top: 100%;
      width: 1px;
      height: 14px;
      background: rgba(255,255,255,0.5);
    }
    .hero-noren::before { left: 30%; }
    .hero-noren::after  { right: 30%; }

    @keyframes fadeDown {
      from { opacity: 0; transform: translateY(-12px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    .hero-title {
      font-family: 'Zen Kurenaido', serif;
      font-size: clamp(5rem, 18vw, 11rem);
      color: #fff;
      line-height: 1;
      letter-spacing: 0.15em;
      margin-bottom: 0.3rem;
      animation: fadeUp 1s 0.2s ease both;
      text-shadow: 0 4px 20px rgba(0,0,0,0.4);
    }

    .hero-ruby {
      display: block;
      font-family: 'Shippori Mincho', serif;
      font-size: clamp(0.75rem, 2vw, 1rem);
      letter-spacing: 0.5em;
      color: rgba(255,255,255,0.6);
      margin-bottom: 1.8rem;
      animation: fadeUp 1s 0.4s ease both;
    }

    .hero-tagline {
      font-size: clamp(0.8rem, 2.2vw, 1rem);
      color: rgba(255,220,150,0.9);
      letter-spacing: 0.2em;
      line-height: 2;
      margin-bottom: 2.5rem;
      animation: fadeUp 1s 0.6s ease both;
    }

    .hero-divider {
      display: flex;
      align-items: center;
      gap: 1rem;
      justify-content: center;
      margin-bottom: 2.5rem;
      animation: fadeUp 1s 0.7s ease both;
    }

    .hero-divider::before,
    .hero-divider::after {
      content: '';
      flex: 1;
      max-width: 60px;
      height: 1px;
      background: rgba(255,255,255,0.25);
    }

    .hero-divider span {
      color: rgba(255,200,100,0.7);
      font-size: 1.2rem;
    }

    .hero-btns {
      display: flex;
      gap: 1rem;
      justify-content: center;
      flex-wrap: wrap;
      animation: fadeUp 1s 0.85s ease both;
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(16px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    .btn-main {
      background: var(--noren-red);
      color: #fff;
      padding: 0.85rem 2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.88rem;
      letter-spacing: 0.2em;
      text-decoration: none;
      border-radius: 2px;
      transition: all 0.25s;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      box-shadow: 0 3px 12px rgba(0,0,0,0.25);
    }

    .btn-main:hover {
      background: #e74c3c;
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(0,0,0,0.3);
    }

    .btn-sub {
      background: rgba(255,255,255,0.1);
      color: rgba(255,255,255,0.9);
      padding: 0.85rem 2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.88rem;
      letter-spacing: 0.2em;
      text-decoration: none;
      border-radius: 2px;
      border: 1px solid rgba(255,255,255,0.25);
      transition: all 0.25s;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
    }

    .btn-sub:hover {
      background: rgba(255,255,255,0.18);
      transform: translateY(-2px);
    }

    .hero-info-strip {
      position: absolute;
      bottom: 5rem;
      left: 0; right: 0;
      display: flex;
      justify-content: center;
      gap: 3rem;
      z-index: 2;
      flex-wrap: wrap;
      padding: 0 1rem;
    }

    .hero-info-item {
      text-align: center;
      color: rgba(255,255,255,0.7);
    }

    .hero-info-label {
      font-size: 0.58rem;
      letter-spacing: 0.35em;
      color: rgba(255,200,100,0.7);
      display: block;
      margin-bottom: 0.3rem;
    }

    .hero-info-val {
      font-size: 0.82rem;
      letter-spacing: 0.1em;
    }

    /* ━━━━━━━━━━━━ SECTION BASE ━━━━━━━━━━━━ */
    .section-wrap {
      max-width: 960px;
      margin: 0 auto;
      padding: 5rem 1.5rem;
    }

    .section-heading {
      text-align: center;
      margin-bottom: 3rem;
    }

    .section-heading .label {
      display: inline-block;
      font-size: 0.6rem;
      letter-spacing: 0.45em;
      color: var(--noren-red);
      background: rgba(192,57,43,0.08);
      padding: 0.25rem 1rem;
      margin-bottom: 0.8rem;
      border: 1px solid rgba(192,57,43,0.2);
    }

    .section-heading h2 {
      font-family: 'Zen Kurenaido', serif;
      font-size: clamp(1.7rem, 4vw, 2.5rem);
      letter-spacing: 0.12em;
      color: var(--ink);
      line-height: 1.3;
    }

    .section-heading p {
      font-size: 0.8rem;
      color: var(--muted);
      letter-spacing: 0.15em;
      margin-top: 0.5rem;
    }

    .hanko-divider {
      display: flex;
      align-items: center;
      gap: 1rem;
      margin: 1.2rem 0;
      justify-content: center;
    }

    .hanko-divider::before,
    .hanko-divider::after {
      content: '';
      flex: 1;
      max-width: 80px;
      height: 1px;
      background: var(--line);
    }

    .hanko {
      width: 32px; height: 32px;
      border: 2px solid var(--noren-red);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-family: 'Zen Kurenaido', serif;
      font-size: 0.7rem;
      color: var(--noren-red);
      letter-spacing: 0;
    }

    /* ━━━━━━━━━━━━ ABOUT / INTRO ━━━━━━━━━━━━ */
    .about-bg {
      background: var(--paper);
      border-top: 3px solid var(--noren-red);
    }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 4rem;
      align-items: center;
    }

    .about-text p {
      font-size: 0.88rem;
      line-height: 2.4;
      color: var(--text);
      margin-bottom: 1rem;
    }

    .about-text p strong {
      color: var(--noren-red);
    }

    .about-stamp-area {
      position: relative;
    }

    /* Illustrated izakaya sign — SVG decorative element */
    .about-sign {
      background: var(--noren-dark);
      border-radius: 4px;
      padding: 2.5rem 2rem;
      text-align: center;
      position: relative;
      box-shadow: 4px 4px 0 rgba(0,0,0,0.15), 8px 8px 0 rgba(0,0,0,0.08);
    }

    .about-sign::before {
      content: '';
      position: absolute;
      inset: 8px;
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 2px;
      pointer-events: none;
    }

    .sign-top-rope {
      display: flex;
      justify-content: center;
      gap: 3rem;
      margin-bottom: 1rem;
    }

    .sign-top-rope span {
      display: block;
      width: 2px;
      height: 24px;
      background: rgba(255,255,255,0.3);
      margin: 0 auto;
    }

    .sign-lantern {
      display: inline-flex;
      flex-direction: column;
      align-items: center;
      gap: 0.2rem;
    }

    .lantern-body {
      background: var(--noren-red);
      color: #fff;
      font-family: 'Zen Kurenaido', serif;
      font-size: 1.5rem;
      writing-mode: vertical-rl;
      letter-spacing: 0.1em;
      padding: 1.2rem 0.7rem;
      border-radius: 40% 40% 45% 45% / 30% 30% 50% 50%;
      box-shadow: inset 0 0 20px rgba(0,0,0,0.2), 0 4px 12px rgba(0,0,0,0.3);
      min-height: 100px;
    }

    .lantern-top, .lantern-bottom {
      width: 28px;
      height: 5px;
      background: #b8860b;
      border-radius: 2px;
    }

    .sign-store-name {
      font-family: 'Zen Kurenaido', serif;
      font-size: 3rem;
      color: #fff;
      letter-spacing: 0.2em;
      margin: 1.5rem 0 0.5rem;
      text-shadow: 0 2px 8px rgba(0,0,0,0.4);
    }

    .sign-en {
      font-size: 0.65rem;
      color: rgba(255,220,150,0.7);
      letter-spacing: 0.4em;
    }

    .sign-badge {
      display: inline-block;
      margin-top: 1.2rem;
      background: rgba(255,208,100,0.15);
      border: 1px solid rgba(255,208,100,0.4);
      color: rgba(255,220,150,0.9);
      font-size: 0.68rem;
      letter-spacing: 0.2em;
      padding: 0.4rem 1rem;
    }

    .stamp {
      position: absolute;
      bottom: -1rem;
      right: 1.5rem;
      width: 72px; height: 72px;
      border: 3px solid var(--noren-red);
      border-radius: 50%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      background: var(--warm-bg);
      transform: rotate(-15deg);
      box-shadow: 0 2px 8px rgba(0,0,0,0.12);
    }

    .stamp span {
      font-family: 'Zen Kurenaido', serif;
      font-size: 0.6rem;
      color: var(--noren-red);
      letter-spacing: 0.05em;
      line-height: 1.6;
      text-align: center;
    }

    .about-nums {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1px;
      background: var(--line);
      margin-top: 2rem;
      border: 1px solid var(--line);
    }

    .about-num-item {
      background: var(--paper);
      padding: 1rem;
      text-align: center;
    }

    .about-num-val {
      font-family: 'Kaisei Tokumin', serif;
      font-size: 1.8rem;
      color: var(--noren-red);
      font-weight: 700;
      line-height: 1;
    }

    .about-num-label {
      font-size: 0.68rem;
      color: var(--muted);
      letter-spacing: 0.1em;
      margin-top: 0.3rem;
    }

    /* ━━━━━━━━━━━━ PICKUP / お品書き ━━━━━━━━━━━━ */
    .pickup-bg {
      background: var(--warm-bg);
    }

    /* oshinagaki (お品書き) style menu */
    .oshinagaki-wrap {
      border: 1px solid var(--wood-light);
      background: var(--paper);
      padding: 1px;
    }

    .oshinagaki-inner {
      border: 1px solid rgba(139,94,60,0.3);
      padding: 2rem 2.5rem;
      position: relative;
    }

    .oshinagaki-title {
      font-family: 'Zen Kurenaido', serif;
      font-size: 1.1rem;
      letter-spacing: 0.3em;
      color: var(--ink);
      text-align: center;
      margin-bottom: 1.5rem;
      display: flex;
      align-items: center;
      gap: 1rem;
    }

    .oshinagaki-title::before,
    .oshinagaki-title::after {
      content: '';
      flex: 1;
      height: 1px;
      background: var(--line);
    }

    .menu-tabs {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      justify-content: center;
      margin-bottom: 2rem;
    }

    .menu-tab {
      background: transparent;
      border: 1px solid var(--wood-light);
      color: var(--muted);
      padding: 0.4rem 1rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.78rem;
      letter-spacing: 0.15em;
      cursor: pointer;
      transition: all 0.2s;
      border-radius: 1px;
    }

    .menu-tab:hover,
    .menu-tab.active {
      background: var(--noren-red);
      color: #fff;
      border-color: var(--noren-red);
    }

    .menu-grid {
      display: none;
      grid-template-columns: repeat(2, 1fr);
      gap: 0;
    }

    .menu-grid.active { display: grid; }

    .menu-item {
      display: flex;
      justify-content: space-between;
      align-items: baseline;
      padding: 0.65rem 0.5rem;
      border-bottom: 1px dashed rgba(139,94,60,0.2);
      gap: 0.5rem;
      transition: background 0.15s;
    }

    .menu-item:hover { background: rgba(192,57,43,0.04); }

    .menu-item-name {
      font-size: 0.82rem;
      letter-spacing: 0.04em;
      color: var(--text);
      line-height: 1.4;
    }

    .menu-item-name small {
      display: block;
      font-size: 0.68rem;
      color: var(--muted);
    }

    .menu-item-dots {
      flex: 1;
      height: 0;
      border-bottom: 1px dotted rgba(139,94,60,0.3);
      min-width: 10px;
    }

    .menu-item-price {
      font-family: 'Kaisei Tokumin', serif;
      font-size: 0.88rem;
      color: var(--noren-red);
      white-space: nowrap;
      font-weight: 700;
    }

    .menu-note {
      text-align: center;
      margin-top: 1.5rem;
      font-size: 0.72rem;
      color: var(--muted);
      letter-spacing: 0.08em;
    }

    /* ━━━━━━━━━━━━ FEATURED DISHES ━━━━━━━━━━━━ */
    .featured-bg {
      background: #2c1a0e;
      padding: 5rem 1.5rem;
    }

    .featured-inner { max-width: 960px; margin: 0 auto; }

    .featured-bg .section-heading .label {
      color: rgba(255,200,100,0.8);
      background: rgba(255,200,100,0.08);
      border-color: rgba(255,200,100,0.2);
    }

    .featured-bg .section-heading h2 { color: #fff; }
    .featured-bg .section-heading p { color: rgba(255,255,255,0.4); }
    .featured-bg .hanko-divider::before,
    .featured-bg .hanko-divider::after { background: rgba(255,255,255,0.15); }
    .featured-bg .hanko { border-color: rgba(255,200,100,0.5); color: rgba(255,200,100,0.8); }

    .featured-cards {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1.5rem;
      margin-top: 2.5rem;
    }

    .featured-card {
      background: rgba(255,255,255,0.04);
      border: 1px solid rgba(255,255,255,0.08);
      padding: 1.8rem 1.5rem;
      text-align: center;
      position: relative;
      transition: transform 0.3s, background 0.3s;
    }

    .featured-card:hover {
      transform: translateY(-4px);
      background: rgba(255,255,255,0.07);
    }

    .featured-card-num {
      position: absolute;
      top: -1px; left: 50%;
      transform: translateX(-50%);
      background: var(--noren-red);
      color: #fff;
      font-family: 'Kaisei Tokumin', serif;
      font-size: 0.65rem;
      letter-spacing: 0.2em;
      padding: 0.15rem 0.8rem;
    }

    .featured-card-icon {
      font-size: 2.8rem;
      margin: 1rem 0 0.8rem;
      line-height: 1;
    }

    .featured-card h3 {
      font-family: 'Zen Kurenaido', serif;
      font-size: 1.1rem;
      color: #fff;
      letter-spacing: 0.1em;
      margin-bottom: 0.5rem;
    }

    .featured-card-price {
      font-family: 'Kaisei Tokumin', serif;
      font-size: 1rem;
      color: rgba(255,200,100,0.9);
      font-weight: 700;
      margin-bottom: 0.8rem;
    }

    .featured-card p {
      font-size: 0.75rem;
      color: rgba(255,255,255,0.5);
      line-height: 1.9;
      letter-spacing: 0.05em;
    }

    /* ━━━━━━━━━━━━ REVIEWS ━━━━━━━━━━━━ */
    .reviews-bg { background: var(--paper); }

    .reviews-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1.5rem;
    }

    .review-card {
      background: var(--warm-bg);
      border: 1px solid var(--line);
      padding: 1.5rem;
      position: relative;
    }

    .review-card::before {
      content: '❝';
      position: absolute;
      top: 0.8rem; right: 1rem;
      font-size: 2.5rem;
      color: rgba(192,57,43,0.1);
      font-family: Georgia, serif;
      line-height: 1;
    }

    .review-stars {
      color: #f0a500;
      font-size: 0.85rem;
      letter-spacing: 0.1em;
      margin-bottom: 0.7rem;
    }

    .review-text {
      font-size: 0.8rem;
      line-height: 2;
      color: var(--text);
      margin-bottom: 1rem;
    }

    .review-meta {
      font-size: 0.66rem;
      color: var(--muted);
      letter-spacing: 0.08em;
      border-top: 1px dashed var(--line);
      padding-top: 0.6rem;
    }

    /* ━━━━━━━━━━━━ HOURS + INFO ━━━━━━━━━━━━ */
    .info-bg {
      background: var(--warm-bg);
      border-top: 1px solid var(--line);
    }

    .info-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 4rem;
      align-items: start;
    }

    .info-block-title {
      font-family: 'Zen Kurenaido', serif;
      font-size: 1.1rem;
      letter-spacing: 0.15em;
      color: var(--ink);
      margin-bottom: 1.2rem;
      padding-bottom: 0.7rem;
      border-bottom: 2px solid var(--noren-red);
      display: flex;
      align-items: center;
      gap: 0.6rem;
    }

    .info-block-title span {
      font-size: 1.1rem;
    }

    .hours-table {
      width: 100%;
      border-collapse: collapse;
    }

    .hours-table tr {
      border-bottom: 1px dashed var(--line);
    }

    .hours-table td {
      padding: 0.75rem 0.25rem;
      font-size: 0.85rem;
    }

    .hours-table td:first-child {
      width: 4.5rem;
      color: var(--muted);
      letter-spacing: 0.05em;
    }

    .hours-table td.open {
      color: var(--text);
      font-weight: 600;
    }

    .hours-table td.closed {
      color: var(--muted);
    }

    .hours-badge {
      display: inline-block;
      background: var(--matcha);
      color: #fff;
      font-size: 0.58rem;
      letter-spacing: 0.1em;
      padding: 0.1rem 0.4rem;
      border-radius: 2px;
      margin-left: 0.4rem;
      vertical-align: middle;
    }

    .hours-badge.closed-badge {
      background: var(--muted);
    }

    .hours-note {
      margin-top: 1rem;
      font-size: 0.72rem;
      color: var(--muted);
      line-height: 1.9;
      letter-spacing: 0.06em;
      background: rgba(139,94,60,0.06);
      padding: 0.8rem;
      border-left: 3px solid var(--wood-light);
    }

    .info-list {
      list-style: none;
    }

    .info-list li {
      display: flex;
      gap: 1rem;
      padding: 0.9rem 0;
      border-bottom: 1px dashed var(--line);
      font-size: 0.84rem;
      align-items: flex-start;
    }

    .info-list li .il-label {
      flex-shrink: 0;
      width: 4.5rem;
      color: var(--muted);
      font-size: 0.72rem;
      letter-spacing: 0.1em;
      padding-top: 0.1rem;
    }

    .info-list li .il-val {
      color: var(--text);
      line-height: 1.8;
    }

    .info-list li .il-val a {
      color: var(--noren-red);
      text-decoration: none;
      font-weight: 600;
    }

    /* ━━━━━━━━━━━━ PHONE CTA BANNER ━━━━━━━━━━━━ */
    .tel-banner {
      background: var(--noren-red);
      padding: 3.5rem 1.5rem;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .tel-banner::before {
      content: '';
      position: absolute;
      inset: 0;
      opacity: 0.06;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='56' height='28'%3E%3Cellipse cx='28' cy='28' rx='28' ry='28' fill='none' stroke='%23fff' stroke-width='1.5'/%3E%3Cellipse cx='0' cy='28' rx='28' ry='28' fill='none' stroke='%23fff' stroke-width='1.5'/%3E%3Cellipse cx='56' cy='28' rx='28' ry='28' fill='none' stroke='%23fff' stroke-width='1.5'/%3E%3C/svg%3E");
      background-size: 56px 28px;
    }

    .tel-banner-inner { position: relative; z-index: 1; }

    .tel-banner p {
      font-size: 0.78rem;
      letter-spacing: 0.3em;
      color: rgba(255,255,255,0.85);
      margin-bottom: 0.8rem;
    }

    .tel-number {
      display: block;
      font-family: 'Kaisei Tokumin', serif;
      font-size: clamp(2.2rem, 7vw, 3.5rem);
      font-weight: 700;
      color: #fff;
      letter-spacing: 0.08em;
      text-decoration: none;
      margin-bottom: 0.5rem;
      transition: opacity 0.2s;
    }

    .tel-number:hover { opacity: 0.85; }

    .tel-hours {
      font-size: 0.75rem;
      color: rgba(255,255,255,0.7);
      letter-spacing: 0.2em;
      margin-bottom: 2rem;
    }

    .btn-tel {
      display: inline-flex;
      align-items: center;
      gap: 0.6rem;
      background: #fff;
      color: var(--noren-red);
      padding: 0.9rem 2.2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.9rem;
      letter-spacing: 0.2em;
      font-weight: 700;
      text-decoration: none;
      border-radius: 2px;
      box-shadow: 0 4px 16px rgba(0,0,0,0.2);
      transition: all 0.25s;
    }

    .btn-tel:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 24px rgba(0,0,0,0.25);
    }

    /* ━━━━━━━━━━━━ ACCESS MAP ━━━━━━━━━━━━ */
    .access-bg { background: var(--paper); }

    .access-grid {
      display: grid;
      grid-template-columns: 1fr 1.5fr;
      gap: 3rem;
      align-items: start;
      margin-top: 2.5rem;
    }

    .access-detail {
      font-size: 0.84rem;
      line-height: 2;
      color: var(--text);
    }

    .access-detail strong {
      display: block;
      font-size: 0.65rem;
      letter-spacing: 0.3em;
      color: var(--muted);
      margin-top: 1.2rem;
      margin-bottom: 0.25rem;
    }

    .map-wrap { position: relative; }

    .map-frame {
      width: 100%;
      height: 340px;
      border: none;
      display: block;
      border: 1px solid var(--line);
    }

    .map-open-btn {
      display: flex;
      align-items: center;
      gap: 0.5rem;
      background: var(--noren-red);
      color: #fff;
      text-decoration: none;
      padding: 0.7rem 1.2rem;
      font-family: 'Shippori Mincho', serif;
      font-size: 0.78rem;
      letter-spacing: 0.15em;
      margin-top: 0.8rem;
      width: fit-content;
      transition: background 0.2s;
    }

    .map-open-btn:hover { background: var(--noren-dark); }

    /* ━━━━━━━━━━━━ FOOTER ━━━━━━━━━━━━ */
    footer {
      background: var(--ink);
      color: rgba(255,255,255,0.55);
      text-align: center;
      padding: 3rem 1.5rem 2rem;
    }

    .footer-logo {
      font-family: 'Zen Kurenaido', serif;
      font-size: 2.5rem;
      color: #fff;
      letter-spacing: 0.2em;
      margin-bottom: 0.5rem;
    }

    .footer-sub {
      font-size: 0.65rem;
      letter-spacing: 0.35em;
      color: rgba(255,255,255,0.3);
      margin-bottom: 1.5rem;
    }

    .footer-info {
      font-size: 0.75rem;
      line-height: 2;
      letter-spacing: 0.08em;
      margin-bottom: 2rem;
    }

    footer hr {
      border: none;
      border-top: 1px solid rgba(255,255,255,0.1);
      margin: 0 auto 1.5rem;
      max-width: 200px;
    }

    .footer-copy {
      font-size: 0.62rem;
      color: rgba(255,255,255,0.2);
      letter-spacing: 0.15em;
    }

    /* ━━━━━━━━━━━━ REVEAL ━━━━━━━━━━━━ */
    .reveal {
      opacity: 0;
      transform: translateY(18px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }

    .reveal.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* ━━━━━━━━━━━━ RESPONSIVE ━━━━━━━━━━━━ */
    @media (max-width: 768px) {
      nav { padding: 0 1rem; }

      .nav-links, .nav-tel { display: none; }

      .hamburger { display: flex; }

      .nav-links.open {
        display: flex;
        flex-direction: column;
        position: fixed;
        top: 58px; left: 0; right: 0;
        background: var(--noren-dark);
        padding: 1.5rem;
        gap: 1.2rem;
        border-top: 1px solid rgba(255,255,255,0.1);
        box-shadow: 0 8px 24px rgba(0,0,0,0.3);
      }

      .nav-links.open a { font-size: 1rem; color: #fff; }

      .hero-info-strip {
        gap: 1.5rem;
        bottom: 4rem;
      }

      .about-grid { grid-template-columns: 1fr; gap: 2.5rem; }

      .featured-cards {
        grid-template-columns: 1fr;
        gap: 1rem;
      }

      .reviews-grid { grid-template-columns: 1fr; }

      .info-grid { grid-template-columns: 1fr; gap: 2.5rem; }

      .access-grid { grid-template-columns: 1fr; gap: 1.5rem; }

      .menu-grid { grid-template-columns: 1fr; }

      .map-frame { height: 260px; }

      .section-wrap { padding: 4rem 1.2rem; }
    }

    @media (max-width: 480px) {
      .hero-info-strip { display: none; }
      .about-nums { grid-template-columns: repeat(3,1fr); }
    }
  </style>
</head>
<body>

<!-- ナビゲーション -->
<nav id="navbar">
  <a class="nav-logo" href="#">
    <div class="nav-logo-mark">ゆ</div>
    ゆきの
  </a>
  <ul class="nav-links" id="navLinks">
    <li><a href="#menu">お品書き</a></li>
    <li><a href="#hours">営業時間</a></li>
    <li><a href="#access">アクセス</a></li>
  </ul>
  <a href="tel:0980523486" class="nav-tel" id="navTel">
    📞 予約・お問い合わせ
  </a>
  <button class="hamburger" id="hamburger" aria-label="メニューを開く">
    <span></span><span></span><span></span>
  </button>
</nav>

<!-- ヒーロー -->
<section class="hero" id="top">
  <div class="hero-kanji-bg">ゆきの</div>
  <div class="hero-inner">
    <div class="hero-noren">名護・宮里の老舗居酒屋</div>
    <h1 class="hero-title">ゆきの</h1>
    <span class="hero-ruby">YUKINO IZAKAYA &amp; TEISHOKU</span>
    <p class="hero-tagline">
      地元の人に愛され続けて、もう何十年。<br>
      沖縄の食材と、おふくろの味を。
    </p>
    <div class="hero-divider">
      <span>✦</span>
    </div>
    <div class="hero-btns">
      <a href="#menu" class="btn-main">📋 お品書きを見る</a>
      <a href="tel:0980523486" class="btn-sub">📞 電話でご予約</a>
    </div>
  </div>
  <div class="hero-info-strip">
    <div class="hero-info-item">
      <span class="hero-info-label">OPEN</span>
      <span class="hero-info-val">17:00 〜 21:30</span>
    </div>
    <div class="hero-info-item">
      <span class="hero-info-label">CLOSED</span>
      <span class="hero-info-val">月・水 定休</span>
    </div>
    <div class="hero-info-item">
      <span class="hero-info-label">TEL</span>
      <span class="hero-info-val">0980-52-3486</span>
    </div>
    <div class="hero-info-item">
      <span class="hero-info-label">LOCATION</span>
      <span class="hero-info-val">名護市宮里</span>
    </div>
  </div>
</section>

<!-- お店について -->
<section class="about-bg">
  <div class="section-wrap">
    <div class="about-grid reveal">
      <div class="about-text">
        <div class="section-heading" style="text-align:left; margin-bottom:1.5rem;">
          <span class="label">ABOUT</span>
          <h2 style="font-size:1.8rem;">名護が誇る、<br>みんなの食堂</h2>
        </div>
        <div class="hanko-divider" style="justify-content:flex-start; margin-bottom:1.5rem;">
          <div class="hanko">ゆ</div>
          <div style="flex:0; height:1px; width:60px; background:var(--line);"></div>
        </div>
        <p>ホテルゆがふいんの真裏、名護市宮里に構える「<strong>ゆきの</strong>」は、地元の方々に長く愛され続けてきた定食・居酒屋です。</p>
        <p>定食だけで<strong>50種以上</strong>、一品料理や沖縄料理まで含めると総メニューは150種以上。アグー豚のやわらかステーキから新鮮な刺身、ゴーヤチャンプルーやラフテーまで、沖縄の恵みをたっぷりと。</p>
        <p>平日でも常に満席になるほどの賑わい。観光でいらした方にも「本物の沖縄の味」を楽しんでいただけます。<strong>予約がおすすめ</strong>です。</p>
        <div class="about-nums">
          <div class="about-num-item">
            <div class="about-num-val">50<span style="font-size:1rem">+</span></div>
            <div class="about-num-label">定食の種類</div>
          </div>
          <div class="about-num-item">
            <div class="about-num-val">150<span style="font-size:1rem">+</span></div>
            <div class="about-num-label">総メニュー数</div>
          </div>
          <div class="about-num-item">
            <div class="about-num-val">★5</div>
            <div class="about-num-label">Google口コミ</div>
          </div>
        </div>
      </div>
      <div class="about-stamp-area">
        <div class="about-sign">
          <div class="sign-top-rope">
            <span></span><span></span><span></span>
          </div>
          <div style="display:flex; justify-content:center; gap:1.5rem; margin-bottom:0.5rem;">
            <div class="sign-lantern">
              <div class="lantern-top"></div>
              <div class="lantern-body">居酒屋</div>
              <div class="lantern-bottom"></div>
            </div>
            <div class="sign-lantern">
              <div class="lantern-top"></div>
              <div class="lantern-body">定食</div>
              <div class="lantern-bottom"></div>
            </div>
          </div>
          <div class="sign-store-name">ゆきの</div>
          <div class="sign-en">YUKINO / NAGO, OKINAWA</div>
          <div class="sign-badge">泡盛ボトルキープ OK ／ 店内禁煙</div>
        </div>
        <div class="stamp">
          <span>地元<br>一番<br>人気</span>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- 人気メニュー PICKUP -->
<section class="featured-bg">
  <div class="featured-inner">
    <div class="section-heading reveal">
      <span class="label">POPULAR</span>
      <h2>おすすめ料理</h2>
      <p>お客さまに特に人気の一品です</p>
      <div class="hanko-divider"><div class="hanko" style="border-color:rgba(255,200,100,0.5); color:rgba(255,200,100,0.8);">推</div></div>
    </div>
    <div class="featured-cards">
      <div class="featured-card reveal">
        <div class="featured-card-num">人気 No.1</div>
        <div class="featured-card-icon">🥩</div>
        <h3>アグーのやわらかステーキ定食</h3>
        <div class="featured-card-price">¥1,600</div>
        <p>沖縄在来のブランド豚「アグー」を使ったやわらかステーキ。小鉢・汁物・ご飯付きでボリューム満点。</p>
      </div>
      <div class="featured-card reveal">
        <div class="featured-card-num">地元の定番</div>
        <div class="featured-card-icon">🍱</div>
        <h3>とんかつ定食</h3>
        <div class="featured-card-price">¥1,050</div>
        <p>「とんかつが旨い」と地元で評判。サクッと揚がった衣と肉汁あふれるカツ。長年愛され続ける看板メニュー。</p>
      </div>
      <div class="featured-card reveal">
        <div class="featured-card-num">沖縄の味</div>
        <div class="featured-card-icon">🍜</div>
        <h3>ゴーヤチャンプルー定食</h3>
        <div class="featured-card-price">¥1,150</div>
        <p>沖縄の夏野菜・ゴーヤをたっぷり使ったチャンプルー。素朴でほっとする、島の家庭料理の味。</p>
      </div>
      <div class="featured-card reveal">
        <div class="featured-card-num">お酒のアテに</div>
        <div class="featured-card-icon">🥟</div>
        <h3>島唐辛子の揚げ餃子</h3>
        <div class="featured-card-price">¥650</div>
        <p>沖縄の島唐辛子を使ったピリッと辛い揚げ餃子。泡盛との相性抜群、常連さんの必ずオーダーする一品。</p>
      </div>
      <div class="featured-card reveal">
        <div class="featured-card-num">刺身好き必見</div>
        <div class="featured-card-icon">🐟</div>
        <h3>刺身盛合せ（大）</h3>
        <div class="featured-card-price">¥3,000</div>
        <p>新鮮な魚介類をたっぷり盛り合わせ。イラブチャーなど沖縄ならではの魚も楽しめます。</p>
      </div>
      <div class="featured-card reveal">
        <div class="featured-card-num">沖縄の定番</div>
        <div class="featured-card-icon">🍖</div>
        <h3>ラフテー</h3>
        <div class="featured-card-price">¥850</div>
        <p>じっくり煮込んだ豚の角煮。味がしっかりしみた本格ラフテー。泡盛と一緒にどうぞ。</p>
      </div>
    </div>
  </div>
</section>

<!-- お品書き / MENU -->
<section class="pickup-bg" id="menu">
  <div class="section-wrap">
    <div class="section-heading reveal">
      <span class="label">MENU</span>
      <h2>お品書き</h2>
      <p>定食・沖縄料理・一品料理など150種以上</p>
      <div class="hanko-divider"><div class="hanko">品</div></div>
    </div>
    <div class="oshinagaki-wrap reveal">
      <div class="oshinagaki-inner">
        <div class="oshinagaki-title">メニュー一覧</div>

        <div class="menu-tabs">
          <button class="menu-tab active" onclick="showTab('teishoku',this)">定食</button>
          <button class="menu-tab" onclick="showTab('curry',this)">カレー</button>
          <button class="menu-tab" onclick="showTab('donburi',this)">丼ぶり</button>
          <button class="menu-tab" onclick="showTab('okinawa',this)">沖縄料理</button>
          <button class="menu-tab" onclick="showTab('sashimi',this)">刺身・寿司</button>
          <button class="menu-tab" onclick="showTab('ippin',this)">一品料理</button>
          <button class="menu-tab" onclick="showTab('men',this)">麺・ご飯</button>
        </div>

        <div class="menu-grid active" id="tab-teishoku">
          <div class="menu-item"><span class="menu-item-name">アグーのやわらかステーキ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,600円</span></div>
          <div class="menu-item"><span class="menu-item-name">アグーのミルフィーユカツ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,250円</span></div>
          <div class="menu-item"><span class="menu-item-name">とんかつ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,050円</span></div>
          <div class="menu-item"><span class="menu-item-name">ヒレカツ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,250円</span></div>
          <div class="menu-item"><span class="menu-item-name">ささみのチーズカツ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">海老フライ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,350円</span></div>
          <div class="menu-item"><span class="menu-item-name">魚フライ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">カキフライ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">赤魚の切身バター焼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">2,000円</span></div>
          <div class="menu-item"><span class="menu-item-name">赤魚の切身煮付定食</span><span class="menu-item-dots"></span><span class="menu-item-price">2,000円</span></div>
          <div class="menu-item"><span class="menu-item-name">刺身定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,800円</span></div>
          <div class="menu-item"><span class="menu-item-name">天ぷら定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,800円</span></div>
          <div class="menu-item"><span class="menu-item-name">うな重定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,700円</span></div>
          <div class="menu-item"><span class="menu-item-name">カットステーキ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,600円</span></div>
          <div class="menu-item"><span class="menu-item-name">焼肉定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,300円</span></div>
          <div class="menu-item"><span class="menu-item-name">しょうが焼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">ゴーヤチャンプルー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,150円</span></div>
          <div class="menu-item"><span class="menu-item-name">沖縄そば定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">チキン唐揚げ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">チキン唐マヨ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,150円</span></div>
          <div class="menu-item"><span class="menu-item-name">チーズハンバーグ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">エビチリ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">牛みそ定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,200円</span></div>
          <div class="menu-item"><span class="menu-item-name">豚肉キムチ炒め定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,200円</span></div>
          <div class="menu-item"><span class="menu-item-name">マーボー豆腐定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">野菜炒め定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">みそ汁定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,050円</span></div>
          <div class="menu-item"><span class="menu-item-name">お子様ランチ</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
        </div>

        <div class="menu-grid" id="tab-curry">
          <div class="menu-item"><span class="menu-item-name">カツカレー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,200円</span></div>
          <div class="menu-item"><span class="menu-item-name">チキン唐揚げカレー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,200円</span></div>
          <div class="menu-item"><span class="menu-item-name">コロッケカレー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">エビフライカレー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,450円</span></div>
          <div class="menu-item"><span class="menu-item-name">カキフライカレー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,200円</span></div>
          <div class="menu-item"><span class="menu-item-name">魚フライカレー定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,200円</span></div>
        </div>

        <div class="menu-grid" id="tab-donburi">
          <div class="menu-item"><span class="menu-item-name">カツ丼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,300円</span></div>
          <div class="menu-item"><span class="menu-item-name">親子丼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,300円</span></div>
          <div class="menu-item"><span class="menu-item-name">天丼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,400円</span></div>
          <div class="menu-item"><span class="menu-item-name">まぐろやまかけ丼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,400円</span></div>
          <div class="menu-item"><span class="menu-item-name">まぐろ丼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,600円</span></div>
          <div class="menu-item"><span class="menu-item-name">鉄火丼定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,600円</span></div>
        </div>

        <div class="menu-grid" id="tab-okinawa">
          <div class="menu-item"><span class="menu-item-name">アグーの柔らかステーキ</span><span class="menu-item-dots"></span><span class="menu-item-price">1,300円</span></div>
          <div class="menu-item"><span class="menu-item-name">やぎ刺</span><span class="menu-item-dots"></span><span class="menu-item-price">1,500円</span></div>
          <div class="menu-item"><span class="menu-item-name">沖縄そば</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">ゴーヤチャンプルー</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">フーチャンプルー</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">野菜チャンプルー</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">ソーメンチャンプルー</span><span class="menu-item-dots"></span><span class="menu-item-price">700円</span></div>
          <div class="menu-item"><span class="menu-item-name">ピリ辛ソーメンチャンプルー</span><span class="menu-item-dots"></span><span class="menu-item-price">700円</span></div>
          <div class="menu-item"><span class="menu-item-name">ラフテー</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">海ぶどう</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">もずく酢</span><span class="menu-item-dots"></span><span class="menu-item-price">600円</span></div>
          <div class="menu-item"><span class="menu-item-name">もずく天ぷら（大）</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">もずく天ぷら（小）</span><span class="menu-item-dots"></span><span class="menu-item-price">500円</span></div>
          <div class="menu-item"><span class="menu-item-name">ぐるくん唐揚</span><span class="menu-item-dots"></span><span class="menu-item-price">750円</span></div>
          <div class="menu-item"><span class="menu-item-name">ジーマーミ豆腐</span><span class="menu-item-dots"></span><span class="menu-item-price">500円</span></div>
          <div class="menu-item"><span class="menu-item-name">スーチカー</span><span class="menu-item-dots"></span><span class="menu-item-price">650円</span></div>
          <div class="menu-item"><span class="menu-item-name">アグーの焼き餃子</span><span class="menu-item-dots"></span><span class="menu-item-price">700円</span></div>
          <div class="menu-item"><span class="menu-item-name">島唐辛子の揚げ餃子</span><span class="menu-item-dots"></span><span class="menu-item-price">650円</span></div>
          <div class="menu-item"><span class="menu-item-name">タロイモの甘うまソースあえ</span><span class="menu-item-dots"></span><span class="menu-item-price">600円</span></div>
          <div class="menu-item"><span class="menu-item-name">中味もやし炒め</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">スーチカーキャベツ炒め</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">人参しりしり</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
        </div>

        <div class="menu-grid" id="tab-sashimi">
          <div class="menu-item"><span class="menu-item-name">マグロ刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">1,050円</span></div>
          <div class="menu-item"><span class="menu-item-name">さば刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">白身刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">1,050円</span></div>
          <div class="menu-item"><span class="menu-item-name">タコ刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">イラブチャー刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">サーモン刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">1,050円</span></div>
          <div class="menu-item"><span class="menu-item-name">セイイカ刺身</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">刺身盛合せ（小）</span><span class="menu-item-dots"></span><span class="menu-item-price">1,500円</span></div>
          <div class="menu-item"><span class="menu-item-name">刺身盛合せ（大）</span><span class="menu-item-dots"></span><span class="menu-item-price">3,000円</span></div>
          <div class="menu-item"><span class="menu-item-name">海鮮みそあえ（小/大）</span><span class="menu-item-dots"></span><span class="menu-item-price">700/1,400円</span></div>
          <div class="menu-item"><span class="menu-item-name">海鮮キムチあえ（小/大）</span><span class="menu-item-dots"></span><span class="menu-item-price">700/1,400円</span></div>
          <div class="menu-item"><span class="menu-item-name">寿司定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,700円</span></div>
          <div class="menu-item"><span class="menu-item-name">ちらし定食</span><span class="menu-item-dots"></span><span class="menu-item-price">1,700円</span></div>
          <div class="menu-item"><span class="menu-item-name">鉄火巻・納豆巻・カッパ巻ほか</span><span class="menu-item-dots"></span><span class="menu-item-price">各700円</span></div>
        </div>

        <div class="menu-grid" id="tab-ippin">
          <div class="menu-item"><span class="menu-item-name">チキン唐揚</span><span class="menu-item-dots"></span><span class="menu-item-price">750円</span></div>
          <div class="menu-item"><span class="menu-item-name">チキン唐マヨ</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">手羽餃子</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">ホタテのウニソース焼</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">カマンベールチーズフライ</span><span class="menu-item-dots"></span><span class="menu-item-price">600円</span></div>
          <div class="menu-item"><span class="menu-item-name">カットステーキ</span><span class="menu-item-dots"></span><span class="menu-item-price">1,300円</span></div>
          <div class="menu-item"><span class="menu-item-name">赤魚の切身バター焼</span><span class="menu-item-dots"></span><span class="menu-item-price">1,700円</span></div>
          <div class="menu-item"><span class="menu-item-name">赤魚の切身煮付</span><span class="menu-item-dots"></span><span class="menu-item-price">1,700円</span></div>
          <div class="menu-item"><span class="menu-item-name">イカゲソ唐揚</span><span class="menu-item-dots"></span><span class="menu-item-price">700円</span></div>
          <div class="menu-item"><span class="menu-item-name">タコ唐揚</span><span class="menu-item-dots"></span><span class="menu-item-price">750円</span></div>
          <div class="menu-item"><span class="menu-item-name">砂肝唐揚</span><span class="menu-item-dots"></span><span class="menu-item-price">700円</span></div>
          <div class="menu-item"><span class="menu-item-name">エビチリ</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">揚げ出し豆腐</span><span class="menu-item-dots"></span><span class="menu-item-price">500円</span></div>
          <div class="menu-item"><span class="menu-item-name">冷奴</span><span class="menu-item-dots"></span><span class="menu-item-price">400円</span></div>
          <div class="menu-item"><span class="menu-item-name">枝豆</span><span class="menu-item-dots"></span><span class="menu-item-price">500円</span></div>
          <div class="menu-item"><span class="menu-item-name">ポテトフライ</span><span class="menu-item-dots"></span><span class="menu-item-price">500円</span></div>
          <div class="menu-item"><span class="menu-item-name">焼鳥（タレ・塩）</span><span class="menu-item-dots"></span><span class="menu-item-price">550円</span></div>
          <div class="menu-item"><span class="menu-item-name">豚バラ串 / つくね</span><span class="menu-item-dots"></span><span class="menu-item-price">各550円</span></div>
          <div class="menu-item"><span class="menu-item-name">さばの塩焼</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">ほっけ</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
        </div>

        <div class="menu-grid" id="tab-men">
          <div class="menu-item"><span class="menu-item-name">沖縄そば</span><span class="menu-item-dots"></span><span class="menu-item-price">850円</span></div>
          <div class="menu-item"><span class="menu-item-name">焼うどん（塩・ケチャップ）</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">焼きそば（塩・ケチャップ）</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">ピリうまキムチうどん</span><span class="menu-item-dots"></span><span class="menu-item-price">900円</span></div>
          <div class="menu-item"><span class="menu-item-name">牛肉もやしそば</span><span class="menu-item-dots"></span><span class="menu-item-price">1,100円</span></div>
          <div class="menu-item"><span class="menu-item-name">チャーハン</span><span class="menu-item-dots"></span><span class="menu-item-price">800円</span></div>
          <div class="menu-item"><span class="menu-item-name">玉子雑炊</span><span class="menu-item-dots"></span><span class="menu-item-price">750円</span></div>
          <div class="menu-item"><span class="menu-item-name">お茶漬け（のり・うめ）</span><span class="menu-item-dots"></span><span class="menu-item-price">600円</span></div>
          <div class="menu-item"><span class="menu-item-name">ライス</span><span class="menu-item-dots"></span><span class="menu-item-price">150円</span></div>
        </div>

        <p class="menu-note">※ 価格はすべて税込。仕入れ状況によりメニュー・価格が変更となる場合があります。</p>
      </div>
    </div>
  </div>
</section>

<!-- お客様の声 -->
<section class="reviews-bg">
  <div class="section-wrap">
    <div class="section-heading reveal">
      <span class="label">REVIEWS</span>
      <h2>お客様の声</h2>
      <p>Google口コミより</p>
      <div class="hanko-divider"><div class="hanko">声</div></div>
    </div>
    <div class="reviews-grid">
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">料理の味・量は大満足。沖縄の郷土料理を美味しく頂けました。地元の方も食べに来ていて、美味しい証拠。非常に満足でした。</p>
        <div class="review-meta">★5 — 8か月前</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">超昔からあるファミリー居酒屋。メニュー数がめちゃくちゃ多くて迷いました。活気がすごくてとても良い雰囲気。名護に行ったらまた行きたいお店です。</p>
        <div class="review-meta">★5 — 5か月前</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">結構好きな店でたまに寄ります。泡盛のボトルキープもできます。定食を頼むと小鉢も多いので定食で一杯やるのもあり。回転しているので多少待てば入れます。</p>
        <div class="review-meta">★5 — 1年前</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">ラフテーは味がしみてて最高。グルクン唐揚げは魚嫌いな息子も絶賛！一口サイズで食べやすかった。17:30に予約なしで行ったらギリでした。行くなら予約推奨！</p>
        <div class="review-meta">★5 — 1年前</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★☆</div>
        <p class="review-text">定食系だけで50種類以上。アルコール類もお手頃で1人3,000円。旅先のファミリー夕食にお安いですよ。手羽餃子・島唐辛子の揚げ餃子もどちらも旨かった！</p>
        <div class="review-meta">★4 — 7か月前</div>
      </div>
      <div class="review-card reveal">
        <div class="review-stars">★★★★★</div>
        <p class="review-text">店内禁煙で良かったです。繁盛していました。夜も定食メニューをしているのでお手頃に沖縄料理が食べられる良心的なお店。座敷が多くて沖縄らしくて良い雰囲気でした。</p>
        <div class="review-meta">★5 — 8か月前</div>
      </div>
    </div>
  </div>
</section>

<!-- 営業時間・店舗情報 -->
<section class="info-bg" id="hours">
  <div class="section-wrap">
    <div class="section-heading reveal">
      <span class="label">INFO</span>
      <h2>営業時間・店舗情報</h2>
      <div class="hanko-divider"><div class="hanko">情</div></div>
    </div>
    <div class="info-grid reveal">
      <div>
        <div class="info-block-title"><span>🕐</span> 営業時間</div>
        <table class="hours-table">
          <tr><td>月曜日</td><td class="closed">定休日 <span class="hours-badge closed-badge">休</span></td></tr>
          <tr><td>火曜日</td><td class="open">17:00 〜 21:30 <span class="hours-badge">営</span></td></tr>
          <tr><td>水曜日</td><td class="closed">定休日 <span class="hours-badge closed-badge">休</span></td></tr>
          <tr><td>木曜日</td><td class="open">17:00 〜 21:30 <span class="hours-badge">営</span></td></tr>
          <tr><td>金曜日</td><td class="open">17:00 〜 21:30 <span class="hours-badge">営</span></td></tr>
          <tr><td>土曜日</td><td class="open">17:00 〜 21:30 <span class="hours-badge">営</span></td></tr>
          <tr><td>日曜日</td><td class="open">17:00 〜 21:30 <span class="hours-badge">営</span></td></tr>
        </table>
        <div class="hours-note">
          ※ 大変混み合うため、お越しの際は<strong>ご予約をおすすめします</strong>。<br>
          ※ 仕入れ状況によりメニューが変わる場合があります。
        </div>
      </div>
      <div>
        <div class="info-block-title"><span>🏮</span> 店舗情報</div>
        <ul class="info-list">
          <li>
            <span class="il-label">店名</span>
            <span class="il-val">ゆきの（定食・居酒屋）</span>
          </li>
          <li>
            <span class="il-label">住所</span>
            <span class="il-val">〒905-0011<br>沖縄県名護市宮里450−8</span>
          </li>
          <li>
            <span class="il-label">電話</span>
            <span class="il-val"><a href="tel:0980523486">0980-52-3486</a></span>
          </li>
          <li>
            <span class="il-label">アクセス</span>
            <span class="il-val">ホテルゆがふいん名護 真裏<br>喜瀬周辺リゾートからも好アクセス</span>
          </li>
          <li>
            <span class="il-label">特徴</span>
            <span class="il-val">店内禁煙 / 泡盛ボトルキープ可<br>座敷あり / 大人数OK</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- 電話予約バナー -->
<div class="tel-banner">
  <div class="tel-banner-inner">
    <p>📞 RESERVATION — ご予約・お問い合わせ</p>
    <a class="tel-number" href="tel:0980523486">0980-52-3486</a>
    <p class="tel-hours">営業時間内受付 ／ 火・木・金・土・日　17:00〜21:30</p>
    <a class="btn-tel" href="tel:0980523486">今すぐ電話する</a>
  </div>
</div>

<!-- アクセス -->
<section class="access-bg" id="access">
  <div class="section-wrap">
    <div class="section-heading reveal">
      <span class="label">ACCESS</span>
      <h2>アクセス</h2>
      <p>沖縄県名護市宮里450−8</p>
      <div class="hanko-divider"><div class="hanko">地</div></div>
    </div>
    <div class="access-grid reveal">
      <div>
        <div class="access-detail">
          <strong>住所</strong>
          〒905-0011<br>沖縄県名護市宮里450−8
          <strong>最寄り目印</strong>
          ホテルゆがふいん名護の真裏<br>
          喜瀬・名護リゾートエリアから車ですぐ
          <strong>営業時間</strong>
          火・木・金・土・日<br>17:00 〜 21:30<br>（月・水 定休）
          <strong>電話番号</strong>
          <a href="tel:0980523486" style="color:var(--noren-red); font-size:1.15rem; font-weight:700; text-decoration:none;">0980-52-3486</a>
        </div>
        <br>
        <a href="https://maps.app.goo.gl/eURE5MPN7vzDD2gp8" target="_blank" rel="noopener" class="map-open-btn">
          📍 Google マップで開く
        </a>
      </div>
      <div class="map-wrap">
        <iframe
          class="map-frame"
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d906.9!2d127.9799!3d26.5865!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x34e5a9e7b6f7b5a9%3A0x1234567890abcdef!2z5oKT56ys5a6kICh55Yuk44Gu5a+M44KB44KJ44K544OG44O844Kt5a+M6Z2S5qCh6Imv5YKZ44GV44KT44Gu6aOf6K2YKeWtpumDqOaVsOWksei0o-mVtw!5e0!3m2!1sja!2sjp!4v1234567890"
          allowfullscreen=""
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
          title="居酒屋ゆきの 地図">
        </iframe>
      </div>
    </div>
  </div>
</section>

<!-- フッター -->
<footer>
  <div class="footer-logo">ゆきの</div>
  <div class="footer-sub">YUKINO IZAKAYA &amp; TEISHOKU / NAGO, OKINAWA</div>
  <div class="footer-info">
    〒905-0011　沖縄県名護市宮里450−8<br>
    TEL：0980-52-3486<br>
    営業：17:00〜21:30（火・木・金・土・日）　定休：月・水
  </div>
  <hr>
  <p class="footer-copy">© ゆきの All Rights Reserved.</p>
</footer>

<script>
  // ── ハンバーガーメニュー ──
  const hamburger = document.getElementById('hamburger');
  const navLinks = document.getElementById('navLinks');
  hamburger.addEventListener('click', () => {
    navLinks.classList.toggle('open');
  });

  // ── ナビ 電話ボタン 出し分け ──
  const navTel = document.getElementById('navTel');
  function checkNav() {
    navTel.style.display = window.innerWidth > 768 ? 'flex' : 'none';
  }
  checkNav();
  window.addEventListener('resize', checkNav);

  // ── メニュータブ ──
  function showTab(id, btn) {
    document.querySelectorAll('.menu-grid').forEach(g => g.classList.remove('active'));
    document.querySelectorAll('.menu-tab').forEach(t => t.classList.remove('active'));
    document.getElementById('tab-' + id).classList.add('active');
    btn.classList.add('active');
  }

  // ── スクロールリビール ──
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver((entries) => {
    entries.forEach((entry, i) => {
      if (entry.isIntersecting) {
        setTimeout(() => entry.target.classList.add('visible'), i * 60);
        observer.unobserve(entry.target);
      }
    });
  }, { threshold: 0.08 });
  reveals.forEach(el => observer.observe(el));
</script>
</body>
</html>
