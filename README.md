<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clark MPA: DOC Recruitment Modernization | Moses Zenon-Laguerre</title>
    <style>
        :root {
            /* Official Clark University Brand Palette */
            --clark-scarlet: #A91024; 
            --clark-black: #000000;
            --clark-white: #FFFFFF;
            --clark-light-gray: #F4F4F4;
            --clark-mid-gray: #D1D1D1;
            --text-dark: #1A1A1A;
            --shadow: 0 10px 30px rgba(0,0,0,0.15);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        
        body { 
            font-family: "Times New Roman", Times, serif; 
            line-height: 1.6; 
            color: var(--text-dark); 
            background-color: var(--clark-white); 
            scroll-behavior: smooth;
            text-align: center; 
        }

        /* Github Navigation Progress Bar */
        #progress-container { position: fixed; top: 0; width: 100%; height: 8px; background: var(--clark-mid-gray); z-index: 1000; }
        #progress-bar { height: 8px; background: var(--clark-scarlet); width: 0%; transition: width 0.1s; }

        section { 
            padding: 100px 10%; 
            min-height: 100vh; 
            display: flex; 
            flex-direction: column; 
            justify-content: center; 
            align-items: center; 
            border-bottom: 3px solid var(--clark-light-gray); 
        }

        .container { max-width: 1000px; margin: 0 auto; width: 100%; }

        /* Typography */
        h1 { font-size: 3.5rem; line-height: 1.1; color: var(--clark-white); margin-bottom: 20px; text-transform: uppercase; font-weight: 900; }
        h2 { 
            color: var(--clark-scarlet); 
            font-size: 2.8rem; 
            margin-bottom: 40px; 
            text-transform: uppercase; 
            display: inline-block;
            border-bottom: 5px solid var(--clark-black); 
            padding-bottom: 15px;
            font-weight: bold;
        }
        h3 { color: var(--clark-black); margin: 30px 0 15px 0; font-size: 2rem; font-weight: bold; }

        /* Clark Logo Placeholder Styling */
        .clark-logo {
            width: 180px;
            height: auto;
            margin-bottom: 30px;
            filter: brightness(0) invert(1); /* Makes logo white for black background */
        }

        .hero-section { 
            background-color: var(--clark-black); 
            color: var(--clark-white); 
            border-bottom: 20px solid var(--clark-scarlet); 
        }

        /* Presentation Style Table */
        table { 
            width: 100%; 
            max-width: 900px;
            border-collapse: collapse; 
            margin: 50px auto; 
            background: var(--clark-white); 
            box-shadow: var(--shadow); 
            text-align: left; 
        }
        th { background: var(--clark-black); color: var(--clark-white); padding: 20px; text-transform: uppercase; font-size: 1rem; letter-spacing: 1px; }
        td { padding: 18px; border: 1px solid var(--clark-mid-gray); font-size: 1.2rem; }
        tr:nth-child(even) { background-color: var(--clark-light-gray); }

        /* Centered Visual Cards */
        .visual-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); 
            gap: 40px; 
            margin: 50px 0; 
            width: 100%;
        }
        .visual-card { 
            padding: 40px; 
            background: var(--clark-white); 
            border: 1px solid var(--clark-mid-gray); 
            border-top: 10px solid var(--clark-scarlet);
            box-shadow: var(--shadow); 
            transition: transform 0.3s ease;
        }
        .visual-card:hover { transform: translateY(-10px); }

        /* Roadmap Elements */
        .roadmap-container { 
            text-align: center;
            max-width: 850px;
            margin: 0 auto;
        }
        .roadmap-item { margin-bottom: 70px; }
        .phase-label {
            background: var(--clark-scarlet);
            color: var(--clark-white);
            padding: 10px 30px;
            font-weight: 900;
            text-transform: uppercase;
            font-size: 1rem;
            margin-bottom: 20px;
            display: inline-block;
            border-radius: 5px;
        }

        .fade-in { opacity: 0; transform: translateY(50px); transition: all 1.3s ease-out; }
        .fade-in.visible { opacity: 1; transform: translateY(0); }

        .callout-quote { 
            background: var(--clark-light-gray); 
            border: 3px solid var(--clark-scarlet); 
            padding: 40px; 
            margin: 40px auto; 
            max-width: 900px;
            font-size: 1.8rem; 
            font-weight: bold; 
            color: var(--clark-black); 
            font-style: italic;
            box-shadow: var(--shadow);
        }

        footer { background: var(--clark-black); color: var(--clark-white); padding: 50px 10%; text-align: center; border-top: 8px solid var(--clark-scarlet); }
    </style>
