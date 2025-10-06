<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title> VVL Traducciones – Traductrice & Interprète</title>
<style>
  :root {
    --sidebar-w: 280px;
    /* Modo claro (por defecto) */
    --bg: #f6f7fb;
    --card: #ffffffcc;
    --text: #0f172a;
    --muted: #64748b;
    --border: #e5e7ebcc;
    --accent: #3b82f6;
    --accent-2: #2563eb;
    --hover: rgba(59,130,246,.08);
    --active: rgba(59,130,246,.16);
  }
  body.dark {
    /* Modo oscuro */
    --bg: #0b1220;
    --card: #0f1b33cc;
    --text: #e5e7eb;
    --muted: #93a4c0;
    --border: #1d2a45aa;
    --accent: #60a5fa;
    --accent-2: #3b82f6;
    --hover: rgba(96,165,250,.12);
    --active: rgba(96,165,250,.22);
  }
  body {
    margin:0;
    font:16px/1.65 Inter, system-ui, sans-serif;
    background:var(--bg);
    color:var(--text);
  }
  /* Sidebar */
  .sidenav {
    position:fixed; inset:0 auto 0 0;
    width:var(--sidebar-w);
    display:flex; flex-direction:column; gap:18px;
    padding:22px;
    background:var(--card);
    border-right:1px solid var(--border);
  }
  .brand { font-weight:800; font-size:18px; }
  nav { display:grid; gap:6px; }
  nav a {
    display:block; padding:10px; border-radius:12px;
    text-decoration:none; color:var(--text); font-weight:600;
  }
  nav a:hover { background:var(--hover); }
  nav a.active { background:var(--active); color:var(--accent); }
  .actions { margin-top:auto; display:grid; gap:10px; }
  .btn {
    padding:10px 12px; border-radius:12px; cursor:pointer;
    border:1px solid var(--border); background:transparent;
    color:var(--text); font-weight:600;
    text-align:center; text-decoration:none;
  }
  .btn:hover { background:var(--hover); }
  .btn.primary { background:var(--accent); color:#fff; border-color:var(--accent-2); }
  .btn.primary:hover { background:var(--accent-2); }
  /* Contenido */
  .content { margin-left:var(--sidebar-w); padding:34px 26px; }
  .section {
    background:var(--card);
    border:1px solid var(--border);
    border-radius:18px;
    padding:26px; margin:26px 0;
  }
  .section h2 { margin-top:0; color:var(--accent); }
  .sub { color:var(--muted); }
  footer { color:var(--muted); text-align:center; padding:30px; }
  /* Responsive */
  @media (max-width:980px){
    .sidenav { transform:translateX(-100%); transition:.25s ease; }
    body.menu-open .sidenav{ transform:translateX(0); }
    .menu-toggle{ display:block; }
    .content{ margin-left:0; padding-top:72px; }
  }
  .menu-toggle{
    position:fixed; top:14px; left:14px;
    display:none; background:var(--card);
    border:1px solid var(--border); padding:10px;
    border-radius:12px; font-weight:800;
    cursor:pointer;
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
    <a href="#importance">Importance</a>
    <a href="#formation">Formation</a>
    <a href="#contact">Contact</a>
  </nav>
  <div class="actions">
    <a class="btn" href="mailto:valeriavega5.vv@gmail.com">✉️ Email</a>
    <a class="btn" target="_blank" href="https://www.linkedin.com/in/valeria-vega-lora-">LinkedIn</a>
    <!-- Botón modo claro/oscuro -->
    <button class="btn" id="toggle-mode" type="button">🌗 Mode clair / sombre</button>
  </div>
</aside>

<main class="content">
  <!-- ACCUEIL -->
  <section id="accueil" class="section">
    <h2>Bienvenue</h2>
    <p class="sub">Traductrice & future interprète — Espagnol · Français · Anglais</p>
    <div style="text-align:center; margin:20px 0;">
      <img src="https://github.com/user-attachments/assets/8fa31692-eafd-4c5d-bb58-c80435ddddfa"
           alt="Valeria Vega Lora"
           style="width:150px; height:auto; border-radius:12px;">
    </div>
    <p>Bonjour, je m’appelle <strong>Valeria Vega Lora</strong>. Je suis licenciée en langues étrangères de l’Université de l’Atlantique (Colombie) et actuellement étudiante en <strong>Master 1 Traduction & Interprétation</strong> à l’Université de Bretagne Occidentale (France).</p>
  </section>

  <!-- PROFIL -->
  <section id="profil" class="section">
    <h2>Profil</h2>
    <p>Traductrice et future interprète, je travaille avec trois langues principales : espagnol, français et anglais.</p>
  </section>

  <!-- COMPÉTENCES -->
  <section id="competences" class="section">
    <h2>Compétences</h2>
    <ul>
      <li>Traduction ES ⇄ FR ⇄ EN</li>
      <li>Révision et correction</li>
      <li>Localisation & communication interculturelle</li>
    </ul>
  </section>

  <!-- IMPORTANCE -->
  <section id="importance" class="section">
    <h2>Importance de la traduction</h2>
    <p>La traduction est un levier stratégique : elle rend l’information accessible, fait circuler les idées et renforce la confiance entre acteurs d’horizons différents.</p>
  </section>

  <!-- FORMATION -->
  <section id="formation" class="section">
    <h2>Formation académique</h2>
    <ul>
      <li>Master 1 Traduction & Interprétation — Université de Bretagne Occidentale, France</li>
      <li>Licence en Langues Étrangères — Université de l’Atlantique, Colombie</li>
    </ul>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="section">
    <h2>Contact</h2>
    <p>📧 <a href="mailto:valeriavega5.vv@gmail.com">valeriavega5.vv@gmail.com</a></p>
    <p>🔗 <a target="_blank" href="https://www.linkedin.com/in/valeria-vega-lora-">Mon LinkedIn</a></p>
  </section>

  <footer>© 2025 Valeria Vega Lora — Tous droits réservés</footer>
</main>

<script>
  // Activar modo claro/oscuro con memoria
  const btnMode = document.getElementById('toggle-mode');
  const key = 'pref-theme';
  const saved = localStorage.getItem(key);
  if (saved === 'dark') document.body.classList.add('dark');
  btnMode.addEventListener('click', () => {
    document.body.classList.toggle('dark');
    localStorage.setItem(key, document.body.classList.contains('dark') ? 'dark' : 'light');
  });
</script>

</body>
</html>
