# Gate_Prep_Journey

<!DOCTYPE html>
bhgu
<html lang="en">
<title>GATE CSE 2027 — Six-Month Flight Plan</title>
jguh
bhguh
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:wght@400;500;600;700&family=IBM+Plex+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
  :root{
  bhbh
    --bg:#0A0C10;

    --panel:#12151C;
    bhbhh
    --panel-2:#171B23;
    --line:#252B36;
    --ink:#E8EAED;
    --ink-dim:#9AA4B2;
    --ink-faint:#5B6472;
    --amber:#FFB640;
    
    --amber-dim:#8A6425;
    --cyan:#5EC8D8;
    --red:#E5605A;
    --mono:'IBM Plex Mono', ui-monospace, monospace;
    --sans:'IBM Plex Sans', system-ui, sans-serif;
  }
  
  *{box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
  
    margin:0; background:var(--bg); color:var(--ink);
    font-family:var(--sans); line-height:1.55; font-size:15px;
    -webkit-font-smoothing:antialiased;
  }
  a{color:var(--cyan);}
  bhbhh
  vhgh
  .wrap{max-width:920px; margin:0 auto; padding:0 24px 120px;}

  /* ===== TOP STATUS BAR ===== */
  
  .statusbar{
    position:sticky; top:0; z-index:50;
    
    background:rgba(10,12,16,0.92); backdrop-filter:blur(8px);
    knjh
    border-bottom:1px solid var(--line);
  }
  .statusbar-inner{
    max-width:920px; margin:0 auto; padding:10px 24px;
    
    display:flex; align-items:center; justify-content:space-between; gap:16px;
    font-family:var(--mono); font-size:12px; color:var(--ink-dim);
  }
  .status-dot{display:inline-block; width:7px; height:7px; border-radius:50%; background:var(--amber); margin-right:7px; box-shadow:0 0 8px var(--amber); animation:pulse 2s infinite;}
  
  @keyframes pulse{0%,100%{opacity:1;}50%{opacity:.35;}}
  #tminus{color:var(--amber); font-weight:600;}

  /* ===== HERO ===== */
  jhuhu
   jbjhh
  .hero{padding:64px 0 28px;}
  .eyebrow{font-family:var(--mono); font-size:12px; letter-spacing:.14em; color:var(--amber); text-transform:uppercase;}
  h1{
    font-family:var(--mono); font-weight:700; font-size:clamp(30px,5vw,46px);
    line-height:1.08; margin:14px 0 0; color:var(--ink); letter-spacing:-0.01em;
  }
  h1 span{color:var(--ink-faint);}
  .hero-sub{color:var(--ink-dim); font-size:16px; max-width:640px; margin:18px 0 0;}
  .target-row{display:flex; gap:10px; flex-wrap:wrap; margin-top:22px;}
  .chip{
    font-family:var(--mono); font-size:12px; padding:6px 12px; border:1px solid var(--line);
    border-radius:20px; color:var(--ink-dim); background:var(--panel);
  }
  .chip b{color:var(--ink);}

  /* ===== TIMELINE (signature element) ===== */
  .timeline-block{margin-top:38px;}
  .timeline-label{display:flex; justify-content:space-between; font-family:var(--mono); font-size:11px; color:var(--ink-faint); margin-bottom:8px; text-transform:uppercase; letter-spacing:.08em;}
  .timeline{display:flex; gap:3px; height:34px;}
  .tl-seg{flex:1; position:relative; background:var(--panel-2); border:1px solid var(--line); border-radius:3px; overflow:hidden;}
  .tl-seg .fill{position:absolute; left:0; top:0; bottom:0; width:0%; background:linear-gradient(90deg, var(--amber-dim), var(--amber));}
  .tl-seg.exam{background:rgba(229,96,90,0.08); border-color:rgba(229,96,90,0.4);}
  .tl-seg span{
    position:absolute; inset:0; display:flex; align-items:center; justify-content:center;
    font-family:var(--mono); font-size:10.5px; color:var(--ink-dim); letter-spacing:.05em; z-index:2;
  }
  .tl-seg.exam span{color:var(--red);}

  /* ===== SECTIONS ===== */
  section{margin-top:64px;}
  .sec-head{display:flex; align-items:baseline; gap:12px; margin-bottom:20px;}
  .sec-num{font-family:var(--mono); color:var(--amber-dim); font-size:13px;}
  h2{font-family:var(--mono); font-size:20px; margin:0; color:var(--ink); letter-spacing:-0.01em;}
  .sec-note{color:var(--ink-faint); font-size:13px; margin:-10px 0 20px;}

  .panel{background:var(--panel); border:1px solid var(--line); border-radius:8px; padding:22px 24px;}
  .panel + .panel{margin-top:12px;}

  /* table */
  table{width:100%; border-collapse:collapse; font-size:13.5px;}
  th{
    text-align:left; font-family:var(--mono); font-size:11px; text-transform:uppercase;
    letter-spacing:.06em; color:var(--ink-faint); font-weight:500; padding:8px 10px;
    border-bottom:1px solid var(--line);
  }
  td{padding:10px 10px; border-bottom:1px solid var(--line); color:var(--ink-dim); vertical-align:top;}
  tr:last-child td{border-bottom:none;}
  td.num, th.num{font-family:var(--mono); color:var(--ink);}
  .tier-A{color:var(--amber); font-family:var(--mono); font-size:12px;}
  .tier-B{color:var(--cyan); font-family:var(--mono); font-size:12px;}
  .tier-C{color:var(--ink-faint); font-family:var(--mono); font-size:12px;}
  .row-highlight td{background:rgba(255,182,64,0.06);}

  /* phase cards */
  .phase{
    display:grid; grid-template-columns:64px 1fr; gap:0; margin-bottom:2px;
  }
  .phase-rail{position:relative; display:flex; flex-direction:column; align-items:center;}
  .phase-dot{width:11px; height:11px; border-radius:50%; background:var(--panel-2); border:2px solid var(--amber-dim); margin-top:6px; flex-shrink:0;}
  .phase-line{flex:1; width:1px; background:var(--line); margin-top:4px;}
  .phase:last-child .phase-line{display:none;}
  .phase-body{padding:0 0 34px 18px;}
  .phase-month{font-family:var(--mono); font-size:11px; color:var(--amber); letter-spacing:.1em; text-transform:uppercase;}
  .phase-title{font-family:var(--sans); font-weight:600; font-size:16px; color:var(--ink); margin:4px 0 8px;}
  .phase-desc{color:var(--ink-dim); font-size:13.5px; margin-bottom:10px;}
  .phase-meta{display:flex; gap:18px; flex-wrap:wrap; font-family:var(--mono); font-size:11.5px; color:var(--ink-faint);}
  .phase-meta b{color:var(--ink-dim); font-weight:500;}

  /* weekly grid */
  .week-grid{display:grid; grid-template-columns:repeat(auto-fit,minmax(120px,1fr)); gap:10px; margin-top:6px;}
  .day-card{background:var(--panel-2); border:1px solid var(--line); border-radius:6px; padding:12px;}
  .day-name{font-family:var(--mono); font-size:11px; color:var(--amber); text-transform:uppercase; letter-spacing:.06em; margin-bottom:8px;}
  .day-card ul{margin:0; padding-left:16px; font-size:12.5px; color:var(--ink-dim);}
  .day-card li{margin-bottom:4px;}

  ul.plain{padding-left:18px; margin:0; color:var(--ink-dim); font-size:13.5px;}
  ul.plain li{margin-bottom:8px;}
  .callout{
    border-left:2px solid var(--amber); padding:2px 0 2px 16px; color:var(--ink-dim); font-size:13.5px; margin:16px 0;
  }
  .callout b{color:var(--ink);}
  .two-col{display:grid; grid-template-columns:1fr 1fr; gap:12px;}
  @media (max-width:640px){.two-col{grid-template-columns:1fr;}}

  footer{margin-top:80px; padding-top:24px; border-top:1px solid var(--line); font-family:var(--mono); font-size:11.5px; color:var(--ink-faint);}
