<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Frontline | Nonprofit Organization</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;600&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Montserrat', sans-serif; color: #f0f0f0; background: #111; }
    header { position: fixed; width: 100%; background: rgba(0,0,0,0.8); padding: 1rem 3rem; display: flex; justify-content: space-between; align-items: center; z-index: 1000; }
    nav a { margin-left: 2rem; color: #fff; text-decoration: none; font-weight: 600; transition: color 0.3s; }
    nav a:hover { color: #ffd700; }

    .logo { display: flex; align-items: center; gap: 0.6rem; font-size: 1.6rem; font-weight: 700; color: #00aaff; }
    .logo span { font-size: 1.5rem; background: linear-gradient(90deg, #00aaff, #ffd700); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }

    .hero { position: relative; height: 100vh; overflow: hidden; }
    .hero video { position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: cover; z-index: -1; }
    .hero .overlay { position: absolute; top:0; left:0; width:100%; height:100%; background: rgba(0,0,0,0.55); }
    .hero-content { position: relative; z-index: 2; height:100%; display:flex; flex-direction: column; justify-content:center; align-items:center; text-align:center; color: #fff; padding: 1rem; }
    .hero-content h2 { font-size: 3rem; margin-bottom: 1rem; background: linear-gradient(90deg, #00aaff, #ffd700); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
    .hero-content p { font-size: 1.2rem; max-width: 700px; margin-bottom: 2rem; }
    .btn { background: linear-gradient(90deg, #00aaff, #ffd700); color: #111; padding: 0.8rem 1.5rem; border-radius: 30px; text-decoration: none; font-weight: 600; margin: 0.5rem; transition: 0.3s; }
    .btn:hover { opacity: 0.8; }

    section { padding: 5rem 2rem; max-width: 1100px; margin: auto; }
    section h2 { text-align: center; font-size: 2.5rem; margin-bottom: 3rem; color: #00aaff; }

    .goal-bar { background: #333; border-radius: 20px; overflow: hidden; margin: 2rem auto; max-width: 600px; height: 25px; }
    .goal-fill { background: linear-gradient(90deg, #00aaff, #ffd700); height: 100%; width: 35%; }

    .team { display: flex; flex-wrap: wrap; justify-content: center; gap: 3rem; }
    .member { background: #1a1a1a; padding: 2rem; border-radius: 15px; width: 280px; text-align: center; transition: transform 0.3s; }
    .member:hover { transform: translateY(-8px); }
    .member img { width: 160px; height: 160px; object-fit: cover; border-radius: 50%; border: 4px solid #00aaff; margin-bottom: 1rem; }
    .member h3 { color: #ffd700; margin-bottom: 0.5rem; }
    .member p { font-size: 0.95rem; line-height: 1.4rem; color: #ddd; }

    .articles { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
    .article { background: #1a1a1a; padding: 2rem; border-radius: 15px; transition: transform 0.3s; }
    .article:hover { transform: scale(1.02); }
    .article h3 { color: #00aaff; margin-bottom: 1rem; }
    .article p { font-size: 0.95rem; color: #ccc; }
    .article a { color: #ffd700; text-decoration: none; font-weight: 600; }

    form { background: #1a1a1a; padding: 2rem; border-radius: 15px; max-width: 600px; margin: 2rem auto; }
    form input, form textarea { width: 100%; padding: 0.8rem; margin: 0.6rem 0; border: none; border-radius: 8px; }
    form button { background: linear-gradient(90deg, #00aaff, #ffd700); border: none; padding: 0.8rem 1.5rem; border-radius: 30px; font-weight: 600; cursor: pointer; }

    footer { background: #000; padding: 2rem; text-align: center; color: #888; }
    footer blockquote { font-style: italic; color: #fff; margin-top: 2rem; }
  </style>
</head>
<body>

  <header>
    <div class="logo">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" width="40" height="40" fill="#00aaff">
        <line x1="50" y1="10" x2="50" y2="90" stroke="#00aaff" stroke-width="3"/>
        <circle cx="50" cy="20" r="6" fill="#00aaff"/>
        <circle cx="50" cy="35" r="6" fill="#00aaff"/>
        <path d="M45 15 C35 25, 35 75, 45 85" stroke="#00aaff" stroke-width="3" fill="none"/>
        <path d="M55 15 C65 25, 65 75, 55 85" stroke="#00aaff" stroke-width="3" fill="none"/>
      </svg>
      <span>Frontline</span>
    </div>
    <nav>
      <a href="#mission">Mission</a>
      <a href="#donate">Donate</a>
      <a href="#team">Team</a>
      <a href="#articles">Articles</a>
      <a href="#volunteer">Volunteer</a>
      <a href="#newsletter">Stay Updated</a>
    </nav>
  </header>

  <section class="hero">
    <video autoplay muted loop>
      <source src="your-video.mp4" type="video/mp4">
    </video>
    <div class="overlay"></div>
    <div class="hero-content">
      <h2>Frontline</h2>
      <p>Aiding people in war-torn regions such as Gaza, Israel, and Ukraine. Together, we can bring hope and relief.</p>
      <a href="#donate" class="btn">Donate Now</a>
      <a href="#volunteer" class="btn">Join as Volunteer</a>
    </div>
  </section>

  <section id="mission">
    <h2>Our Mission</h2>
    <p style="text-align:center; max-width:800px; margin:auto; color:#ccc;">
      We aim to raise $25,000 to support families displaced and affected by conflicts in Gaza, Israel, and Ukraine. Our team works tirelessly to raise awareness, channel resources, and provide aid where it’s needed most.
    </p>
    <div class="goal-bar"><div class="goal-fill"></div></div>
    <p style="text-align:center;">$8,750 raised of $25,000 goal</p>
  </section>

  <section id="donate">
    <h2>Support Our Cause</h2>
    <div style="text-align:center;">
      <a href="https://paypal.me/" class="btn">Donate via PayPal</a>
      <a href="https://gofundme.com/" class="btn">Donate via GoFundMe</a>
      <a href="https://venmo.com/" class="btn">Donate via Venmo</a>
    </div>
  </section>

  <section id="team">
    <h2>Meet Our Team</h2>
    <div class="team">
      <div class="member">
        <img src="priya.jpg" alt="Priya Maydipalle">
        <h3>Priya Maydipalle</h3>
        <p><strong>Founder / Co-President</strong></p>
        <p>I am a rising senior at Westborough High School. I am passionate about dancing, spending most of my childhood performing in the Boston Ballet and Triveni’s School of Karnatic Dance. After graduation, I wish to pursue a career in finance. I am dedicated to this mission because...</p>
      </div>
      <div class="member">
        <img src="hasini.jpg" alt="Hasini Garrepalli">
        <h3>Hasini Garrepalli</h3>
        <p><strong>Co-President / Treasurer</strong></p>
        <p>I am a rising junior at Franklin High School. I am passionate about music, especially singing, and mentor kids with voice lessons throughout the year. I also enjoy dancing and performing. I am dedicated to this mission because...</p>
      </div>
      <div class="member">
        <img src="yashhu.jpg" alt="Yashhu Kukula">
        <h3>Yashhu Kukula</h3>
        <p><strong>Secretary</strong></p>
        <p>[Insert Yashhu’s description here.]</p>
      </div>
    </div>
  </section>

  <section id="articles">
    <h2>Articles & Resources</h2>
    <div class="articles">
      <div class="article">
        <h3>How Aid Reaches War-Torn Areas</h3>
        <p>Learn about the global network of NGOs and volunteers that ensure aid reaches those in Gaza, Israel, and Ukraine.</p>
        <a href="https://www.unhcr.org">Read More →</a>
      </div>
      <div class="article">
        <h3>What You Can Do</h3>
        <p>From donating to volunteering, here are practical steps you can take to support families affected by conflict.</p>
        <a href="https://www.redcross.org">Read More →</a>
      </div>
      <div class="article">
        <h3>Stories of Hope</h3>
        <p>Read real stories of families who have rebuilt their lives with the help of nonprofits and donors like you.</p>
        <a href="https://www.doctorswithoutborders.org">Read More →</a>
      </div>
    </div>
  </section>

  <section id="volunteer">
    <h2>Volunteer With Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Why would you like to volunteer?" rows="4"></textarea>
      <button type="submit">Sign Up</button>
    </form>
  </section>

  <section id="newsletter">
    <h2>Stay Updated</h2>
    <form>
      <input type="email" placeholder="Enter your email to receive updates" required>
      <button type="submit">Subscribe</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Frontline | Built with dedication for humanitarian aid.</p>
    <blockquote>“Not all of us can do great things. But we can do small things with great love.” – Mother Teresa</blockquote>
  </footer>

</body>
</html>
