# Bilds-russia-rp-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Bilds Russia RP</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, Helvetica, sans-serif;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background: #080808;
      color: white;
    }

    /* NAVBAR */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      padding: 18px 7%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: rgba(0, 0, 0, 0.85);
      backdrop-filter: blur(10px);
      z-index: 1000;
      border-bottom: 1px solid #252525;
    }

    .logo {
      font-size: 25px;
      font-weight: 900;
      color: #ff2020;
      letter-spacing: 1px;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 30px;
    }

    nav ul li a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    nav ul li a:hover {
      color: #ff2020;
    }

    /* HERO */
    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 120px 20px 60px;

      background:
        linear-gradient(rgba(0,0,0,.65), rgba(0,0,0,.9)),
        radial-gradient(circle at center, #7b0000, #080808 65%);
    }

    .hero-content {
      max-width: 900px;
    }

    .hero h1 {
      font-size: clamp(45px, 8vw, 95px);
      font-weight: 1000;
      text-transform: uppercase;
      text-shadow: 0 0 30px rgba(255,0,0,.5);
    }

    .hero h1 span {
      color: #ff2020;
    }

    .hero p {
      margin: 20px auto;
      color: #cfcfcf;
      font-size: 20px;
      max-width: 650px;
      line-height: 1.6;
    }

    .buttons {
      margin-top: 35px;
      display: flex;
      justify-content: center;
      gap: 15px;
      flex-wrap: wrap;
    }

    .btn {
      padding: 15px 30px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      transition: .3s;
      display: inline-block;
    }

    .primary {
      background: #e50909;
      color: white;
      box-shadow: 0 0 20px rgba(255,0,0,.25);
    }

    .primary:hover {
      background: #ff3030;
      transform: translateY(-3px);
    }

    .secondary {
      border: 1px solid #555;
      color: white;
    }

    .secondary:hover {
      border-color: #ff2020;
      color: #ff2020;
      transform: translateY(-3px);
    }

    /* SECTIONS */
    section {
      padding: 90px 7%;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 42px;
      text-transform: uppercase;
    }

    .section-title span {
      color: #ff2020;
    }

    .section-title p {
      color: #999;
      margin-top: 10px;
    }

    /* FEATURES */
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 25px;
    }

    .card {
      background: #111;
      border: 1px solid #292929;
      border-radius: 12px;
      padding: 30px;
      text-align: center;
      transition: .3s;
    }

    .card:hover {
      transform: translateY(-8px);
      border-color: #ff2020;
      box-shadow: 0 10px 35px rgba(255,0,0,.12);
    }

    .card .icon {
      font-size: 45px;
      margin-bottom: 15px;
    }

    .card h3 {
      margin-bottom: 10px;
    }

    .card p {
      color: #aaa;
      line-height: 1.6;
    }

    /* ABOUT */
    .about {
      background: #0d0d0d;
    }

    .about-content {
      max-width: 900px;
      margin: auto;
      text-align: center;
    }

    .about-content p {
      color: #bbb;
      font-size: 18px;
      line-height: 1.8;
    }

    /* STATS */
    .stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 20px;
      margin-top: 40px;
    }

    .stat {
      background: #111;
      padding: 30px;
      text-align: center;
      border-radius: 10px;
      border: 1px solid #252525;
    }

    .stat h3 {
      font-size: 38px;
      color: #ff2020;
    }

    .stat p {
      color: #aaa;
      margin-top: 5px;
    }

    /* RULES */
    .rules {
      max-width: 850px;
      margin: auto;
    }

    .rule {
      padding: 20px;
      background: #111;
      margin-bottom: 12px;
      border-left: 4px solid #e50909;
      border-radius: 5px;
    }

    .rule strong {
      color: #ff3030;
    }

    /* DISCORD */
    .discord {
      text-align: center;
      background:
        linear-gradient(rgba(120,0,0,.2), rgba(0,0,0,.7)),
        #090909;
    }

    .discord p {
      color: #bbb;
      margin: 15px auto 25px;
      max-width: 600px;
    }

    /* FOOTER */
    footer {
      background: #050505;
      padding: 30px;
      text-align: center;
      border-top: 1px solid #222;
    }

    footer p {
      color: #777;
    }

    footer span {
      color: #ff2020;
    }

    @media (max-width: 700px) {
      nav {
        padding: 15px 20px;
      }

      nav ul {
        gap: 12px;
      }

      nav ul li a {
        font-size: 12px;
      }

      .hero p {
        font-size: 16px;
      }

      section {
        padding: 70px 20px;
      }
    }
  </style>