</style>
</head>
<body>

<div class="statusbar">
  <div class="statusbar-inner">
    <span><span class="status-dot"></span>GATE CS &amp; IT — 2027 CYCLE</span>
    <span id="tminus">T-minus — days</span>
  </div>
</div>

<div class="wrap">

  <div class="hero">
    <div class="eyebrow">Six-Month Operating Window · Aug 2026 → Feb 2027</div>
    <h1>Flight Plan <span>/ GATE CSE 2027</span></h1>
    <p class="hero-sub">A practical, month-by-month execution plan for the final stretch — built for the target of AIR under 100, with a floor of AIR under 150, aimed at CSE seats at IIT Madras and IIT Bombay.</p>
    <div class="target-row">
      <div class="chip">Exam window <b>Feb 6–21, 2027</b></div>
      <div class="chip">Target AIR <b>&lt; 100</b></div>
      <div class="chip">Floor AIR <b>&lt; 150</b></div>
      <div class="chip">Target score <b>75–80+ / 100</b></div>
    </div>

    <div class="timeline-block">
      <div class="timeline-label"><span>Aug 2026</span><span>Exam</span></div>
      <div class="timeline" id="timeline">
        <div class="tl-seg" data-m="0"><div class="fill"></div><span>AUG</span></div>
        <div class="tl-seg" data-m="1"><div class="fill"></div><span>SEP</span></div>
        <div class="tl-seg" data-m="2"><div class="fill"></div><span>OCT</span></div>
        <div class="tl-seg" data-m="3"><div class="fill"></div><span>NOV</span></div>
        <div class="tl-seg" data-m="4"><div class="fill"></div><span>DEC</span></div>
        <div class="tl-seg" data-m="5"><div class="fill"></div><span>JAN</span></div>
        <div class="tl-seg exam"><span>FEB</span></div>
      </div>
    </div>
  </div>

  <!-- 01 EXAM SNAPSHOT -->
  <section id="snapshot">
    <div class="sec-head"><span class="sec-num">01</span><h2>Exam Snapshot</h2></div>
    <div class="panel">
      <table>
        <tr><td style="color:var(--ink-faint)">Conducting body</td><td>IIT Madras</td></tr>
        <tr><td style="color:var(--ink-faint)">Dates</td><td>Feb 6, 7, 13, 14, 20, 21, 2027 (multi-session, online CBT)</td></tr>
        <tr><td style="color:var(--ink-faint)">Duration</td><td>3 hours</td></tr>
        <tr><td style="color:var(--ink-faint)">Questions / marks</td><td>65 questions — 100 marks</td></tr>
        <tr><td style="color:var(--ink-faint)">Split</td><td>General Aptitude 15 · Engineering Maths ≈13 · Core CS ≈72</td></tr>
        <tr><td style="color:var(--ink-faint)">Marking</td><td>1-mark Qs: −1/3 for wrong · 2-mark Qs: −2/3 for wrong · MSQ/NAT: no negative marking</td></tr>
        <tr><td style="color:var(--ink-faint)">2027 syllabus note</td><td>IIT Madras trimmed the syllabus this cycle — the biggest cuts are in COA, Digital Logic, and Computer Networks. Re-check the official PDF before building topic lists so you're not over-preparing removed content.</td></tr>
      </table>
    </div>
  </section>

  <!-- 02 TARGET CALIBRATION -->
  <section id="calibration">
    <div class="sec-head"><span class="sec-num">02</span><h2>Target Calibration</h2></div>
    <p class="sec-note">What AIR &lt; 100 actually costs, based on recent-cycle marks-vs-rank trends. Treat this as a compass, not a contract — normalization shifts a few marks either way each year.</p>
    <div class="panel">
      <table>
        <tr><th>Rank band</th><th class="num">Marks / 100</th><th>Read</th></tr>
        <tr><td>AIR 1–10</td><td class="num">85+</td><td class="tier-A">Reach</td></tr>
        <tr class="row-highlight"><td>AIR 10–50</td><td class="num">75–80</td><td class="tier-A">Target zone</td></tr>
        <tr class="row-highlight"><td>AIR 50–100</td><td class="num">70–75</td><td class="tier-A">Target zone</td></tr>
        <tr><td>AIR 100–200</td><td class="num">65–70</td><td class="tier-B">Floor / safety net</td></tr>
        <tr><td>AIR 200–500</td><td class="num">60–65</td><td class="tier-C">Below floor</td></tr>
      </table>
    </div>
    <div class="callout">Build the plan around <b>78+ raw marks</b> as the working target — a buffer above the AIR-100 line, since a single hard paper day can shift the cutoff by 3–5 marks. Historically, IIT Bombay and IIT Madras CSE general-category M.Tech cutoffs land in a similar AIR band, but confirm the current year's cutoff on COAP once counselling opens — don't plan admission odds off memory of past years.</div>
  </section>

  <!-- 03 WEIGHTAGE MAP -->
  <section id="weightage">
    <div class="sec-head"><span class="sec-num">03</span><h2>Subject Weightage Map</h2></div>
    <p class="sec-note">Where the 72 core-CS marks tend to concentrate. Tier A subjects get first claim on deep-work hours; Tier C gets revision-only passes.</p>
    <div class="panel">
      <table>
        <tr><th>Subject</th><th class="num">Typical weight</th><th>Tier</th></tr>
        <tr><td>Algorithms &amp; Data Structures</td><td class="num">~13–15</td><td class="tier-A">A · Core</td></tr>
        <tr><td>Programming (C-based)</td><td class="num">~6–8</td><td class="tier-A">A · Core</td></tr>
        <tr><td>Operating Systems</td><td class="num">~8–10</td><td class="tier-A">A · Core</td></tr>
        <tr><td>Databases</td><td class="num">~7–8</td><td class="tier-A">A · Core</td></tr>
        <tr><td>Theory of Computation</td><td class="num">~6–7</td><td class="tier-B">B</td></tr>
        <tr><td>Computer Networks (trimmed)</td><td class="num">~6–7</td><td class="tier-B">B</td></tr>
        <tr><td>Digital Logic (trimmed)</td><td class="num">~5–6</td><td class="tier-B">B</td></tr>
        <tr><td>COA (trimmed)</td><td class="num">~7–8</td><td class="tier-A">A · Core</td></tr>
        <tr><td>Compiler Design</td><td class="num">~4–5</td><td class="tier-C">C</td></tr>
        <tr><td>Engineering Mathematics</td><td class="num">~13</td><td class="tier-A">A · High-yield</td></tr>
        <tr><td>General Aptitude</td><td class="num">15</td><td class="tier-A">A · High-yield, low-effort</td></tr>
      </table>
    </div>
    <div class="callout">Engineering Maths and GA together carry <b>~28 marks</b> for a fraction of the syllabus depth of DS/Algo or OS — they're the highest marks-per-hour return in the whole paper, which is why they stay on a parallel daily track instead of being pushed to the end.</div>
  </section>

  <!-- 04 SIX MONTH PLAN -->
  <section id="plan">
    <div class="sec-head"><span class="sec-num">04</span><h2>Six-Month Execution Plan</h2></div>
    <p class="sec-note">Each phase builds on the last — nothing here is a clean restart, so slippage in one month compounds. Treat month-end milestones as hard checkpoints, not suggestions.</p>

    <div class="phase">
      <div class="phase-rail"><div class="phase-dot"></div><div class="phase-line"></div></div>
      <div class="phase-body">
        <div class="phase-month">Aug 2026</div>
        <div class="phase-title">Foundation lock — Tier A core</div>
        <div class="phase-desc">Algorithms + Data Structures and Operating Systems in full depth. Programming fundamentals refreshed alongside. GA + Maths daily track starts now, not later.</div>
        <div class="phase-meta"><span><b>Mocks:</b> 1 sectional / week</span><span><b>Output:</b> topic-wise notes for both subjects, first error log opened</span></div>
      </div>
    </div>

    <div class="phase">
      <div class="phase-rail"><div class="phase-dot"></div><div class="phase-line"></div></div>
      <div class="phase-body">
        <div class="phase-month">Sep 2026</div>
        <div class="phase-title">Databases + COA</div>
        <div class="phase-desc">DBMS in full (normalization, transactions, indexing, SQL/relational algebra) paired with the trimmed COA syllabus. First full-length mock at month-end to baseline against the 78-mark target.</div>
        <div class="phase-meta"><span><b>Mocks:</b> 1 sectional / week + 1 full-length</span><span><b>Output:</b> baseline score, first ranked weak-topic list</span></div>
      </div>
    </div>

    <div class="phase">
      <div class="phase-rail"><div class="phase-dot"></div><div class="phase-line"></div></div>
      <div class="phase-body">
        <div class="phase-month">Oct 2026</div>
        <div class="phase-title">TOC + Compiler Design + Digital Logic</div>
        <div class="phase-desc">Tier B/C subjects cleared in one sweep while Tier A subjects shift to a weekly maintenance pass (problem sets, not fresh reading). This is also when Computer Networks gets its first full pass.</div>
        <div class="phase-meta"><span><b>Mocks:</b> 1 sectional / week + 2 full-length</span><span><b>Output:</b> full syllabus "first pass" complete</span></div>
      </div>
    </div>

    <div class="phase">
      <div class="phase-rail"><div class="phase-dot"></div><div class="phase-line"></div></div>
      <div class="phase-body">
        <div class="phase-month">Nov 2026</div>
        <div class="phase-title">Full-syllabus problem-solving phase</div>
        <div class="phase-desc">No new topics after the first week. Every subject gets subject-wise PYQs (last 10–15 years) end to end. This is where speed and accuracy separate from "I understand the concept."</div>
        <div class="phase-meta"><span><b>Mocks:</b> 1 full-length / week</span><span><b>Output:</b> PYQ accuracy tracked per subject</span></div>
      </div>
    </div>

    <div class="phase">
      <div class="phase-rail"><div class="phase-dot"></div><div class="phase-line"></div></div>
      <div class="phase-body">
        <div class="phase-month">Dec 2026</div>
        <div class="phase-title">Second revision cycle + mock intensification</div>
        <div class="phase-desc">Full syllabus, second pass — condensed, from your own notes only, not textbooks. Mock frequency steps up. GATE application window closes this month — file it and don't let admin tasks eat study days.</div>
        <div class="phase-meta"><span><b>Mocks:</b> 2 full-length / week</span><span><b>Output:</b> condensed revision sheet per subject</span></div>
      </div>
    </div>

    <div class="phase">
      <div class="phase-rail"><div class="phase-dot"></div></div>
      <div class="phase-body">
        <div class="phase-month">Jan 2027 → Exam</div>
        <div class="phase-title">Peak mocks, then taper</div>
        <div class="phase-desc">Weeks 1–3: alternate-day full mocks under strict timing, each followed by a same-day error-log review. Final week before your first session: revision-only from formula sheets and error logs — no new problems, protect sleep and exam-day logistics (admit card, center, timing).</div>
        <div class="phase-meta"><span><b>Mocks:</b> alternate days → taper to none in final 3 days</span><span><b>Output:</b> exam-ready formula sheet, zero open weak topics</span></div>
      </div>
    </div>
  </section>

  <!-- 05 WEEKLY RHYTHM -->
  <section id="rhythm">
    <div class="sec-head"><span class="sec-num">05</span><h2>Weekly Rhythm Template</h2></div>
    <p class="sec-note">The recurring shape each week should take, month to month — the subject in the "deep work" slot changes per phase above, this structure doesn't.</p>
    <div class="week-grid">
      <div class="day-card"><div class="day-name">Mon–Fri</div><ul>
        <li>AM: deep-work block, current phase's core subject</li>
        <li>Midday: 30–45 min GA/Maths (parallel track)</li>
        <li>PM: problem sets on yesterday's topic</li>
      </ul></div>
      <div class="day-card"><div class="day-name">Saturday</div><ul>
        <li>Sectional or full-length mock</li>
        <li>Same-day error-log entry</li>
      </ul></div>
      <div class="day-card"><div class="day-name">Sunday</div><ul>
        <li>Mock review + re-derive every wrong answer</li>
        <li>Light week-ahead planning</li>
        <li>Genuine rest block — protect it</li>
      </ul></div>
    </div>
  </section>

  <!-- 06 MOCK PROTOCOL -->
  <section id="mocks">
    <div class="sec-head"><span class="sec-num">06</span><h2>Mock Test Protocol</h2></div>
    <div class="two-col">
      <div class="panel">
        <table>
          <tr><th>Phase</th><th>Cadence</th></tr>
          <tr><td>Aug</td><td>1 sectional/week</td></tr>
          <tr><td>Sep–Oct</td><td>1 sectional + 1–2 full/week</td></tr>
          <tr><td>Nov</td><td>1 full-length/week</td></tr>
          <tr><td>Dec</td><td>2 full-length/week</td></tr>
          <tr><td>Jan</td><td>Alternate days, then taper</td></tr>
        </table>
      </div>
      <div class="panel">
        <ul class="plain">
          <li>Every mock is timed strictly at 3 hours, no pauses.</li>
          <li>Log every wrong or guessed answer: topic, error type (concept / silly / time pressure), and the fix.</li>
          <li>Re-attempt the same mock's wrong questions cold, 3–4 days later, before moving on.</li>
          <li>Track raw marks against the 78-mark target line, not against other test-takers.</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- 07 NON-NEGOTIABLES -->
  <section id="risks">
    <div class="sec-head"><span class="sec-num">07</span><h2>Non-Negotiables</h2></div>
    <div class="panel">
      <ul class="plain">
        <li><b style="color:var(--ink)">No new topics after mid-November.</b> Everything past that point is depth, speed, and error correction on what's already covered.</li>
        <li><b style="color:var(--ink)">The error log is the real syllabus in the last two months</b> — it tells you exactly where marks are still leaking, which generic revision doesn't.</li>
        <li><b style="color:var(--ink)">GA and Maths never get skipped for "more important" subjects</b> — at 28 combined marks, skipping them to buy Algorithms time is a bad trade.</li>
        <li><b style="color:var(--ink)">Application, admit card, and exam-center logistics get handled in December</b>, not the week of the exam.</li>
        <li><b style="color:var(--ink)">Sleep and one full rest day per week are part of the plan, not outside it</b> — six months is a long runway, and burnout in month four costs more than it saves in month one.</li>
      </ul>
    </div>
  </section>

  <footer>
    Built for the GATE CSE 2027 cycle · exam dates and syllabus per IIT Madras' official 2027 notification — reverify against gate2027.iitm.ac.in as the exam date approaches, since schedules can shift.
  </footer>

