 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>UnifyED - Empowering Education & Development</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; }
    body { font-family:'Roboto',sans-serif; background:#f9f9f9; color:#2c3e50; }
    a { text-decoration:none; color:inherit; }
    section { padding:60px 0; }
    .container { width:90%; max-width:1200px; margin:0 auto; }
    header { background:#2c3e50; padding:20px 0; }
    .navbar { display:flex; justify-content:space-between; align-items:center; flex-wrap:wrap; }
    .logo { font-size:2em; font-weight:bold; color:#fff; }
    .tagline { color: #fff; font-size: 0.9em; margin-top: 4px; }
    nav a { margin-left:1.5em; color:#fff; font-size:1em; transition:color .2s; }
    nav a:hover { color:#ddd; }
    .hero { background:linear-gradient(135deg,#3498db,#9b59b6); color:#fff; text-align:center; padding:40px 0; }
    .hero h1 { font-size:3em; margin-bottom:0.5em; }
    .hero p { font-size:1.2em; margin-bottom:1.5em; opacity:0.9; }
    .hero-stats { display:flex; justify-content:center; flex-wrap:wrap; gap:2em; }
    .stat-card { background:rgba(255,255,255,0.2); backdrop-filter:blur(10px); padding:1em 1.5em; border-radius:8px; min-width:160px; }
    .stat-card h3 { font-size:1.1em; margin-bottom:0.3em; }
    .stat-card p { font-size:1.5em; font-weight:700; }
    .highlight { background:#fff7e6; border-left:6px solid #f39c12; padding:1em 1.5em; border-radius:8px; margin-top:2em; box-shadow:0 2px 5px rgba(0,0,0,0.05); }
    .highlight h3 { margin-bottom:0.5em; color:#d35400; }
    .highlight p { font-size:1em; }
    .tabs-container { background:#ecf0f1; border-radius:8px; overflow:hidden; margin-top:2em; }
    .tab-list { display:flex; flex-wrap:wrap; }
    .tab-list button { flex:1 1 120px; padding:1em; background:none; border:none; font-size:1em; cursor:pointer; display:flex; align-items:center; justify-content:center; gap:0.5em; transition:background .2s; }
    .tab-list button:hover { background:#dcdde1; }
    .tab-list .active { background:#fff; border-bottom:4px solid #e67e22; color:#e67e22; }
    .tab-content { display:none; background:#fff; border-radius:0 0 8px 8px; box-shadow:0 2px 8px rgba(0,0,0,0.1); padding:2em; }
    .tab-content.active { display:block; }
    table { width:100%; border-collapse:collapse; margin-top:1em; }
    th, td { border:1px solid #ccc; padding:10px; text-align:left; }
    th { background:#f4f4f4; }
    footer { background:#2c3e50; color:#fff; text-align:center; padding:2em 0; margin-top:3em; }
    footer p { font-size:0.9em; margin-bottom:0.5em; }
    footer a { color:#fff; margin:0 0.5em; font-size:0.9em; }
    .institution { background: #eaf2f8; border-left: 6px solid #2980b9; margin: 2em auto; padding: 1.5em; border-radius: 8px; box-shadow: 0 2px 8px rgba(0,0,0,0.05); }
    .institution h3 { margin-bottom: 0.8em; color: #2c3e50; }
    .institution ul { list-style: none; padding-left: 1em; }
    .institution li { margin-bottom: 0.4em; }
    @media (max-width: 768px) {
      .hero h1 { font-size: 2em; }
      .hero p { font-size: 1em; }
      .tab-list button { font-size: 0.9em; padding: 0.8em; }
      .stat-card p { font-size: 1.2em; }
    }
  </style>
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      function showTab(tabIndex) {
        const contents = document.querySelectorAll('.tab-content');
        const buttons = document.querySelectorAll('.tab-list button');
        if (!contents[tabIndex] || !buttons[tabIndex]) return;
        contents.forEach((content, i) => {
          content.classList.toggle('active', i === tabIndex);
          buttons[i].classList.toggle('active', i === tabIndex);
        });
      }
      const tabButtons = document.querySelectorAll('.tab-list button');
      tabButtons.forEach((btn, idx) => {
        btn.addEventListener('click', () => showTab(idx));
      });
      showTab(0);
    });
  </script>
</head>
<body>
  <header>
    <div class="container navbar">
      <div class="logo">UnifyED</div>
      <div class="tagline">Unite • Network • Inspire • Facilitate • Youth • Education & Development</div>
    </div>
  </header>

  <section class="hero">
    <h1>Empowering Futures in a Smart Way</h1>
    <p>Enhancing institutional transparency and student success through technology.</p>
    <div class="hero-stats">
      <div class="stat-card"><h3>Active Users</h3><p>5,234</p></div>
      <div class="stat-card"><h3>Students Connecting</h3><p>1,024</p></div>
      <div class="stat-card"><h3>Platform Rating</h3><p>4.6 ★</p></div>
    </div>
  </section>

  <div class="container institution">
    <h3>Institutional Details</h3>
    <ul>
      <li><strong>Name:</strong> Horizon Academy</li>
      <li><strong>Address:</strong> 123 Learning Lane, EduCity</li>
      <li><strong>Phone:</strong> +91-9876543210</li>
      <li><strong>Streams Offered:</strong> Science, Commerce, Arts, Science Bifocal, Commerce Bifocal</li>
      <li><strong>Professors:</strong>
        <ul>
          <li>Dr. Meena Rao - Physics, Ph.D., 12 years</li>
          <li>Mr. Arjun Verma - Accounts, M.Com, 8 years</li>
          <li>Ms. Leena Das - History, M.A., 10 years</li>
          <li>Dr. Ankit Shah - Chemistry, Ph.D., 9 years</li>
          <li>Ms. Kavita Joshi - Mathematics, M.Sc., 11 years</li>
        </ul>
      </li>
    </ul>
  </div>

  <div class="container">
    <div class="highlight">
      <h3>🌟 Top Ranker Highlight</h3>
      <p><strong>Name:</strong> Aarya Sharma<br>
         <strong>Class:</strong> 10th Grade<br>
         <strong>Score:</strong> 98.7% Overall</p>
    </div>

    <div class="tabs-container">
      <div class="tab-list">
        <button><i class="fas fa-book"></i> Syllabus Progress</button>
        <button><i class="fas fa-chalkboard-teacher"></i> Teacher Remarks</button>
        <button><i class="fas fa-graduation-cap"></i> Performance</button>
        <button><i class="fas fa-tasks"></i> To-Do</button>
        <button><i class="fas fa-money-bill"></i> Fees</button>
        <button><i class="fas fa-file-pdf"></i> Fee Receipt</button>
        <button><i class="fas fa-question-circle"></i> Doubts</button>
        <button><i class="fas fa-bullhorn"></i> Announcements</button>
        <button><i class="fas fa-history"></i> 45 Day History</button>
        <button><i class="fas fa-comments"></i> Chatbox</button>
        <button><i class="fas fa-sticky-note"></i> Memo</button>
      </div>
      <div class="tab-content active"><h2>Syllabus Progress</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Teacher Remarks</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Performance</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>To-Do</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Fees</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Fee Receipt</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Doubts</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Announcements</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>45 Day History</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Chatbox</h2><p>Coming soon...</p></div>
      <div class="tab-content"><h2>Memo</h2><p>Coming soon...</p></div>
    </div>
  </div>

  <footer>
    <div class="container">
      <p>&copy; 2025 UnifyED. All rights reserved.</p>
      <p>
        <a href="https://unifyed.in/privacy-policy" target="_blank">Privacy Policy</a> | 
        <a href="https://unifyed.in/terms" target="_blank">Terms of Use</a>
      </p>
    </div>
  </footer>
</body>
</html>
