<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Frontline | Humanitarian Nonprofit</title>

  <!-- ONE FONT ONLY -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Inter', sans-serif;
    }

    body {
      background: #ffffff;
      color: #222;
      line-height: 1.6;
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      background: white;
      padding: 1rem 3rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      box-shadow: 0 2px 12px rgba(0,0,0,0.08);
      z-index: 1000;
    }

    .logo {
      display: flex;
      align-items: center;
      gap: 0.7rem;
      font-size: 1.5rem;
      font-weight: 700;
    }

    .logo img {
      width: 42px;
      height: auto;
    }

    nav a {
      margin-left: 2rem;
      text-decoration: none;
      color: #333;
      font-weight: 500;
    }

    nav a:hover {
      color: #ff5fa2;
    }

    .btn {
      display: inline-block;
      background: linear-gradient(90deg, #ff5fa2, #4facfe);
      color: white;
      padding: 0.9rem 1.8rem;
      border-radius: 30px;
      text-decoration: none;
      font-weight: 600;
      box-shadow: 0 10px 25px rgba(79,172,254,0.35);
      transition: transform 0.25s ease, box-shadow 0.25s ease;
    }

    .btn:hover {
      transform: translateY(-3px);
      box-shadow: 0 14px 30px rgba(255,95,162,0.45);
    }

    section {
      padding: 6rem 2rem;
      max-width: 1100px;
      margin: auto;
    }

    .hero {
      padding-top: 8rem;
      text-align: center;
    }

    .hero h1 {
      font-size: 3.2rem;
      margin-bottom: 1rem;
      background: linear-gradient(90deg, #ff5fa2, #4facfe);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    .hero p {
      max-width: 720px;
      margin: auto;
      font-size: 1.1rem;
      color: #555;
      margin-bottom: 2rem;
    }

    .goal-bar {
      background: #ececf2;
      border-radius: 20px;
      overflow: hidden;
      height: 24px;
      margin: 1.5rem auto;
      max-width: 500px;
    }

    .goal-fill {
      height: 100%;
      width: 35%;
      background: linear-gradient(90deg, #ff5fa2, #4facfe);
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      margin-top: 3rem;
    }

    .card {
      background: #f9f9fc;
      border-radius: 18px;
      padding: 2rem;
      box-shadow: 0 12px 30px rgba(0,0,0,0.08);
    }

    .card h3 {
      margin-bottom: 0.8rem;
      color: #333;
    }

    .card a {
      color: #4facfe;
      font-weight: 600;
      text-decoration: none;
    }

    .team {
      display: flex;
      flex-wrap: wrap;
      gap: 2.5rem;
      justify-content: center;
      margin-top: 3rem;
    }

    .member {
      width: 280px;
      text-align: center;
      background: #f9f9fc;
      padding: 2rem;
      border-radius: 20px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.08);
    }

    .member img {
      width: 160px;
      height: 160px;
      object-fit: cover;
      border-radius: 50%;
      border: 5px solid #4facfe;
      margin-bottom: 1rem;
    }

    form {
      max-width: 600px;
      margin: auto;
      background: #f9f9fc;
      padding: 2rem;
      border-radius: 20px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.08);
    }

    form input, form textarea {
      width: 100%;
      padding: 0.9rem;
      margin: 0.6rem 0;
      border-radius: 10px;
      border: 1px solid #ddd;
      font-size: 1rem;
    }

    footer {
      background: #f4f6fb;
      padding: 3rem 2rem;
      text-align: center;
      color: #555;
    }

    footer blockquote {
      font-style: italic;
      margin-top: 1.5rem;
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
      color: #333;
    }
  </style>
</head>

<body>

<header>
  <div class="logo">
    <img src="logo.png" alt="Frontline Logo">
    Frontline
  </div>
  <nav>
    <a href="#mission">Mission</a>
    <a href="#donate">Donate</a>
    <a href="#team">Team</a>
    <a href="#articles">Articles</a>
    <a href="#volunteer">Volunteer</a>
  </nav>
</header>

<section class="hero">
  <h1>Standing With Those on the Frontline</h1>
  <p>
    Frontline is dedicated to aiding civilians impacted by war in Gaza, Israel,
    and Ukraine by raising funds, awareness, and action.
  </p>
  <a class="btn" href="#donate">Donate Now</a>

  <div class="goal-bar">
    <div class="goal-fill"></div>
  </div>
  <p><strong>$8,750 raised of $25,000 goal</strong></p>
</section>

<section id="mission">
  <h2>Our Mission</h2>
  <p>
    We aim to support humanitarian relief efforts by funding trusted organizations,
    mobilizing volunteers, and educating communities on how to help civilians affected
    by war.
  </p>
</section>

<section id="donate">
  <h2>Support the Cause</h2>
  <div class="cards">
    <div class="card">
      <h3>Donate via PayPal</h3>
      <a href="https://paypal.me/">Give Now →</a>
    </div>
    <div class="card">
      <h3>Donate via GoFundMe</h3>
      <a href="https://gofundme.com/">Support Campaign →</a>
    </div>
    <div class="card">
      <h3>Donate via Venmo</h3>
      <a href="https://venmo.com/">Send Donation →</a>
    </div>
  </div>
</section>

<section id="articles">
  <h2>Learn & Take Action</h2>
  <div class="cards">
    <div class="card">
      <h3>UNHCR: Aid in Conflict Zones</h3>
      <a href="https://www.unhcr.org">Read Article →</a>
    </div>
    <div class="card">
      <h3>Red Cross: Helping Civilians</h3>
      <a href="https://www.redcross.org">Read Article →</a>
    </div>
    <div class="card">
      <h3>Doctors Without Borders</h3>
      <a href="https://www.doctorswithoutborders.org">Read Article →</a>
    </div>
  </div>
</section>

<section id="team">
  <h2>Our Team</h2>
  <div class="team">
    <div class="member">
      <img src="priya.jpg" alt="Priya Maydipalle">
      <h3>Priya Maydipalle</h3>
      <p><strong>Founder / Co-President</strong></p>
      <p>
        Rising senior at Westborough High School. Passionate dancer with years of
        performance experience. Aspires to pursue finance and lead meaningful impact.
      </p>
    </div>

    <div class="member">
      <img src="hasini.png" alt="Hasini Garrepalli">
      <h3>Hasini Garrepalli</h3>
      <p><strong>Co-President / Treasurer</strong></p>
      <p>
        Rising junior at Franklin High School. Singer, mentor, and performer dedicated
        to empowering others through creativity and service.
      </p>
    </div>
  </div>
</section>

<section id="volunteer">
  <h2>Volunteer With Us</h2>
  <form>
    <input type="text" placeholder="Full Name" required>
    <input type="email" placeholder="Email Address" required>
    <textarea placeholder="Why do you want to volunteer?" rows="4"></textarea>
    <button class="btn" type="submit">Join Frontline</button>
  </form>
</section>

<footer>
  <p>© 2025 Frontline. All rights reserved.</p>
  <blockquote>
    “Not all of us can do great things. But we can do small things with great love.”
    — Mother Teresa
  </blockquote>
</footer>

</body>
</html>
