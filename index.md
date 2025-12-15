
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AK | Portfolio</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* Global Styles */
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Inter', sans-serif;
      background: #f5f7fa;
      color: #1a1a1a;
      line-height: 1.6;
    }
    a { color: #3b82f6; text-decoration: none; }
    a:hover { text-decoration: underline; }

    /* Container */
    .container {
      max-width: 900px;
      margin: 50px auto;
      padding: 0 20px;
    }

    /* Header */
    header {
      text-align: center;
      margin-bottom: 50px;
    }
    header h1 { font-size: 3rem; font-weight: 700; margin-bottom: 10px; }
    header p { font-size: 1.2rem; color: #555; }

    /* Section Titles */
    h2 {
      font-size: 2rem;
      margin-bottom: 15px;
      border-left: 5px solid #3b82f6;
      padding-left: 10px;
      margin-top: 40px;
    }

    /* Cards */
    .card {
      background: #fff;
      padding: 20px;
      border-radius: 12px;
      margin-bottom: 20px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.05);
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 12px 30px rgba(0,0,0,0.1);
    }

    /* Buttons */
    .btn {
      display: inline-block;
      margin-top: 10px;
      background: #3b82f6;
      color: #fff;
      padding: 12px 25px;
      border-radius: 8px;
      font-weight: 600;
      transition: background 0.3s;
    }
    .btn:hover { background: #2563eb; }

    /* Footer */
    footer {
      text-align: center;
      margin-top: 60px;
      color: #777;
    }

    /* Responsive */
    @media (max-width: 600px) {
      header h1 { font-size: 2.2rem; }
      h2 { font-size: 1.6rem; }
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Header -->
    <header>
      <h1>AK</h1>
      <p>Business Analyst | Product | Growth</p>
    </header>

    <!-- Experience Section -->
    <section>
      <h2>Experience</h2>
      <div class="card">
        <h3>Vedanta Resources – Business Analyst (CMO's Office)</h3>
        <ul>
          <li>Improved CSAT score by 23%</li>
          <li>Launched India’s first e-commerce platform for non-ferrous metals</li>
          <li>Worked across Product, Marketing, Sales, and Operations</li>
        </ul>
      </div>
    </section>

    <!-- Projects Section -->
    <section>
      <h2>Projects</h2>
      <div class="card">
        <h3>Customer Experience Analytics</h3>
        <p>Analyzed customer journey & implemented feedback loops to increase satisfaction.</p>
      </div>
      <div class="card">
        <h3>Product Launch Strategy</h3>
        <p>Developed go-to-market strategy for non-ferrous metal e-commerce platform.</p>
      </div>
    </section>

    <!-- Documents Section -->
    <section>
      <h2>Documents</h2>
      <div class="card">
        <a href="resume.pdf" class="btn" download>⬇ Download Resume</a>
      </div>
      <div class="card">
        <a href="work.pdf" class="btn" download>⬇ Download Work Samples</a>
      </div>
    </section>

    <!-- Contact Section -->
    <section>
      <h2>Contact</h2>
      <div class="card">
        <p>Email: <a href="mailto:your@email.com">your@email.com</a></p>
        <p>LinkedIn: <a href="https://linkedin.com/in/yourprofile" target="_blank">linkedin.com/in/yourprofile</a></p>
      </div>
    </section>

    <footer>
      &copy; 2025 AK | All Rights Reserved
    </footer>
  </div>
</body>
</html>


