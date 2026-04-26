<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>HcheirosoMA • Perfumes Importados</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;500;600;700&family=Montserrat:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --marrom:     #7b2f0c;
      --marrom-esc: #4a1c05;
      --marrom-med: #8c3a10;
      --ouro:       #c9a84c;
      --ouro-cl:    #e8d08a;
      --creme:      #f5ead8;
      --mut:        #c8a882;
      --card:       rgba(255,255,255,0.05);
      --borda:      rgba(201,168,76,0.25);
      --radius:     16px;
    }
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    body {
      font-family: 'Montserrat', sans-serif;
      background: var(--marrom);
      color: var(--creme);
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
      overflow-x: hidden;
    }
    a { color: inherit; text-decoration: none; }
    img { max-width: 100%; display: block; }

    /* HEADER */
    header {
      position: fixed;
      top: 0; left: 0; right: 0;
      z-index: 999;
      background: rgba(74,28,5,0.88);
      backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(201,168,76,0.15);
      padding: 16px 0;
    }
    .nav {
      max-width: 1200px; margin: 0 auto; padding: 0 24px;
      display: flex; align-items: center; justify-content: space-between;
    }
    .logo {
      font-family: 'Cormorant Garamond', serif;
      font-size: 20px; font-weight: 600; letter-spacing: 0.08em;
    }
    .logo span { color: var(--ouro); }
    .nav-links { display: flex; gap: 36px; list-style: none; }
    .nav-links a {
      font-size: 11px; font-weight: 500;
      letter-spacing: 0.28em; text-transform: uppercase;
      opacity: 0.85; transition: color 0.2s, opacity 0.2s;
    }
    .nav-links a:hover { opacity: 1; color: var(--ouro); }
    .menu-btn {
      display: none; background: none; border: none;
      cursor: pointer; flex-direction: column; gap: 5px; padding: 4px;
    }
    .menu-btn span {
      display: block; width: 22px; height: 2px;
      background: var(--creme); border-radius: 2px;
    }
    .nav-mobile {
      display: none; flex-direction: column;
      background: rgba(74,28,5,0.97);
      padding: 16px 24px;
      border-top: 1px solid rgba(201,168,76,0.1);
    }
    .nav-mobile.aberto { display: flex; }
    .nav-mobile a {
      padding: 12px 0; font-size: 13px;
      letter-spacing: 0.22em; text-transform: uppercase;
      border-bottom: 1px solid rgba(201,168,76,0.1);
    }
    .nav-mobile a:hover { color: var(--ouro); }

    /* HERO */
    .hero {
      min-height: 100vh;
      display: flex; align-items: center;
      padding: 100px 24px 60px;
      background: radial-gradient(ellipse at 65% 45%, #9b3f12 0%, #5e2208 45%, #3a1404 100%);
      position: relative; overflow: hidden;
    }
    .hero::before {
      content: '';
      position: absolute; inset: 0;
      background: radial-gradient(circle at 75% 55%, rgba(201,168,76,0.07) 0%, transparent 55%);
    }
    .hero-inner {
      max-width: 1200px; width: 100%; margin: 0 auto;
      display: grid; grid-template-columns: 1fr 1fr;
      gap: 60px; align-items: center;
      position: relative; z-index: 2;
    }
    .hero-label {
      font-size: 11px; font-weight: 500;
      letter-spacing: 0.35em; text-transform: uppercase;
      color: var(--ouro); margin-bottom: 16px;
      display: flex; align-items: center; gap: 10px;
    }
    .hero-label::before {
      content: ''; display: block;
      width: 28px; height: 1px; background: var(--ouro);
    }
    .hero-titulo {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(48px, 6vw, 86px);
      font-weight: 300; line-height: 0.95; margin-bottom: 22px;
    }
    .hero-titulo em { font-style: italic; color: var(--ouro-cl); }
    .hero-desc {
      font-size: 13px; color: var(--mut);
      max-width: 400px; margin-bottom: 32px;
      letter-spacing: 0.04em; line-height: 1.9;
    }
    .hero-btns { display: flex; gap: 12px; flex-wrap: wrap; margin-bottom: 44px; }
    .btn {
      font-family: 'Montserrat', sans-serif;
      font-size: 11px; font-weight: 700;
      letter-spacing: 0.26em; text-transform: uppercase;
      padding: 14px 32px; border-radius: 999px;
      cursor: pointer; transition: all 0.22s;
      display: inline-flex; align-items: center; gap: 8px; border: none;
    }
    .btn-creme { background: var(--creme); color: var(--marrom-esc); }
    .btn-creme:hover { background: var(--ouro-cl); transform: translateY(-2px); box-shadow: 0 10px 28px rgba(0,0,0,0.35); }
    .btn-borda { background: transparent; color: var(--creme); border: 1px solid rgba(245,234,216,0.35); }
    .btn-borda:hover { border-color: var(--ouro); color: var(--ouro); }
    .hero-selos { display: flex; gap: 24px; flex-wrap: wrap; }
    .selo-num {
      font-family: 'Cormorant Garamond', serif;
      font-size: 26px; font-weight: 600; color: var(--ouro); line-height: 1;
    }
    .selo-txt { font-size: 10px; letter-spacing: 0.18em; text-transform: uppercase; color: var(--mut); }
    .selo-div { width: 1px; background: rgba(201,168,76,0.2); align-self: stretch; }
    .hero-img-lado {
      display: flex; align-items: center; justify-content: center; position: relative;
    }
    .hero-glow {
      position: absolute; width: 300px; height: 300px;
      background: radial-gradient(circle, rgba(201,168,76,0.14) 0%, transparent 70%);
      border-radius: 50%;
    }
    .hero-foto {
      width: 100%; max-width: 400px; border-radius: 12px;
      box-shadow: 0 40px 80px rgba(0,0,0,0.55);
      position: relative; z-index: 2;
    }

    /* CONTAINER */
    .container { max-width: 1200px; margin: 0 auto; padding: 0 24px; }

    /* SEÇÕES */
    .secao { padding: 80px 0; }
    .secao-label {
      font-size: 10px; font-weight: 600;
      letter-spacing: 0.35em; text-transform: uppercase;
      color: var(--ouro); margin-bottom: 8px;
      display: flex; align-items: center; gap: 10px;
    }
    .secao-label::before { content: ''; display: block; width: 22px; height: 1px; background: var(--ouro); }
    .secao-titulo {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(28px, 4vw, 46px);
      font-weight: 400; color: var(--creme); margin-bottom: 8px; line-height: 1.1;
    }
    .secao-sub { font-size: 13px; color: var(--mut); margin-bottom: 40px; max-width: 500px; line-height: 1.8; }

    /* SOBRE */
    #sobre { background: linear-gradient(180deg, var(--marrom) 0%, var(--marrom-esc) 100%); }
    .sobre-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 56px; align-items: center; }
    .sobre-img-box { position: relative; border-radius: var(--radius); overflow: visible; }
    .sobre-foto { width: 100%; height: 440px; object-fit: cover; border-radius: var(--radius); box-shadow: 0 24px 60px rgba(0,0,0,0.45); display: block; }
    .sobre-ornamento {
      position: absolute; bottom: -14px; right: -14px;
      width: 64px; height: 64px; background: var(--ouro);
      border-radius: 50%; display: flex; align-items: center;
      justify-content: center; font-size: 26px;
      box-shadow: 0 8px 24px rgba(0,0,0,0.3); z-index: 2;
    }
    .sobre-texto p { font-size: 14px; color: var(--mut); line-height: 1.9; margin-bottom: 16px; }
    .features { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-top: 24px; }
    .feature {
      display: flex; align-items: flex-start; gap: 10px;
      background: var(--card); border: 1px solid var(--borda);
      border-radius: 10px; padding: 12px;
    }
    .feature-ico { font-size: 18px; flex-shrink: 0; }
    .feature-txt { font-size: 12px; color: var(--mut); }
    .feature-txt strong { display: block; color: var(--creme); margin-bottom: 2px; font-size: 13px; }

    /* DESTAQUES */
    #destaques { background: rgba(0,0,0,0.12); }
    .destaques-scroll {
      display: flex; gap: 16px; overflow-x: auto; padding-bottom: 10px;
      scrollbar-width: thin; scrollbar-color: var(--ouro) transparent;
    }
    .destaques-scroll::-webkit-scrollbar { height: 3px; }
    .destaques-scroll::-webkit-scrollbar-thumb { background: var(--ouro); border-radius: 999px; }
    .d-card {
      min-width: 200px; max-width: 200px;
      background: var(--card); border: 1px solid var(--borda);
      border-radius: var(--radius); overflow: hidden; flex-shrink: 0;
      transition: transform 0.22s, box-shadow 0.22s;
    }
    .d-card:hover { transform: translateY(-5px); box-shadow: 0 20px 40px rgba(0,0,0,0.4); }
    .d-img-wrap {
      width: 100%; height: 155px;
      background: rgba(201,168,76,0.06);
      display: flex; align-items: center; justify-content: center;
      overflow: hidden; position: relative;
    }
    .d-img-wrap img { width: 100%; height: 100%; object-fit: cover; }
    .d-sem-img { font-size: 10px; color: var(--mut); text-align: center; letter-spacing: 0.1em; }
    .d-upload {
      position: absolute; bottom: 6px; right: 6px;
      background: rgba(0,0,0,0.6); border: 1px solid var(--ouro);
      border-radius: 999px; padding: 3px 9px;
      font-size: 9px; color: var(--ouro); cursor: pointer; letter-spacing: 0.1em;
    }
    .d-upload:hover { background: var(--ouro); color: var(--marrom-esc); }
    .d-info { padding: 12px; }
    .d-marca { font-size: 10px; letter-spacing: 0.22em; text-transform: uppercase; color: var(--ouro); margin-bottom: 3px; }
    .d-nome { font-family: 'Cormorant Garamond', serif; font-size: 15px; font-weight: 500; margin-bottom: 4px; }
    .d-preco { font-size: 14px; font-weight: 600; color: var(--ouro); margin-bottom: 6px; }
    .est-mini { display: flex; align-items: center; gap: 6px; margin-bottom: 8px; }
    .dot { width: 7px; height: 7px; border-radius: 50%; flex-shrink: 0; }
    .dot-ok  { background: #4caf50; }
    .dot-low { background: #ff9800; }
    .dot-out { background: #f44336; }
    .est-txt { font-size: 10px; color: var(--mut); letter-spacing: 0.1em; }
    .d-btn {
      display: block; text-align: center;
      font-size: 10px; font-weight: 700; letter-spacing: 0.2em;
      text-transform: uppercase; padding: 8px 12px; border-radius: 999px;
      background: linear-gradient(135deg, var(--ouro), var(--ouro-cl));
      color: var(--marrom-esc); transition: filter 0.15s, transform 0.15s;
    }
    .d-btn:hover { filter: brightness(1.08); transform: translateY(-1px); }

    /* BUSCA */
    .busca-wrap { margin-bottom: 32px; }
    .busca-box {
      display: flex; align-items: center; gap: 10px;
      background: rgba(255,255,255,0.05); border: 1px solid var(--borda);
      border-radius: 999px; padding: 11px 20px; max-width: 420px;
      transition: border-color 0.2s;
    }
    .busca-box:focus-within { border-color: var(--ouro); }
    .busca-box input {
      background: none; border: none; outline: none;
      color: var(--creme); font-size: 13px;
      font-family: 'Montserrat', sans-serif; width: 100%;
    }
    .busca-box input::placeholder { color: var(--mut); }

    /* PRODUTOS */
    #produtos { background: var(--marrom-esc); }
    .produtos-grid { display: grid; grid-template-columns: repeat(3, minmax(0,1fr)); gap: 20px; }
    .p-card {
      background: var(--card); border: 1px solid var(--borda);
      border-radius: var(--radius); overflow: hidden;
      display: flex; flex-direction: column;
      transition: transform 0.22s, box-shadow 0.22s;
    }
    .p-card:hover { transform: translateY(-6px); box-shadow: 0 28px 56px rgba(0,0,0,0.5); }
    .p-img-wrap {
      width: 100%; height: 190px;
      background: rgba(201,168,76,0.05);
      display: flex; align-items: center; justify-content: center;
      overflow: hidden; position: relative;
    }
    .p-img-wrap img { width: 100%; height: 100%; object-fit: cover; }
    .p-sem-img { font-size: 11px; color: var(--mut); text-align: center; padding: 10px; letter-spacing: 0.08em; }
    .p-upload {
      position: absolute; bottom: 8px; right: 8px;
      background: rgba(0,0,0,0.65); border: 1px solid var(--ouro);
      border-radius: 999px; padding: 4px 10px;
      font-size: 10px; color: var(--ouro); cursor: pointer; letter-spacing: 0.1em;
    }
    .p-upload:hover { background: var(--ouro); color: var(--marrom-esc); }
    .p-corpo { padding: 16px; flex: 1; display: flex; flex-direction: column; gap: 8px; }
    .p-marca { font-size: 10px; letter-spacing: 0.24em; text-transform: uppercase; color: var(--ouro); }
    .p-nome { font-family: 'Cormorant Garamond', serif; font-size: 20px; font-weight: 500; line-height: 1.2; }
    .p-desc { font-size: 12px; color: var(--mut); line-height: 1.7; }
    .est-row {
      display: flex; align-items: center; justify-content: space-between;
      padding: 8px 0;
      border-top: 1px solid rgba(201,168,76,0.1);
      border-bottom: 1px solid rgba(201,168,76,0.1);
    }
    .est-badge { font-size: 10px; font-weight: 600; letter-spacing: 0.14em; text-transform: uppercase; padding: 3px 9px; border-radius: 999px; }
    .b-ok  { background: rgba(76,175,80,0.12); color: #6fcf6f; border: 1px solid rgba(76,175,80,0.3); }
    .b-low { background: rgba(255,152,0,0.12); color: #ffb74d; border: 1px solid rgba(255,152,0,0.3); }
    .b-out { background: rgba(244,67,54,0.12); color: #e57373; border: 1px solid rgba(244,67,54,0.3); }
    .est-un { font-size: 11px; color: var(--mut); }
    .qty-row { display: flex; align-items: center; gap: 8px; }
    .qty-label { font-size: 11px; color: var(--mut); margin-right: auto; }
    .qty-btn {
      width: 26px; height: 26px; border-radius: 50%;
      border: 1px solid rgba(201,168,76,0.3); background: transparent;
      color: var(--ouro); font-size: 16px; cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      transition: all 0.15s; line-height: 1;
    }
    .qty-btn:hover { background: var(--ouro); color: var(--marrom-esc); }
    .qty-input {
      width: 38px; text-align: center;
      background: rgba(255,255,255,0.05); border: 1px solid var(--borda);
      border-radius: 6px; padding: 4px; font-size: 13px; color: var(--creme);
      font-family: 'Montserrat', sans-serif;
    }
    .preco-row { display: flex; align-items: baseline; justify-content: space-between; }
    .preco { font-family: 'Cormorant Garamond', serif; font-size: 26px; font-weight: 600; color: var(--ouro); }
    .preco-tag { font-size: 10px; color: var(--mut); border: 1px solid var(--borda); padding: 2px 8px; border-radius: 999px; }
    .tamanhos { display: flex; gap: 8px; flex-wrap: wrap; }
    .tam-chip { font-size: 10px; letter-spacing: 0.1em; padding: 3px 10px; border-radius: 999px; border: 1px solid rgba(201,168,76,0.2); color: var(--mut); }
    .p-cta {
      display: block; text-align: center;
      font-size: 11px; font-weight: 700; letter-spacing: 0.24em; text-transform: uppercase;
      padding: 12px 16px; border-radius: 999px;
      background: linear-gradient(135deg, var(--ouro), var(--ouro-cl));
      color: var(--marrom-esc); margin-top: 4px; transition: filter 0.15s, transform 0.15s;
    }
    .p-cta:hover { filter: brightness(1.08); transform: translateY(-2px); }
    .sem-resultado { display: none; grid-column: 1/-1; text-align: center; padding: 40px; font-size: 14px; color: var(--mut); }

    /* PAGAMENTO */
    #pagamento { background: var(--marrom); }
    .pag-grid { display: grid; grid-template-columns: repeat(4, minmax(0,1fr)); gap: 14px; }
    .pag-card {
      background: var(--card); border: 1px solid var(--borda);
      border-radius: var(--radius); padding: 22px 16px;
      text-align: center; transition: transform 0.2s, border-color 0.2s;
    }
    .pag-card:hover { transform: translateY(-4px); border-color: rgba(201,168,76,0.5); }
    .pag-destaque { background: linear-gradient(135deg, var(--ouro), var(--ouro-cl)); border-color: transparent; }
    .pag-destaque .pag-nome { color: var(--marrom-esc); }
    .pag-destaque .pag-desc { color: var(--marrom-med); }
    .pag-ico { font-size: 26px; margin-bottom: 10px; }
    .pag-nome { font-family: 'Cormorant Garamond', serif; font-size: 18px; font-weight: 500; color: var(--creme); margin-bottom: 4px; }
    .pag-desc { font-size: 12px; color: var(--mut); line-height: 1.6; }

    /* COMO COMPRAR */
    #como-comprar { background: rgba(0,0,0,0.12); }
    .passos { display: grid; grid-template-columns: repeat(3, minmax(0,1fr)); gap: 18px; }
    .passo {
      background: var(--card); border: 1px solid var(--borda);
      border-radius: var(--radius); padding: 28px 20px;
      position: relative; transition: transform 0.2s;
    }
    .passo:hover { transform: translateY(-4px); }
    .passo-num {
      font-family: 'Cormorant Garamond', serif; font-size: 50px;
      font-weight: 300; color: rgba(201,168,76,0.12);
      position: absolute; top: 14px; right: 18px; line-height: 1;
    }
    .passo-ico { font-size: 24px; margin-bottom: 12px; }
    .passo-tit { font-family: 'Cormorant Garamond', serif; font-size: 20px; font-weight: 500; color: var(--creme); margin-bottom: 6px; }
    .passo-txt { font-size: 12px; color: var(--mut); line-height: 1.8; }

    /* DEPOIMENTOS */
    #depoimentos { background: var(--marrom-esc); }
    .dep-grid { display: grid; grid-template-columns: repeat(3, minmax(0,1fr)); gap: 18px; }
    .dep { background: var(--card); border: 1px solid var(--borda); border-radius: var(--radius); padding: 22px; }
    .dep-stars { color: var(--ouro); font-size: 13px; margin-bottom: 10px; }
    .dep-txt { font-size: 13px; color: var(--mut); line-height: 1.8; font-style: italic; margin-bottom: 14px; }
    .dep-autor { display: flex; align-items: center; gap: 10px; }
    .dep-avatar {
      width: 34px; height: 34px; border-radius: 50%;
      background: linear-gradient(135deg, var(--ouro), var(--marrom));
      display: flex; align-items: center; justify-content: center;
      font-size: 13px; font-weight: 700; color: var(--marrom-esc); flex-shrink: 0;
    }
    .dep-nome { font-size: 13px; font-weight: 600; color: var(--creme); }
    .dep-label { font-size: 11px; color: var(--mut); }

    /* CONTATO */
    #contato { background: var(--marrom); }
    .cta-box {
      background: linear-gradient(135deg, rgba(201,168,76,0.1), rgba(201,168,76,0.03));
      border: 1px solid var(--borda); border-radius: 22px;
      padding: 52px 44px; display: flex;
      align-items: center; justify-content: space-between;
      gap: 28px; flex-wrap: wrap;
    }
    .cta-tit { font-family: 'Cormorant Garamond', serif; font-size: 34px; font-weight: 400; color: var(--creme); margin-bottom: 8px; line-height: 1.2; }
    .cta-desc { font-size: 14px; color: var(--mut); line-height: 1.8; max-width: 500px; }
    .cta-acoes { display: flex; gap: 12px; flex-wrap: wrap; }

    /* FOOTER */
    footer { background: var(--marrom-esc); border-top: 1px solid rgba(201,168,76,0.12); padding: 26px 0; }
    .footer-inner { display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap; gap: 12px; }
    .footer-logo { font-family: 'Cormorant Garamond', serif; font-size: 18px; font-weight: 600; letter-spacing: 0.08em; }
    .footer-logo span { color: var(--ouro); }
    .footer-links { display: flex; gap: 28px; list-style: none; }
    .footer-links a { font-size: 11px; letter-spacing: 0.2em; text-transform: uppercase; color: var(--mut); transition: color 0.2s; }
    .footer-links a:hover { color: var(--ouro); }
    .footer-copy { font-size: 11px; color: var(--mut); }

    /* RESPONSIVO */
    @media (max-width: 1024px) {
      .hero-inner { grid-template-columns: 1fr; text-align: center; gap: 40px; }
      .hero-label { justify-content: center; }
      .hero-btns { justify-content: center; }
      .hero-selos { justify-content: center; }
      .sobre-grid { grid-template-columns: 1fr; }
    }
    @media (max-width: 768px) {
      .nav-links { display: none; }
      .menu-btn { 
