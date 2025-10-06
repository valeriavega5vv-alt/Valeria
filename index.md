<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Valeria Vega Lora – Traductrice & Interprète</title>
<style>
  /* =================== Thème (CSS variables) =================== */
  :root {
    --sidebar-w: 288px;

    /* Clair (défaut) */
    --bg: #f6f7fb;
    --bg-accent: linear-gradient(120deg,#f6f7fb 0%,#eef2f9 100%);
    --card: #ffffffcc;
    --glass: blur(8px) saturate(110%);
    --text: #0f172a;
    --muted: #64748b;
    --border: #e5e7ebcc;
    --shadow: 0 10px 30px rgba(2,6,23,.06);
    --accent: #3b82f6;
    --accent-2: #2563eb;
    --ok: #16a34a;

    --gradient-line: linear-gradient(90deg,#93c5fd 0%, #e5e7eb 100%);
    --hover: rgba(59,130,246,.08);
    --active: rgba(59,130,246,.16);

    --input-bg:#fff; --input-b:#dbe3f1; --input-t:#0f172a; --input-ph:#94a3b8;
  }

  body.dark {
    --bg: #0b1220;
    --bg-accent: radial-gradient(900px 600px at 10% 10%, #101a33 0%, #0b1220 60%),
                 radial-gradient(800px 500px at 90% 20%, #0e1a34 0%, #0b1220 60%);
    --card: #0f1b33cc;
    --glass: blur(10px) saturate(120%);
    --text: #e5e7eb;
    --muted: #93a4c0;
    --border: #1d2a45aa;
    --shadow: 0 18px 50px rgba(0,0,0,.35);
    --accent: #60a5fa;
    --accent-2: #3b82f6;
    --ok: #22c55e;

    --gradient-line: linear-gradient(90deg,#60a5fa 0%, #1d2a45 100%);
    --hover: rgba(96,165,250,.12);
    --active: rgba(96,165,250,.22);

    --input-bg:#0f1b33; --input-b:#1f2b49; --input-t:#e5e7eb; --input-ph:#93a4c0;
  }

  html { scroll-behavior: smooth; }
  body {
    margin: 0;
    font: 16px/1.65 Inter, system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    color: var(--text);
    background: var(--bg-accent), var(--bg);
    background-attachment: fixed;
  }
  *, *::before, *::after { box-sizing: border-box; }

  /* =================== Sidebar =================== */
  .sidenav {
    position: fixed; inset: 0 auto 0 0; width: var(--sidebar-w);
    display: flex; flex-direction: column; gap: 18px;
    padding: 22px 18px;
    backdrop-filter: var(--glass);
    background: var(--card);
    border-right: 1px solid var(--border);
    box-shadow: var(--shadow);
    z-index: 1000;
  }
  .brand {
    display: flex; align-items: center; gap: 10px;
    font-weight: 800; font-size: 18px; letter-spacing: .2px;
  }
  .brand .dot {
    width: 12px; height: 12px; border-radius: 999px;
    background: conic-gradient(from 0deg, var(--accent), #94a3b8, var(--accent));
    box-shadow: 0 0 12px var(--accent);
    animation: spin 6s linear infinite;
  }
  @keyframes spin { to { transform: rotate(360deg); } }

  nav { display: grid; gap: 6px; }
  nav a {
    display: flex; align-items: center; gap: 10px;
    padding: 10px 12px; border-radius: 12px;
    text-decoration: none; color: var(--text); font-weight: 600;
    border: 1px solid transparent; transition: .18s ease;
  }
  nav a:hover { background: var(--hover); }
  nav a.active { background: var(--active); border-color: var(--border); color: var(--accent); }
  nav a .dot-li { width: 6px; height: 6px; border-radius: 999px; background: var(--accent); opacity: .65; }

  .divider { height: 1px; background: var(--border); margin: 6px 0 2px; }

  /* Toggle & actions */
  .actions { margin-top: auto; display: grid; gap: 10px; }
  .btn {
    display: inline-flex; align-items: center; justify-content: center; gap: 8px;
    padding: 10px 12px; border-radius: 12px; cursor: pointer;
    border: 1px solid var(--border); background: transparent; color: var(--text); font-weight: 700;
    text-decoration: none;
  }
  .btn:hover { background: var(--hover); }
  .btn.primary { background: var(--accent); color: white; border-color: var(--accent-2); }
  .btn.primary:hover { background: var(--accent-2); }

  .menu-toggle {
    position: fixed; top: 14px; left: 14px; z-index: 1100;
    display: none; background: var(--card); border: 1px solid var(--border); color: var(--text);
    border-radius: 12px; padding: 10px 12px; font-weight: 800;
    backdrop-filter: var(--glass);
  }

  /* =================== Contenu =================== */
  .content { margin-left: var(--sidebar-w); padding: 34px 26px 60px; max-width: 1100px; }
  .section {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 18px;
    padding: 26px;
    margin: 26px 0 34px;
    box-shadow: var(--shadow);
    scroll-margin-top: 18px;
    position: relative;
    overflow: hidden;
  }
  .section::after {
    content: "";
    position: absolute; inset: -30% -30% auto auto; width: 300px; height: 300px;
    background: radial-gradient(120px 120px at 70% 30%, var(--active), transparent 60%);
    opacity: .25; pointer-events: none; transform: rotate(25deg);
  }
  .section header h2 { margin: 0 0 8px 0; font-size: 26px; color: var(--accent); }
  .sub { color: var(--muted); margin-top: 0; }
  .underline { height: 4px; width: 120px; border-radius: 999px; background: var(--gradient-line); margin: 8px 0 12px 0; }

  ul { margin: 0; padding-left: 18px; }
  li { margin: 6px 0; }
  .check li::marker { content: "✔ "; color: var(--ok); font-weight: 700; }

  /* Timeline formation */
  .timeline { position: relative; padding-left: 22px; }
  .timeline::before { content: ""; position: absolute; left: 9px; top: 2px; bottom: 2px; width: 2px;
                       background: linear-gradient(var(--accent), transparent); border-radius: 999px; }
  .tl-item { position: relative; margin: 12px 0; }
  .tl-item::before { content: ""; position: absolute; left: -2px; top: 6px; width: 10px; height: 10px; border-radius: 999px;
                      background: var(--accent); box-shadow: 0 0 0 4px var(--active); }

  /* ====== Formulaire ====== */
  .field{ display:grid; gap:6px; margin:10px 0 }
  label{ font-weight:600; color:var(--text) }
  .input, textarea{
    background: var(--input-bg);
    border:1px solid var(--input-b);
    color: var(--input-t);
    border-radius:12px; padding:12px 14px; outline:none;
  }
  .input::placeholder, textarea::placeholder{ color:var(--input-ph) }
  textarea{ min-height:150px; resize:vertical }
  .error{ color:#ef4444; font-size:14px; display:none }
  .notice{ font-size:14px; color:var(--muted) }
  .form-actions{ display:flex; gap:10px; flex-wrap:wrap; align-items:center }
  .alert{ padding:10px 12px; border-radius:10px; border:1px solid var(--border); display:none }
  .alert.ok{ color:#065f46; background:#d1fae5; border-color:#a7f3d0 }
  .alert.err{ color:#7f1d1d; background:#fee2e2; border-color:#fecaca }

  footer { color: var(--muted); text-align: center; padding: 30px 0 60px; }

  /* Responsive: sidebar */
  @media (max-width: 980px){
    .sidenav { transform: translateX(-100%); transition: .25s ease; }
    body.menu-open .sidenav { transform: translateX(0); }
    .menu-toggle { display: inline-block; }
  }
</style>
</head>
<body>

<button class="menu-toggle" aria-label="Ouvrir le menu" onclick="document.body.classList.toggle('menu-open')">☰ Menu</button>

<aside class="sidenav" aria-label="Navigation latérale">
  <div class="brand"><span class="dot"></span> Valeria Vega Lora</div>

  <nav>
    <a href="#accueil"><span class="dot-li"></span> Accueil</a>
    <a href="#profil"><span class="dot-li"></span> Profil</a>
    <a href="#competences"><span class="dot-li"></span> Compétences</a>
    <a href="#domaines"><span class="dot-li"></span> Domaines</a>
    <a href="#methode"><span class="dot-li"></span> Méthode</a>
    <a href="#importance"><span class="dot-li"></span> Importance</a>
    <a href="#formation"><span class="dot-li"></span> Formation</a>
    <a href="#contact"><span class="dot-li"></span> Contact</a>
  </nav>

  <div class="divider"></div>

  <div class="actions">
    <button class="btn" id="toggle-mode" type="button">🌗 Mode clair / sombre</button>
    <a class="btn primary" href="#contact">Demander un devis</a>
  </div>
</aside>

<main class="content">
  <!-- ACCUEIL -->
  <section id="accueil" class="section">
    <header>
      <h2>Bienvenue</h2>
      <div class="underline"></div>
      <p class="sub">Traductrice & future interprète — Espagnol · Français · Anglais</p>
    </header>
    <p>Bonjour, je m’appelle <strong>Valeria Vega Lora</strong>. Je suis licenciée en langues étrangères de l’Université de l’Atlantique (Colombie) et actuellement étudiante en <strong>Master 1 Traduction & Interprétation</strong> à l’Université de Bretagne Occidentale (France).</p>
    <p>Je transforme des textes et des messages en passerelles claires et naturelles entre cultures. Mon objectif : une communication sans friction, fidèle au sens et adaptée au lectorat.</p>
  </section>

  <!-- PROFIL -->
  <section id="profil" class="section">
    <header>
      <h2>Profil</h2>
      <div class="underline"></div>
    </header>
    <p>Traductrice et future interprète, je travaille avec trois langues principales : <strong>espagnol</strong>, <strong>français</strong> et <strong>anglais</strong>. Mon approche est centrée sur la rigueur terminologique, la cohérence stylistique et l’adaptation culturelle afin d’assurer des textes fluides, crédibles et efficaces.</p>
  </section>

  <!-- COMPÉTENCES -->
  <section id="competences" class="section">
    <header>
      <h2>Compétences</h2>
      <div class="underline"></div>
    </header>
    <ul class="check">
      <li>Traduction ES ⇄ FR ⇄ EN (général & spécialisé)</li>
      <li>Révision, correction et adaptation stylistique</li>
      <li>Pré-traitement & post-édition (outils TAO)</li>
      <li>Recherche terminologique & mémoires de traduction</li>
      <li>Localisation & communication interculturelle</li>
      <li>Respect des délais & confidentialité</li>
    </ul>
  </section>

  <!-- DOMAINES -->
  <section id="domaines" class="section">
    <header>
      <h2>Domaines de spécialité</h2>
      <div class="underline"></div>
    </header>
    <ul class="check">
      <li>Académique & éducation</li>
      <li>Affaires & communication institutionnelle</li>
      <li>Culture, tourisme & patrimoine</li>
      <li>Marketing & réseaux sociaux</li>
      <li>Humanités & sciences sociales</li>
    </ul>
  </section>

  <!-- MÉTHODE -->
  <section id="methode" class="section">
    <header>
      <h2>Méthode de travail</h2>
      <div class="underline"></div>
    </header>
    <ol>
      <li><strong>Analyse du besoin</strong> : public, registre, objectif, supports.</li>
      <li><strong>Recherche & terminologie</strong> : références fiables et glossaires.</li>
      <li><strong>Traduction & cohérence</strong> : style adapté, vérifications croisées.</li>
      <li><strong>Révision finale</strong> : correction, mise en page, préparation livrable.</li>
    </ol>
  </section>

  <!-- IMPORTANCE -->
  <section id="importance" class="section">
    <header>
      <h2>Importance de la traduction</h2>
      <div class="underline"></div>
    </header>
    <p>La traduction est un levier stratégique : elle rend l’information accessible, fait circuler les idées et renforce la confiance entre acteurs d’horizons différents. Au-delà des mots, elle transmet des références culturelles et des nuances indispensables pour être compris sans ambiguïté.</p>
    <p>Une traduction professionnelle garantit pertinence, naturel et impact — conditions essentielles pour éduquer, convaincre, vendre ou coopérer à l’international.</p>
  </section>

  <!-- FORMATION -->
  <section id="formation" class="section">
    <header>
      <h2>Formation académique</h2>
      <div class="underline"></div>
    </header>
    <div class="timeline">
      <div class="tl-item">
        <strong>Master 1 Traduction & Interprétation</strong> — Université de Bretagne Occidentale, France
      </div>
      <div class="tl-item">
        <strong>Licence en Langues Étrangères</strong> — Université de l’Atlantique, Colombie
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="section">
    <header>
      <h2>Contact</h2>
      <div class="underline"></div>
    </header>

    <form id="contactForm" novalidate>
      <div class="field">
        <label for="name">Nom complet</label>
        <input id="name" name="name" class="input" type="text" placeholder="Votre nom" required>
        <div class="error" id="err-name">Veuillez saisir votre nom.</div>
      </div>

      <div class="field">
        <label for="email">E-mail</label>
        <input id="email" name="email" class="input" type="email" placeholder="exemple@domaine.com" required>
        <div class="error" id="err-email">Veuillez saisir un e-mail valide.</div>
      </div>

      <div class="field">
        <label for="subject">Objet</label>
        <input id="subject" name="subject" class="input" type="text" placeholder="Sujet du message" required>
        <div class="error" id="err-subject">Veuillez indiquer l’objet.</div>
      </div>

      <div class="field">
        <label for="message">Message</label>
        <textarea id="message" name="message" placeholder="Écrivez votre message…" required></textarea>
        <div class="error" id="err-message">Veuillez écrire un message.</div>
      </div>

      <div class="form-actions">
        <button class="btn primary" id="sendBtn" type="submit">Envoyer</button>
        <span class="notice">En cliquant sur “Envoyer”, vous acceptez que je vous réponde par e-mail.</span>
      </div>

      <div class="alert ok" id="successMsg">✅ Message envoyé avec succès !</div>
      <div class="alert err" id="failMsg">❌ Échec de l’envoi. Veuillez réessayer.</div>
    </form>
  </section>

  <footer>© 2025 Valeria Vega Lora — Tous droits réservés</footer>
</main>

<script>
  // Nav actif
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
  links.forEach(a=>a.addEventListener('click', ()=>document.body.classList.remove('menu-open')));

  // Toggle mode clair/sombre
  const btnMode = document.getElementById('toggle-mode');
  const key = 'pref-theme';
  const saved = localStorage.getItem(key);
  if (saved === 'dark') document.body.classList.add('dark');
  btnMode.addEventListener('click', ()=>{
    document.body.classList.toggle('dark');
    localStorage.setItem(key, document.body.classList.contains('dark') ? 'dark' : 'light');
  });

  // Menu mobile
  document.querySelector('.menu-toggle')
    .addEventListener('click', ()=>document.body.classList.toggle('menu-open'));

  // Validation formulaire
  const form=document.getElementById('contactForm');
  const ok=document.getElementById('successMsg'), fail=document.getElementById('failMsg');
  form.addEventListener('submit',e=>{
    e.preventDefault();
    let valid=true;
    ['name','email','subject','message'].forEach(id=>{
      const input=document.getElementById(id);
      const err=document.getElementById('err-'+id);
      if(!input.value.trim() || (id==='email' && !/.+@.+\..+/.test(input.value))){
        err.style.display='block'; valid=false;
      } else err.style.display='none';
    });
    if(valid){
      ok.style.display='block'; fail.style.display='none';
      form.reset();
    } else {
      ok.style.display='none'; fail.style.display='block';
    }
  });
</script>

</body>
</html>