</div>

<script>
  // Exam T-0: first CS session (Feb 6, 2027, IST) — used only for the countdown display.
  var examDate = new Date("2027-02-06T00:00:00+05:30");
  var planStart = new Date("2026-08-01T00:00:00+05:30");
  var planEnd = new Date("2027-02-01T00:00:00+05:30"); // approx end of Jan phase

  function update(){
    var now = new Date();
    var msPerDay = 86400000;
    var daysLeft = Math.max(0, Math.ceil((examDate - now) / msPerDay));
    document.getElementById('tminus').textContent = 'T-minus ' + daysLeft + ' days to exam window';

    // fill month segments proportionally based on elapsed time within the 6-month window
    var totalSpan = planEnd - planStart;
    var elapsed = now - planStart;
    var progressFrac = Math.min(1, Math.max(0, elapsed / totalSpan)); // 0..1 across 6 months
    var totalMonths = 6;
    var monthsElapsed = progressFrac * totalMonths;

    document.querySelectorAll('.tl-seg[data-m]').forEach(function(seg){
      var idx = parseInt(seg.getAttribute('data-m'), 10);
      var fillPct = Math.min(1, Math.max(0, monthsElapsed - idx)) * 100;
      seg.querySelector('.fill').style.width = fillPct + '%';
    });
  }
  update();
</script>

</body>
</html>
