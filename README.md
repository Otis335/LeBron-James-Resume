<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LeBron James - Premium Aesthetic Resume</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap');

        :root {
            /* Aesthetic Jewel-Tone Palette */
            --bg-gradient: linear-gradient(135deg, #0b0d19 0%, #16122c 50%, #25112e 100%);
            --bg-card: rgba(26, 22, 46, 0.85); 
            --bg-box: rgba(36, 31, 64, 0.5);
            --text-light: #f8fafc;      /* Crisp off-white */
            --text-muted: #cbd5e1;      /* Soft silver-blue */
            --text-dim: #94a3b8;        /* Subtle slate */
            --border-subtle: rgba(129, 140, 248, 0.15); /* Soft iridescent line */
            
            /* Premium Accent Palette */
            --accent-gold: #f59e0b;     /* Championship Gold */
            --accent-purple: #a78bfa;   /* Royal Lavender */
            --accent-glow: rgba(245, 158, 11, 0.12);
        }

        body {
            font-family: 'Inter', sans-serif;
            background: var(--bg-gradient);
            background-attachment: fixed;
            color: var(--text-muted);
            margin: 0;
            padding: 60px 20px;
            -webkit-font-smoothing: antialiased;
        }

        .resume {
            max-width: 840px;
            margin: 0 auto;
            background: var(--bg-card);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            padding: 50px 60px;
            box-shadow: 0 40px 100px rgba(10, 5, 25, 0.6), 0 0 80px rgba(167, 139, 250, 0.03);
            border-radius: 24px;
            border: 1px solid rgba(255, 255, 255, 0.06);
        }

        /* Sophisticated Header */
        .header {
            display: flex;
            align-items: center;
            gap: 40px;
            padding-bottom: 35px;
            margin-bottom: 40px;
            border-bottom: 1px solid var(--border-subtle);
            position: relative;
        }

        .header-text {
            flex: 1;
        }

        .photo {
            width: 120px;
            height: 120px;
            overflow: hidden;
            flex-shrink: 0;
            border-radius: 20px; 
            border: 2px solid var(--accent-gold);
            box-shadow: 0 0 25px rgba(245, 158, 11, 0.2);
            will-change: transform;
            transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            background: rgba(255, 255, 255, 0.03);
        }

        .photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }

        .name {
            font-size: 3.2rem;
            font-weight: 800;
            letter-spacing: -1.5px;
            margin: 0 0 6px 0;
            color: var(--text-light);
            background: linear-gradient(to right, #ffffff, #e2e8f0);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .title {
            font-size: 1.05rem;
            font-weight: 700;
            color: var(--accent-gold);
            margin: 0 0 14px 0;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .contact {
            font-size: 0.9rem;
            color: var(--text-dim);
            line-height: 1.6;
        }

        /* Section Styling */
        .section {
            margin-bottom: 45px;
        }
        .section:last-child {
            margin-bottom: 0;
        }

        .section-title {
            font-size: 0.95rem;
            font-weight: 800;
            color: var(--accent-purple);
            text-transform: uppercase;
            letter-spacing: 2.5px;
            margin-bottom: 22px;
            display: flex;
            align-items: center;
            gap: 15px;
        }
        .section-title::after {
            content: '';
            flex: 1;
            height: 1px;
            background: linear-gradient(to right, var(--border-subtle), transparent);
        }

        /* Modernized Cards */
        .content-box, .grid-box {
            position: relative;
            background: var(--bg-box);
            border: 1px solid var(--border-subtle);
            border-radius: 16px;
            padding: 24px;
            margin-bottom: 20px;
            transform-style: preserve-3d;
            will-change: transform;
            overflow: hidden; 
            transition: border-color 0.3s ease, background-color 0.3s ease;
        }
        .content-box:last-child { margin-bottom: 0; }

        .content-box *, .grid-box * {
            position: relative;
            z-index: 2;
        }

        /* Dynamic Spotlight Overlay */
        .content-box::before, .grid-box::before {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background: radial-gradient(250px circle at var(--mouse-x, 0px) var(--mouse-y, 0px), var(--accent-glow), transparent 80%);
            z-index: 1;
            pointer-events: none;
            opacity: 0;
            transition: opacity 0.4s ease;
        }
        .content-box:hover::before, .grid-box:hover::before {
            opacity: 1;
        }

        .content-box p {
            margin: 0;
            font-size: 0.95rem;
            line-height: 1.65;
            color: var(--text-muted);
        }

        .row {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 12px;
        }

        .job-title {
            font-weight: 700;
            font-size: 1.15rem;
            color: var(--text-light);
        }

        .company {
            color: var(--accent-gold);
            font-weight: 600;
            font-size: 0.95rem;
            margin-top: 3px;
            letter-spacing: 0.5px;
        }

        .date {
            color: var(--accent-purple);
            font-size: 0.8rem;
            font-weight: 700;
            background: rgba(167, 139, 250, 0.08);
            padding: 5px 14px;
            border-radius: 8px;
            border: 1px solid rgba(167, 139, 250, 0.15);
            letter-spacing: 0.5px;
        }

        ul {
            padding-left: 16px;
            margin-top: 12px;
            margin-bottom: 0;
        }

        li {
            margin-bottom: 8px;
            color: var(--text-muted);
            font-size: 0.95rem;
            line-height: 1.6;
        }
        li:last-child { margin-bottom: 0; }
        
        li::marker {
            color: var(--accent-gold);
        }

        /* Grid Framework */
        .grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 16px;
        }

        .grid-box {
            padding: 22px;
            margin-bottom: 0; 
            background: rgba(36, 31, 64, 0.4);
        }

        .grid-box strong {
            display: inline-block;
            font-weight: 700;
            color: var(--text-light);
            margin-bottom: 6px;
            font-size: 1.05rem;
        }

        /* Premium Minimalist Badges */
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .skill {
            background: rgba(167, 139, 250, 0.06);
            color: #e2e8f0;
            padding: 8px 16px;
            border-radius: 10px;
            font-size: 0.88rem;
            font-weight: 600;
            border: 1px solid var(--border-subtle);
            cursor: default;
            will-change: transform;
            transition: all 0.25s cubic-bezier(0.4, 0, 0.2, 1);
        }

        .skill:hover {
            border-color: var(--accent-gold);
            color: var(--accent-gold);
            background: rgba(245, 158, 11, 0.08);
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(245, 158, 11, 0.1);
        }

        footer {
            text-align: center;
            margin-top: 60px;
            color: rgba(148, 163, 184, 0.4);
            font-size: 0.8rem;
            font-weight: 600;
            letter-spacing: 1.5px;
            text-transform: uppercase;
        }
    </style>
</head>

<body>
    <div class="resume">
        <!-- Header -->
        <div class="header">
            <div class="header-text">
                <h1 class="name">LeBron James</h1>
                <p class="title">Professional Basketball Player & Entrepreneur</p>
                <p class="contact">
                    Los Angeles, California • (310) 555-0198 • lebron@jamesfamily.com<br>
                    lebronjames.com • @KingJames
                </p>
            </div>
            <div class="photo">
                <img src="https://cdn.nba.com/headshots/nba/latest/1040x760/2544.png" alt="LeBron James">
            </div>
        </div>

        <!-- Summary -->
        <div class="section">
            <h2 class="section-title">Professional Summary</h2>
            <div class="content-box">
                <p>
                    Four-time NBA Champion and four-time Finals MVP with over 20 years of professional experience. Known for exceptional leadership, high performance, and significant impact both on and off the court.
                </p>
            </div>
        </div>

        <!-- Experience -->
        <div class="section">
            <h2 class="section-title">Professional Experience</h2>
            
            <div class="content-box">
                <div class="row">
                    <div>
                        <div class="job-title">Small Forward</div>
                        <div class="company">Los Angeles Lakers</div>
                    </div>
                    <div class="date">2018 – Present</div>
                </div>
                <ul>
                    <li>Led the team to the 2020 NBA Championship and earned Finals MVP</li>
                    <li>Consistently delivered elite statistical performances (25+ PPG, 8+ RPG, 8+ APG)</li>
                    <li>Mentored young players while maintaining high team performance standards</li>
                </ul>
            </div>

            <div class="content-box">
                <div class="row">
                    <div>
                        <div class="job-title">Small Forward</div>
                        <div class="company">Cleveland Cavaliers</div>
                    </div>
                    <div class="date">2014 – 2018</div>
                </div>
                <ul>
                    <li>Won 2016 NBA Championship with historic 3-1 series comeback</li>
                </ul>
            </div>

            <div class="content-box">
                <div class="row">
                    <div>
                        <div class="job-title">Small Forward</div>
                        <div class="company">Miami Heat</div>
                    </div>
                    <div class="date">2010 – 2014</div>
                </div>
                <ul>
                    <li>Won back-to-back NBA Championships (2012 & 2013)</li>
                </ul>
            </div>
        </div>

        <!-- Achievements -->
        <div class="section">
            <h2 class="section-title">Key Achievements</h2>
            <div class="grid">
                <div class="grid-box">
                    <ul>
                        <li>4× NBA Champion</li>
                        <li>4× NBA Finals MVP</li>
                        <li>4× NBA Most Valuable Player</li>
                    </ul>
                </div>
                <div class="grid-box">
                    <ul>
                        <li>20× NBA All-Star</li>
                        <li>NBA All-Time Leading Scorer</li>
                        <li>20× All-NBA Team Selection</li>
                    </ul>
                </div>
            </div>
        </div>

        <!-- Off-Court -->
        <div class="section">
            <h2 class="section-title">Off-Court Ventures</h2>
            <div class="grid">
                <div class="grid-box">
                    <strong>SpringHill Company</strong><br>
                    Co-Founder of a leading multimedia and entertainment company.
                </div>
                <div class="grid-box">
                    <strong>LeBron James Family Foundation</strong><br>
                    Founder – Dedicated to education and youth development in Akron, Ohio.
                </div>
                <div class="grid-box">
                    <strong>Business Investments</strong><br>
                    Investor in Blaze Pizza, Liverpool FC, and various tech & wellness companies.
                </div>
                <div class="grid-box">
                    <strong>Brand Partnerships</strong><br>
                    Long-term global ambassador for Nike and other premium brands.
                </div>
            </div>
        </div>

        <!-- Skills -->
        <div class="section">
            <h2 class="section-title">Skills</h2>
            <div class="content-box">
                <div class="skills">
                    <div class="skill">Leadership</div>
                    <div class="skill">Teamwork</div>
                    <div class="skill">High Performance</div>
                    <div class="skill">Mentorship</div>
                    <div class="skill">Public Speaking</div>
                    <div class="skill">Brand Building</div>
                    <div class="skill">Strategic Thinking</div>
                    <div class="skill">Basketball IQ</div>
                </div>
            </div>
        </div>

        <footer>Created By: Otis Chung</footer>
    </div>

    <!-- JavaScript Interactive System Core -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const structuralCards = document.querySelectorAll('.content-box, .grid-box');
            const avatar = document.querySelector('.photo');

            // 3D Tilt & Micro-Spotlight Interactions
            structuralCards.forEach(card => {
                card.addEventListener('mousemove', (e) => {
                    const rect = card.getBoundingClientRect();
                    const x = e.clientX - rect.left; 
                    const y = e.clientY - rect.top;  

                    const transformX = (x / rect.width) - 0.5;
                    const transformY = (y / rect.height) - 0.5;

                    card.style.setProperty('--mouse-x', `${x}px`);
                    card.style.setProperty('--mouse-y', `${y}px`);

                    const maxRotation = 3; 
                    card.style.transform = `perspective(1000px) rotateX(${-transformY * maxRotation}deg) rotateY(${transformX * maxRotation}deg) translateY(-2px)`;
                    card.style.borderColor = 'rgba(245, 158, 11, 0.25)';
                    card.style.backgroundColor = 'rgba(46, 40, 82, 0.6)';
                    card.style.transition = 'transform 0.05s linear, border-color 0.2s ease, background-color 0.2s ease';
                });

                card.addEventListener('mouseleave', () => {
                    card.style.transform = 'perspective(1000px) rotateX(0deg) rotateY(0deg) translateY(0)';
                    card.style.borderColor = '';
                    card.style.backgroundColor = '';
                    card.style.transition = 'transform 0.4s ease, border-color 0.3s ease, background-color 0.3s ease';
                });
            });

            // Clean Avatar Interactions
            if(avatar) {
                avatar.addEventListener('mouseenter', () => {
                    avatar.style.transform = 'scale(1.05) rotate(-1deg)';
                    avatar.style.boxShadow = '0 0 30px rgba(245, 158, 11, 0.4)';
                });
                avatar.addEventListener('mouseleave', () => {
                    avatar.style.transform = 'scale(1) rotate(0deg)';
                    avatar.style.boxShadow = '';
                });
            }
        });
    </script>
</body>

</html>