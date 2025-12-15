<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AK | Portfolio</title>

  <!-- Google Font -->
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
      max-width: 1000px;
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
      display: block;
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
      height: 85vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      border-radius: 18px;
      background: linear-gradient(135deg, #3b82f6, #6366f1);
      color: white;
      margin-bottom: 60px;
    }

    header h1 { font-size: 4rem; font-weight: 700; }
    header p { font-size: 1.3rem; opacity: 0.9; }

    /* ===== SECTIONS ===== */
    section { margin-top: 60px; }

    h2 {
      font-size: 2rem;
      margin-bottom: 20px;
      border-left: 6px solid #3b82f6;
      padding-left: 12px;
    }

    .card {
      background: white;
      padding: 25px;
      border-radius: 18px;
      margin-bottom: 25px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.08);
      transition: 0.3s;
    }

    body.dark .card {
      background: #1e293b;
    }

    .card:hover {
      transform: translateY(-6px);
    }

    /* ===== BUTTONS ===== */
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
    .skill {
      margin-bottom: 18px;
    }

    .skill-bar {
      background: #e5e7eb;
      border-radius: 12px;
      overflow: hidden;
      height: 20px;
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
      margin: 80px 0 40px;
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
      <p>Assosiate Product Manager | Business Analyst | Business Growth</p>
    </header>

    <!-- EXPERIENCE -->
    <section>
      <h2>Experience</h2>
      <div class="card">
        <h3>Vedanta Resources — Business Analyst (CMO’s Office)</h3>
        <ul>
          <li>Increased CSAT by 23%</li>
          <li>Launched India’s first non-ferrous metal e-commerce platform</li>
          <li>Worked across Product, Marketing, Sales & Operations</li>
        </ul>
      </div>
    </section>

    <!-- PROJECTS -->
    <section>
      <h2>Projects</h2>
      <div class="card">
        <h3>Customer Experience Analytics</h3>
        <p>Optimized journey analytics & feedback loops.</p>
      </div>
      <div class="card">
        <h3>Product Launch Strategy</h3>
        <p>End-to-end GTM strategy for B2B e-commerce.</p>
      </div>
    </section>

    <!-- SKILLS -->
    <section>
      <h2>Skills</h2>
      <div class="card">
        <div class="skill">Product Analytics<div class="skill-bar"><span data-width="90%"></span></div></div>
        <div class="skill">Customer Experience<div class="skill-bar"><span data-width="85%"></span></div></div>
        <div class="skill">Marketing Strategy<div class="skill-bar"><span data-width="80%"></span></div></div>
        <div class="skill">Project Management<div class="skill-bar"><span data-width="75%"></span></div></div>
      </div>
    </section>

    <!-- CONTACT -->
    <section>
      <h2>Contact</h2>
      <div class="card">
        <p>Email: <a href="mailto:your@email.com">your@email.com</a></p>
        <p>LinkedIn: <a href="https://linkedin.com/in/yourprofile" target="_blank">linkedin.com/in/yourprofile</a></p>
      </div>
    </section>

    <footer>
      © 2025 AK — Crafted to Impress
    </footer>

  </div>

  <script>
    // Toggle Dark / Light
    const toggle = document.getElementById('theme-toggle');
    toggle.addEventListener('change', () => {
      document.body.classList.toggle('dark');
      document.body.classList.toggle('light');
    });

    // Animate skill bars
    window.addEventListener('load', () => {
      document.querySelectorAll('.skill-bar span').forEach(bar => {
        bar.style.width = bar.dataset.width;
      });
    });
  </script>

</body>
</html>


