
    
    
     
       
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
      var idx = parseInt(seg.getAttribute('data-
      seg.querySelector('.fill').style.width = fillPct + '%';
    });
  }
  update();
</script>

</body>
</html>
