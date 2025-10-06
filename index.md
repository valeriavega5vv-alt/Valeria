<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Valeria Vega Lora – Traductrice & Interprète</title>
<style>
  /* ========= Paletas ========= */
  :root {
    --sidebar-w: 270px;

    /* Paleta clara */
    --bg: #f9fafb;
    --card: #ffffff;
    --text: #1f2937;
    --muted: #6b7280;
    --border: #e5e7eb;
    --accent: #3b82f6;
  }

  body.dark {
    --bg: #0b1226;
    --card: #0f1c3b;
    --text: #e5e7eb;
    --muted: #93a4c0;
    --border: #1f2a51;
    --accent: #60a5fa;
  }

  html { scroll-behavior: smooth; }
  body {
    margin:0;
    font:16px/1.65 Inter, system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    background: var(--bg);
    color: var(--text);
  }

  /* Sidebar */
  .sidenav {
    position:fixed; inset:0 auto 0 0; width:var(--sidebar-w);
    background: var(--card);
    border-right:1px solid var(--border);
    display:flex; flex-direction:column; gap:18px; padding:22px 18px;
    z-index:1000;
  }
  .brand { font-weight:800; font-size:18px; color:var(--accent); margin-bottom:6px; }
  nav a {
    display:block;
    padding:10px 12px;
    border-radius:8px;
    text-decoration:none;
    color:var(--text);
    font-weight:600;
  }
  nav a:hover { background: rgba(59,130,246,.08); }
  nav a.active { background: rgba(59,130,246,.15); color:var(--accent); }

  /* Botón de modo */
  .toggle-mode {
    margin-top:auto;
    padding:10px 12px;
    border-radius:8px;
    text-align:center;
    cursor:pointer;
    border:1px solid var(--border);
    background:var(--bg);
    color:var(--text);
    font-weight:600;
  }
  .toggle-mode:hover { background: rgba(59,130,246,.08); }

  /* Contenido */
  .content {
    margin-left:var(--sidebar-w);
    padding:34px 26px 60px;
    max-width:1100px;
  }
  .section {
    background:var(--card);
    border:1px solid var(--border);
    border-radius:16px;
    padding:26px;
    margin:26px 0 34px;
    scroll-margin-top: 18px;
    box-shadow:0 6px 18px rgba(0,0,0,.06);
  }
  .section header h2 { margin:0 0 8px 0; font-size:26px; color:var(--accent); }
  .sub { color:var(--muted); margin-top:0; }

  ul { margin:0; padding-left:18px }
  li { margin:6px 0 }
  .check li::marker { content: "✔ "; color: var(--accent); }

  footer {
    color:var(--muted);
    text-align:center;
    padding:30px 0 60px;
  }

  /* Responsivo */
  @media (max-width: 960px){
    .sidenav{ transform: translateX(-100%); transition:.25s ease; }
    body.menu-open .sidenav{ transform: translateX(0); }
    .menu-toggle{ display:block }
    .content{ margin-left:0; padding-top:70px }
  }
  .menu-toggle{
    position:fixed; top:14px; left:14px; z-index:1100;
    display:none; background:var(--card); border:1px solid var(--border); color:var(--text);
    border-radius:10px; padding:10px 12px; font-weight:800;
  }
</style>
</head>
<body>

<button class="menu-toggle" onclick="document.body.classList.toggle('menu-open')">☰ Menu</button>

<aside class="sidenav">
  <div class="brand">Valeria Vega Lora</div>
  <nav>
    <a href="#accueil">Accueil</a>
    <a href="#profil">Profil</a>
    <a href="#competences">Compétences</a>
    <a href="#domaines">Domaines</a>
    <a href="#methode">Méthode</a>
    <a href="#importance">Importance</a>
    <a href="#formation">Formation</a>
    <a href="#contact">Contact</a>
  </nav>
  <div class="toggle-mode" onclick="document.body.classList.toggle('dark')">🌗 Mode clair / sombre</div>
</aside>

