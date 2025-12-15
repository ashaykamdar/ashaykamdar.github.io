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
