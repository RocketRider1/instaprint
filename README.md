<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Instaprint — Instant photo prints & products</title>
  <meta name="description" content="Instaprint — turn your photos into prints, gifts, and merch in minutes. Fast shipping. Amazing color." />

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#94a3b8;
      --accent1:#1e40af; /* tech blue */
      --accent2:#f97316; /* orange */
      --glass: rgba(255,255,255,0.03);
      font-family: 'Inter', system-ui, sans-serif;
      color-scheme: dark;
    }

    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(180deg, #071026 0%, var(--bg) 60%);
      color: #e6eef8;
      line-height:1.45;
    }

    .wrap{max-width:1100px;margin:0 auto;padding:28px;}

    /* NAV */
    .nav{display:flex;align-items:center;justify-content:space-between;gap:18px;margin-bottom:28px;}
    .brand{display:flex;gap:12px;align-items:center;text-decoration:none;color:inherit;}
    .brand svg{width:44px;height:44px;}
    .brand h1{font-size:18px;margin:0;font-weight:800;letter-spacing:-0.3px}
    .brand p{margin:0;font-size:12px;color:var(--muted);font-weight:600}

    .nav-actions{display:flex;gap:12px;align-items:center}
    .btn{
      display:inline-flex;align-items:center;gap:8px;
      padding:10px 14px;border-radius:10px;
      border:1px solid transparent;
      background:linear-gradient(90deg, rgba(255,255,255,0.04), rgba(255,255,255,0.02));
      color:inherit;text-decoration:none;font-weight:600;
      cursor:pointer;transition:transform .12s ease;
    }
    .btn:active{transform:translateY(1px)}
    .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted);}
    .primary{
      background:linear-gradient(90deg,var(--accent1),var(--accent2));
      color:white;
      box-shadow:0 6px 20px rgba(7,12,30,0.6);
    }

    /* HERO */
    .hero{
      display:grid;grid-template-columns:1fr 420px;
      gap:28px;align-items:center;
      padding:28px;border-radius:16px;
      border:1px solid rgba(255,255,255,0.03);
      background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);
    }
    .hero-left h2{font-size:40px;margin:0 0 12px;color:#f8fbff;}
    .lead{color:var(--muted);margin-bottom:18px;font-size:16px;}
    .cta-row{display:flex;gap:12px;flex-wrap:wrap}
    .stats{display:flex;gap:14px;margin-top:18px}
    .stat{background:var(--glass);padding:10px 12px;border-radius:10px;font-weight:700;font-size:14px}

    /* MOCK CARD */
    .mock-card{background:var(--glass);padding:14px;border-radius:12px;}
    .print-preview{
      height:320px;border-radius:8px;overflow:hidden;
      background:linear-gradient(180deg, #07112666, #0f213333);
      display:flex;align-items:center;justify-content:center;
    }
    .print-preview img{width:92%;border-radius:6px;}

    .mock-meta{display:flex;justify-content:space-between;align-items:center;margin-top:12px;}
    .price{font-weight:800}
    .tag{font-size:12px;color:var(--muted);padding:6px 8px;border-radius:8px;background:rgba(255,255,255,0.02)}

    /* FEATURES */
    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:22px;}
    .feature{background:var(--glass);padding:12px;border-radius:10px;}
    .feature h4{margin:0 0 6px;font-size:15px}
    .feature p{margin:0;color:var(--muted);font-size:13px}

    /* FOOTER */
    footer{margin-top:28px;color:var(--muted);font-size:13px;text-align:center;padding:20px 0}

    /* RESPONSIVE */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .features{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:600px){
      .features{grid-template-columns:1fr}
      .hero-left h2{font-size:28px}
      .print-preview{height:240px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <nav class="nav">
      <a class="brand" href="/">
        <svg viewBox="0 0 64 64">
          <defs>
            <linearGradient id="logo" x1="0" x2="1" y1="0" y2="1">
              <stop offset="0" stop-color="#1e40af"/>
              <stop offset="1" stop-color="#f97316"/>
            </linearGradient>
          </defs>
          <rect x="6" y="10" width
