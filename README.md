<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Mejía Bet - Apuestas Deportivas</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Montserrat:wght@400;700&display=swap');

    body {
      font-family: 'Montserrat', sans-serif;
      background: #0b132b;
      color: #fff;
      margin: 0;
      padding: 0;
      overflow-x: hidden;
    }

    header {
      background: linear-gradient(90deg, #1c2541, #3a506b);
      padding: 1em;
      text-align: center;
      animation: slideDown 1s ease-out;
    }

    header h1 {
      font-family: 'Bebas Neue', cursive;
      color: #ffcc00;
      font-size: 4em;
      margin: 0;
      letter-spacing: 2px;
      animation: pulse 2s infinite;
    }

    .banner {
      width: 100%;
      height: 300px;
      background: url('https://images.unsplash.com/photo-1609334765680-49bd2e8c0d56?fit=crop&w=1400&q=80') center/cover no-repeat;
      position: relative;
      animation: fadeIn 2s ease-in;
    }

    .banner::after {
      content: "¡La emoción del juego en cada clic!";
      position: absolute;
      bottom: 20px;
      left: 30px;
      font-size: 2em;
      background: rgba(0,0,0,0.6);
      padding: 0.7em 1.2em;
      border-radius: 10px;
      color: #ffcc00;
      animation: floatText 3s infinite;
    }

    .matches {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5em;
      padding: 2em;
    }

    .match-card {
      background: #3a506b;
      padding: 1.2em;
      border-radius: 20px;
      box-shadow: 0 0 15px rgba(0,0,0,0.4);
      text-align: center;
      transition: transform 0.3s;
    }

    .match-card:hover {
      transform: translateY(-10px);
    }

    .teams {
      display: flex;
      justify-content: space-around;
      align-items: center;
      margin-bottom: 1em;
    }

    .team-logo {
      width: 60px;
      height: 60px;
      border-radius: 50%;
      object-fit: cover;
    }

    .odds {
      font-size: 1.2em;
      margin: 0.5em 0;
      color: #ffcc00;
    }

    .btn {
      background: #ffcc00;
      color: #000;
      padding: 0.6em 2em;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      transition: background 0.3s;
    }

    .btn:hover {
      background: #ffd700;
    }

    .ads {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 1em;
      padding: 2em;
    }

    .ads img {
      max-width: 300px;
      border-radius: 10px;
      transition: transform 0.3s;
    }

    .ads img:hover {
      transform: scale(1.05);
    }

    footer {
      background: #1c2541;
      text-align: center;
      padding: 1em;
      color: #999;
      margin-top: 2em;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.05); }
      100% { transform: scale(1); }
    }

    @keyframes slideDown {
      from { transform: translateY(-100px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    @keyframes floatText {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-5px); }
    }
  </style>
</head>
<body>

  <header>
    <h1>MEJÍA BET</h1>
  </header>

  <div class="banner"></div>

  <section class="matches">
    <div class="match-card">
      <h3>Real Madrid vs Barcelona</h3>
      <div class="teams">
        <img src="https://upload.wikimedia.org/wikipedia/en/5/56/Real_Madrid_CF.svg" class="team-logo">
        <span>VS</span>
        <img src="https://upload.wikimedia.org/wikipedia/en/4/47/FC_Barcelona_%28crest%29.svg" class="team-logo">
      </div>
      <div class="odds">Cuota: 3.50 / 4.10 / 2.90</div>
      <button class="btn">Apostar Ahora</button>
    </div>

    <div class="match-card">
      <h3>Man. City vs PSG</h3>
      <div class="teams">
        <img src="https://upload.wikimedia.org/wikipedia/en/e/eb/Manchester_City_FC_badge.svg" class="team-logo">
        <span>VS</span>
        <img src="https://upload.wikimedia.org/wikipedia/en/a/a7/Paris_Saint-Germain_F.C..svg" class="team-logo">
      </div>
      <div class="odds">Cuota: 2.80 / 3.90 / 3.10</div>
      <button class="btn">Apostar Ahora</button>
    </div>

    <div class="match-card">
      <h3>Argentina vs Brasil</h3>
      <div class="teams">
        <img src="https://upload.wikimedia.org/wikipedia/en/1/1f/Argentina_national_football_team_logo.svg" class="team-logo">
        <span>VS</span>
        <img src="https://upload.wikimedia.org/wikipedia/en/b/ba/Brazil_national_football_team_logo.svg" class="team-logo">
      </div>
      <div class="odds">Cuota: 3.75 / 3.60 / 2.70</div>
      <button class="btn">Apostar Ahora</button>
    </div>

    <div class="match-card">
      <h3>Boca Juniors vs River Plate</h3>
      <div class="teams">
        <img src="https://upload.wikimedia.org/wikipedia/en/7/7c/Club_Atl%C3%A9tico_Boca_Juniors_logo.svg" class="team-logo">
        <span>VS</span>
        <img src="https://upload.wikimedia.org/wikipedia/en/7/74/Club_Atl%C3%A9tico_River_Plate_logo.svg" class="team-logo">
      </div>
      <div class="odds">Cuota: 4.00 / 3.50 / 2.50</div>
      <button class="btn">Apostar Ahora</button>
    </div>
  </section>

  <section class="ads">
    <img src="https://images.unsplash.com/photo-1600267185522-4773f9c8b762?fit=crop&w=600&q=80" alt="Publicidad 1">
    <img src="https://images.unsplash.com/photo-1598965875413-7c7d12e7981a?fit=crop&w=600&q=80" alt="Publicidad 2">
    <img src="https://images.unsplash.com/photo-1621220341876-7a4f89ab4a83?fit=crop&w=600&q=80" alt="Publicidad 3">
  </section>

  <footer>
    &copy; 2025 Mejía Bet - ¡Gana en grande con nosotros!
  </footer>

</body>
</html>
