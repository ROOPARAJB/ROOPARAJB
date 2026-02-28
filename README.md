<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1"/>
<title>ROOPARAJB — GitHub Profile</title>
<link href="https://fonts.googleapis.com/css2?family=Share+Tech+Mono&family=VT323&display=swap" rel="stylesheet"/>
<style>
*{margin:0;padding:0;box-sizing:border-box;}
:root{--g:#00ff41;--dg:#00cc33;--bg:#000;--border:#003300;--muted:#005500;--dim:#050f05;}
body{background:var(--bg);color:var(--g);font-family:'Share Tech Mono',monospace;min-height:100vh;overflow-x:hidden;}
#matrix-canvas{position:fixed;top:0;left:0;width:100%;height:100%;z-index:0;opacity:0.06;pointer-events:none;}
body::after{content:'';position:fixed;inset:0;background:repeating-linear-gradient(0deg,transparent,transparent 2px,rgba(0,0,0,0.04) 2px,rgba(0,0,0,0.04) 4px);pointer-events:none;z-index:1;}

/* browser bar */
.bar{position:relative;z-index:10;background:#050505;border-bottom:1px solid var(--border);padding:8px 16px;display:flex;align-items:center;gap:10px;}
.dots{display:flex;gap:5px;}
.dot{width:11px;height:11px;border-radius:50%;}
.dot.r{background:#ff5f57;}.dot.y{background:#febc2e;}.dot.g{background:#28c840;}
.url{flex:1;text-align:center;background:#0a0a0a;border:1px solid var(--border);border-radius:4px;padding:3px 12px;color:var(--dg);font-size:11px;}

.page{position:relative;z-index:5;max-width:760px;margin:0 auto;padding:0 28px 60px;}

/* HERO */
.hero{text-align:center;padding:52px 0 24px;}
.hero h1{font-family:'VT323',monospace;font-size:72px;letter-spacing:8px;color:var(--g);text-shadow:0 0 20px var(--g),0 0 60px rgba(0,255,65,0.3);animation:flicker 5s infinite;}
.hero .title{font-size:12px;color:var(--dg);letter-spacing:4px;margin-top:6px;}
@keyframes flicker{0%,94%,100%{opacity:1;}95%{opacity:0.6;}96%{opacity:1;}97%{opacity:0.4;}98%{opacity:1;}99%{opacity:0.8;}}

/* TERMINAL */
.terminal{background:var(--dim);border:1px solid var(--border);border-radius:4px;padding:16px 20px;margin:24px 0 28px;font-size:13px;line-height:2.1;}
.p{color:var(--muted);}
.cursor{display:inline-block;width:8px;height:14px;background:var(--g);animation:blink 1s step-end infinite;vertical-align:middle;}
@keyframes blink{50%{opacity:0;}}

/* CHIPS */
.chips{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:32px;}
.chip{padding:5px 13px;border:1px solid var(--border);border-radius:3px;font-size:11px;color:var(--dg);letter-spacing:1px;background:var(--dim);}
.chip.hot{border-color:var(--g);color:var(--g);}

/* DIVIDER */
hr{border:none;border-top:1px solid var(--border);margin:28px 0;}

/* SECTION LABEL */
.label{font-size:10px;color:var(--muted);letter-spacing:3px;text-transform:uppercase;margin-bottom:14px;}

/* SKILLS */
.skill-row{display:flex;align-items:baseline;gap:0;margin-bottom:10px;font-size:12px;}
.skill-cat{color:var(--muted);min-width:100px;font-size:11px;letter-spacing:1px;}
.tags{display:flex;flex-wrap:wrap;gap:6px;}
.tag{padding:3px 11px;border:1px solid var(--border);border-radius:2px;color:#aaffcc;font-size:11px;background:var(--dim);}
.tag.hi{border-color:#00aa33;color:var(--g);}

/* CONNECT */
.connect{display:flex;gap:10px;flex-wrap:wrap;}
.cbadge{padding:8px 18px;border:1px solid var(--border);border-radius:3px;font-size:11px;color:var(--dg);letter-spacing:1px;background:var(--dim);transition:border-color 0.2s,color 0.2s;cursor:default;}
.cbadge:hover{border-color:var(--g);color:var(--g);}

/* ACHIEVEMENTS */
.ach{font-size:13px;line-height:2.4;}
.ach div::before{content:'[★] ';color:#aacc00;}
.ach div{color:#aaffcc;}

/* FOOTER */
.footer{text-align:center;padding:44px 0 0;font-size:11px;color:var(--muted);letter-spacing:1px;}
</style>
</head>
<body>

<canvas id="matrix-canvas"></canvas>

<div class="bar">
  <div class="dots"><div class="dot r"></div><div class="dot y"></div><div class="dot g"></div></div>
  <div class="url">🔒 github.com/ROOPARAJB</div>
</div>

<div class="page">

  <!-- HERO -->
  <div class="hero">
    <h1>ROOPARAJ B</h1>
    <div class="title">SECURITY ANALYST · CHENNAI</div>
  </div>

  <!-- TERMINAL -->
  <div class="terminal">
    <span class="p">~$ </span>whoami<br/>
    <span style="color:#aaffcc">Cybersecurity grad · Penetration tester · SOC builder · CEH V13 Elite</span><br/><br/>
    <span class="p">~$ </span>status<br/>
    <span style="color:var(--g)">Analyst Trainee @ Finstein, Chennai</span> <span class="cursor"></span>
  </div>

  <!-- CHIPS -->
  <div class="chips">
    <span class="chip hot">⚔️ TryHackMe Top 2%</span>
    <span class="chip">🎓 B.E. Cyber Security · 2025</span>
    <span class="chip">📍 Chennai, India</span>
  </div>

  <hr/>

  <!-- SKILLS -->
  <div class="label">// skills</div>
  <div class="skill-row"><span class="skill-cat">Offensive</span><div class="tags"><span class="tag hi">Metasploit</span><span class="tag hi">Burp Suite</span><span class="tag">Nmap</span><span class="tag">OSINT</span></div></div>
  <div class="skill-row"><span class="skill-cat">Defensive</span><div class="tags"><span class="tag hi">Splunk</span><span class="tag">Snort IDS</span><span class="tag">Sophos XDR</span><span class="tag">Wireshark</span></div></div>
  <div class="skill-row"><span class="skill-cat">Dev</span><div class="tags"><span class="tag">Python</span><span class="tag">Java</span></div></div>
  <div class="skill-row"><span class="skill-cat">OS</span><div class="tags"><span class="tag">Kali Linux</span><span class="tag">Windows</span></div></div>

  <hr/>

  <!-- ACHIEVEMENTS -->
  <div class="label">// achievements</div>
  <div class="ach">
    <div>TryHackMe — Top 2% globally</div>
    <div>Haunted Network CTF — Techbyheart</div>
  </div>

  <hr/>

  <!-- CONNECT -->
  <div class="label">// connect</div>
  <div class="connect">
    <a href="https://linkedin.com/in/rooparajb" style="text-decoration:none"><span class="cbadge">🔗 linkedin / rooparajb</span></a>
    <a href="https://tryhackme.com/p/ROOPARAJ" style="text-decoration:none"><span class="cbadge">⚔️ tryhackme / ROOPARAJ</span></a>
    <a href="mailto:ragulbalasundaram@gmail.com" style="text-decoration:none"><span class="cbadge">📧 ragulbalasundaram@gmail.com</span></a>
  </div>

  <div class="footer">
    &lt;/&gt; &nbsp;"The quieter you become, the more you are able to hear." — Kali Linux
  </div>

</div>

<script>
const canvas = document.getElementById('matrix-canvas');
const ctx = canvas.getContext('2d');
canvas.width = window.innerWidth; canvas.height = window.innerHeight;
const chars = 'アイウエオ0123456789ABCDEF<>/|{}';
const fs = 13, cols = Math.floor(canvas.width / fs);
const drops = Array(cols).fill(1);
function draw(){
  ctx.fillStyle='rgba(0,0,0,0.05)'; ctx.fillRect(0,0,canvas.width,canvas.height);
  ctx.fillStyle='#00ff41'; ctx.font=fs+'px monospace';
  drops.forEach((y,i)=>{
    ctx.fillText(chars[Math.floor(Math.random()*chars.length)],i*fs,y*fs);
    if(y*fs>canvas.height&&Math.random()>0.975) drops[i]=0;
    drops[i]++;
  });
}
setInterval(draw,40);
window.addEventListener('resize',()=>{canvas.width=window.innerWidth;canvas.height=window.innerHeight;});
</script>
</body>
</html>
