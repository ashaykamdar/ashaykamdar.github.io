<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ashay Kamdar | Product Portfolio</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Inter', sans-serif;
      line-height: 1.6;
      transition: background 0.5s, color 0.5s;
    }

    body.light { background: #f5f7fa; color: #111; }
    body.dark { background: #0f172a; color: #e5e7eb; }

    a { color: inherit; text-decoration: none; }
    a:hover { text-decoration: underline; }

    .container {
      max-width: 1050px;
      margin: auto;
      padding: 20px;
    }

    /* ===== THEME SLIDER ===== */
    .theme-switch {
      position: fixed;
      top: 20px;
      right: 20px;
      z-index: 1000;
    }

    .theme-switch input { display: none; }

    .theme-switch label {
      width: 60px;
      height: 30px;
      background: #cbd5f5;
      border-radius: 50px;
      cursor: pointer;
      position: relative;
      transition: background 0.3s;
    }

    .theme-switch label::after {
      content: '☀';
      width: 24px;
      height: 24px;
      background: white;
      position: absolute;
      top: 3px;
      left: 3px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 14px;
      transition: 0.3s;
    }

    .theme-switch input:checked + label {
      background: #3b82f6;
    }

    .theme-switch input:checked + label::after {
      transform: translateX(30px);
      content: '🌙';
    }

    /* ===== HEADER ===== */
    header {
      height: 90vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      border-radius: 18px;
      background: linear-gradient(135deg, #3b82f6, #6366f1);
      color: white;
      margin-bottom: 70px;
      padding: 20px;
    }

    header h1 { font-size: 4rem; font-weight: 700; }
    header p { font-size: 1.3rem; opacity: 0.95; max-width: 700px; }

    section { margin-top: 70px; }

    h2 {
      font-size: 2rem;
      margin-bottom: 25px;
      border-left: 6px solid #3b82f6;
      padding-left: 12px;
    }

    .card {
      background: white;
      padding: 28px;
      border-radius: 18px;
      margin-bottom: 28px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.08);
      transition: 0.3s;
    }

    body.dark .card { background: #1e293b; }

    .card:hover { transform: translateY(-6px); }

    .btn {
      display: inline-block;
      background: #3b82f6;
      color: white;
      padding: 12px 28px;
      border-radius: 12px;
      font-weight: 600;
      transition: 0.3s;
    }

    .btn:hover { background: #2563eb; }

    /* ===== SKILLS ===== */
    .skill { margin-bottom: 18px; }

    .skill-bar {
      background: #e5e7eb;
      border-radius: 12px;
      overflow: hidden;
      height: 20px;
      margin-top: 6px;
    }

    .skill-bar span {
      display: block;
      height: 100%;
      width: 0;
      background: #3b82f6;
      border-radius: 12px;
      transition: width 2s;
    }

    /* ===== FLOATING RESUME ===== */
    .floating-btn {
      position: fixed;
      bottom: 30px;
      right: 30px;
      background: #3b82f6;
      color: white;
      padding: 16px 22px;
      border-radius: 16px;
      font-weight: 600;
      box-shadow: 0 12px 30px rgba(0,0,0,0.25);
      z-index: 1000;
    }

    footer {
      text-align: center;
      margin: 90px 0 40px;
      opacity: 0.6;
    }

    @media(max-width: 768px) {
      header h1 { font-size: 3rem; }
    }
  </style>
</head>

<body class="light">

  <!-- THEME SLIDER -->
  <div class="theme-switch">
    <input type="checkbox" id="theme-toggle">
    <label for="theme-toggle"></label>
  </div>

  <!-- FLOATING RESUME -->
  <a href="resume.pdf" download class="floating-btn">⬇ Resume</a>

  <div class="container">

    <!-- HEADER -->
    <header>
      <h1>Ashay Kamdar</h1>
      <p>
        Product enthusiast with hands-on experience shipping user-first B2C and enterprise products.
        Thrive in ambiguity with a bias for execution, problem-first thinking, and strong ownership.
      </p>
    </header>

    <!-- EXPERIENCE -->
    <section>
      <h2>Work Experience</h2>

      <div class="card">
        <h3>ASBL — Associate Product Manager Intern</h3>
        <p><em>Aug 2025 – Present | Hyderabad</em></p>
        <ul>
          <li>Led UX & workflow redesigns reducing task completion time by ~30%</li>
          <li>Streamlined planning, scheduling, contracts & manpower workflows, cutting manual effort by 40%</li>
          <li>Owned end-to-end product lifecycle across web & mobile, reducing rework by 35%</li>
          <li>Improved release quality & system stability, reducing recurring issues by ~40%</li>
        </ul>
      </div>

      <div class="card">
        <h3>UPivot — Associate Product Manager Intern</h3>
        <p><em>May 2025 – Jul 2025 | Bengaluru</em></p>
        <ul>
          <li>Conducted 50+ user interviews and built personas & journey maps</li>
          <li>Defined MVP scope, wrote PRDs, launched AI resume screening & feedback tools</li>
          <li>A/B tested features reducing drop-offs by 25% and improving clarity</li>
          <li>Improved engagement by 28% and onboarded 1,200+ users</li>
        </ul>
      </div>

      <div class="card">
        <h3>Vedanta Resources — Business Analyst (Marketing)</h3>
        <p><em>Aug 2023 – Feb 2025 | Mumbai</em></p>
        <ul>
          <li>Analyzed large-scale sales data using SQL & Excel to drive growth</li>
          <li>Drove 5% market share increase via market & competitive analysis</li>
          <li>Automated MCX–LME arbitrage tracking, boosting profitability by 23%</li>
          <li>Built BI dashboards & executive presentations for CXOs and investors</li>
          <li>Automated pricing & order workflows, improving efficiency by 37%</li>
        </ul>
      </div>
    </section>

    <!-- ACHIEVEMENTS -->
    <section>
      <h2>Key Achievements</h2>
      <div class="card">
        <ul>
          <li>🚀 Reduced task completion time by 30% through UX redesigns</li>
          <li>📈 Improved product engagement by 28% and onboarded 1,200+ users</li>
          <li>💰 Increased profitability by 23% via automated arbitrage analysis</li>
          <li>📊 Delivered 5% market share growth through competitive insights</li>
          <li>⚙️ Improved operational efficiency by 37–40% across teams</li>
        </ul>
      </div>
    </section>

    <!-- EDUCATION -->
    <section>
      <h2>Education</h2>
      <div class="card">
        <p><strong>MBA</strong> — FLAME University (2023)</p>
        <p><strong>B.Tech (Computer Engineering)</strong> — CHARUSAT University (2021)</p>
      </div>
    </section>

    <!-- SKILLS -->
    <section>
      <h2>Skills</h2>
      <div class="card">
        <div class="skill">Product Management<div class="skill-bar"><span data-width="90%"></span></div></div>
        <div class="skill">User Research & Analytics<div class="skill-bar"><span data-width="85%"></span></div></div>
        <div class="skill">SQL · BI · Data Visualization<div class="skill-bar"><span data-width="80%"></span></div></div>
        <div class="skill">Stakeholder Management<div class="skill-bar"><span data-width="75%"></span></div></div>
      </div>
    </section>

    <!-- CONTACT -->
    <section>
      <h2>Contact</h2>
      <div class="card">
        <p>Email: <a href="mailto:ashaykamdar1812@gmail.com">ashaykamdar1812@gmail.com</a></p>
        <p>LinkedIn: <a href="https://www.linkedin.com/in/ashaykamdar" target="_blank">linkedin.com/in/ashaykamdar</a></p>
      </div>
    </section>

    <footer>
      © 2025 Ashay Kamdar · Built to stand out
    </footer>

  </div>

  <script>
    const toggle = document.getElementById('theme-toggle');
    toggle.addEventListener('change', () => {
      document.body.classList.toggle('dark');
      document.body.classList.toggle('light');
    });

    window.addEventListener('load', () => {
      document.querySelectorAll('.skill-bar span').forEach(bar => {
        bar.style.width = bar.dataset.width;
      });
    });
  </script>

</body>
</html>
