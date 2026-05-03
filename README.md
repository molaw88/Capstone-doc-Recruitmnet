<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Clark MPA Capstone | DOC Recruitment Modernization</title>

  <style>
    :root {
      --clark-scarlet: #A91024;
      --clark-black: #000000;
      --clark-white: #FFFFFF;
      --clark-light-gray: #FBFBFB;
      --clark-mid-gray: #E0E0E0;
      --text-dark: #1A1A1A;
      --text-muted: #666666;
      /* Sharper, more crisp shadows */
      --shadow: 0 10px 30px rgba(0,0,0,0.08);
      --soft-shadow: 0 4px 12px rgba(0,0,0,0.05);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      /* Switched to Times New Roman for academic gravity */
      font-family: "Times New Roman", Times, serif;
      line-height: 1.8;
      color: var(--text-dark);
      background: var(--clark-white);
      overflow-x: hidden;
      -webkit-font-smoothing: antialiased;
    }

    #progress-container {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 6px;
      background: var(--clark-mid-gray);
      z-index: 9999;
    }

    #progress-bar {
      height: 6px;
      width: 0%;
      background: var(--clark-scarlet);
      transition: width 0.1s ease;
    }

    nav {
      position: fixed;
      top: 6px;
      width: 100%;
      background: rgba(0,0,0,0.92);
      backdrop-filter: blur(10px);
      z-index: 999;
      padding: 16px 8%;
      display: flex;
      justify-content: center;
      gap: 24px;
      flex-wrap: wrap;
      border-bottom: 1px solid rgba(255,255,255,0.1);
    }

    nav a {
      color: var(--clark-white);
      text-decoration: none;
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 2px;
      font-weight: bold;
      opacity: 0.7;
      transition: 0.3s ease;
    }

    nav a:hover {
      opacity: 1;
      color: var(--clark-scarlet);
    }

    section {
      min-height: 100vh;
      padding: 140px 10%;
      display: flex;
      align-items: center;
      justify-content: center;
      border-bottom: 1px solid var(--clark-mid-gray);
      position: relative;
    }

    .container {
      width: 100%;
      max-width: 1120px;
      margin: 0 auto;
    }

    .center {
      text-align: center;
    }

    .eyebrow {
      text-transform: uppercase;
      letter-spacing: 5px;
      font-size: 0.9rem;
      font-weight: bold;
      color: var(--clark-scarlet);
      margin-bottom: 24px;
    }

    h1 {
      font-size: clamp(3rem, 7vw, 5.5rem);
      line-height: 1.05;
      letter-spacing: -1px;
      font-weight: normal; /* Times looks better at high weight without bolding */
      margin-bottom: 35px;
    }

    h2 {
      font-size: clamp(2.2rem, 4.5vw, 3.5rem);
      line-height: 1.1;
      letter-spacing: -0.5px;
      font-weight: normal;
      margin-bottom: 40px;
    }

    h3 {
      font-size: 1.8rem;
      line-height: 1.2;
      margin-bottom: 18px;
      font-weight: bold;
      color: var(--clark-scarlet);
    }

    p {
      font-size: 1.25rem;
      color: inherit;
    }

    .lead {
      font-size: clamp(1.3rem, 2vw, 1.6rem);
      max-width: 950px;
      margin: 0 auto;
      color: inherit;
      opacity: 0.9;
      line-height: 1.6;
    }

    .hero {
      background:
        linear-gradient(rgba(0,0,0,0.82), rgba(0,0,0,0.85)),
        radial-gradient(circle at top left, rgba(169,16,36,0.5), transparent 40%),
        var(--clark-black);
      color: var(--clark-white);
      text-align: center;
      border-bottom: 20px solid var(--clark-scarlet);
      padding-top: 180px;
    }

    .hero .subtitle {
      font-size: clamp(1.4rem, 2.6vw, 2.1rem);
      opacity: 0.85;
      max-width: 900px;
      margin: 0 auto 70px;
      font-style: italic;
    }

    .hero-card {
      margin: 80px auto 0;
      max-width: 850px;
      padding: 40px;
      border-top: 1px solid rgba(255,255,255,0.2);
      border-bottom: 1px solid rgba(255,255,255,0.1);
      color: var(--clark-white);
    }

    .hero-card p {
      font-size: 1.3rem;
      opacity: 0.9;
      margin-bottom: 10px;
    }

    .dark {
      background: var(--clark-black);
      color: var(--clark-white);
    }

    .scarlet {
      background: var(--clark-scarlet);
      color: var(--clark-white);
    }

    .light {
      background: var(--clark-light-gray);
    }

    .split {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 70px;
      align-items: center;
    }

    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 35px;
      margin-top: 55px;
    }

    .card {
      background: var(--clark-white);
      color: var(--text-dark);
      padding: 45px;
      border: 1px solid var(--clark-mid-gray);
      border-top: 8px solid var(--clark-scarlet);
      box-shadow: var(--soft-shadow);
      transition: all 0.4s cubic-bezier(0.165, 0.84, 0.44, 1);
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: var(--shadow);
      border-top-width: 12px;
    }

    .dark .card {
      background: #111111;
      color: var(--clark-white);
      border-color: #222;
    }

    .metric-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
      gap: 30px;
      margin-top: 60px;
    }

    .metric {
      background: var(--clark-black);
      color: var(--clark-white);
      padding: 45px 30px;
      text-align: center;
      border-bottom: 10px solid var(--clark-scarlet);
      box-shadow: var(--soft-shadow);
    }

    .metric-number {
      font-size: 3.8rem;
      font-weight: bold;
      line-height: 1;
      margin-bottom: 15px;
      color: var(--clark-white);
    }

    .metric-label {
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 2.5px;
      font-weight: bold;
      opacity: 0.8;
    }

    .quote {
      margin: 60px auto;
      max-width: 980px;
      padding: 55px;
      background: var(--clark-light-gray);
      border-left: 12px solid var(--clark-scarlet);
      box-shadow: var(--soft-shadow);
      font-family: "Times New Roman", Times, serif;
      font-size: clamp(1.5rem, 2.5vw, 2.4rem);
      line-height: 1.4;
      font-style: italic;
      font-weight: bold;
      color: var(--clark-black);
    }

    .scarlet .quote,
    .dark .quote {
      background: rgba(255,255,255,0.05);
      color: var(--clark-white);
      border-left-color: var(--clark-white);
    }

    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 60px;
      background: var(--clark-white);
      box-shadow: var(--shadow);
      overflow: hidden;
      border: 1px solid var(--clark-mid-gray);
    }

    th {
      background: var(--clark-black);
      color: var(--clark-white);
      padding: 24px;
      text-align: left;
      text-transform: uppercase;
      font-size: 0.8rem;
      letter-spacing: 2px;
    }

    td {
      padding: 24px;
      border-bottom: 1px solid var(--clark-mid-gray);
      font-size: 1.15rem;
      text-align: left;
    }

    tr:last-child td {
        border-bottom: none;
    }

    tr:nth-child(even) {
      background: var(--clark-light-gray);
    }

    .tag {
      display: inline-block;
      padding: 6px 16px;
      background: var(--clark-scarlet);
      color: var(--clark-white);
      border-radius: 4px; /* More professional than pills for this aesthetic */
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 1.5px;
      font-weight: bold;
      margin-bottom: 20px;
    }

    .timeline {
      margin-top: 60px;
      border-left: 4px solid var(--clark-scarlet);
      padding-left: 45px;
    }

    .timeline-item {
      margin-bottom: 55px;
      position: relative;
    }

    .timeline-item::before {
      content: "";
      position: absolute;
      left: -57px;
      top: 8px;
      width: 20px;
      height: 20px;
      background: var(--clark-scarlet);
      border-radius: 50%;
      border: 4px solid var(--clark-white);
      box-shadow: 0 0 0 2px var(--clark-scarlet);
    }

    .timeline-item h3 {
      color: var(--clark-scarlet);
    }

    .big-statement {
      font-size: clamp(2.5rem, 6vw, 5rem);
      line-height: 1.1;
      letter-spacing: -1.5px;
      font-weight: normal;
      max-width: 1050px;
      margin: 0 auto;
    }

    .footer {
      background: var(--clark-black);
      color: var(--clark-white);
      text-align: center;
      padding: 70px 8%;
      border-top: 12px solid var(--clark-scarlet);
    }

    .fade-in {
      opacity: 0;
      transform: translateY(40px);
      transition: all 1.2s cubic-bezier(0.22, 1, 0.36, 1);
    }

    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }

    @media (max-width: 850px) {
      nav {
        display: none;
      }

      section {
        padding: 100px 7%;
      }

      .split {
        grid-template-columns: 1fr;
        gap: 40px;
      }

      h1 {
        font-size: 2.8rem;
      }
    }
  </style>
