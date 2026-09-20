<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>P Aadhithiya — Profile README</title>
<style>
:root{
  --bg:#fafafa; --panel:#ffffff; --line:#e5e5e5; --text:#1a1a1a; --muted:#666;
  --red:#dc2626; --red-soft:#ef4444; --ink:#0a0a0a; --chip:#f1f1f1; --green:#16a34a;
}
@media (prefers-color-scheme: dark){
  :root:not([data-theme="light"]){
    --bg:#0a0a0a; --panel:#111111; --line:#2a1414; --text:#f3f4f6; --muted:#9ca3af;
    --red:#dc2626; --red-soft:#ef4444; --ink:#0a0a0a; --chip:#1a1a1a; --green:#22c55e;
  }
}
:root[data-theme="dark"]{
  --bg:#0a0a0a; --panel:#111111; --line:#2a1414; --text:#f3f4f6; --muted:#9ca3af;
  --red:#dc2626; --red-soft:#ef4444; --ink:#0a0a0a; --chip:#1a1a1a; --green:#22c55e;
}
*{box-sizing:border-box}
html{background:var(--bg)}
body{margin:0;background:var(--bg);color:var(--text);
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif;line-height:1.6}
.wrap{max-width:900px;margin:0 auto;padding:24px 20px 56px;text-align:center}
a{color:var(--red-soft);text-decoration:none}
a:hover{text-decoration:underline}
a:focus-visible{outline:2px solid var(--red-soft);outline-offset:3px;border-radius:4px}
hr{border:0;border-top:1px solid var(--line);margin:36px 0}
h2{font-size:1.6rem;margin:0 0 14px}
h3{margin:0 0 6px}
h4{margin:0 0 4px}
.mono{font-family:"Fira Code",ui-monospace,SFMono-Regular,Menlo,Consolas,monospace}
svg{max-width:100%;height:auto}

/* badges */
.row{display:flex;flex-wrap:wrap;justify-content:center;gap:10px;margin:14px 0}
.badge{display:inline-flex;align-items:stretch;border-radius:5px;overflow:hidden;font-weight:700;
  font-size:.78rem;letter-spacing:.02em;color:#fff;text-decoration:none!important;
  border:1px solid transparent;transition:transform .12s ease}