<main class="content">
  <section id="accueil" class="section">
    <header>
      <h2>Bienvenue</h2>
      <p class="sub">Traductrice & future interprète — Espagnol · Français · Anglais</p>
    </header>
    <p>Bonjour, je m’appelle <strong>Valeria Vega Lora</strong>. Je suis licenciée en langues étrangères de l’Université de l’Atlantique (Colombie) et actuellement étudiante en <strong>Master 1 Traduction & Interprétation</strong> à l’Université de Bretagne Occidentale (France).</p>
    <p>Je transforme des textes et des messages en passerelles claires et naturelles entre cultures. Mon objectif : une communication sans friction, fidèle au sens et adaptée au lectorat.</p>
  </section>

  <section id="profil" class="section">
    <header><h2>Profil</h2></header>
    <p>Traductrice et future interprète, je travaille avec trois langues principales : <strong>espagnol</strong>, <strong>français</strong> et <strong>anglais</strong>. Mon approche est centrée sur la rigueur terminologique, la cohérence stylistique et l’adaptation culturelle afin d’assurer des textes fluides, crédibles et efficaces.</p>
  </section>

  <section id="competences" class="section">
    <header><h2>Compétences</h2></header>
    <ul class="check">
      <li>Traduction ES ⇄ FR ⇄ EN (général & spécialisé).</li>
      <li>Révision, correction et adaptation stylistique.</li>
      <li>Pré-traitement & post-édition (outils TAO).</li>
      <li>Recherche terminologique & mémoires de traduction.</li>
      <li>Communication interculturelle et localisation.</li>
      <li>Respect des délais & confidentialité.</li>
    </ul>
  </section>

  <section id="domaines" class="section">
    <header><h2>Domaines de spécialité</h2></header>
    <ul class="check">
      <li>Académique & éducation</li>
      <li>Affaires & communication institutionnelle</li>
      <li>Culture, tourisme & patrimoine</li>
      <li>Marketing & réseaux sociaux</li>
      <li>Humanités & sciences sociales</li>
    </ul>
  </section>

  <section id="methode" class="section">
    <header><h2>Méthode de travail</h2></header>
    <ol>
      <li><strong>Analyse du besoin</strong> : public, registre, objectif, supports.</li>
      <li><strong>Recherche & terminologie</strong> : références fiables et glossaires.</li>
      <li><strong>Traduction & cohérence</strong> : style adapté, vérifications croisées.</li>
      <li><strong>Révision finale</strong> : correction, mise en page, préparation livrable.</li>
    </ol>
  </section>

  <section id="importance" class="section">
    <header><h2>Importance de la traduction</h2></header>
    <p>La traduction est un levier stratégique : elle rend l’information accessible, fait circuler les idées et renforce la confiance entre acteurs d’horizons différents. Au-delà des mots, elle transmet des références culturelles et des nuances indispensables pour être compris sans ambiguïté.</p>
    <p>Une traduction professionnelle garantit pertinence, naturel et impact — conditions essentielles pour éduquer, convaincre, vendre ou coopérer à l’international.</p>
  </section>

  <section id="formation" class="section">
    <header><h2>Formation académique</h2></header>
    <ul>
      <li><strong>Licence en Langues Étrangères</strong> — Université de l’Atlantique, Colombie.</li>
      <li><strong>Master 1 Traduction & Interprétation</strong> — Université de Bretagne Occidentale, France.</li>
    </ul>
  </section>

  <section id="contact" class="section">
    <header><h2>Contact</h2></header>
    <p>📧 Email : <a href="mailto:valeriavega5.vv@gmail.com">valeriavega5.vv@gmail.com</a></p>
    <p>🔗 LinkedIn : <a target="_blank" href="https://www.linkedin.com/in/valeria-vega-lora-">www.linkedin.com/in/valeria-vega-lora-</a></p>
  </section>

  <footer>
    © 2025 Valeria Vega Lora — Tous droits réservés
  </footer>
</main>

<script>
  // Resalta la sección activa
  const links = [...document.querySelectorAll('.sidenav nav a')];
  const map = new Map(links.map(a => [a.getAttribute('href'), a]));
  const io = new IntersectionObserver((entries)=>{
    entries.forEach(e=>{
      if(e.isIntersecting){
        const id = '#'+e.target.id;
        links.forEach(a=>a.classList.remove('active'));
        const l = map.get(id); if(l) l.classList.add('active');
      }
    });
  }, { rootMargin: '-50% 0px -40% 0px' });
  document.querySelectorAll('main .section[id]').forEach(s=>io.observe(s));
  links.forEach(a=>a.addEventListener('click', ()=>document.body.classList.remove('menu-open')));
</script>

</body>
</html>
