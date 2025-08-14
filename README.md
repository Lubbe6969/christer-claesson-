<!DOCTYPE html>
<html lang="sv">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Claesson Transport – Clister Majister</title>
  <meta name="description" content="Hej hej, jag heter Clister Majister och jag jobbar på Claesson Transport." />
  <style>
    :root {
      --bg: #0f172a;         /* mörk blågrå */
      --card: #ffffff;       /* kortbakgrund */
      --text: #0b1020;       /* huvudtext */
      --accent: #ea4335;     /* röd accent */
    }
    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0; font-family: system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji";
      background: linear-gradient(180deg, #1e293b, #0f172a);
      color: #fff;
      display: grid; place-items: center;
      padding: 24px;
    }
    .card {
      width: min(100%, 980px);
      background: var(--card);
      color: var(--text);
      border-radius: 22px;
      box-shadow: 0 20px 50px rgba(0,0,0,.35);
      overflow: hidden;
    }
    header {
      padding: 22px 24px;
      background: #0f172a;
      color: #fff;
      display: flex; align-items: center; justify-content: space-between;
      gap: 16px;
    }
    header .brand {
      display: flex; align-items: center; gap: 12px; font-weight: 700; letter-spacing: .3px;
    }
    header .brand .logo {
      width: 36px; height: 36px; border-radius: 10px; background: #fff; color: #0f172a; display: grid; place-items: center; font-weight: 800;
    }
    .hero { padding: clamp(18px, 3vw, 28px); display: grid; gap: 18px; }
    .hero h1 { margin: 0; font-size: clamp(26px, 3vw, 34px); }
    .hero p.lead { margin: 0; opacity: .8; }

    .image-wrap {
      position: relative; border-radius: 18px; overflow: hidden;
      background: #e5e7eb; /* light gray placeholder */
    }
    .image-wrap img {
      width: 100%; height: auto; display: block;
    }
    .caption { font-size: 14px; opacity: .7; margin-top: 6px; }

    footer {
      padding: 16px 24px; display: flex; justify-content: space-between; align-items: center; color: #94a3b8; background: #0b1224;
    }
    a.button { display: inline-block; background: var(--accent); color: #fff; padding: 10px 14px; border-radius: 12px; text-decoration: none; font-weight: 700; }
  </style>
</head>
<body>
  <div class="card" role="main">
    <header>
      <div class="brand">
        <div class="logo" aria-hidden="true">C</div>
        <div>Claesson Transport</div>
      </div>
      <a class="button" href="#kontakt">Kontakta oss</a>
    </header>

    <section class="hero">
      <h1>Hej hej, jag heter Clister Majister</h1>
      <p class="lead">…och jag jobbar på Claesson Transport.</p>

      <div class="image-wrap">
        <!-- Byt filnamn nedan till din bilds filnamn i samma mapp som denna HTML -->
        <img src="clister-majister.png" alt="Illustration: Clister Majister framför en Claesson Transport-lastbil med pratbubbla." />
      </div>
      <p class="caption">Ladda upp bilden i samma mapp som <code>index.html</code> och namnge den <code>clister-majister.png</code> (eller uppdatera sökvägen ovan).</p>
    </section>

    <footer>
      <small>&copy; <span id="year"></span> Claesson Transport</small>
      <small id="kontakt">Kontakt: info@claessontransport.se</small>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
  </script>
</body>
</html>
