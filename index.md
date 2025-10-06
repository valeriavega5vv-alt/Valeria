<!doctype html>
<html lang="fr">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Valeria Vega Lora – Traductrice & Interprète</title>
<style>
  :root{
    --sidebar-w: 270px;

    /* Paleta neutra y sobria */
    --bg: #f7f8fa;           /* fondo claro neutro */
    --text: #1f2937;         /* gris oscuro */
    --muted:#6b7280;         /* gris medio */
    --card:#ffffff;          /* tarjetas blancas */
    --border:#e5e7eb;        /* bordes suaves */
    --shadow: 0 12px 28px rgba(0,0,0,.08);

    --c1:#4b6b9b;  /* azul grisáceo */
    --c2:#3c5a84;  /* azul más profundo */
    --c3:#2f4666;  /* azul marino suave */
  }

  html{scroll-behavior:smooth}
  body{
    margin:0; font:16px/1.65 Inter, system-ui, -apple-system, "Segoe UI", Roboto, Arial, sans-serif;
    color:var(--text); background:var(--bg);
  }

  /* ====== Sidebar ====== */
  .sidenav{
    position:fixed; inset:0 auto 0 0; width:var(--sidebar-w);
    background:#ffffff;
    border-right:1px solid var(--border);
    box-shadow:var(--shadow);
    display:flex; flex-direction:column; gap:18px; padding:22px 18px;
    z-index:1000;
  }
  .brand{
    font-weight:800; letter-spacing:.2px; font-size:18px; color:var(--c2);
  }
  nav a{
    display:flex; align-items:center; gap:10px;
    padding:10px 12px; border-radius:10px; text-decoration:none; color:var(--text);
    border:1px solid transparent; transition:.2s ease; font-weight:600;
  }
  nav a:hover{ background:#f3f4f6; border-color:#e5e7eb; }
  nav a.active{ background:#e7edf8; color:var(--c2); border-color:#d7e0f0; }

  /* Toggle móvil */
  .menu-toggle{
    position:fixed; top:14px; left:14px; z-index:1100;
    display:none; background:#ffffff; border:1px solid var(--border); color:var(--text);
    border-radius:10px; padding:10px 12px; font-weight:800;
  }

  /* ====== Contenido ====== */
  .content{
    margin-left:var(--sidebar-w);
    padding:34px 26px 60px;
    max-width:1100px;
  }
  .section{
    background:var(--card);
    border:1px solid var(--border); border-radius:16px; box-shadow:var(--shadow);
    padding:26px; margin:26px 0 34px;
    scroll-margin-top: 18px;
  }
  .section header h2{ margin:0 0 8px 0; font-size:26px; color:var(--c2) }
  .sub{ color:var(--muted); margin-top:0; }

  /* Barras de color discretas */
  .bar{ height:6px; border-radius:999px; margin:0 0 16px 0; background:#e9eef5; }
  .bar.c1{background:linear-gradient(90deg, #cfd8e6, #e9eef5)}
  .bar.c2{background:linear-gradient(90deg, #c8d4e6, #e9eef5)}
  .bar.c3{background:linear-gradient(90deg, #c3cfdf, #e9eef5)}

  .grid{ display:grid; gap:18px; }
  .cols-2{ grid-template-columns: 1.2fr .8fr; }
  @media (max-width: 960px){ .content{ margin-left:0; padding-top:70px } .cols-2{ grid-template-columns: 1fr } }

  /* Badges / KPIs */
  .badges{ display:flex; gap:10px; flex-wrap:wrap }
  .badge{ font-size:12px; padding:6px 10px; border-radius:999px; border:1px solid #dde4ee; background:#f6f8fb; color:#42556e }
  .kpis{ display:grid; gap:14px; grid-template-columns: repeat(3,1fr); }
  .kpi{ text-align:center; padding:16px; border:1px solid var(--border); border-radius:12px; background:#fafbfc }
  .kpi b{ display:block; font-size:22px; color:var(--c2) }

  /* Listas */
  ul{ margin:0; padding-left:18px }
  li{ margin:6px 0 }
  .check li::marker{ content: "✔ "; color: var(--c2) }

  /* CTA */
  .cta{ display:flex; gap:12px; flex-wrap:wrap; margin-top:6px }
  .btn{
    display:inline-block; text-decoration:none; font-weight:700; color:var(--c2);
    border:1px solid #c7d3e3; padding:10px 14px; border-radius:10px; background:#ffffff;
  }
  .btn.primary{ background:linear-gradient(180deg, #e9eff7, #ffffff); border-color:#c0cfe5; }
  .btn:hover{ transform: translateY(-1px) }

  /* Avatar (usa tu foto valeria.jpg) */
  .avatar{
    width:220px; height:220px; border-radius:999px; border:8px solid #ffffff;
    box-shadow:var(--shadow); object-fit:cover; display:block; margin:0 auto;
  }
  .avatar-wrap{ text-align:center; }

  /* Footer */
  footer{ color:var(--muted); text-align:center; padding:30px 0 60px; }

  /* Responsivo: menú lateral colapsable */
  @media (max-width: 960px){
    .sidenav{ transform: translateX(-100%); transition: .25s ease; }
    body.menu-open .sidenav{ transform: translateX(0); }
    .menu-toggle{ display:block }
  }
</style>
</head>
<body>

<button class="menu-toggle" aria-label="Ouvrir le menu" onclick="document.body.classList.toggle('menu-open')">☰ Menu</button>

<aside class="siden
