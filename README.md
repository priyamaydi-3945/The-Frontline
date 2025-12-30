<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Frontline Fundraising</title>
  <style>
    :root {
      --primary-green: #4caf50;
      --light-green: #81c784;
      --light-teal: #81d4fa;
      --lighter-teal: #b3e5fc;
      --dark-text: #2c3e50;
      --bg-color: #f5f5f5;
    }

    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background-color: var(--bg-color);
      color: var(--dark-text);
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    header {
      background: linear-gradient(90deg, var(--primary-green), var(--light-green));
      color: white;
      padding: 15px 0;
      width: 100%;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    .logo {
      width: 80px;
      display: block;
      margin: 0 auto 10px auto;
    }

    h1 {
      font-size: 28px;
      margin: 0;
    }

    .progress-container {
      width: 80%;
      max-width: 600px;
      background-color: #ddd;
      border-radius: 20px;
      overflow: hidden;
      margin-top: 30px;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    }

    .progress-bar {
      height: 35px;
      width: 0;
      background: linear-gradient(90deg, var(--primary-green), var(--light-green));
      text-align: center;
      color: white;
      line-height: 35px;
      border-radius: 20px;
      transition: width 1s ease-in-out;
      font-weight: bold;
    }

    p {
      font-size: 18px;
      margin-top: 10px;
    }

    section {
      max-width: 900px;
      margin: 40px auto;
      padding: 0 20px;
    }

    .hero {
      background-color: white;
      border-radius: 15px;
      padding: 30px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .team {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
    }

    .member {
      background-color: white;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      padding: 15px;
      width: 200px;
    }

    .member img {
      width: 100%;
      border-radius: 10px;
    }

    .member h3 {
      margin: 10px 0 5px;
      color: var(--primary-green);
    }

    footer {
      margin-top: 60px;
      padding: 20px;
      background-color: white;
      width: 100%;
      box-shadow: 0 -2px 8px rgba(0,0,0,0.1);
    }

    .quote {
      font-family: 'Comic Sans MS', cursive, sans-serif;
      font-weight: 700;
      color: var(--dark-text);
      font-size: 26px;
      margin-top: 40px;
      line-height: 1.4;
      text-shadow: 2px 2px 0 var(--lighter-teal), 4px 4px 0 var(--light-teal);
      letter-spacing: 2px;
      text-transform: uppercase;
    }
  </style>
</head>

<body>
  <header>
    <img src="download.png" alt="Hermes Health Symbol" class="logo" />
    <h1>Frontline Fundraising Progress</h1>
  </header>

  <main>
    <div class="progress-container">
      <div id="progress-bar" class="progress-bar">0%</div>
    </div>
    <p id="progress-text">$0 raised of $1000 goal</p>

    <section class="hero">
      <h2>Our Mission</h2>
      <p>Frontline is dedicated to supporting healthcare workers and communities through volunteer efforts and fundraising campaigns. Every dollar goes toward helping those who help others.</p>
    </section>

    <section id="team">
      <h2>Our Team</h2>
      <div class="team">
        <div class="member">
          <img src="hasini.jpg" alt="Hasini Garrepalli">
          <h3>Hasini Garrepalli</h3>
          <p>Rising junior at Franklin High School. Passionate about service and community impact.</p>
        </div>
        <div class="member">
          <img src="priya.jpg" alt="Priya">
          <h3>Priya</h3>
          <p>President of Frontline. Dedicated to empowering youth through meaningful volunteering.</p>
        </div>
      </div>
    </section>

    <div class="quote">
      “It’s not how much we give but how much love we put into giving.”  
      <br>– Mother Teresa
    </div>
  </main>

  <footer>
    <p>© 2025 Frontline | Made with heart and purpose 💚</p>
  </footer>

  <script>
    const goal = 1000;
    const venmoAmount = 0; // update manually

    async function updateProgress() {
      try {
        // Replace with your actual GoFundMe campaign link
        const response = await fetch("https://www.gofundme.com/f/YOUR_GOFUNDME_CAMPAIGN_URL/widget/medium");
        const text = await response.text();
        const match = text.match(/"current_amount":(\d+)/);
        const gofundmeTotal = match ? parseInt(match[1]) / 100 : 0;
        const totalRaised = gofundmeTotal + venmoAmount;
        const percent = Math.min((totalRaised / goal) * 100, 100);

        const bar = document.getElementById("progress-bar");
        const textEl = document.getElementById("progress-text");
        bar.style.width = percent + "%";
        bar.textContent = Math.round(percent) + "%";
        textEl.textContent = `$${totalRaised.toFixed(2)} raised of $${goal} goal`;
      } catch (error) {
        console.error("Error fetching GoFundMe data:", error);
      }
    }

    updateProgress();
  </script>
</body>
</html>
