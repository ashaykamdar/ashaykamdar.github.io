
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AK | Portfolio</title>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* Global Styles */
    *{margin:0;padding:0;box-sizing:border-box;}
    body{font-family:'Inter',sans-serif;line-height:1.6;transition:background 0.5s,color 0.5s;}
    a{color:inherit;text-decoration:none;}
    a:hover{text-decoration:underline;}
    .container{max-width:1000px;margin:0 auto;padding:20px;}
    
    /* Dark/Light Mode */
    body.light{background:#f5f7fa;color:#1a1a1a;}
    body.dark{background:#121212;color:#f5f5f5;}
    
    /* Toggle Button */
    .toggle-btn{position:fixed;top:20px;right:20px;background:#3b82f6;color:white;padding:10px 15px;border-radius:10px;cursor:pointer;z-index:1000;transition:background 0.3s;}
    .toggle-btn:hover{background:#2563eb;}

    /* Header */
    header{height:80vh;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;color:white;border-radius:15px;background:linear-gradient(135deg,#3b82f6,#6366f1);transition:background 1s;}
    header h1{font-size:4rem;font-weight:700;margin-bottom:10px;}
    header p{font-size:1.3rem;opacity:0.9;}
    
    /* Section Titles */
    h2{font-size:2rem;border-left:6px solid #3b82f6;padding-left:12px;margin-bottom:20px;margin-top:60px;}

    /* Card */
    .card{background:white;border-radius:15px;padding:25px;margin-bottom:25px;box-shadow:0 8px 20px rgba(0,0,0,0.05);transition:0.3s;}
    body.dark .card{background:#1e1e1e;box-shadow:0 8px 20px rgba(0,0,0,0.2);}
    .card:hover{transform:translateY(-5px);box-shadow:0 12px 30px rgba(0,0,0,0.1);}
    
    /* Buttons */
    .btn{display:inline-block;padding:12px 25px;background:#3b82f6;color:white;border-radius:10px;font-weight:600;margin-top:10px;transition:0.3s;}
    .btn:hover{background:#2563eb;}

    /* Skills */
    .skill-bar{background:#e0e0e0;border-radius:10px;overflow:hidden;margin-bottom:15px;}
    .skill-bar span{display:block;height:20px;width:0%;background:#3b82f6;transition:width 2s;border-radius:10px;}

    /* Fade-in animation */
    .fade-in{opacity:0;transform:translateY(20px);animation:fadeInUp 0.8s forwards;}
    @keyframes fadeInUp{to{opacity:1;transform:translateY(0);}}

    /* Floating Download Button */
    .floating-btn{position:fixed;bottom:30px;right:30px;background:#3b82f6;color:white;padding:15px 20px;border-radius:15px;font-weight:600;box-shadow:0 8px 20px rgba(0,0,0,0.2);transition:0.3s;z-index:1000;}
    .floating-btn:hover{background:#2563eb;}

    /* Footer */
    footer{text-align:center;margin-top:80px;color:#777;}
    
    /* Responsive */
    @media(max-width:768px){header h1{font-size:3rem;}h2{font-size:1.6rem;}}
  </style>
</head>
<body class="light">
  <!-- Dark/Light Toggle -->
  <div class="toggle-btn" onclick="toggleMode()">Toggle Dark/Light</div>

  <!-- Floating Resume Button -->
  <a href="resume.pdf" download class="floating-btn">⬇ Resume</a>

  <div class="container">
    <!-- Header -->
    <header class="fade-in">
      <h1>AK</h1>
      <p>Business Analyst | Product | Growth</p>
    </header>

    <!-- Experience -->
    <section class="fade-in">
      <h2>Experience</h2>
      <div class="card">
        <h3>Vedanta Resources – Business Analyst (CMO's Office)</h3>
        <ul>
          <li>Improved CSAT score by 23%</li>
          <li>Launched India’s first non-ferrous metal e-commerce platform</li>
          <li>Worked across Product, Marketing, Sales, and Operations</li>
        </ul>
      </div>
    </section>

    <!-- Projects -->
    <section class="fade-in">
      <h2>Projects</h2>
      <div class="card">
        <h3>Customer Experience Analytics</h3>
        <p>Analyzed customer journey & implemented feedback loops to increase satisfaction.</p>
      </div>
      <div class="card">
        <h3>Product Launch Strategy</h3>
        <p>Developed go-to-market strategy for the non-ferrous metal e-commerce platform.</p>
      </div>
    </section>

    <!-- Skills -->
    <section class="fade-in">
      <h2>Skills</h2>
      <div class="card">
        <p>Product Analytics</p>
        <div class="skill-bar"><span data-width="90%"></span></div>
        <p>Customer Experience</p>
        <div class="skill-bar"><span data-width="85%"></span></div>
        <p>Marketing Strategy</p>
        <div class="skill-bar"><span data-width="80%"></span></div>
        <p>Project Management</p>
        <div class="skill-bar"><span data-width="75%"></span></div>
      </div>
    </section>

    <!-- Documents -->
    <section class="fade-in">
      <h2>Documents</h2>
      <div class="card">
        <a href="resume.pdf" download class="btn">⬇ Download Resume</a>
      </div>
      <div class="card">
        <a href="work.pdf" download class="btn">⬇ Download Work Samples</a>
      </div>
    </section>

    <!-- Contact -->
    <section class="fade-in">
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

  <script>
    // Fade-in on scroll
    const faders = document.querySelectorAll('.fade-in');
    const appearOptions = { threshold:0.2 };
    const appearOnScroll = new IntersectionObserver((entries, observer) => {
      entries.forEach(entry => { if(entry.isIntersecting){ entry.target.style.animation='fadeInUp 0.8s forwards'; observer.unobserve(entry.target); } });
    }, appearOptions);
    faders.forEach(fader => appearOnScroll.observe(fader));

    // Skill bar animation
    window.addEventListener('load', () => {
      const bars = document.querySelectorAll('.skill-bar span');
      bars.forEach(bar => {
        bar.style.width = bar.getAttribute('data-width');
      });
    });

    // Dark/Light Mode Toggle
    function toggleMode() {
      document.body.classList.toggle('dark');
      document.body.classList.toggle('light');
    }
  </script>
</body>
</html>