</head>

<body>

  <div id="progress-container">
    <div id="progress-bar"></div>
  </div>

  <nav>
    <a href="#hero">Title</a>
    <a href="#intent">Intent</a>
    <a href="#challenge">Challenge</a>
    <a href="#methods">Methods</a>
    <a href="#yield">Evidence</a>
    <a href="#framework">Framework</a>
    <a href="#roadmap">Roadmap</a>
    <a href="#development">Growth</a>
    <a href="#discussion">Discussion</a>
  </nav>

  <section class="hero" id="hero">
    <div class="container fade-in">
      <div class="eyebrow">MPA 3999 Capstone Presentation</div>
      <h1>Diagnosing and Modernizing Public-Safety Hiring</h1>
      <p class="subtitle">
        A systems approach to recruitment velocity, candidate attrition, and workforce stability within the Massachusetts Department of Correction.
      </p>

      <div class="hero-card">
        <p><strong>Moses Zenon-Laguerre</strong></p>
        <p>Clark University | Master of Public Administration Candidate</p>
        <p>Massachusetts Department of Correction | Recruitment & Workforce Development</p>
        <p><em>Academic Year 2026</em></p>
      </div>
    </div>
  </section>

  <section id="intent">
    <div class="container fade-in center">
      <div class="eyebrow">Project Intent</div>
      <h2>From Candidate Interest to Workforce Stability</h2>
      <p class="lead">
        This capstone examines why correction officer candidates disengage before academy entry and proposes a modernization framework to improve recruitment yield, candidate velocity, and long-term staffing stability.
      </p>

      <div class="card-grid">
        <div class="card">
          <span class="tag">Problem</span>
          <h3>Recruitment is not only a supply issue.</h3>
          <p>The Department generates interest, but the system struggles to preserve candidate momentum across long administrative timelines.</p>
        </div>

        <div class="card">
          <span class="tag">Purpose</span>
          <h3>Diagnose the pipeline.</h3>
          <p>The project identifies where candidates slow down, disengage, or disappear between initial outreach and academy entry.</p>
        </div>

        <div class="card">
          <span class="tag">Stakeholders</span>
          <h3>Who benefits?</h3>
          <p>DOC leadership, recruitment staff, HR, civil service partners, facility operations, candidates, and the public safety system.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="scarlet">
    <div class="container fade-in center">
      <div class="eyebrow" style="color:white;">Central Finding</div>
      <div class="big-statement">
        The system loses momentum before it loses candidates.
      </div>
      <p class="lead" style="margin-top: 40px;">
        Attrition is not simply a matter of weak interest. It is produced by time, silence, fragmented ownership, and procedural latency.
      </p>
    </div>
  </section>

  <section id="challenge" class="light">
    <div class="container fade-in">
      <div class="split">
        <div>
          <div class="eyebrow">The Core Challenge</div>
          <h2>Compliance and Momentum Move at Different Speeds</h2>
          <p class="lead">
            The recruitment process is governed by two competing realities: the fast pace of modern candidate engagement and the slower pace of civil service hiring, screening, and institutional review.
          </p>
        </div>

        <div class="quote">
          Administrative latency acts as a hidden filter, removing candidates who still have interest but no longer have confidence in the process.
        </div>
      </div>

      <div class="card-grid">
        <div class="card">
          <h3>The Fast Loop</h3>
          <p>Outreach, digital intake, recruiter follow-up, candidate questions, and immediate engagement.</p>
          <p><strong>Candidate expectation:</strong> speed, clarity, and regular contact.</p>
        </div>

        <div class="card">
          <h3>The Slow Loop</h3>
          <p>Civil service exam cycles, eligible lists, certification, background, medical, psychological review, and academy scheduling.</p>
          <p><strong>Institutional reality:</strong> sequence, compliance, and delay.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="methods">
    <div class="container fade-in center">
      <div class="eyebrow">Methods and Outputs</div>
      <h2>How the Project Was Conducted</h2>
      <p class="lead">
        This project used an applied systems case study approach, combining recruitment pipeline analysis, operational observation, database review, and public administration theory.
      </p>

      <div class="card-grid">
        <div class="card">
          <span class="tag">Method 01</span>
          <h3>Applied Case Study</h3>
          <p>Focused on the DOC recruitment-to-academy pipeline, using RTC 339 as the primary diagnostic cohort.</p>
        </div>

        <div class="card">
          <span class="tag">Method 02</span>
          <h3>Pipeline Analysis</h3>
          <p>Tracked candidate movement from initial interest through exam registration, eligible list placement, screening, and academy entry.</p>
        </div>

        <div class="card">
          <span class="tag">Method 03</span>
          <h3>Systems Diagnosis</h3>
          <p>Identified friction points, dead time, candidate velocity loss, and conversion breakdowns across multiple ownership stages.</p>
        </div>

        <div class="card">
          <span class="tag">Output</span>
          <h3>Modernization Framework</h3>
          <p>Produced a Dual-Loop Recruitment Framework and a phased roadmap for reducing attrition and improving candidate flow.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="yield" class="light">
    <div class="container fade-in center">
      <div class="eyebrow">The Evidence</div>
      <h2>RTC 339 Yield Forensic</h2>
      <p class="lead">
        The pipeline shows that the Department does not merely need more candidates. It needs a better system for sustaining the candidates it already reaches.
      </p>

      <div class="metric-grid">
        <div class="metric">
          <div class="metric-number">2,000</div>
          <div class="metric-label">Initial Leads</div>
        </div>

        <div class="metric">
          <div class="metric-number">800</div>
          <div class="metric-label">Exam Registered</div>
        </div>

        <div class="metric">
          <div class="metric-number">600</div>
          <div class="metric-label">Eligible Roster</div>
        </div>

        <div class="metric">
          <div class="metric-number">150</div>
          <div class="metric-label">Academy Entry</div>
        </div>
      </div>

      <table>
        <thead>
          <tr>
            <th>Hiring Milestone</th>
            <th>Candidate Volume</th>
            <th>Yield</th>
            <th>Interpretation</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Initial Interest</td>
            <td>2,000</td>
            <td>100%</td>
            <td>Outreach generates attention and initial engagement.</td>
          </tr>
          <tr>
            <td>Exam Registered</td>
            <td>800</td>
            <td>40%</td>
            <td>First major friction point: conversion from interest to formal civil service action.</td>
          </tr>
          <tr>
            <td>Eligible Roster</td>
            <td>600</td>
            <td>30%</td>
            <td>Administrative waiting periods begin weakening candidate momentum.</td>
          </tr>
          <tr>
            <td><strong>Academy Entry</strong></td>
            <td><strong>150</strong></td>
            <td><strong>7.5%</strong></td>
            <td><strong>Velocity breakdown between eligibility, screening, and final appointment.</strong></td>
          </tr>
        </tbody>
      </table>

      <p style="font-size:1.6rem; font-weight:bold; color:var(--clark-scarlet); margin-top:45px;">
        The central problem is not candidate attraction alone. It is candidate preservation.
      </p>
    </div>
  </section>

  <section id="framework" class="dark">
    <div class="container fade-in center">
      <div class="eyebrow">Original Framework</div>
      <h2>The Dual-Loop Recruitment Framework</h2>
      <p class="lead">
        The DOC recruitment system is not one pipeline. It is two systems moving at different speeds, with candidates caught between them.
      </p>

      <div class="card-grid">
        <div class="card">
          <span class="tag">Fast Loop</span>
          <h3>Recruitment Engagement</h3>
          <p>Lead generation, job fairs, digital intake, recruiter contact, candidate education, and exam reminders.</p>
          <p><strong>Key risk:</strong> candidate excitement decays when communication stops.</p>
        </div>

        <div class="card">
          <span class="tag">Slow Loop</span>
          <h3>Civil Service and Screening</h3>
          <p>Exam cycles, list certification, ranked selection, background, medical, psychological, and final academy readiness.</p>
          <p><strong>Key risk:</strong> legal and procedural timelines overpower recruitment momentum.</p>
        </div>

        <div class="card">
          <span class="tag">Failure Point</span>
          <h3>Dead Time</h3>
          <p>Periods where candidates remain technically active but psychologically disengage because nothing appears to be happening.</p>
        </div>

        <div class="card">
          <span class="tag">Modernization Target</span>
          <h3>Candidate Velocity</h3>
          <p>The speed at which candidates move from interest to action, from action to eligibility, and from eligibility to appointment.</p>
        </div>
      </div>

      <div class="quote">
        Recruitment does not fail at the point of interest. It fails in the space between interest and institutional action.
      </div>
    </div>
  </section>

  <section>
    <div class="container fade-in">
      <div class="eyebrow">Diagnosis</div>
      <h2>Three Patterns Explain the Attrition</h2>

      <div class="timeline">
        <div class="timeline-item">
          <h3>1. Friction Points</h3>
          <p>Administrative steps that slow candidates down, create confusion, or require action without enough guidance.</p>
        </div>

        <div class="timeline-item">
          <h3>2. Velocity Deficit</h3>
          <p>The loss of candidate momentum caused by long intervals between outreach, exam movement, list certification, screening, and academy scheduling.</p>
        </div>

        <div class="timeline-item">
          <h3>3. Psychological Attrition</h3>
          <p>Candidates do not always leave because they are disqualified. Many leave because silence teaches them to move on.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="roadmap" class="light">
    <div class="container fade-in center">
      <div class="eyebrow">Recommendations</div>
      <h2>Modernization Roadmap</h2>
      <p class="lead">
        The goal is not to remove compliance. The goal is to build a recruitment operating system that preserves momentum inside a compliance-heavy environment.
      </p>

      <div class="card-grid">
        <div class="card">
          <span class="tag">0–3 Months</span>
          <h3>The 7-Day Pulse Rule</h3>
          <p>Replace dead time with recurring candidate contact, automated reminders, list-status updates, and recruiter touchpoints.</p>
        </div>

        <div class="card">
          <span class="tag">3–12 Months</span>
          <h3>Candidate Velocity Dashboard</h3>
          <p>Track days since last contact, candidate stage, touch count, ghosting risk, screening status, and academy readiness.</p>
        </div>

        <div class="card">
          <span class="tag">1–3 Years</span>
          <h3>Parallel Gate Architecture</h3>
          <p>Move from strictly sequential processing toward earlier preparation, simultaneous readiness checks, and tighter handoffs.</p>
        </div>

        <div class="card">
          <span class="tag">Long-Term</span>
          <h3>Workforce Flow Model</h3>
          <p>Integrate recruitment, HR, background, civil service timelines, and academy planning around throughput instead of siloed compliance.</p>
        </div>
      </div>
    </div>
  </section>

  <section class="scarlet">
    <div class="container fade-in center">
      <div class="eyebrow" style="color:white;">Strategic Recommendation</div>
      <div class="big-statement">
        Treat every eligible list as a decaying asset.
      </div>
      <p class="lead" style="margin-top:40px;">
        Once a candidate becomes reachable, the clock is already running. The Department must manage that list with urgency, rhythm, and ownership.
      </p>
    </div>
  </section>

  <section>
    <div class="container fade-in center">
      <div class="eyebrow">Final Deliverable</div>
      <h2>What This Capstone Produces</h2>

      <div class="card-grid">
        <div class="card">
          <h3>Diagnostic Framework</h3>
          <p>A clear way to explain why recruitment systems lose candidates even when initial interest exists.</p>
        </div>

        <div class="card">
          <h3>Operational Language</h3>
          <p>Terms such as dead time, velocity deficit, friction points, and psychological attrition give leadership a vocabulary for action.</p>
        </div>

        <div class="card">
          <h3>Modernization Plan</h3>
          <p>A phased roadmap for improving outreach, tracking, communication, list activation, screening flow, and academy readiness.</p>
        </div>
      </div>

      <div class="quote">
        The Department does not need to choose between fairness and speed. It needs a system where fairness does not unintentionally destroy momentum.
      </div>
    </div>
  </section>

  <section id="development" class="light">
    <div class="container fade-in center">
      <div class="eyebrow">Professional Development</div>
      <h2>What I Developed Through the Capstone</h2>

      <div class="card-grid">
        <div class="card">
          <h3>Systems Thinking</h3>
          <p>I learned to diagnose recruitment not as a single staffing issue, but as a flow, time, and design problem.</p>
        </div>

        <div class="card">
          <h3>Executive Communication</h3>
          <p>I strengthened my ability to translate operational data into leadership-ready insights, dashboards, and recommendations.</p>
        </div>

        <div class="card">
          <h3>Public Administration Judgment</h3>
          <p>I learned to balance modernization with civil service law, procedural fairness, public accountability, and institutional constraints.</p>
        </div>

        <div class="card">
          <h3>Strategic Leadership</h3>
          <p>I developed a stronger ability to impose structure on ambiguity and move from observation to actionable design.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="discussion" class="dark">
    <div class="container fade-in center">
      <div class="eyebrow">Conclusion</div>
      <h2>A System Is What It Does</h2>
      <p class="lead">
        If the current hiring system produces delay, silence, and candidate loss, then modernization must focus on architecture, not effort alone.
      </p>

      <div class="quote">
        To change the outcome, we must change the design.
      </div>

      <div style="margin-top: 80px;">
        <h3 style="font-size:2.5rem; color:var(--clark-scarlet);">Thank You</h3>
        <p style="font-size:1.35rem; margin-top:15px;">Questions and Discussion</p>
        <p style="margin-top:45px; opacity:0.8; font-size:1.1rem;">
          Moses Zenon-Laguerre | Clark University MPA Candidate | Massachusetts Department of Correction
        </p>
      </div>
    </div>
  </section>

  <footer class="footer">
    <p><strong>Strategic Recruitment Modernization</strong></p>
    <p>Clark University | MPA 3999 Capstone Presentation | 2026</p>
    <p style="font-size:0.9rem; opacity:0.7; margin-top:15px;">
      Data and analysis developed from DOC recruitment pipeline review, RTC 339 case analysis, and applied public administration research.
    </p>
  </footer>

  <script>
    window.addEventListener("scroll", function () {
      const winScroll = document.body.scrollTop || document.documentElement.scrollTop;
      const height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
      const scrolled = (winScroll / height) * 100;
      document.getElementById("progress-bar").style.width = scrolled + "%";
    });

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("visible");
        }
      });
    }, { threshold: 0.15 });

    document.querySelectorAll(".fade-in").forEach(el => observer.observe(el));
  </script>

</body>
</html>
