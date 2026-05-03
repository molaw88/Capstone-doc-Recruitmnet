<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DOC Recruitment: Systemic Modernization</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css" rel="stylesheet">
    <style>
        :root {
            --bg-dark: #0B1F3B;
            --accent-orange: #FF8C42;
            --accent-green: #4CAF50;
            --text-light: #F4F4F4;
            --gray: #888;
        }

        body {
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: var(--bg-dark);
            color: var(--text-light);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        section {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 50px 20px;
            box-sizing: border-box;
            position: relative;
        }

        .container {
            max-width: 1000px;
            width: 100%;
        }

        /* Typography */
        h1 { font-size: 4rem; margin-bottom: 1rem; letter-spacing: -1px; }
        h2 { font-size: 2.5rem; color: var(--accent-orange); }
        p { font-size: 1.5rem; line-height: 1.6; color: #ccc; }
        .highlight { color: var(--accent-orange); font-weight: bold; }

        /* Data Visualization Components */
        .funnel-container {
            width: 100%;
            max-width: 600px;
            margin: 40px auto;
        }

        .funnel-stage {
            background: rgba(255,255,255,0.1);
            margin: 10px 0;
            padding: 20px;
            border-left: 5px solid var(--accent-orange);
            transition: all 0.5s ease;
        }

        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }

        .stat-card {
            background: rgba(255,255,255,0.05);
            padding: 30px;
            border-radius: 10px;
            border-bottom: 4px solid var(--accent-green);
        }

        .stat-number { font-size: 3.5rem; font-weight: 800; display: block; }

        /* Scroll Effects */
        .reveal { opacity: 0; transform: translateY(30px); transition: all 0.8s ease-out; }
        .reveal.active { opacity: 1; transform: translateY(0); }

        footer {
            padding: 40px;
            text-align: center;
            font-size: 0.9rem;
            color: var(--gray);
            border-top: 1px solid rgba(255,255,255,0.1);
        }
    </style>
</head>
<body>

    <section>
        <div class="container animate__animated animate__fadeIn">
            <h1>The <span class="highlight">Velocity</span> Deficit</h1>
            <p>Diagnosing and Modernizing the Public-Safety Hiring Process.</p>
            <div style="margin-top: 30px; color: var(--accent-green);">↓ Scroll to Audit the System</div>
        </div>
    </section>

    <section>
        <div class="container reveal">
            <h2>01. The Yield Gap</h2>
            <p>We start with <strong>2,000</strong> candidates. We end with <strong>150</strong>. This is not a supply issue—it is a leak in the system.</p>
            
            <div class="funnel-container">
                <div class="funnel-stage" style="width: 100%;">Database: 2,000</div>
                <div class="funnel-stage" style="width: 40%;">Exam Registered: 800</div>
                <div class="funnel-stage" style="width: 30%;">Eligible Roster: 600</div>
                <div class="funnel-stage" style="width: 7.5%; border-left-color: var(--accent-green);">Academy: 150</div>
            </div>
            <p style="font-size: 1.1rem; color: var(--gray);">*Data reflects Cohort 339 analysis.</p>
        </div>
    </section>

    <section style="background: #0d2545;">
        <div class="container reveal">
            <h2>02. The "Dead Time" Metric</h2>
            <p>Latency is the silent killer of candidate momentum. Between registration and examination, the "Slow Loop" creates a vacuum.</p>
            
            <div class="stats-grid">
                <div class="stat-card">
                    <span class="stat-number">90</span>
                    <span>Days of Systemic Silence</span>
                </div>
                <div class="stat-card">
                    <span class="stat-number">24%</span>
                    <span>Exposed to Max Latency</span>
                </div>
                <div class="stat-card">
                    <span class="stat-number">10.2</span>
                    <span>Avg. Months to Process</span>
                </div>
            </div>
        </div>
    </section>

    <section>
        <div class="container reveal">
            <h2>03. The Strategic Shift</h2>
            <p>Moving from <strong>Reactive Hiring</strong> to an <strong>Engineered Workforce Flow</strong>.</p>
            
            <div class="stats-grid">
                <div class="stat-card" style="border-bottom-color: var(--accent-orange);">
                    <h3>The Fast Loop</h3>
                    <p style="font-size: 1rem;">Aggressive engagement, digital intake (Formstack), and 7-day touchpoints.</p>
                </div>
                <div class="stat-card" style="border-bottom-color: var(--accent-orange);">
                    <h3>The Slow Loop</h3>
                    <p style="font-size: 1rem;">Administrative milestones and background checks optimized for velocity.</p>
                </div>
            </div>
        </div>
    </section>

    <section>
        <div class="container reveal text-center">
            <h1>Ready for <span style="color: var(--accent-green);">Stability</span>.</h1>
            <p>This framework identifies redundant friction points to ensure the DOC becomes the employer of choice in a competitive market.</p>
        </div>
    </section>

    <footer>
        <p>Master of Public Administration Capstone | Systems Approach to Workforce Stability</p>
    </footer>

    <script>
        // Simple Scroll Reveal Logic
        const observerOptions = { threshold: 0.2 };
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.reveal').forEach(el => observer.observe(el));
    </script>
</body>
</html>
