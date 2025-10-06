<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Valeria Vega Lora – Traductrice & Interprète</title>
  <style>
    :root {
      --header-h: 70px;
      --accent: #1d4ed8; /* bleu professionnel */
      --bg: #f9fafb;
      --text: #111827;
    }
    html { scroll-behavior: smooth; }
    body {
      margin:0; font:17px/1.6 "Segoe UI", Roboto, sans-serif;
      background: var(--bg); color: var(--text);
    }
    header.site-nav {
      position: sticky; top: 0; z-index: 999;
      background: #fff; border-bottom: 1px solid #e5e7eb;
      height: var(--header-h); display:flex; align-items:center;
      box-shadow: 0 2px 6px rgba(0,0,0,.05);
    }
    nav { display:flex; gap:24px; margin:0 auto; max-width: 1100px; width:100%; padding:0 16px; }
    nav a {
      text-decoration:none; color:var(--text);
      padding:10px 12px; border-radius:8px; font-weight:500;
      transition: background .2s;
    }
    nav a:hover { background:#f1f5f9; }
    nav a.active { background:#eff6ff; color:var(--accent); }

    main { max-width: 900px; margin:0 auto; padding:32px 16px; }
    section { padding:64px 0; border-bottom:1px solid #e5e7eb; }
    section:last-child { border-bottom:none; }
    section { scroll-margin-top: calc(var(--header-h) + 12px); }

    h1,h2 { margin-top:0; font-weight:700; color:#0f172a; }
    h1 { font-size:2rem; margin-bottom:12px; }
    h2 { font-size:1.5rem; margin-bottom:10px; color:var(--accent); }

    p { margin:12px 0; }

    ul { padding-left:20px; }
    li { margin:6px 0; }

    footer {
      text-align:center; font-size:14px; color:#6b7280;
      margin-top:60px; padding:20px 0; border-top:1px solid #e5e7eb;
    }

    .to-top{
      position: fixed; right: 16px; bottom: 16px;
      border: 1px solid #e5e7eb; background:#fff;
      border-radius:999px; padding:10px 12px;
      text-decoration:none; color:#0f172a; font-weight:600;
      box-shadow:0 2px 6px rgba(0,0,0,.1);
    }
  </style>
</head>
<body>

<header class="site-nav">
  <nav>
    <a href="#accueil">Accueil</a>
    <a href="#profil">Profil</a>
    <a href="#formation">Formation</a>
    <a href="#importance">Importance</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<main>
  <!-- Section accueil -->
  <section id="accueil">
    <h1>Bienvenue</h1>
    <p>Bonjour, je m’appelle <strong>Valeria Vega Lora</strong>. Je suis licenciée en langues étrangères de l’Université de l’Atlantique en Colombie et actuellement étudiante en Master 1 de Traduction et Interprétation à l’Université de Bretagne Occidentale.</p>
  </section>

  <!-- Section profil -->
  <section id="profil">
    <h2>Profil</h2>
    <p>Traductrice et future interprète, je travaille avec trois langues principales : <strong>espagnol, français et anglais</strong>. Mon objectif est de faciliter la communication interculturelle avec précision et professionnalisme.</p>
  </section>

  <!-- Section formation -->
  <section id="formation">
    <h2>Formation académique</h2>
    <ul>
      <li><strong>Licence en Langues Étrangères</strong> – Université de l’Atlantique, Colombie</li>
      <li><strong>Master 1 Traduction et Interprétation</strong> – Université de Bretagne Occidentale, France</li>
    </ul>
  </section>

  <!-- Section importance -->
  <section id="importance">
    <h2>Importance de la traduction</h2>
    <p>La traduction joue un rôle essentiel dans un monde de plus en plus globalisé. Elle permet aux individus, aux entreprises et aux institutions de communiquer efficacement au-delà des frontières linguistiques et culturelles. Grâce à la traduction, les idées circulent librement, les connaissances deviennent accessibles et les relations internationales se renforcent.</p>
    <p>Au-delà des mots, traduire signifie transmettre une culture, un contexte et une vision du monde. C’est un pont indispensable pour favoriser la compréhension mutuelle et encourager la coopération entre les peuples.</p>
  </section>

  <!-- Section contact -->
  <section id="contact">
    <h2>Contact</h2>
    <p>📧 Email : <a href="mailto:valeriavega5.vv@gmail.com">valeriavega5.vv@gmail.com</a></p>
    <p>🔗 LinkedIn : <a href="https://www.linkedin.com/in/valeria-vega-lora-" target="_blank">www.linkedin.com/in/valeria-vega-lora-</a></p>
  </section>
</main>

<a class="to-top" href="#accueil" title="Revenir en haut">↑</a>

<footer>
  © 2025 Valeria Vega Lora – Tous droits réservés
</footer>

<script>
  // Resalte automatique du menu
  const links = [...document.querySelectorAll('header.site-nav a')];
  const map = new Map(links.map(a => [a.getAttribute('href'), a]));
  const observer = new IntersectionObserver((entries)=>{
    for(const e of entries){
      if(e.isIntersecting){
        const id = '#' + e.target.id;
        links.forEach(a=>a.classList.remove('active'));
        const link = map.get(id);
        if(link) link.classList.add('active');
      }
    }
  }, { rootMargin: '-50% 0px -40% 0px', threshold: 0.01 });
  document.querySelectorAll('main section[id]').forEach(sec=>observer.observe(sec));
</script>

</body>
</html>
