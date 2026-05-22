<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LeBron James - Resume</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap');

        body {
            font-family: 'Roboto', sans-serif;
            background: #f0f4f8;
            margin: 0;
            padding: 40px 20px;
        }

        .resume {
            max-width: 920px;
            margin: 0 auto;
            background: white;
            padding: 50px 60px;
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.12);
            border-radius: 12px;
        }

        .header {
            display: flex;
            align-items: center;
            gap: 40px;
            padding-bottom: 30px;
            margin-bottom: 40px;
            border-bottom: 4px solid #1565C0;
        }

        .header-text {
            flex: 1;
        }

        .photo {
            width: 135px;
            height: 160px;
            overflow: hidden;
            flex-shrink: 0;
            border-radius: 6px;
        }

        .photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .name {
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 6px;
            color: #0f2b5b;
        }

        .title {
            font-size: 1.3rem;
            color: #1565C0;
            margin-bottom: 12px;
        }

        .contact {
            font-size: 1.02rem;
            color: #444;
            line-height: 1.7;
        }

        .section {
            margin-bottom: 45px;
        }

        .section-title {
            font-size: 1.45rem;
            font-weight: 700;
            color: #0f2b5b;
            border-bottom: 3px solid #1565C0;
            padding-bottom: 10px;
            margin-bottom: 25px;
        }

        .content-box {
            background: #fafcff;
            border: 1px solid #d0e0ff;
            border-radius: 10px;
            padding: 22px;
            margin-bottom: 25px;
            box-shadow: 0 4px 12px rgba(21, 101, 192, 0.08);
        }

        .row {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 10px;
        }

        .job-title {
            font-weight: 700;
            font-size: 1.15rem;
            color: #0f2b5b;
        }

        .company {
            color: #1565C0;
            font-weight: 500;
        }

        .date {
            color: #555;
            font-size: 0.97rem;
        }

        ul {
            padding-left: 22px;
            margin-top: 12px;
        }

        li {
            margin-bottom: 8px;
            color: #333;
            line-height: 1.55;
        }

        .grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .grid-box {
            background: #f8fbff;
            border: 1px solid #c5d8ff;
            border-radius: 10px;
            padding: 18px;
        }

        /* Simple Skills */
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 14px;
        }

        .skill {
            background: #f1f5f9;
            color: #1e3a8a;
            padding: 7px 18px;
            border-radius: 6px;
            font-size: 1rem;
            border: 1px solid #cbd5e1;
        }

        footer {
            text-align: center;
            margin-top: 50px;
            color: #666;
            font-size: 0.95rem;
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
                <img src="https://cdn.nba.com/headshots/nba/latest/1040x760/2544.png" 
                     alt="LeBron James">
            </div>
        </div>

        <!-- Summary -->
        <div class="section">
            <h2 class="section-title">Professional Summary</h2>
            <div class="content-box">
                <p>
                    Four-time NBA Champion and four-time Finals MVP with over 20 years of professional experience. 
                    Known for exceptional leadership, high performance, and significant impact both on and off the court.
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
                    <li>Mentored young players while maintaining high team standards</li>
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
                    <li>Won 2016 NBA Championship with historic 3-1 comeback</li>
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

        <footer>
           Created By: Otis Chung
        </footer>

    </div>

</body>
</html>