</head>
<body>

    <div id="progress-container"><div id="progress-bar"></div></div>

    <section class="hero-section">
        <div class="container">
            <img src="https://upload.wikimedia.org/wikipedia/en/thumb/d/d3/Clark_University_seal.svg/1200px-Clark_University_seal.svg.png" alt="Clark University Logo" class="clark-logo">
            <p style="text-transform: uppercase; letter-spacing: 6px; font-weight: bold; color: var(--clark-scarlet); margin-bottom: 20px;">MPA 3999 Capstone Presentation</p>
            <h1>Diagnosing and Modernizing <br>Public-Safety Hiring</h1>
            <p style="font-size: 2rem; opacity: 0.9;">A Systems Approach to Workforce Stability</p>
            <div style="margin-top: 80px; font-size: 1.5rem; border-top: 1px solid rgba(255,255,255,0.4); padding-top: 40px;">
                <strong>Moses Zenon-Laguerre</strong><br>
                Massachusetts Department of Correction<br>
                <em>Academic Year 2026</em>
            </div>
        </div>
    </section>

    <section>
        <div class="container fade-in">
            <h2>The Core Challenge</h2>
            <p style="font-size: 1.5rem; max-width: 900px; margin: 0 auto;">Our recruitment deficit is a result of <strong>structurally misaligned hiring loops</strong> that favor compliance over momentum.</p>
            
            <div class="callout-quote">
                "Administrative latency acts as a filter that removes high-quality candidates who possess the most market options."
            </div>

            <div class="visual-grid">
                <div class="visual-card">
                    <h3 style="color: var(--clark-scarlet);">The Fast Loop</h3>
                    <p>Modern recruitment, digital leads, and immediate outreach. Expectations: <strong>Instant Engagement.</strong></p>
                </div>
                <div class="visual-card">
                    <h3 style="color: var(--clark-scarlet);">The Slow Loop</h3>
                    <p>Civil Service gates, background audits, and administrative compliance. Reality: <strong>10.2 Month Average.</strong></p>
                </div>
            </div>
        </div>
    </section>

    <section style="background-color: var(--clark-light-gray);">
        <div class="container fade-in">
            <h2>The Yield Forensic: RTC 339</h2>
            <p style="font-size: 1.2rem; margin-bottom: 20px;">Tracking 2,000 leads to identify the velocity of systemic attrition.</p>
            <table>
                <thead>
                    <tr>
                        <th>Hiring Milestone</th>
                        <th>Candidate Volume</th>
                        <th>Yield %</th>
                        <th>Critical Failure Point</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Initial Interest (Leads)</td>
                        <td>2,000</td>
                        <td>100%</td>
                        <td>Outreach Peak</td>
                    </tr>
                    <tr>
                        <td>Exam Registered</td>
                        <td>800</td>
                        <td>40%</td>
                        <td>First-Gate Friction</td>
                    </tr>
                    <tr>
                        <td>Eligible Roster</td>
                        <td>600</td>
                        <td>30%</td>
                        <td>Administrative Silence</td>
                    </tr>
                    <tr>
                        <td><strong>Academy Entry</strong></td>
                        <td><strong>150</strong></td>
                        <td><strong>7.5%</strong></td>
                        <td><strong>Systemic Collapse</strong></td>
                    </tr>
                </tbody>
            </table>
            <p style="font-weight: bold; font-size: 1.4rem; color: var(--clark-scarlet); margin-top: 30px;">92.5% of the potential workforce is lost to process latency.</p>
        </div>
    </section>

    <section>
        <div class="container fade-in">
            <h2>Modernization Roadmap</h2>
            <div class="roadmap-container">
                <div class="roadmap-item">
                    <span class="phase-label">Phase 01: Momentum</span>
                    <h3>The 7-Day Pulse Rule</h3>
                    <p>Replacing "Dead Time" with automated, high-value touchpoints every 7 days to preserve candidate intent during background audits.</p>
                </div>
                <div class="roadmap-item">
                    <span class="phase-label">Phase 02: Efficiency</span>
                    <h3>Parallel Gate Architecture</h3>
                    <p>Moving from Serial to Parallel processing—initiating background investigations simultaneously with Civil Service scoring.</p>
                </div>
                <div class="roadmap-item">
                    <span class="phase-label">Phase 03: Integration</span>
                    <h3>Workforce Flow Model</h3>
                    <p>Unified recruitment and background operations focusing on Academy throughput rather than siloed compliance.</p>
                </div>
            </div>
        </div>
    </section>

    <section style="background-color: var(--clark-scarlet); color: var(--clark-white);">
        <div class="container fade-in">
            <h1 style="font-size: 4.5rem; letter-spacing: 2px;">"A system is what it does."</h1>
            <p style="font-size: 2.2rem; margin-top: 20px; font-style: italic; opacity: 0.9;">To change the outcome, we must change the architecture.</p>
            
            <div style="margin-top: 100px; border-top: 2px solid rgba(255,255,255,0.4); padding-top: 50px;">
                <p style="font-weight: 900; font-size: 2rem;">Moses Zenon-Laguerre</p>
                <p style="font-size: 1.3rem;">Clark University | MPA Candidate</p>
                <p style="font-size: 1.1rem; opacity: 0.8; margin-top: 10px;">Massachusetts Department of Correction</p>
            </div>
        </div>
    </section>

    <footer>
        <p>Strategic Recruitment Modernization | Clark MPA 3999 | 2026</p>
        <p style="font-size: 0.8rem; margin-top: 10px; opacity: 0.6;">All Data Audited via RTC 339 Recruitment Pipeline Report</p>
    </footer>

    <script>
        // Github Progress Bar Logic
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("progress-bar").style.width = scrolled + "%";
        };

        // Scroll Intersection Observer for Professional Fade Effects
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, { threshold: 0.15 });

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
    </script>
</body>
</html>

