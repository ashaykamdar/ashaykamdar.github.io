
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ashay Kamdar | Product Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">

<style>
*{margin:0;padding:0;box-sizing:border-box}
body{font-family:Inter,sans-serif;transition:.4s}
body.light{background:#f5f7fa;color:#111}
body.dark{background:#0f172a;color:#e5e7eb}
a{color:inherit;text-decoration:none}

nav{
  position:fixed;top:0;width:100%;
  background:rgba(255,255,255,.85);
  backdrop-filter:blur(10px);
  display:flex;justify-content:space-between;
  padding:16px 30px;z-index:999
}
body.dark nav{background:rgba(15,23,42,.9)}
nav a{margin-left:20px;font-weight:600}

.container{max-width:1100px;margin:auto;padding:120px 20px}

.theme-switch{position:fixed;top:18px;right:20px}
.theme-switch input{display:none}
.theme-switch label{
  width:56px;height:28px;background:#cbd5f5;
  display:block;border-radius:50px;cursor:pointer;
  position:relative
}
.theme-switch label::after{
  content:'☀';width:22px;height:22px;background:#fff;
  position:absolute;top:3px;left:3px;border-radius:50%;
  display:flex;align-items:center;justify-content:center;
  transition:.3s
}
.theme-switch input:checked+label{background:#3b82f6}
.theme-switch input:checked+label::after{
  transform:translateX(28px);content:'🌙'
}

header{
  display:grid;grid-template-columns:1.2fr .8fr;
  gap:40px;align-items:center;
  background:linear-gradient(135deg,#3b82f6,#6366f1);
  color:white;border-radius:22px;padding:60px
}
header img{
  width:240px;height:240px;border-radius:50%;
  object-fit:cover;border:6px solid rgba(255,255,255,.4)
}

h1{font-size:3.5rem}
h2{margin:70px 0 20px;border-left:6px solid #3b82f6;padding-left:12px}

.card{
  background:white;padding:28px;border-radius:18px;
  box-shadow:0 10px 25px rgba(0,0,0,.08);
  margin-bottom:25px
}
body.dark .card{background:#1e293b}

.icon{width:22px;height:22px;vertical-align:middle;margin-right:8px}

footer{text-align:center;margin:80px 0;opacity:.6}

@media(max-width:900px){
  header{grid-template-columns:1fr;text-align:center}
  header img{margin:auto}
}
</style>
</head>

<body class="light">

<!-- NAVIGATION -->
<nav>
  <strong>Ashay Kamdar</strong>
  <div>
    <a href="index.html">Home</a>
    <a href="case-studies.html">Case Studies</a>
    <a href="blogs.html">Blogs</a>
  </div>
</nav>

<!-- THEME SLIDER -->
<div class="theme-switch">
  <input type="checkbox" id="toggle">
  <label for="toggle"></label>
</div>

<div class="container">

<!-- HEADER -->
<header>
  <div>
    <h1>Ashay Kamdar</h1>
    <p>
      Product enthusiast with end-to-end experience building user-first B2C and
      enterprise products. Strong in problem discovery, execution, and translating
      complexity into impact.
    </p>
  </div>
  <img src="profile.jpg" alt="Profile Photo">
</header>

<!-- WORK EXPERIENCE -->
<h2>Work Experience</h2>

<div class="card">
  <h3>ASBL — Associate Product Manager Intern</h3>
  <p><em>Aug 2025 – Present</em></p>
  <ul>
    <li>Reduced task completion time by ~30% through UX & workflow redesign</li>
    <li>Improved operational efficiency by 40% by streamlining core workflows</li>
    <li>Owned end-to-end product delivery across web & mobile</li>
  </ul>
</div>

<div class="card">
  <h3>UPivot — Associate Product Manager Intern</h3>
  <p><em>May 2025 – Jul 2025</em></p>
  <ul>
    <li>Interviewed 50+ users and built personas & journey maps</li>
    <li>Improved engagement by 28% and onboarded 1,200+ users</li>
  </ul>
</div>

<div class="card">
  <h3>Vedanta Resources — Business Analyst</h3>
  <p><em>Aug 2023 – Feb 2025</em></p>
  <ul>
    <li>Drove 5% market share growth via market & competitive analysis</li>
    <li>Boosted profitability by 23% through automated arbitrage tracking</li>
    <li>Improved operational efficiency by 37%</li>
  </ul>
</div>

<!-- EDUCATION -->
<h2>Education</h2>

<div class="card">
  <p><strong>MBA</strong> — FLAME University (2023)</p>
  <p><strong>B.Tech (Computer Engineering)</strong> — CHARUSAT University (2021)</p>
</div>

<!-- CONTACT -->
<h2>Contact</h2>

<div class="card">
  <p>
    <svg class="icon" viewBox="0 0 24 24">
      <path fill="currentColor" d="M20 4H4a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2Zm0 4-8 5-8-5V6l8 5 8-5Z"/>
    </svg>
    <a href="mailto:ashaykamdar1812@gmail.com">ashaykamdar1812@gmail.com</a>
  </p>

  <p>
    <svg class="icon" viewBox="0 0 24 24">
      <path fill="currentColor" d="M4.98 3.5a2.5 2.5 0 1 0 0 5 2.5 2.5 0 0 0 0-5ZM3 8.98h3.96V21H3ZM9.5 8.98H13v1.64h.05c.49-.93 1.68-1.9 3.45-1.9 3.69 0 4.37 2.43 4.37 5.6V21h-3.97v-5.4c0-1.29-.03-2.95-1.8-2.95-1.8 0-2.08 1.4-2.08 2.85V21H9.5Z"/>
    </svg>
    <a href="https://linkedin.com/in/ashaykamdar" target="_blank">LinkedIn</a>
  </p>
</div>

<footer>© 2025 Ashay Kamdar</footer>
</div>

<script>
document.getElementById('toggle').addEventListener('change',()=>{
  document.body.classList.toggle('dark')
  document.body.classList.toggle('light')
})
</script>

</body>
</html>