</head>

<body>

  <!-- NAVIGATION -->
  <nav>
    <div class="logo">BILDS RUSSIA RP</div>

    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#features">Features</a></li>
      <li><a href="#rules">Rules</a></li>
      <li><a href="#discord">Discord</a></li>
    </ul>
  </nav>


  <!-- HERO -->
  <section class="hero" id="home">
    <div class="hero-content">

      <h1>BILDS <span>RUSSIA</span> RP</h1>

      <p>
        Welcome to Bilds Russia RP — build your character,
        create your story and experience an immersive roleplay world.
      </p>

      <div class="buttons">
        <a href="#discord" class="btn primary">
          JOIN DISCORD
        </a>

        <a href="#about" class="btn secondary">
          LEARN MORE
        </a>
      </div>

    </div>
  </section>


  <!-- ABOUT -->
  <section class="about" id="about">

    <div class="section-title">
      <h2>About <span>Us</span></h2>
      <p>Enter the world of Bilds Russia RP</p>
    </div>

    <div class="about-content">

      <p>
        Bilds Russia RP is a roleplay community where players can
        create their own characters, join organizations, build careers,
        interact with other players and create their own stories.
      </p>

      <div class="stats">

        <div class="stat">
          <h3>24/7</h3>
          <p>Roleplay</p>
        </div>

        <div class="stat">
          <h3>100+</h3>
          <p>Players</p>
        </div>

        <div class="stat">
          <h3>50+</h3>
          <p>Events</p>
        </div>

        <div class="stat">
          <h3>∞</h3>
          <p>Stories</p>
        </div>

      </div>

    </div>
  </section>


  <!-- FEATURES -->
  <section id="features">

    <div class="section-title">
      <h2>Server <span>Features</span></h2>
      <p>Everything you need for an exciting RP experience</p>
    </div>

    <div class="cards">

      <div class="card">
        <div class="icon">🎭</div>
        <h3>Roleplay</h3>
        <p>
          Create your own character and develop your unique story.
        </p>
      </div>

      <div class="card">
        <div class="icon">🚓</div>
        <h3>Organizations</h3>
        <p>
          Join government, police, medical and other organizations.
        </p>
      </div>

      <div class="card">
        <div class="icon">💰</div>
        <h3>Economy</h3>
        <p>
          Work, earn money, purchase items and build your character.
        </p>
      </div>

      <div class="card">
        <div class="icon">🔥</div>
        <h3>Events</h3>
        <p>
          Participate in exciting community events and activities.
        </p>
      </div>

    </div>
  </section>


  <!-- RULES -->
  <section id="rules" class="about">

    <div class="section-title">
      <h2>Server <span>Rules</span></h2>
      <p>Respect the community and keep roleplay enjoyable</p>
    </div>

    <div class="rules">

      <div class="rule">
        <strong>01.</strong>
        Respect all players and staff members.
      </div>

      <div class="rule">
        <strong>02.</strong>
        No cheating, exploiting or unauthorized modifications.
      </div>

      <div class="rule">
        <strong>03.</strong>
        Follow Roleplay rules at all times.
      </div>

      <div class="rule">
        <strong>04.</strong>
        Do not use RDM, VDM, DM or other prohibited actions.
      </div>

      <div class="rule">
        <strong>05.</strong>
        Do not abuse bugs or glitches.
      </div>

      <div class="rule">
        <strong>06.</strong>
        Listen to server administration and follow their decisions.
      </div>

    </div>
  </section>


  <!-- DISCORD -->
  <section class="discord" id="discord">

    <div class="section-title">
      <h2>Join <span>Our Community</span></h2>
    </div>

    <p>
      Join the official Bilds Russia RP Discord to receive
      announcements, updates, events and community information.
    </p>

    <!-- Replace the link below with your Discord invite -->
    <a
      href="https://discord.gg/YOURINVITE"
      target="_blank"
      class="btn primary">
      JOIN DISCORD
    </a>

  </section>


  <!-- FOOTER -->
  <footer>
    <p>
      © 2026 <span>Bilds Russia RP</span>.
      All Rights Reserved.
    </p>
  </footer>

</body>
</html>
