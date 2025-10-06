<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Valeria Vega Lora – Traductrice & Interprète</title>
<style>
  :root{
    --sidebar-w: 250px;
    --bg: #f9fafb;     /* gris très clair */
    --text: #1f2937;   /* gris foncé */
    --muted:#6b7280;   /* gris moyen */
    --card:#ffffff;
    --border:#e5e7eb;
    --shadow: 0 6px 18px rgba(0,0,0,.08);

    /* Palette sobre */
    --c1:#3b82f6; /* bleu moyen */
    --c2:#2563eb; /* bleu foncé */
    --c3:#1e40af; /* bleu marine */
  }

  html{scroll-behavior:smooth}
  body{
    margin:0; font:16px/1.65 "Segoe UI", Roboto, sans-serif;
    background: var(--bg); color: var(--text);
  }

  /* Sidebar */
  .sidenav{
    position:fixed; inset:0 auto 0 0; width:var(--sidebar-w);
    background:#ffffff;
    border-right:1px solid var(--border);
    box-shadow:var(--shadow);
    display:flex; flex-direction:column; gap:14px; padding:22px 18px;
    z-index:1000;
  }
  .brand{ font-weight:700; font-size:18px; color:var(--c2); margin-bottom:8px; }
  nav a{
    display:block;
    padding:10px 12px; border-radius:8px;
    text-decoration:none; color:var(--text);
    font-weight:500;
  }
  nav a:hover{ background:#f3f4f6; }
  nav a.active{ background:#e0e7ff; color:var(--c2); }

  /* Toggle móvil */
  .menu-toggle{
    position:fixed; top:14px; left:14px; z-index:1100;
    display:none; background:#ffffff; border:1px solid var(--border); color:var(--text);
    border-radius:8px; padding:10px 12px; font-weight:700;
  }

  /* Contenido */
  .content{
    margin-left:var(--sidebar-w);
    padding:32px 26px 60px;
    max-width:960px;
  }
  .section{
    background:var(--card);
    border:1px solid var(--border); border-radius:12px; box-shadow:var(--shadow);
    padding:24px; margin:26px 0;
    scroll-margin-top: 18px;
  }
  h2{ margin-top:0; color:var(--c2); }
  .sub{ color:var(--muted); margin-top:0; }

  /* Listas */
  ul{ padding-left:20px; margin:0 }
  li{ margin:6px 0 }
  .check li::marker{ content:"✔ "; color:var(--c2) }

  /* Botones */
  .btn{
    display:inline-block; text-decoration:none; font-weight:600; color:var(--c2);
    border:1px solid var(--c2); padding:10px 14px; border-radius:8px;
  }
  .btn.primary{ background:var(--c2); color:#fff; }
  .btn.primary:hover{ background:var(--c3); }

  footer{ color:var(--muted); text-align:center; padding:30px 0 60px; }

  @media (max-width: 900px){
    .sidenav{ transform: translateX(-100%); transition:.25s; }
    body.menu-open .sidenav{ transform: translateX(0); }
    .menu-toggle{ display:block }
    .content{ margin-left:0; padding-top:70px }
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
</aside>

<main class="content">
  <section id="accueil" class="section">
    <h2>Bienvenue</h2>
    <p class="sub">Traductrice & future interprète — Espagnol · Français · Anglais</p>
    <p>Bonjour, je m’appelle <strong>Valeria Vega Lora</strong>. Je suis licenciée en langues étrangères de l’Université de l’Atlantique (Colombie) et actuellement étudiante en <strong>Master 1 Traduction & Interprétation</strong> à l’Université de Bretagne Occidentale (France).</p>
  </section>

  <section id="profil" class="section">
    <h2>Profil</h2>
    <p>Traductrice et future interprète, je travaille avec trois langues principales : espagnol, français et anglais. Mon approche repose sur la rigueur, la clarté et l’adaptation culturelle. Mon objectif est d’offrir des textes fluides, crédibles et adaptés à chaque contexte.</p>
  </section>

  <section id="competences" class="section">
    <h2>Compétences</h2>
    <ul class="check">
      <li>Traduction ES ⇄ FR ⇄ EN (général & spécialisé)</li>
      <li>Révision, correction et adaptation stylistique</li>
      <li>Localisation et communication interculturelle</li>
      <li>Recherche terminologique et gestion de glossaires</li>
    </ul>
  </section>

  <section id="domaines" class="section">
    <h2>Domaines de spécialité</h2>
    <ul class="check">
      <li>Académique et éducation</li>
      <li>Affaires et communication institutionnelle</li>
      <li>Culture, tourisme et patrimoine</li>
      <li>Marketing et réseaux sociaux</li>
    </ul>
  </section>

  <section id="methode" class="section">
    <h2>Méthode de travail</h2>
    <ol>
      <li>Analyse du besoin et du public cible</li>
      <li>Recherche terminologique rigoureuse</li>
      <li>Traduction fidèle et adaptée</li>
      <li>Révision finale et livraison ponctuelle</li>
    </ol>
  </section>

  <section id="importance" class="section">
    <h2>Importance de la traduction</h2>
    <p>La traduction est une passerelle indispensable entre cultures et sociétés. Elle rend l’information accessible, facilite la circulation des idées et renforce la coopération internationale. Une traduction professionnelle garantit non seulement la précision linguistique, mais aussi l’efficacité de la communication.</p>
  </section>

  <section id="formation" class="section">
    <h2>Formation académique</h2>
    <ul>
      <li><strong>Licence en Langues Étrangères</strong> — Université de l’Atlantique, Colombie</li>
      <li><strong>Master 1 Traduction & Interprétation</strong> — Université de Bretagne Occidentale, France</li>
    </ul>
  </section>

  <section id="contact" class="section">
    <h2>Contact</h2>
    <p>📧 Email : <a class="btn primary" href="mailto:valeriavega5.vv@gmail.com">valeriavega5.vv@gmail.com</a></p>
    <p>🔗 LinkedIn : <a class="btn" target="_blank" href="https://www.linkedin.com/in/valeria-vega-lora-">www.linkedin.com/in/valeria-vega-lora-</a></p>
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
        links.forEach(a=>a.classList.remove('active'));
        const l = map.get('#'+e.target.id);
        if(l) l.classList.add('active');
      }
    });
  }, {rootMargin:'-50% 0px -40% 0px'});
  document.querySelectorAll('.section[id]').forEach(s=>io.observe(s));
  links.forEach(a=>a.addEventListener('click', ()=>document.body.classList.remove('menu-open')));
</script>

</body>
</html>
