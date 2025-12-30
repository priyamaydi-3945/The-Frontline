
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Frontline | Humanitarian Aid</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet">
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">

    <style>
        :root {
            --primary-blue: #00AEEF;
            --primary-pink: #EC6DB0;
            --text-gray: #555;
            --light-bg: #F9FAFB;
            --card-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            --gradient: linear-gradient(90deg, #00AEEF, #EC6DB0);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #ffffff;
            color: var(--text-gray);
            line-height: 1.6;
        }

        /* --- Navigation --- */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            background: white;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo i {
            font-size: 2.5rem;
            color: #5D5FEF; /* Purple medical icon */
        }

        nav a {
            text-decoration: none;
            color: #333;
            margin-left: 20px;
            font-weight: 600;
            font-size: 0.9rem;
        }

        /* --- Hero Section --- */
        .hero {
            padding: 60px 8%;
            text-align: center;
            background-color: var(--light-bg);
        }

        .hero-card {
            background: white;
            padding: 60px 40px;
            border-radius: 20px;
            box-shadow: var(--card-shadow);
            max-width: 900px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3.5rem;
            background: linear-gradient(90deg, #6a82fb, #fc5c7d);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.1rem;
            max-width: 700px;
            margin: 0 auto 30px;
        }

        /* --- Buttons --- */
        .btn-gradient {
            border: none;
            padding: 14px 30px;
            border-radius: 30px;
            color: white;
            font-weight: 700;
            font-size: 0.9rem;
            cursor: pointer;
            background: var(--gradient);
            box-shadow: 0 4px 15px rgba(236, 109, 176, 0.3);
            margin: 10px;
            transition: transform 0.2s, box-shadow 0.2s;
        }

        .btn-gradient:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(236, 109, 176, 0.4);
        }

        /* --- Sections --- */
        section {
            padding: 60px 8%;
            text-align: center;
        }

        .section-title {
            color: var(--primary-blue);
            font-size: 2.2rem;
            margin-bottom: 25px;
            font-weight: 700;
        }

        .content-text {
            max-width: 800px;
            margin: 0 auto 30px;
            font-size: 1rem;
        }

        /* --- Fundraising Progress --- */
        .progress-container {
            background: #EAEAEA;
            height: 25px;
            border-radius: 12px;
            max-width: 600px;
            margin: 20px auto;
            overflow: hidden;
        }

        .progress-bar {
            width: 0%; /* 0% as seen in your screenshot */
            height: 100%;
            background: #D1D1D1;
        }

        .raised-status {
            font-weight: 600;
            margin-bottom: 50px;
            color: #777;
        }

        /* --- Team Grid --- */
        .team-grid {
            display: flex;
            gap: 25px;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 40px;
        }

        .team-card {
            background: white;
            padding: 40px 25px;
            border-radius: 20px;
            flex: 1;
            min-width: 300px;
            max-width: 380px;
            box-shadow: var(--card-shadow);
            text-align: left;
        }

        .profile-circle {
            width: 160px;
            height: 160px;
            border-radius: 50%;
            border: 5px solid var(--primary-blue);
            margin: 0 auto 25px;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #eee;
        }

        .profile-circle img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .team-card h3 {
            color: var(--primary-blue);
            margin-bottom: 5px;
            font-size: 1.4rem;
        }

        .role {
            font-weight: 700;
            color: #333;
            margin-bottom: 15px;
            display: block;
        }

        .bio {
            font-size: 0.9rem;
            color: #666;
        }

        /* --- Forms & Footer --- */
        .input-group {
            max-width: 500px;
            margin: 0 auto;
        }

        input, textarea {
            width: 100%;
            padding: 15px 20px;
            margin-bottom: 15px;
            border: 1px solid #ddd;
            border-radius: 10px;
            font-family: inherit;
            background: #fff;
        }

        footer {
            padding: 80px 8% 40px;
            text-align: center;
            background: white;
        }

        .social-icons {
            margin: 30px 0;
            font-size: 1.5rem;
        }

        .social-icons i {
            margin: 0 15px;
            color: #6a82fb;
            cursor: pointer;
        }

        .footer-info {
            font-size: 0.85rem;
            color: #aaa;
            margin-top: 20px;
        }

        .quote {
            font-style: italic;
            margin-top: 15px;
            color: #888;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo"><i class="fas fa-caduceus"></i></div>
        <nav>
            <a href="#">Mission</a>
            <a href="#">Donate</a>
            <a href="#">Team</a>
            <a href="#">Articles</a>
            <a href="#">Volunteer</a>
            <a href="#">Updates</a>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-card">
            <h1>Frontline</h1>
            <p>Aiding people in war-affected regions like Gaza and Ukraine — supplying immediate relief and longer-term support.</p>
            <button class="btn-gradient">Donate Now</button>
            <button class="btn-gradient">Join as Volunteer</button>
        </div>
    </section>

    <section id="mission">
        <h2 class="section-title">Our Mission</h2>
        <p class="content-text">We aim to raise $25,000 to support families displaced and affected by conflicts. We channel resources through vetted partners and local volunteers to make relief fast and accountable.</p>
        
        <div class="progress-container">
            <div class="progress-bar"></div>
        </div>
        <p class="raised-status">$0 raised of $25,000 goal</p>

        <h2 class="section-title">Support Our Cause</h2>
        <button class="btn-gradient">Donate via PayPal</button>
        <button class="btn-gradient">Donate via GoFundMe</button>
        <button class="btn-gradient">Donate via Venmo</button>
    </section>

    <section id="team" style="background-color: var(--light-bg);">
        <h2 class="section-title">Meet Our Team</h2>
        <div class="team-grid">
            <div class="team-card">
                <div class="profile-circle">
                    <img src="https://via.placeholder.com/160" alt="Priya">
                </div>
                <h3>Priya Maydipalle</h3>
                <span class="role">President</span>
                <p class="bio">I am a rising senior at Westborough High School. I am passionate about dancing, spending most of my childhood performing in the Boston Ballet... I believe true progress comes from rebuilding lives even through the smallest acts.</p>
            </div>

            <div class="team-card">
                <div class="profile-circle">
                    <img src="https://via.placeholder.com/160" alt="Hasini">
                </div>
                <h3>Hasini Garrepalli</h3>
                <span class="role">Treasurer</span>
                <p class="bio">I am a rising junior at Franklin High School. I am passionate about music, especially singing, and mentor kids with voice lessons throughout the year... I believe taking time to uplift others is one of the most valuable things one can do.</p>
            </div>

            <div class="team-card">
                <div class="profile-circle">
                    <img src="https://via.placeholder.com/160" alt="Yashhu">
                </div>
                <h3>Yashhu Kukula</h3>
                <span class="role">Secretary</span>
                <p class="bio">I am a rising junior at Ashland Highschool. I am passionate about music, art, and reading... I am apart of the varsity tennis team and I believe offering compassion to people affected by war has the power to heal.</p>
            </div>
        </div>
    </section>

    <section id="volunteer">
        <h2 class="section-title">Volunteer With Us</h2>
        <div class="input-group">
            <input type="text" placeholder="Your Name">
            <input type="email" placeholder="Your Email">
            <textarea rows="4" placeholder="Why would you like to volunteer?"></textarea>
            <button class="btn-gradient">Sign Up</button>
        </div>
    </section>

    <footer>
        <h2 class="section-title">Stay Updated</h2>
        <div class="input-group">
            <input type="email" placeholder="Enter Your Email To Receive Updates">
            <button class="btn-gradient">Subscribe</button>
        </div>
        
        <div class="social-icons">
            <i class="fab fa-instagram"></i>
            <i class="fab fa-x-twitter"></i>
            <i class="fab fa-facebook-f"></i>
        </div>

        <div class="footer-info">
            <p>© 2025 Frontline | Built with dedication for humanitarian aid.</p>
            <p class="quote">"Not all of us can do great things. But we can do small things with great love." — Mother Teresa</p>
        </div>
    </footer>

</body>
</html>
