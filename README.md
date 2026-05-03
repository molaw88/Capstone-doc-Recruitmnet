
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DOC Recruitment: Systemic Modernization | Moses Zenon-Laguerre</title>
    <style>
        :root {
            --red: #14558F;
            --berkshires-green: #388557;
            --duckling-yellow: #F6C51B;
            --granite-gray: #F2F2F2;
            --text-dark: #333333;
            --white: #FFFFFF;
            --danger-red: #C62828;
            --shadow: 0 4px 12px rgba(0,0,0,0.1);
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { 
            font-family: "Times New Roman", Times, serif; 
            line-height: 1.6; 
            color: var(--text-dark); 
            background-color: var(--white); 
            scroll-behavior: smooth;
            text-align: center; /* Center-aligning the base text */
        }

        #progress-container { position: fixed; top: 0; width: 100%; height: 6px; background: #ccc; z-index: 1000; }
        #progress-bar { height: 6px; background: var(--duckling-yellow); width: 0%; transition: width 0.1s; }

        section { 
            padding: 100px 10%; 
            min-height: 100vh; 
            display: flex; 
            flex-direction: column; 
            justify-content: center; 
            align-items: center; /* Centering sections */
            border-bottom: 1px solid #ddd; 
        }

        .container { max-width: 1000px; margin: 0 auto; width: 100%; }

        h1 { font-size: 3.8rem; line-height: 1.1; color: var(--white); margin-bottom: 20px; }
        h2 { 
            color: var(--bay-blue); 
            font-size: 2.8rem; 
            margin-bottom: 30px; 
            text-transform: uppercase; 
            display: inline-block;
            border-bottom: 6px solid var(--duckling-yellow); 
            padding-bottom: 10px;
        }
        h3 { color: var(--bay-blue); margin: 25px 0 15px 0; font-size: 1.8rem; }

        .hero-section { 
            background-color: var(--bay-blue); 
            color: var(--white); 
            border-bottom: 12px solid var(--duckling-yellow); 
        }

        /* Centered Table */
        table { 
            width: 100%; 
            max-width: 900px;
            border-collapse: collapse; 
            margin: 40px auto; 
            background: white; 
            box-shadow: var(--shadow); 
            text-align: left; /* Keep table text legible but center the block */
        }
        th { background: var(--bay-blue); color: white; padding: 18px; text-transform: uppercase; font-size: 0.9rem; }
        td { padding: 15px; border: 1px solid #ddd; font-size: 1.1rem; }

        /* Logic Grid */
        .logic-grid { 
            display: grid; 
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); 
            gap: 30px; 
            margin: 40px 0; 
            width: 100%;
        }
        .logic-card { 
            padding: 30px; 
            background: var(--white); 
            border: 1px solid #ddd; 
            box-shadow: var(--shadow); 
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        /* Roadmap Visualization */
        .roadmap-list { 
            list-style: none; 
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
        }
        .roadmap-list li { margin-bottom: 50px; }
        .phase-badge {
            background: var(--bay-blue);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 0.8rem;
            margin-bottom: 15px;
            display: inline-block;
        }

        .fade-in { opacity: 0; transform: translateY(40px); transition: all 1.2s ease-out; }
        .fade-in.visible { opacity: 1; transform: translateY(0); }

        .impact-statement { 
            background: #fff5f5; 
            border: 2px solid var(--danger-red); 
            padding: 30px; 
            margin: 30px auto; 
            max-width: 800px;
            font-size: 1.5rem; 
            font-weight: bold; 
            color: var(--danger-red); 
        }

        footer { background: #1a1a1a; color: white; padding: 40px 10%; text-align: center; }
    </style>
</head>
<body>

    <div id="progress-container"><div id="progress-bar"></div></div>

    <section class="hero-section">
        <div class="container">
            <p style="text-transform: uppercase; letter-spacing: 4px; font-weight: bold; color: var(--duckling-yellow); margin-bottom: 20px;">MPA Capstone Senior Leadership Briefing</p>
            <h1>Diagnosing and Modernizing <br>Public-Safety Hiring</h1>
            <p style="font-size: 1.8rem; opacity: 0.9;">A Systems Approach to Workforce Stability</p>
            <div style="margin-top: 60px; font-size: 1.3rem; border-top: 1px solid rgba(255,255,255,0.3); padding-top: 30px;">
                <strong>Moses Zenon-Laguerre</strong><br>
                Massachusetts Department of Correction<br>
                <em>May 4th, 2026</em>
            </div>
        </div>
    </section>

    <section>
        <div class="container fade-in">
            <h2>The Systemic Bottleneck</h2>
            <p style="font-size: 1.4rem; max-width: 800px; margin: 0 auto;">The current recruitment challenges facing the DOC are a product of <strong>structurally misaligned hiring loops</strong>.</p>
            <div class="impact-statement">
                "Administrative latency acts as a filter that removes high-quality candidates who possess the most market options."
            </div>
            <div class="logic-grid">
                <div class="logic-card">
                    <h3 style="color: var(--berkshires-green);">Fast Loop (Market)</h3>
                    <p>High-velocity engagement, social presence, and instant leads. The candidate expectation is modern and immediate.</p>
                </div>
                <div class="logic-card">
                    <h3 style="color: var(--bay-blue);">Slow Loop (Compliance)</h3>
                    <p>Structural constraints of Civil Service and background compliance. The system reality averages 10.2 months.</p>
                </div>
            </div>
        </div>
    </section>

    <section style="background-color: var(--granite-gray);">
        <div class="container fade-in">
            <h2>Data Forensic: Cohort 339</h2>
            <p>An audit of 2,000 leads reveals the precise velocity of the "Yield Gap."</p>
            <table>
                <thead>
                    <tr>
                        <th>Hiring Milestone</th>
                        <th>Volume</th>
                        <th>Yield %</th>
                        <th>Friction Point</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Initial Leads</td>
                        <td>2,000</td>
                        <td>100%</td>
                        <td>Outreach Success</td>
                    </tr>
                    <tr>
                        <td>Exam Registered</td>
                        <td>800</td>
                        <td>40%</td>
                        <td>Initial Friction</td>
                    </tr>
                    <tr>
                        <td>Eligible Roster</td>
                        <td>600</td>
                        <td>30%</td>
                        <td>Dead Time Silence</td>
                    </tr>
                    <tr>
                        <td><strong>Academy Entry</strong></td>
                        <td><strong>150</strong></td>
                        <td><strong>7.5%</strong></td>
                        <td><strong>Systemic Attrition</strong></td>
                    </tr>
                </tbody>
            </table>
            <p style="font-weight: bold; font-size: 1.2rem; color: var(--bay-blue); margin-top: 20px;">Average Process Time: 10.2 Months</p>
        </div>
    </section>

    <section>
        <div class="container fade-in">
            <h2>The Cost of Inaction</h2>
            <div class="logic-grid">
                <div class="logic-card" style="border-top: 6px solid var(--danger-red);">
                    <h4 style="color: var(--danger-red); font-size: 1.4rem;">Financial Cost</h4>
                    <p>Mandatory overtime and increased turnover costs related to staffing vacancies.</p>
                </div>
                <div class="logic-card" style="border-top: 6px solid var(--danger-red);">
                    <h4 style="color: var(--danger-red); font-size: 1.4rem;">Operational Risk</h4>
                    <p>Degradation of institutional safety and staff burnout from prolonged staffing deficits.</p>
                </div>
            </div>
        </div>
    </section>

    <section style="background-color: var(--granite-gray);">
        <div class="container fade-in">
            <h2>Strategic Roadmap</h2>
            <ul class="roadmap-list">
                <li>
                    <span class="phase-badge">Phase 1</span>
                    <h3>Momentum Preservation</h3>
                    <p>Implementing the <strong>7-Day Pulse Rule</strong>. Eliminating "Dead Time" through automated status updates every week to maintain candidate engagement.</p>
                </li>
                <li>
                    <span class="phase-badge">Phase 2</span>
                    <h3>Parallel Architecture</h3>
                    <p>Transitioning from Serial to Parallel processing. Overlapping background audits and medical screenings with list finalization to compress cycles.</p>
                </li>
                <li>
                    <span class="phase-badge">Phase 3</span>
                    <h3>Unit Synchronization</h3>
                    <p>Integrating Recruitment and Background units into a unified "Workforce Flow" model to stabilize Academy throughput.</p>
                </li>
            </ul>
        </div>
    </section>

    <section style="background-color: var(--bay-blue); color: white;">
        <div class="container fade-in">
            <h1 style="color: var(--duckling-yellow); font-size: 4rem;">"A system is what it does."</h1>
            <p style="font-size: 1.8rem; margin-top: 20px; font-style: italic; opacity: 0.9;">To change the outcome, we must change the architecture.</p>
            
            <div style="margin-top: 80px; border-top: 1px solid rgba(255,255,255,0.3); padding-top: 40px;">
                <p style="font-weight: bold; font-size: 1.6rem;">Moses Zenon-Laguerre</p>
                <p>Massachusetts Department of Correction | Clark University MPA</p>
                <p>May 2026</p>
            </div>
        </div>
    </section>

    <footer>
        <p>Diagnosing and Modernizing Public-Safety Hiring | Senior Leadership Presentation</p>
    </footer>

    <script>
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("progress-bar").style.width = scrolled + "%";
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) entry.target.classList.add('visible');
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
    </script>
</body>
</html>