.badge:hover{transform:translateY(-1px)}
.badge .l{background:#0a0a0a;padding:8px 12px;display:flex;align-items:center;gap:6px}
.badge .r{background:var(--red);padding:8px 14px;display:flex;align-items:center}
.badge.dark .r{background:#111;color:var(--red-soft)}
.badge.gold .r{background:#ffa116;color:#000}
.badge.sm{font-size:.7rem;font-weight:600;border-radius:3px}
.badge.sm .l,.badge.sm .r{padding:4px 9px}
.badge.sm.gray .r{background:#111;color:#fff}
.badge.sm.green .r{background:#111;color:#fff}
.ico{width:14px;height:14px;fill:currentColor}

/* typing */
.typing{min-height:2.4rem;font-size:1.2rem;font-weight:600;color:var(--red-soft);margin:6px 0 18px}
.typing.small{font-size:.95rem;font-weight:500;color:#f87171;min-height:1.6rem}
.caret{display:inline-block;width:2px;height:1.1em;background:currentColor;margin-left:3px;vertical-align:-.15em;animation:blink 1s steps(1) infinite}
@keyframes blink{50%{opacity:0}}

/* cards */
table.grid{width:100%;border-collapse:separate;border-spacing:12px;margin:18px auto}
table.grid td{width:50%;background:var(--panel);border:1px solid var(--line);border-radius:12px;padding:16px;vertical-align:top}
.card{background:var(--panel);border:1px solid var(--line);border-radius:12px;padding:24px;margin:16px auto}
.muted{color:var(--muted)}
sub{font-size:.8rem;color:var(--muted)}

/* code window */
.codewin{width:340px;max-width:100%;margin:14px auto;border-radius:12px;overflow:hidden;background:#0d0d0d;
  border:1px solid #3a1515;text-align:left;box-shadow:0 8px 30px rgba(220,38,38,.18)}
.codewin .bar{display:flex;gap:6px;padding:10px 12px;background:#161616}
.codewin .bar i{width:10px;height:10px;border-radius:50%;background:#ef4444;display:block}
.codewin .bar i:nth-child(2){background:#f59e0b}.codewin .bar i:nth-child(3){background:#22c55e}
.codewin pre{margin:0;padding:14px 16px;font-size:.78rem;line-height:1.6;color:#e5e7eb;min-height:150px;white-space:pre-wrap}
.k{color:#ef4444}.s{color:#fca5a5}.c{color:#6b7280}

/* stack */
.stack-title{font-weight:700;margin:22px 0 8px}
.chips{display:flex;flex-wrap:wrap;justify-content:center;gap:8px}
.chip{background:var(--chip);border:1px solid var(--line);border-radius:10px;padding:7px 12px;font-size:.82rem;font-weight:600;display:inline-flex;align-items:center;gap:8px}
.chip b{display:inline-grid;place-items:center;width:22px;height:22px;border-radius:6px;background:#0a0a0a;color:var(--red-soft);font-size:.62rem;font-weight:800;font-family:ui-monospace,Menlo,monospace}

/* stat cards */
.stat{background:#0a0a0a;color:#f3f4f6;border:1px solid var(--red-soft);border-radius:10px;padding:16px 18px;text-align:left;flex:1 1 300px;max-width:440px}
.stat h5{margin:0 0 8px;color:var(--red-soft);font-size:1rem}
.stat p{margin:0;font-size:.85rem;color:#9ca3af}
.stat.lc{border:0;border-radius:12px;background:#1a1a1a;max-width:480px;width:100%}
.stat.lc h5{color:#ffa116}
.bars{display:flex;gap:6px;align-items:flex-end;height:44px;margin-top:12px}
.bars i{flex:1;background:repeating-linear-gradient(0deg,#3a1515 0 3px,#2a1010 3px 6px);border-radius:2px;display:block}
.note{font-size:.78rem;color:var(--muted);margin-top:8px}

/* snake */
.snake{background:#0a0a0a;border:1px solid var(--line);border-radius:10px;padding:14px;overflow-x:auto}
.snake canvas{display:block;margin:0 auto;max-width:100%}

@media (max-width:640px){
  table.grid,table.grid tbody,table.grid tr,table.grid td{display:block;width:100%}
  table.grid{border-spacing:0}
  table.grid td{margin-bottom:12px}
}
@media (prefers-reduced-motion: reduce){.caret{animation:none}}
</style>
</head>
<body>
<div class="wrap">

  <!-- HEADER (recreated from assets/header.svg) -->
  <svg viewBox="0 0 900 190" role="img" aria-label="P Aadhithiya header" style="width:100%;border-radius:12px">
    <defs>
      <linearGradient id="hg" x1="0" x2="1"><stop offset="0" stop-color="#0a0a0a"/><stop offset=".6" stop-color="#2a0808"/><stop offset="1" stop-color="#7f1d1d"/></linearGradient>
    </defs>
    <rect width="900" height="190" fill="url(#hg)"/>
    <g stroke="#ef4444" stroke-opacity=".18" fill="none">
      <path d="M0 150 Q225 90 450 130 T900 100"/><path d="M0 170 Q225 110 450 150 T900 120"/>
    </g>
    <text x="450" y="88" text-anchor="middle" fill="#fff" font-size="40" font-weight="800" font-family="Segoe UI,Helvetica,Arial,sans-serif">P Aadhithiya</text>
    <text x="450" y="128" text-anchor="middle" fill="#fca5a5" font-size="16" font-family="ui-monospace,Menlo,monospace">Full-Stack · AI · </text>
  </svg>

  <div class="typing mono" id="typing1" aria-live="off"><span class="t"></span><span class="caret"></span></div>

  <div class="row">
    <a class="badge" href="https://www.linkedin.com/in/aadhithiya-p-4700393b3/" target="_blank" rel="noopener"><span class="l">in&nbsp;LinkedIn</span><span class="r">Connect</span></a>
    <a class="badge" href="https://www.instagram.com/itz__adhix?stkn=cXdhZGI0cGcxZjll" target="_blank" rel="noopener"><span class="l">Instagram</span><span class="r">Follow</span></a>
    <a class="badge" href="mailto:aadthif@gmail.com"><span class="l">✉ Email</span><span class="r">Contact</span></a>
    <a class="badge" href="https://drive.google.com/file/d/1GY9lUeE9zneL9efZNbQOiWyH55UYrBXz/view?usp=sharing" target="_blank" rel="noopener"><span class="l">Resume</span><span class="r">Drive</span></a>
    <a class="badge dark" href="https://github.com/aadthif-web" target="_blank" rel="noopener"><span class="l">GitHub</span><span class="r">Follow</span></a>
  </div>

  <div class="row">
    <span class="badge"><span class="l">PROFILE VIEWS</span><span class="r">—</span></span>
  </div>
  <p class="note" style="margin-top:-4px">The view counter is served live by GitHub's profile, so it shows a dash here.</p>

  <hr>

  <h2>🔴 About Me</h2>
  <div class="typing small mono"><span class="t" id="quote"></span><span class="caret"></span></div>

  <div class="codewin" aria-hidden="true">
    <div class="bar"><i></i><i></i><i></i></div>
    <pre id="code"></pre>
  </div>

  <p>Hey! I'm <b>P Aadhithiya</b>, a passionate <b>B.Tech AI&DS student &amp; developer</b> based in India.<br>
  I specialize in architecting scalable full-stack web platforms, deploying machine learning solutions to solve practical real-world problems.</p>

  <div class="row">
    <span class="badge sm green"><span class="l">Status</span><span class="r">🟢 Building &amp; Shipping</span></span>
    <span class="badge sm"><span class="l">Degree</span><span class="r">B.Tech AI&DS</span></span>
    <span class="badge sm gray"><span class="l">Focus</span><span class="r">Full Stack &amp; AI</span></span>
  </div>

  <p>💬 <b>Let's Discuss:</b> Java, C++, JavaScript, React, Spring Boot, System Architecture &amp; Git Workflows.<br>
  ⚡ <b>Philosophy:</b> <i>"I love turning random late-night thoughts into fully deployed production software!"</i></p>

  <table class="grid">
    <tr>
      <td><h4>🔭 Portfolio</h4><a href="https://aadhithiya.vercel.app/" target="_blank" rel="noopener"><b>Portfolio</b></a><br><sub>Da &amp; intro</sub></td>
      <td><h4>🌱 Agriloop </h4><b>DSA &amp; Spring Boot</b><br><sub>React Ecosystem &amp; System Design</sub></td>
    </tr>
    <tr>
      <td><h4>🤝 Collaboration</h4><b>AI, Web &amp; </b><br><sub>Open to exciting new projects</sub></td>
    </tr>
  </table>

  <hr>

  <h2>🔴 Featured Project Spotlight</h2>
  <div class="card">
    <h3>🔬 Agriloop</h3>
    <p><i>A smart  &amp; web-enabled dairy health monitoring system designed for early anomaly detection and real-time livestock welfare tracking.</i></p>
    <div class="row">
      <a class="badge" href="file:///C:/Users/ELCOT/Downloads/nexa%20tech%20sih%20demo.html" target="_blank" rel="noopener"><span class="l">Live Demo</span><span class="r">🚀 Visit Platform</span></a>
      <a class="badge dark" href="https://github.com/aadthif-web" target="_blank" rel="noopener"><span class="l">Source Code</span><span class="r">💻 View Projects</span></a>
    </div>
  </div>

  <hr>


  <h2>🛠️ Tech Stack &amp; Skills</h2>

  <div class="stack-title">Core Programming Languages</div>
  <div class="chips">
    <span class="chip"><b>C++</b>C++</span><span class="chip"><b>JV</b>Java</span><span class="chip"><b>PY</b>Python</span>
    <span class="chip"><b>JS</b>JavaScript</span><span class="chip"><b>TS</b>TypeScript</span><span class="chip"><b>H5</b>HTML</span><span class="chip"><b>C3</b>CSS</span>
  </div>

  <div class="stack-title">Frontend &amp; Mobile Development</div>
  <div class="chips">
    <span class="chip"><b>Re</b>React</span><span class="chip"><b>Ng</b>Angular</span><span class="chip"><b>Fl</b>Flutter</span>
    <span class="chip"><b>As</b>Android Studio</span><span class="chip"><b>Tw</b>Tailwind</span><span class="chip"><b>Bs</b>Bootstrap</span>
  </div>

  <div class="stack-title">Backend, Cloud &amp; Databases</div>
  <div class="chips">
    <span class="chip"><b>Sp</b>Spring</span><span class="chip"><b>No</b>Node.js</span><span class="chip"><b>Ex</b>Express</span>
    <span class="chip"><b>Mg</b>MongoDB</span><span class="chip"><b>My</b>MySQL</span><span class="chip"><b>Fb</b>Firebase</span><span class="chip"><b>AW</b>AWS</span>
  </div>

  <div class="stack-title">AI, Data Science, &amp; DevOps</div>
  <div class="chips">
    <span class="chip"><b>Cv</b>OpenCV</span><span class="chip"><b>Ar</b>Arduino</span><span class="chip"><b>Gt</b>Git</span>
    <span class="chip"><b>GH</b>GitHub</span><span class="chip"><b>Pm</b>Postman</span><span class="chip"><b>Lx</b>Linux</span><span class="chip"><b>Fg</b>Figma</span>
  </div>
  <div class="row" style="margin-top:16px">
    <span class="badge sm dark"><span class="l">🐼 pandas</span></span>
    <span class="badge sm dark"><span class="l">scikit-learn</span></span>
    <span class="badge sm dark"><span class="l">Seaborn</span></span>
    <span class="badge sm dark"><span class="l">Selenium</span></span>
  </div>

  <hr>

  <h2>📊 GitHub Analytics &amp; Activity</h2>
  <div class="row" style="align-items:stretch">
    <a class="stat" href="https://github.com/DeepakAmalWinstarJ" target="_blank" rel="noopener" style="text-decoration:none">
      <h5>GitHub Stats</h5><p>Stars, commits, PRs and issues are generated live by github-readme-stats on GitHub.</p>
    </a>
    <a class="stat" href="https://github.com/DeepakAmalWinstarJ" target="_blank" rel="noopener" style="text-decoration:none;max-width:350px">
      <h5>Top Languages</h5><p>Language breakdown, also generated live on GitHub.</p>
    </a>
  </div>
  <div class="row">
    <a class="stat" href="https://github.com/DeepakAmalWinstarJ" target="_blank" rel="noopener" style="text-decoration:none;max-width:480px">
      <h5>GitHub Streak</h5><p>Current and longest streak are computed live from your contribution graph.</p>
    </a>
  </div>

  <!-- quote (recreated from assets/quote.svg) -->
  <svg viewBox="0 0 720 90" role="img" aria-label="Code and Art Quote" style="width:100%;max-width:720px;margin-top:8px">
    <rect width="720" height="90" rx="10" fill="#0a0a0a" stroke="#ef4444" stroke-opacity=".5"/>
    <text x="360" y="52" text-anchor="middle" fill="#fca5a5" font-size="17" font-family="ui-monospace,Menlo,monospace">Driven by curiosity. Building for impact.</text>
  </svg>

  <hr>

  <h2>⚡ Contribution Journey</h2>
  <div class="snake">
    <canvas id="snake" width="760" height="120" aria-label="Animated snake crossing a contribution grid"></canvas>
  </div>
  <p class="note">A decorative stand-in. The real snake is generated from your actual contributions by a GitHub Action.</p>

  <hr>

  <h2>📬 Let's Connect &amp; Collaborate</h2>
  <p class="muted"><i>Whether you want to discuss system architecture, explore open-source collaboration, or just say hello — my inbox is always open!</i></p>
  <table class="grid" style="max-width:760px">
    <tr>
      <td style="width:33%"><a href="https://www.linkedin.com/in/aadhithiya-p-4700393b3/" target="_blank" rel="noopener"><div style="font-size:2rem">💼</div><span class="badge"><span class="l">LinkedIn</span><span class="r">Connect</span></span></a><br><sub><b>Professional Network</b></sub></td>
      <td style="width:33%"><a href="https://www.instagram.com/itz__adhix?stkn=cXdhZGI0cGcxZjll" target="_blank" rel="noopener"><div style="font-size:2rem">📸</div><span class="badge"><span class="l">Instagram</span><span class="r">@itz_aadhix</span></span></a><br><sub><b>Articles &amp; Tech Guides</b></sub></td>
      <td style="width:33%"><a href="mailto:aadthif@gmail.com"><div style="font-size:2rem">✉️</div><span class="badge"><span class="l">Email</span><span class="r">Contact Me</span></span></a><br><sub><b>Direct Collaboration</b></sub></td>
    </tr>
  </table>

  <!-- footer (recreated from assets/footer.svg) -->
  <svg viewBox="0 0 900 90" role="img" aria-label="Footer" style="width:100%;border-radius:12px;margin-top:8px">
    <defs><linearGradient id="fg" x1="0" x2="1"><stop offset="0" stop-color="#7f1d1d"/><stop offset="1" stop-color="#0a0a0a"/></linearGradient></defs>
    <rect width="900" height="90" fill="url(#fg)"/>
    <text x="450" y="52" text-anchor="middle" fill="#fff" font-size="16" font-family="ui-monospace,Menlo,monospace">Thank you for visiting </text>
  </svg>
</div>

<script>
(function(){
  var reduce = window.matchMedia && matchMedia('(prefers-reduced-motion: reduce)').matches;

  // Typing effect (cycling lines like the typing-svg)
  function typer(el, lines, loop){
    var li=0, ci=0, del=false;
    if(reduce){ el.textContent = lines[0]; return; }
    (function tick(){
      var cur = lines[li];
      el.textContent = cur.slice(0,ci);
      var delay = del ? 28 : 65;
      if(!del && ci===cur.length){
        if(!loop && li===lines.length-1) return;
        del=true; delay=1400;
      } else if(del && ci===0){
        del=false; li=(li+1)%lines.length; delay=300;
      } else { ci += del ? -1 : 1; }
      setTimeout(tick, delay);
    })();
  }
  typer(document.querySelector('#typing1 .t'), [
    "Hi there! I'm P Aadhithiya 👋",
    "B.Tech AI&DS Engineer & Developer 🎓",
    "Full-Stack 💻",
    "AI, Machine Learning   🤖",
    "Turning random ideas into production code ⚡"
  ], true);
  typer(document.getElementById('quote'), ["Driven by curiosity. Building for impact. Coding the future."], false);

  // Code window typing
  var code = document.getElementById('code');
  var src = [
    '<span class="c">//  Aadhi.js</span>',
    '<span class="k">const</span> dev = {',
    '  name: <span class="s">"P Aadhithiya"</span>,',
    '  focus: [<span class="s">"Full Stack"</span>, <span class="s">"AI"</span>],',
    '  status: <span class="s">"Building &amp; Shipping"</span>',
    '};'
  ];
  if(reduce){ code.innerHTML = src.join('\n'); }
  else {
    var n=0; (function add(){ if(n<src.length){ code.innerHTML = src.slice(0,++n).join('\n'); setTimeout(add,650);} })();
  }

  // Contribution snake stand-in
  var cv = document.getElementById('snake'), ctx = cv.getContext('2d');
  var cols=52, rows=7, size=11, gap=3, ox=20, oy=12;
  var seed=7; function rnd(){ seed=(seed*9301+49297)%233280; return seed/233280; }
  var cells=[]; for(var x=0;x<cols;x++){ for(var y=0;y<rows;y++){ cells.push({x:x,y:y,l:Math.floor(rnd()*4.2)}); } }
  var shades=['#1a1212','#5b1a1a','#9b1f1f','#ef4444','#fca5a5'];
  var path=[]; for(var x2=0;x2<cols;x2++){ for(var yy=0;yy<rows;yy++){ path.push({x:x2,y:(x2%2===0)?yy:rows-1-yy}); } }
  var head=0, eaten={};
  function draw(){
    ctx.clearRect(0,0,cv.width,cv.height);
    cells.forEach(function(c){
      var k=c.x+','+c.y; var lv = eaten[k]?0:c.l;
      ctx.fillStyle = shades[lv];
      ctx.fillRect(ox+c.x*(size+gap), oy+c.y*(size+gap), size, size);
    });
    ctx.fillStyle='#ef4444';
    for(var i=0;i<10;i++){
      var p=path[(head-i+path.length)%path.length];
      ctx.globalAlpha = 1 - i*0.08;
      ctx.fillRect(ox+p.x*(size+gap)-1, oy+p.y*(size+gap)-1, size+2, size+2);
    }
    ctx.globalAlpha=1;
  }
  function step(){
    var p=path[head]; eaten[p.x+','+p.y]=true;
    head++; if(head>=path.length){ head=0; eaten={}; }
    draw();
  }
  draw();
  if(!reduce) setInterval(step, 45);
})();
</script>
</body>
</html>

