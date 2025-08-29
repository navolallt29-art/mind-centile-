<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Mindcentile — Career Roadmap Test</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
  :root{
    --black:#0b0c10;
    --white:#ffffff;
    --purple:#2b0b4a; /* dark purple */
    --muted:#8b8b9a;
    --gold:#b98f1f;
    --glass: rgba(255,255,255,0.06);
  }
  *{box-sizing:border-box}
  body{
    margin:0;
    font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
    background: linear-gradient(180deg,#fafafa,#f2f4f8);
    color:var(--black);
    -webkit-font-smoothing:antialiased;
    -moz-osx-font-smoothing:grayscale;
    line-height:1.6;
  }

  /* Header */
  header{
    background: linear-gradient(180deg, rgba(43,11,74,0.98), rgba(11,12,16,0.95));
    color: #fff;
    padding:56px 20px;
    text-align:center;
    border-bottom: 4px solid rgba(255,255,255,0.03);
  }
  header h1{
    font-family:'Playfair Display',serif;
    font-size:44px;
    margin:0 0 6px;
    color:var(--gold);
    letter-spacing:1px;
  }
  header p{
    color:#EDEDED;
    margin:0 0 18px;
    max-width:980px;
    margin-left:auto;margin-right:auto;
    font-size:18px;
  }
  .hero-ctas{display:flex;gap:12px;justify-content:center;flex-wrap:wrap}
  .btn {
    display:inline-flex;
    align-items:center;
    gap:10px;
    padding:12px 18px;
    border-radius:999px;
    font-weight:600;
    text-decoration:none;
    cursor:pointer;
    border: none;
  }
  .btn-primary{
    background:var(--gold);
    color:var(--black);
    box-shadow:0 8px 28px rgba(0,0,0,0.18);
  }
  .btn-ghost{
    background:transparent;
    color:#fff;
    border:1.5px solid rgba(255,255,255,0.12);
    padding:10px 16px;
    border-radius:999px;
  }
  .btn-secondary{
    background:var(--purple);
    color:#fff;
    border:1px solid rgba(255,255,255,0.06);
  }

  main{max-width:1150px;margin:-36px auto 80px;padding:0 18px}

  /* Card / Section */
  .card{
    background:var(--white);
    border-radius:14px;
    padding:26px;
    box-shadow:0 10px 30px rgba(16,24,40,0.06);
    margin-bottom:20px;
  }
  h2{font-family:'Playfair Display',serif;font-size:24px;margin-bottom:12px;color:var(--purple)}
  p.lead{color:var(--muted);margin-top:0;margin-bottom:14px}

  /* Paths */
  .paths{display:flex;gap:14px;flex-wrap:wrap}
  .path{
    flex:1 1 300px;
    min-width:230px;
    border-radius:12px;
    padding:18px;
    background:linear-gradient(180deg,#fff,#fcfcff);
    border:1px solid #eee;
    cursor:pointer;
    transition:transform .18s ease, box-shadow .18s ease;
    text-align:left;
  }
  .path:hover{transform:translateY(-6px);box-shadow:0 14px 36px rgba(11,12,16,0.06)}
  .path h3{margin:0 0 8px;font-size:18px;color:var(--purple)}
  .path p{margin:0;color:var(--muted);font-size:14px}

  /* Quiz area */
  #quiz { display:none; }
  .progress { font-size:13px; color:var(--muted); margin-bottom:8px; }
  .question{margin-bottom:18px}
  .options{display:flex;flex-direction:column;gap:10px}
  .option-btn{
    background:#f7f7f8;border:1px solid #e6e6e8;padding:12px 14px;border-radius:10px;text-align:left;cursor:pointer;font-weight:700;
  }
  .option-btn:hover{background:#fff;border-color:var(--purple);color:var(--purple)}
  .scale-row{display:flex;gap:8px}
  .scale-btn{flex:1;padding:10px;border-radius:8px;border:1px solid #e9e9eb;background:#fff;cursor:pointer}
  .scale-btn:hover{border-color:var(--purple);color:var(--purple)}
  input[type="text"], textarea { width:100%; padding:10px 12px;border-radius:8px;border:1px solid #e9e9eb;font-size:15px; }

  /* Controls */
  .controls{display:flex;justify-content:space-between;gap:10px;margin-top:18px}
  .controls .left{display:flex;gap:8px}

  /* Result */
  #result { display:none; }
  .result-hero{display:flex;gap:18px;align-items:center;flex-wrap:wrap}
  .pill{display:inline-block;padding:6px 12px;border-radius:999px;background:var(--gold);color:var(--black);font-weight:700;margin-right:8px}
  .muted-small{color:var(--muted);font-size:13px}
  .roadmap{background:linear-gradient(180deg,#fff9e8,#fffbf0);border-left:4px solid var(--gold);padding:14px;border-radius:8px;margin-top:12px}
  .bio-data{background:#fafaff;border-radius:8px;padding:12px;border:1px solid #f0eff3;margin-top:12px}

  /* App section */
  .app-card{display:flex;gap:18px;align-items:center;flex-wrap:wrap}
  .app-preview{flex:0 0 220px;height:160px;background:linear-gradient(180deg,#1f0836,#350b5a);border-radius:12px;color:#fff;display:flex;align-items:center;justify-content:center;font-weight:700}

  /* footer */
  footer{padding:28px;text-align:center;color:#666;font-size:14px}
  footer a{color:var(--purple);text-decoration:none;font-weight:600}

  /* responsive */
  @media (max-width:900px){
    header h1{font-size:32px}
    .paths{flex-direction:column}
  }
</style>
</head>
<body>

  <header>
    <h1>Mindcentile</h1>
    <p>Take the career test that gives you a practical, no-fluff 1 / 3 / 5 year roadmap. Unique questions, clear steps, and shareable results.</p>
    <div class="hero-ctas">
      <a class="btn btn-primary" href="https://www.youtube.com/@Mindcentile" target="_blank" rel="noopener noreferrer">📺 Subscribe — Mindcentile</a>
      <a class="btn btn-ghost" href="https://www.youtube.com/@Mindcentile" target="_blank" rel="noopener noreferrer">🔎 View Channel</a>
      <button class="btn btn-secondary" onclick="document.getElementById('start').scrollIntoView({behavior:'smooth'})">🧭 Start Test</button>
    </div>
  </header>

  <main>
    <section class="card">
      <h2>Why this test</h2>
      <p class="lead">This test is built to reveal what you truly value, how you work, and the exact steps you should take in the next 1, 3 and 5 years. No fluff — every question is designed to surface decision-making signals that matter for real careers.</p>
    </section>

    <section id="start" class="card">
      <h2>Choose your path</h2>
      <p class="muted-small">Each path has 30 thoughtful questions tailored to your stage — students, entrepreneurs, and young professionals have different decision problems. Pick the one that fits and begin.</p>

      <div class="paths">
        <div class="path" onclick="begin('student')">
          <h3>🎓 Student</h3>
          <p>Learning, portfolios, majors, internships — find the fastest route to real-world mastery.</p>
          <div style="margin-top:12px"><button class="btn btn-primary" onclick="begin('student'); event.stopPropagation()">Start Student Test</button></div>
        </div>

        <div class="path" onclick="begin('entrepreneur')">
          <h3>💼 Entrepreneur / Creator</h3>
          <p>Idea validation, product-market-fit, early traction and scalable systems.</p>
          <div style="margin-top:12px"><button class="btn btn-primary" onclick="begin('entrepreneur'); event.stopPropagation()">Start Entrepreneur Test</button></div>
        </div>

        <div class="path" onclick="begin('professional')">
          <h3>🌍 Young Professional</h3>
          <p>Promotions, leadership, side projects, personal brand and long-term positioning.</p>
          <div style="margin-top:12px"><button class="btn btn-primary" onclick="begin('professional'); event.stopPropagation()">Start Professional Test</button></div>
        </div>
      </div>
    </section>

    <!-- Quiz -->
    <section id="quiz" class="card">
      <div style="display:flex;justify-content:space-between;align-items:center">
        <div>
          <h2 id="quizTitle">Career Insight — <span id="pathLabel"></span></h2>
          <div class="progress"><span id="qNum">1</span> / <span id="qTotal">30</span></div>
        </div>
        <div class="muted-small">Answer honestly. Some questions accept short text for personalization.</div>
      </div>

      <div id="quizContainer" style="margin-top:18px"></div>

      <div class="controls">
        <div class="left"><button class="btn btn-ghost" onclick="prevQ()">← Previous</button></div>
        <div><button class="btn btn-primary" id="nextBtn" onclick="nextQ()">Next →</button></div>
      </div>
    </section>

    <!-- Result -->
    <section id="result" class="card">
      <div class="result-hero">
        <div class="result-title">
          <div class="pill">Mindcentile Roadmap</div>
          <h2 id="resultHeading">Your personalized career roadmap</h2>
          <p id="resultIntro" class="muted-small">Below is your biodata summary and an actionable 1 / 3 / 5 year plan. Share it, act on it, and don’t let life pass by without clarity.</p>
        </div>
      </div>

      <div id="resultContent" style="margin-top:12px"></div>

      <div style="margin-top:16px;display:flex;gap:12px;flex-wrap:wrap">
        <button class="btn btn-primary" onclick="copyLink()">📋 Copy Result Link</button>
        <button class="btn btn-ghost" onclick="shareResult()">🔗 Share</button>
        <button class="btn btn-secondary" onclick="restart()">↺ Take Another Test</button>
      </div>

      <div style="margin-top:14px;color:#c62828;font-weight:700">⚠️ If you hadn’t taken this today, you could waste years guessing. Act on it and share it with one friend who needs clarity now.</div>
    </section>

    <!-- App Coming Soon -->
    <section class="card">
      <h2>Mindcentile App — Coming Soon</h2>
      <div class="app-card">
        <div class="app-preview">APP PREVIEW</div>
        <div style="flex:1">
          <p class="muted-small">We are building a gamified app with daily challenges, streaks, quizzes and personal progress tracking. When the app is ready you can download it here and link it to this site for saved roadmaps.</p>
          <div style="margin-top:12px"><button class="btn btn-primary" onclick="alert('Thanks — we will notify you when the app launches')">Notify Me</button></div>
        </div>
      </div>
    </section>

  </main>

  <footer>
    © 2025 Mindcentile — Build the Top 1% Mindset · <a href="https://www.youtube.com/@Mindcentile" target="_blank" rel="noopener">Subscribe on YouTube</a>
  </footer>

<script>
/* ----------------------------------------------------------------
   Full 30 q per path (total 90). Types: mc, scale, text
   Each entry: {id, type, q, options?, placeholder?}
------------------------------------------------------------------*/
const QUESTIONS = {
  student: [
    {id:'s0', type:'text', q:"In one phrase, what would you like to be known for in 10 years?", placeholder:"e.g., 'building accessible learning apps'"},
    {id:'s1', type:'mc', q:"When learning, what excites you most?", options:["Building projects","Solving theory","Teaching others","Winning competitions"]},
    {id:'s2', type:'mc', q:"Which do you value more right now?", options:["Depth in one subject","Breadth across subjects"]},
    {id:'s3', type:'scale', q:"How disciplined are you with daily routines? (1 low — 5 high)"},
    {id:'s4', type:'mc', q:"What’s a better use of your time right now?", options:["Build a real project","Study textbooks","Intern/work experience","Create content"]},
    {id:'s5', type:'text', q:"Name one skill that would dramatically change your options (be precise).", placeholder:"e.g., 'Python', 'data analysis', 'presentations'"},
    {id:'s6', type:'mc', q:"When stuck, you usually:", options:["Prototype a quick solution","Read references","Ask peers/mentors","Take a break and reflect"]},
    {id:'s7', type:'mc', q:"Do you prefer working alone or in small teams?", options:["Alone","Small teams","Large groups","Either"]},
    {id:'s8', type:'scale', q:"How comfortable are you sharing imperfect work publicly? (1 low — 5 high)"},
    {id:'s9', type:'mc', q:"What matters most to you in 3 years?", options:["Skill mastery","Portfolio of projects","Network & mentors","Internship/job"]},
    {id:'s10', type:'text', q:"Describe the ideal project you’d build in 3 months.", placeholder:"Short description"},
    {id:'s11', type:'mc', q:"Which feedback helps you most?", options:["Detailed corrections","Practical tips","Big-picture direction","Moral support"]},
    {id:'s12', type:'mc', q:"Do you learn better from examples or from rules?", options:["Examples","Rules/theory","Mix of both"]},
    {id:'s13', type:'scale', q:"How often do you finish what you start? (1 rarely — 5 always)"},
    {id:'s14', type:'mc', q:"What drains your energy after focused study?", options:["Too much theory","Shallow learning","Isolation","No clear progress"]},
    {id:'s15', type:'text', q:"If you had one mentor, what single thing would you ask them to teach you?", placeholder:"Short answer"},
    {id:'s16', type:'mc', q:"Which outcome would you prefer after one year?", options:["A portfolio project","A high grade","A mentor relationship","A mini-business"]},
    {id:'s17', type:'scale', q:"How well do you take corrective feedback? (1 low — 5 high)"},
    {id:'s18', type:'mc', q:"What best describes your curiosity?", options:["Detail-oriented","Idea-oriented","People-oriented","Tool-oriented"]},
    {id:'s19', type:'text', q:"Write one measurable 6-month goal you can achieve.", placeholder:"e.g., 'Ship a website'"},
    {id:'s20', type:'mc', q:"Which environment helps you learn best?", options:["Quiet & focused","Interactive classes","Hackathons","Mentored projects"]},
    {id:'s21', type:'mc', q:"What skill would you prioritise learning next?", options:["Coding","Writing","Design","Communication"]},
    {id:'s22', type:'scale', q:"Rate your willingness to fail publicly to learn quickly (1 low — 5 high)"},
    {id:'s23', type:'mc', q:"When choosing topics, you prefer:", options:["High ROI skills","Passion projects","Faculty-led topics","Market-demand subjects"]},
    {id:'s24', type:'text', q:"Who inspires you academically or professionally? Name one and why.", placeholder:"Short answer"},
    {id:'s25', type:'mc', q:"How important is a public portfolio to you?", options:["Critical","Helpful","Optional","Not now"]},
    {id:'s26', type:'mc', q:"If you could spend a month only learning, you'd:", options:["Build a project","Study intensively","Intern","Teach others"]},
    {id:'s27', type:'scale', q:"How decisive are you when selecting a major or specialization? (1 low — 5 high)"},
    {id:'s28', type:'mc', q:"Do you prefer structure or creative freedom in projects?", options:["Structure","Creative freedom","A blend"]},
    {id:'s29', type:'text', q:"One sentence: What will you regret not doing before age 25?", placeholder:"Short answer"}
  ],

  entrepreneur: [
    {id:'e0', type:'text', q:"In one sentence, what problem do you want to solve or what impact do you want to make?", placeholder:"Precise, short mission statement"},
    {id:'e1', type:'mc', q:"What motivates you most as a founder?", options:["Solve real pain","Build wealth","Create autonomy","Build community"]},
    {id:'e2', type:'mc', q:"How do you test ideas initially?", options:["Talk to users","Build prototypes","Run ads","Make landing pages"]},
    {id:'e3', type:'scale', q:"How comfortable are you with unstable income? (1 low — 5 high)"},
    {id:'e4', type:'mc', q:"What cost theme drains you: time, money, or attention?", options:["Time","Money","Attention","All equal"]},
    {id:'e5', type:'text', q:"Name a founder or company you study and what you learn from them.", placeholder:"Short answer"},
    {id:'e6', type:'mc', q:"Which early metric matters most to you?", options:["Retention","Revenue","Engagement","Growth rate"]},
    {id:'e7', type:'mc', q:"Do you prefer building tech or building teams/operations?", options:["Tech","Teams/operations","Both","Depends"]},
    {id:'e8', type:'scale', q:"How quickly do you iterate on feedback? (1 slow — 5 very fast)"},
    {id:'e9', type:'mc', q:"What do you fear most in a venture?", options:["Running out of money","No product-market fit","Losing team","Legal/regulatory issues"]},
    {id:'e10', type:'text', q:"Describe your ideal first customer in one sentence.", placeholder:"Short answer"},
    {id:'e11', type:'mc', q:"What's your current network strength?", options:["Strong","Average","Weak","Non-existent"]},
    {id:'e12', type:'mc', q:"Which role energizes you the most?", options:["Product building","Growth/marketing","Sales","Strategy/vision"]},
    {id:'e13', type:'scale', q:"How consistent are you with daily execution (1 low — 5 high)"},
    {id:'e14', type:'mc', q:"When learning about markets, you prefer:", options:["Talk to users","Read reports","Analyze competitors","Prototype"]},
    {id:'e15', type:'text', q:"What is the smallest test you can run this week to validate your idea?", placeholder:"One-sentence test"},
    {id:'e16', type:'mc', q:"Do you prefer to bootstrap or raise capital early?", options:["Bootstrap","Raise capital","Not sure yet"]},
    {id:'e17', type:'mc', q:"How do you hire your first teammate?", options:["Skill testing","Trial projects","Referrals","Ads/posting"]},
    {id:'e18', type:'scale', q:"How strong is your storytelling (pitch) ability? (1 low — 5 high)"},
    {id:'e19', type:'mc', q:"Which growth channel would you prioritize first?", options:["Content","Paid ads","Partnerships","Direct sales"]},
    {id:'e20', type:'text', q:"What would success look like for you in 12 months? Be specific.", placeholder:"Short measurable goal"},
    {id:'e21', type:'mc', q:"What is your risk tolerance for personal time/savings?", options:["High","Medium","Low"]},
    {id:'e22', type:'mc', q:"To build traction you will spend more time on:", options:["Talking with users","Building features","Marketing","Operations"]},
    {id:'e23', type:'text', q:"What one habit will most improve your odds as a founder?", placeholder:"Short habit"},
    {id:'e24', type:'mc', q:"Do you prefer product-led growth or sales-led growth initially?", options:["Product-led","Sales-led","Hybrid"]},
    {id:'e25', type:'scale', q:"How willing are you to pivot if initial signals are negative? (1 low — 5 high)"},
    {id:'e26', type:'mc', q:"Which advantage matters most long term?", options:["Network","Capital","Skillset","Timing"]},
    {id:'e27', type:'text', q:"Write one sentence that describes your unfair advantage.", placeholder:"Short answer"},
    {id:'e28', type:'mc', q:"How much of your time can you allocate weekly to the venture?", options:["<10 hrs","10-20 hrs","20-40 hrs",">40 hrs"]},
    {id:'e29', type:'mc', q:"What's your biggest constraint today?", options:["Time","Money","Skillset","Team"]}
  ],

  professional: [
    {id:'p0', type:'text', q:"What job title or role do you aim for in 3–5 years? (brief)", placeholder:"e.g., 'Product Manager', 'Head of Design'"},
    {id:'p1', type:'mc', q:"What motivates you most at work?", options:["Solving complex problems","Coaching others","Delivering results","Building teams"]},
    {id:'p2', type:'mc', q:"How do you learn best in a professional setting?", options:["Stretch assignments","Courses","Mentoring","Books & cases"]},
    {id:'p3', type:'scale', q:"How comfortable are you leading a small team? (1 low — 5 high)"},
    {id:'p4', type:'mc', q:"What typically blocks your progress at work?", options:["Ambiguity","Lack of visibility","Politics","Execution capacity"]},
    {id:'p5', type:'text', q:"Name a recent work achievement you are proud of.", placeholder:"Short answer"},
    {id:'p6', type:'mc', q:"Which is more important now?", options:["Skill growth","Promotion","Work-life balance","Compensation"]},
    {id:'p7', type:'scale', q:"How actively do you plan your career? (1 low — 5 high)"},
    {id:'p8', type:'mc', q:"When facing a hard decision, you:", options:["Map outcomes","Ask mentors","Trial a small test","Defer for more info"]},
    {id:'p9', type:'text', q:"What skill gap, if closed, would accelerate your career most?", placeholder:"Short answer"},
    {id:'p10', type:'mc', q:"Do you aim to become a specialist or a generalist?", options:["Specialist","Generalist","Blend"]},
    {