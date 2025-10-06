<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Valeria Vega Lora – Traductrice & Interprète</title>
<style>
  /* ========= Variables de couleur ========= */
  :root{
    --sidebar-w: 270px;
    --bg: #0b1226;
    --bg-2: #0e1a3a;
    --text: #e5e7eb;
    --muted:#93a4c0;
    --card:#0f1c3b;
    --border:#1f2a51;
    --shadow: 0 18px 50px rgba(0,0,0,.35);

    /* Accents (usaremos varios para “más colores”) */
    --c1:#60a5fa; /* bleu */
    --c2:#22c55e; /* vert */
    --c3:#f59e0b; /* jaune */
    --c4:#a78bfa; /* violet */
    --c5:#f472b6; /* rose */
    --c6:#38bdf8; /* cyan */
  }

  html{scroll-behavior:smooth}
  body{
    margin:0; font:16px/1.65 Inter, system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    color:var(--text);
    background:
      radial-gradient(1200px 700px at 10% 10%, #18224a 0%, #0b1226 60%),
      radial-gradient(1000px 700px at 90% 20%, #1b2b60 0%, #0b1226 60%),
      linear-gradient(180deg, var(--bg-2), var(--bg));
  }

  /* ========= Sidebar ========= */
  .sidenav{
    position:fixed; inset:0 auto 0 0; width:var(--sidebar-w);
    background:
      radial-gradient(800px 500px at 30% -20%, #1b2b60 0%, transparent 60%),
      linear-gradient(180deg, #121c3a 0%, #0c1430 100%);
    border-right:1px solid #1a2550;
    box-shadow:var(--shadow);
    display:flex; flex-direction:column; gap:18px; padding:22px 18px;
    z-index:1000;
  }
  .brand{
    display:flex; align-items:center; gap:10px;
    font-weight:800; letter-spacing:.2px; font-size:18px;
  }
  .brand .dot{
    width:14px; height:14px; border-radius:999px;
    background: conic-gradient(from 0deg, var(--c1), var(--c2), var(--c3), var(--c4), var(--c5), var(--c6), var(--c1));
    box-shadow:0 0 12px #60a5fa66;
  }
  nav a{
    display:flex; align-items:center; gap:10px;
    padding:10px 12px; border-radius:10px; text-decoration:none; color:var(--text);
    border:1px solid transparent; transition:.2s ease;
    font-weight:600;
  }
  nav a:hover{ background:#0e1a3f; border-color:#243163; }
  nav a.active{
    background: linear-gradient(90deg, #0e1a45, #0f2256);
    border-color:#2e3b75;
    box-shadow:0 8px 18px rgba(0,0,0,.25) inset;
  }
  .legend{
    display:grid; grid-template-columns: repeat(6, 1fr); gap:8px; margin-top:4px;
  }
  .legend span{
    height:6px; border-radius:999px;
  }
  .l1{background:var(--c1)} .l2{background:var(--c2)} .l3{background:var(--c3)}
  .l4{background:var(--c4)} .l5{background:var(--c5)} .l6{background:var(--c6)}

  /* Toggle móvil */
  .menu-toggle{
    position:fixed; top:14px; left:14px; z-index:1100;
    display:none; background:#0f1c3b; border:1px solid #22306a; color:var(--text);
    border-radius:12px; padding:10px 12px; font-weight:800;
  }

  /* ========= Contenido ========= */
  .content{
    margin-left:var(--sidebar-w);
    padding:34px 26px 60px;
    max-width:1100px;
  }
  .section{
    background:linear-gradient(180deg, #0c1633, #0b1631);
    border:1px solid var(--border); border-radius:18px; box-shadow:var(--shadow);
    padding:26px; margin:26px 0 34px;
    scroll-margin-top: 18px;
  }
  .section header h2{ margin:0 0 8px 0; font-size:26px; }
  .sub{ color:var(--muted); margin-top:0; }

  /* Cabeceras con líneas de color */
  .bar{
    height:6px; border-radius:999px; margin:0 0 16px 0; background:#20316b;
  }
  .bar.c1{background:linear-gradient(90deg, var(--c1), transparent)}
  .bar.c2{background:linear-gradient(90deg, var(--c2), transparent)}
  .bar.c3{background:linear-gradient(90deg, var(--c3), transparent)}
  .bar.c4{background:linear-gradient(90deg, var(--c4), transparent)}
  .bar.c5{background:linear-gradient(90deg, var(--c5), transparent)}
  .bar.c6{background:linear-gradient(90deg, var(--c6), transparent)}

  .grid{ display:grid; gap:18px; }
  .cols-2{ grid-template-columns: 1fr 1fr; }
  @media (max-width: 960px){ .content{ margin-left:0; padding-top:70px } }

  /* Badges / KPIs */
  .badges{ display:flex; gap:10px; flex-wrap:wrap }
  .badge{ font-size:12px; padding:6px 10px; border-radius:999px; border:1px solid #27407a; background:#0f1d43 }
  .kpis{ display:grid; gap:14px; grid-template-columns: repeat(3,1fr); }
  .kpi{ text-align:center; padding:16px; border:1px solid #233a73; border-radius:14px; background:#0f1d43 }
  .kpi b{ display:block; font-size:22px; }

  /* Listas */
  ul{ margin:0; padding-left:18px }
  li{ margin:6px 0 }
  .check li::marker{ content: "✔ "; color: var(--c2) }

  /* CTA */
  .cta{ display:flex; gap:12px; flex-wrap:wrap; margin-top:6px }
  .btn{
    display:inline-block; text-decoration:none; font-weight:700; color:var(--text);
    border:1px solid #2a3e7c; padding:12px 16px; border-radius:12px; background:#0f1d43;
  }
  .btn.primary{ border-color:#3c5fd3; background:linear-gradient(180deg, #1d2f6f, #122457); }
  .btn:hover{ transform: translateY(-1px) }

  /* Avatar */
  .avatar{
    width:220px; height:220px; border-radius:999px; border:6px solid #0b1226; box-shadow:var(--shadow);
    background:#162a5c url('https://images.unsplash.com/photo-1544005313-94ddf0286df2?w=600&q=80') center/cover no-repeat; /* Reemplaza por tu foto */
    margin:auto;
  }

  /* Footer */
  footer{ color:var(--muted); text-align:center; padding:30px 0 60px; }

  /* Responsividad: menú lateral colapsable */
  @media (max-width: 960px){
    .sidenav{ transform: translateX(-100%); transition: .25s ease; }
    body.menu-open .sidenav{ transform: translateX(0); }
    .menu-toggle{ display:block }
  }
</style>
</head>
<body>

<button class="menu-toggle" aria-label="Ouvrir le menu" onclick="document.body.classList.toggle('menu-open')">☰ Menu</button>

<aside class="sidenav" aria-label="Navigation latérale">
  <div class="brand"><span class="dot"></span> Valeria Vega Lora</div>
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
  <div class="legend">
    <span class="l1"></span><span class="l2"></span><span class="l3"></span>
    <span class="l4"></span><span class="l5"></span><span class="l6"></span>
  </div>
</aside>

<main class="content">
  <!-- ACCUEIL -->
  <section id="accueil" class="section">
    <div class="bar c1"></div>
    <header>
      <h2>Bienvenue</h2>
      <p class="sub">Traductrice & future interprète — Espagnol · Français · Anglais</p>
    </header>
    <div class="grid cols-2">
      <div>
        <p>Bonjour, je m’appelle <strong>Valeria Vega Lora</strong>. Je suis licenciée en langues étrangères de l’Université de l’Atlantique (Colombie) et actuellement étudiante en <strong>Master 1 Traduction & Interprétation</strong> à l’Université de Bretagne Occidentale (France).</p>
        <p>Je transforme des textes et des messages en passerelles claires et naturelles entre cultures. Mon objectif : une communication sans friction, fidèle au sens et adaptée au lectorat.</p>
        <div class="badges">
          <span class="badge">Qualité & précision</span>
          <span class="badge">Délais fiables</span>
          <span class="badge">Confidentialité</span>
        </div>
        <div class="cta">
          <a class="btn primary" href="#contact">Demander un devis</a>
          <a class="btn" href="#domaines">Voir mes domaines</a>
        </div>
      </div>
      <div>
        <div class="avatar" aria-label="Photo de profil"></div>
        <p class="sub" style="text-align:center; margin-top:10px;">(Remplace l’image par ta photo ou retire ce bloc)</p>
      </div>
    </div>

    <div class="kpis" style="margin-top:18px">
      <div class="kpi"><b>3</b> langues de travail</div>
      <div class="kpi"><b>ES · FR · EN</b> combinaisons</div>
      <div class="kpi"><b>Académique</b> + pratique</div>
    </div>
  </section>

  <!-- PROFIL -->
  <section id="profil" class="section">
    <div class="bar c2"></div>
    <header><h2>Profil</h2></header>
    <p>Traductrice et future interprète, je travaille avec trois langues principales : <strong>espagnol</strong>, <strong>français</strong> et <strong>anglais</strong>. Mon approche est centrée sur la rigueur terminologique, la cohérence stylistique et l’adaptation culturelle afin d’assurer des textes fluides, crédibles et efficaces.</p>
  </section>

  <!-- COMPÉTENCES -->
  <section id="competences" class="section">
    <div class="bar c3"></div>
    <header><h2>Compétences</h2></header>
    <div class="grid cols-2">
      <div>
        <ul class="check">
          <li>Traduction ES ⇄ FR ⇄ EN (général & spécialisé).</li>
          <li>Révision, correction et adaptation stylistique.</li>
          <li>Pré-traitement & post-édition (outils TAO).</li>
          <li>Recherche terminologique & mémoires de traduction.</li>
        </ul>
      </div>
      <div>
        <ul class="check">
          <li>Gestion de glossaires multilingues.</li>
          <li>Communication interculturelle et localisation.</li>
          <li>Respect du brief, des délais et de la confidentialité.</li>
          <li>Coordination avec équipes éditoriales et techniques.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- DOMAINES -->
  <section id="domaines" class="section">
    <div class="bar c4"></div>
    <header><h2>Domaines de spécialité</h2></header>
    <div class="grid cols-2">
      <div>
        <ul class="check">
          <li>Académique & éducation</li>
          <li>Affaires & communication institutionnelle</li>
          <li>Culture, tourisme & patrimoine</li>
        </ul>
      </div>
      <div>
        <ul class="check">
          <li>Marketing & réseaux sociaux</li>
          <li>Humanités & sciences sociales</li>
          <li>Traduction générale de qualité</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- MÉTHODE -->
  <section id="methode" class="section">
    <div class="bar c5"></div>
    <header><h2>Méthode de travail</h2></header>
    <ol>
      <li><strong>Analyse du besoin</strong> : public, registre, objectif, supports.</li>
      <li><strong>Recherche & terminologie</strong> : références fiables et glossaires.</li>
      <li><strong>Traduction & cohérence</strong> : style adapté, vérifications croisées.</li>
      <li><strong>Révision finale</strong> : correction, mise en page, préparation livrable.</li>
    </ol>
  </section>

  <!-- IMPORTANCE -->
  <section id="importance" class="section">
    <div class="bar c6"></div>
    <header><h2>Importance de la traduction</h2></header>
    <p>La traduction est un levier stratégique : elle rend l’information accessible, fait circuler les idées et renforce la confiance entre acteurs d’horizons différents. Au-delà des mots, elle transmet des références culturelles et des nuances indispensables pour être compris sans ambiguïté.</p>
    <p>Une traduction professionnelle garantit pertinence, naturel et impact—conditions essentielles pour éduquer, convaincre, vendre ou coopérer à l’international.</p>
  </section>

  <!-- FORMATION -->
  <section id="formation" class="section">
    <div class="bar c1"></div>
    <header><h2>Formation académique</h2></header>
    <ul>
      <li><strong>Licence en Langues Étrangères</strong> — Université de l’Atlantique, Colombie.</li>
      <li><strong>Master 1 Traduction & Interprétation</strong> — Université de Bretagne Occidentale, France.</li>
    </ul>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="section">
    <div class="bar c2"></div>
    <header><h2>Contact</h2></header>
    <p>📧 Email : <a class="btn" href="mailto:valeriavega5.vv@gmail.com">valeriavega5.vv@gmail.com</a></p>
    <p>🔗 LinkedIn : <a class="btn" target="_blank" href="https://www.linkedin.com/in/valeria-vega-lora-">www.linkedin.com/in/valeria-vega-lora-</a></p>
  </section>

  <footer>
    © 2025 Valeria Vega Lora — Tous droits réservés
  </footer>
</main>

<script>
  // Resalte del item activo en el menú lateral
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
  }, { rootMargin: '-50% 0px -40% 0px', threshold: 0.01 });

  document.querySelectorAll('main .section[id]').forEach(s=>io.observe(s));

  // Cerrar el menú al seleccionar en móvil
  links.forEach(a=>a.addEventListener('click', ()=>document.body.classList.remove('menu-open')));
</script>

</body>
</html>
