<!DOCTYPE html>
<html lang="en" translate="no" class="notranslate">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="google" content="notranslate">
<meta http-equiv="Content-Language" content="en">
<title>ENGLISH EXAM, 10TH GRADE - DESCRIPTIVE - PEOPLE</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:opsz,wght@9..144,500;9..144,600;9..144,700&family=Inter:wght@400;500;600;700;800&family=JetBrains+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#1c1b22;
    --paper:#f6f4ee;
    --paper-card:#ffffff;
    --line:#e4e1d6;
    --muted:#7b7768;
    --navy:#161a2e;
    --cream:#f3ead9;
    --good:#1f9d68;
    --good-bg:#e7f6ee;
    --bad:#d5473a;
    --bad-bg:#fceceb;

    --t1:#7c5cd6;
    --t1-bg:#f2eefb;
    --t2:#0e9488;
    --t2-bg:#e9f7f5;
    --t3:#c98a1f;
    --t3-bg:#fbf1de;
    --t4:#d1477a;
    --t4-bg:#fbeaf1;
  }

  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--paper);
    color:var(--ink);
    font-family:'Inter',system-ui,sans-serif;
    line-height:1.55;
    padding-bottom:96px;
    -webkit-user-select:none;
    -moz-user-select:none;
    -ms-user-select:none;
    user-select:none;
    -webkit-touch-callout:none;
  }
  input, textarea, select{
    -webkit-user-select:text;
    -moz-user-select:text;
    -ms-user-select:text;
    user-select:text;
  }
  img{ -webkit-user-drag:none; pointer-events:none; }

  h1,h2,h3{font-family:'Fraunces',Georgia,serif;margin:0;}
  .wrap{max-width:820px;margin:0 auto;padding:0 20px;}

  .cover{
    background:var(--navy); color:var(--cream);
    padding:40px 0 30px; border-bottom:6px solid var(--t1);
  }
  .eyebrow{
    font-family:'JetBrains Mono',monospace; font-size:12px;
    letter-spacing:.14em; text-transform:uppercase; color:#a9a6c4; margin-bottom:10px;
  }
  .cover h1{
    font-size:clamp(24px,4.2vw,32px); font-weight:600; line-height:1.18; max-width:640px;
  }
  .cover p.desc{ color:#c9c6da; max-width:560px; margin-top:12px; font-size:14.5px; }
  .id-card{
    margin-top:22px; background:rgba(255,255,255,.06); border:1px solid rgba(255,255,255,.16);
    border-radius:14px; padding:16px 18px; display:grid; grid-template-columns:1fr 1fr; gap:14px;
  }
  @media (max-width:520px){ .id-card{grid-template-columns:1fr;} }
  .id-field label{
    display:block; font-family:'JetBrains Mono',monospace; font-size:11px;
    letter-spacing:.08em; text-transform:uppercase; color:#a9a6c4; margin-bottom:6px;
  }
  .id-field input{
    width:100%; background:rgba(255,255,255,.08); border:1px solid rgba(255,255,255,.2);
    border-radius:8px; padding:10px 12px; color:#fff; font-size:16px; font-family:'Inter',sans-serif; outline:none;
  }
  .id-field input::placeholder{color:#8b88a3;}
  .id-field input:focus{border-color:var(--t3);background:rgba(255,255,255,.13);}

  .progress-shell{
    position:sticky; top:0; z-index:30; background:var(--paper);
    border-bottom:1px solid var(--line); padding:10px 0;
  }
  .progress-inner{ display:flex; align-items:center; gap:12px; flex-wrap:wrap; }
  .progress-track{ flex:1 1 140px; height:8px; background:var(--line); border-radius:99px; overflow:hidden; min-width:100px; }
  .progress-fill{ height:100%; width:0%; background:linear-gradient(90deg,var(--t1),var(--t4)); transition:width .3s ease; }
  .progress-label{ font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--muted); white-space:nowrap; }
  .palette-toggle{
    font-family:'Inter',sans-serif; font-size:12.5px; font-weight:600;
    background:#fff; border:1px solid var(--line); color:var(--ink);
    padding:6px 12px; border-radius:99px; cursor:pointer;
    transition:background .15s ease, border-color .15s ease;
    display:flex; align-items:center; gap:6px;
  }
  .palette-toggle:hover{background:#f3f1ea; border-color:#d7d3c4;}

  .timer-badge{
    font-family:'JetBrains Mono',monospace; font-size:13px; font-weight:700; color:var(--ink);
    background:#eef0fb; border:1px solid #c9cdf0; padding:6px 12px; border-radius:99px; white-space:nowrap;
  }
  .timer-badge.warn{background:var(--t3-bg); border-color:var(--t3); color:#7a4e0a;}
  .timer-badge.danger{background:var(--bad-bg); border-color:var(--bad); color:var(--bad); animation:timerPulse 1s infinite;}
  .timer-badge.paused{background:#fff3cd; border-color:#ffeeba; color:#856404;}
  @keyframes timerPulse{ 0%,100%{opacity:1;} 50%{opacity:.55;} }

  .online-badge{
    font-family:'JetBrains Mono',monospace; font-size:12.5px; font-weight:700;
    padding:6px 12px; border-radius:99px; white-space:nowrap; display:flex; align-items:center; gap:6px;
  }
  .online-badge .online-dot{ width:8px; height:8px; border-radius:50%; display:inline-block; flex:none; }
  .online-badge.online{ background:var(--good-bg); border:1px solid var(--good); color:var(--good); }
  .online-badge.online .online-dot{ background:var(--good); animation:onlinePulse 1.6s infinite; }
  .online-badge.offline{ background:var(--bad-bg); border:1px solid var(--bad); color:var(--bad); }
  .online-badge.offline .online-dot{ background:var(--bad); }
  @keyframes onlinePulse{ 0%,100%{opacity:1;} 50%{opacity:.4;} }

  .palette-panel{
    display:none; background:var(--paper-card); border:1px solid var(--line); border-radius:12px;
    padding:16px; margin-top:14px;
  }
  .palette-panel.open{display:block;}
  .palette-legend{
    display:flex; gap:14px; flex-wrap:wrap; font-size:11.5px; color:var(--muted);
    margin-bottom:12px; font-family:'JetBrains Mono',monospace;
  }
  .palette-legend span{display:inline-flex; align-items:center; gap:5px;}
  .legend-dot{width:9px; height:9px; border-radius:3px; display:inline-block;}
  .palette-grid{ display:grid; grid-template-columns:repeat(auto-fill,minmax(38px,1fr)); gap:8px; }
  .pnum{
    aspect-ratio:1; border-radius:8px; border:1.5px solid var(--line); background:#fff;
    font-family:'JetBrains Mono',monospace; font-size:13px; font-weight:700; color:var(--muted);
    cursor:pointer; display:flex; align-items:center; justify-content:center; transition:transform .1s ease;
  }
  .pnum:hover{transform:translateY(-1px);}
  .pnum.pn-current{border-color:var(--navy); border-width:2px; color:var(--navy);}
  .pnum.pn-answered{background:#eef0fb; border-color:#c9cdf0; color:var(--navy);}
  .pnum.pn-correct{background:var(--good-bg); border-color:var(--good); color:var(--good);}
  .pnum.pn-incorrect{background:var(--bad-bg); border-color:var(--bad); color:var(--bad);}

  .results{
    display:none; background:var(--paper-card); border:1px solid var(--line); border-radius:14px;
    padding:24px 26px; margin:24px 0 6px; text-align:center;
  }
  .results.show{display:block;}
  .results .score-big{ font-family:'Fraunces',serif; font-size:48px; font-weight:700; line-height:1; color:var(--navy); margin-bottom:6px; }
  .results .score-sub{color:var(--muted); font-size:14px; margin-bottom:14px;}
  .results .score-msg{ font-size:15px; font-weight:600; padding:9px 16px; border-radius:99px; display:inline-block; }
  .submit-row{margin-top:18px; display:flex; flex-direction:column; align-items:center; gap:8px;}
  .submit-row .primary{padding:12px 22px; font-size:14.5px;}
  .submit-row .primary:disabled{opacity:.55; cursor:not-allowed; transform:none;}
  .send-note{font-family:'JetBrains Mono',monospace; font-size:12.5px; min-height:16px;}
  .send-note.ok{color:var(--good);}
  .send-note.err{color:var(--bad);}
  .retry-send{border-color:var(--bad); color:var(--bad);}
  .retry-send:hover{background:var(--bad-bg);}

  .stage{margin-top:22px;}
  .stage-head{ display:flex; align-items:center; justify-content:space-between; gap:10px; margin-bottom:14px; flex-wrap:wrap; }
  .genre-tag{
    font-family:'JetBrains Mono',monospace; font-size:11.5px; letter-spacing:.09em; text-transform:uppercase;
    padding:5px 11px; border-radius:99px; font-weight:600;
  }
  .stage-index{ font-family:'JetBrains Mono',monospace; font-size:12.5px; color:var(--muted); }

  .passage{
    background:var(--paper-card); border:1px solid var(--line); border-left-width:5px;
    border-radius:10px; padding:20px 22px; margin-bottom:20px; font-size:14.5px;
  }
  .passage h3{font-size:17px; margin-bottom:10px; font-weight:600;}
  .passage p{margin:0 0 11px; color:#33313c;}
  .passage p:last-child{margin-bottom:0;}
  .passage .meta{
    font-family:'JetBrains Mono',monospace; font-size:11.5px; color:var(--muted); margin-bottom:12px; letter-spacing:.03em;
  }

  .q-card{
    background:var(--paper-card); border:1px solid var(--line); border-radius:12px;
    padding:20px 22px 22px; transition:border-color .2s ease, box-shadow .2s ease;
  }
  .q-card.correct{border-color:var(--good); box-shadow:0 0 0 1px var(--good);}
  .q-card.incorrect{border-color:var(--bad); box-shadow:0 0 0 1px var(--bad);}

  .q-top{display:flex; gap:12px; align-items:flex-start; margin-bottom:14px;}
  .q-num{
    font-family:'JetBrains Mono',monospace; font-weight:700; font-size:14px;
    min-width:32px; height:32px; border-radius:99px; display:flex; align-items:center; justify-content:center; flex-shrink:0;
  }
  .q-prompt{font-size:16px; font-weight:600; padding-top:4px;}
  .q-hint{ font-size:12px; color:var(--muted); font-style:italic; margin:-6px 0 12px 44px; }

  .options{display:flex; flex-direction:column; gap:9px; margin-left:44px;}
  .opt{
    display:flex; align-items:flex-start; gap:10px; padding:10px 13px; border:1px solid var(--line); border-radius:8px;
    cursor:pointer; font-size:14.5px; background:#fff; transition:background .15s ease, border-color .15s ease;
  }
  .opt:hover{background:#faf9f5;}
  .opt input{margin-top:3px; accent-color:currentColor; flex-shrink:0;}
  .opt.selected{background:#f1eefc; border-color:var(--t1);}
  .opt.opt-correct{background:var(--good-bg); border-color:var(--good);}
  .opt.opt-wrong{background:var(--bad-bg); border-color:var(--bad);}
  .opt .tag{
    margin-left:auto; font-family:'JetBrains Mono',monospace; font-size:10.5px;
    text-transform:uppercase; letter-spacing:.05em; font-weight:700; padding-left:8px;
  }
  .opt.opt-correct .tag{color:var(--good);}
  .opt.opt-wrong .tag{color:var(--bad);}
  .opt input:disabled{cursor:default;}
  .opt.locked{cursor:default;}

  @media (max-width:640px){
    .stage{margin-top:16px;}
    .passage{padding:16px; font-size:15.5px; line-height:1.6;}
    .passage h3{font-size:16.5px;}
    .q-card{padding:16px 14px 18px;}
    .q-top{gap:10px; margin-bottom:12px;}
    .q-num{min-width:28px; height:28px; font-size:13px;}
    .q-prompt{font-size:15.5px; line-height:1.42;}
    .q-hint{margin-left:0; margin-top:2px; line-height:1.4;}
    .options{margin-left:0; gap:8px;}
    .opt{padding:11px 12px; font-size:15px; line-height:1.4; gap:9px;}
    .matrix{margin-left:0;}
    .match-box{margin-left:0;}
    .answer-note{margin-left:0;}
  }

  .matrix{margin-left:44px; border:1px solid var(--line); border-radius:8px; overflow:hidden;}
  .matrix table{width:100%; border-collapse:collapse; font-size:14px;}
  .matrix th{
    font-family:'JetBrains Mono',monospace; font-size:10.5px; text-transform:uppercase; letter-spacing:.06em;
    color:var(--muted); background:#faf9f5; padding:9px 10px; text-align:center; border-bottom:1px solid var(--line);
  }
  .matrix th:first-child{text-align:left;}
  .matrix td{padding:10px; border-bottom:1px solid var(--line); vertical-align:middle;}
  .matrix tr:last-child td{border-bottom:none;}
  .matrix td.stmt{color:#33313c;}
  .matrix td.pick{text-align:center; width:90px;}
  .matrix td.pick.right-cell{background:var(--good-bg);}
  .matrix td.pick.wrong-cell{background:var(--bad-bg);}
  .matrix input{accent-color:currentColor;}

  .match-box{margin-left:44px; border:1px solid var(--line); border-radius:8px; overflow:hidden;}
  .match-box table{width:100%; border-collapse:collapse; font-size:14px;}
  .match-box th{
    font-family:'JetBrains Mono',monospace; font-size:10.5px; text-transform:uppercase; letter-spacing:.06em;
    color:var(--muted); background:#faf9f5; padding:9px 10px; text-align:left; border-bottom:1px solid var(--line);
  }
  .match-box td{padding:10px; border-bottom:1px solid var(--line); vertical-align:middle;}
  .match-box tr:last-child td{border-bottom:none;}
  .match-box td.word{color:#33313c; font-weight:600; width:150px;}
  .match-box select{
    width:100%; padding:8px 10px; border-radius:8px; border:1px solid var(--line); font-family:'Inter',sans-serif;
    font-size:14px; background:#fff; color:var(--ink);
  }
  .match-box tr.right-row td.word{background:var(--good-bg);}
  .match-box tr.wrong-row td.word{background:var(--bad-bg);}
  .match-choices{margin:10px 0 0 44px; font-size:12.5px; color:var(--muted);}
  .match-choices div{margin-bottom:2px;}

  .answer-note{
    margin:12px 0 0 44px; font-size:13px; padding:9px 12px; border-radius:8px;
    background:var(--bad-bg); color:#8a2e26; display:none;
  }
  .answer-note.show{display:block;}
  .answer-note b{color:var(--bad);}

  .nav-bar{
    position:fixed; bottom:0; left:0; right:0; z-index:40;
    background:var(--navy); border-top:1px solid rgba(255,255,255,.1); padding:8px 0;
  }
  .nav-inner{ display:flex; align-items:center; justify-content:space-between; gap:8px; flex-wrap:wrap; }
  .nav-status{color:#c9c6da; font-size:11px; font-family:'JetBrains Mono',monospace;}
  .nav-btns{display:flex; gap:6px; align-items:center; flex-wrap:wrap;}
  button.navbtn{
    background:rgba(255,255,255,.08); color:#fff; border:1px solid rgba(255,255,255,.2);
    padding:7px 12px; border-radius:99px; font-size:12.5px; cursor:pointer;
    font-family:'Inter',sans-serif; font-weight:600; transition:background .15s ease;
  }
  button.navbtn:hover{background:rgba(255,255,255,.16);}
  button.navbtn:disabled{opacity:.35; cursor:not-allowed;}
  button.primary{
    background:var(--t3); color:#241a05; border:none; font-weight:700;
    padding:7px 14px; border-radius:99px; font-size:12.5px; cursor:pointer;
    font-family:'Inter',sans-serif; transition:transform .12s ease, background .15s ease;
  }
  button.primary:hover{transform:translateY(-1px); background:#dc9b28;}
  button.primary:disabled{opacity:.5; cursor:not-allowed; transform:none;}
  button.ghost{
    background:transparent; color:#c9c6da; border:1px solid rgba(255,255,255,.25);
    padding:7px 12px; border-radius:99px; font-size:12.5px; cursor:pointer; font-family:'Inter',sans-serif;
  }
  button.ghost:hover{border-color:rgba(255,255,255,.5); color:#fff;}

  @media (max-width:480px){
    body{padding-bottom:118px;}
    .nav-bar{padding:6px 0;}
    .nav-inner{gap:6px;}
    .nav-status{font-size:10px; width:100%; text-align:center; order:-1;}
    .nav-btns{width:100%; justify-content:space-between; gap:5px;}
    button.navbtn, button.primary, button.ghost{ padding:6px 9px; font-size:11px; flex:1; text-align:center; }
  }

  ::selection{background:var(--cream);}

  .gate-screen{
    position:fixed; inset:0; z-index:100; background:var(--navy);
    display:flex; align-items:center; justify-content:center; padding:24px;
  }
  .gate-card{
    background:rgba(255,255,255,.06); border:1px solid rgba(255,255,255,.16); border-radius:16px;
    padding:28px 26px; max-width:400px; width:100%; color:var(--cream);
  }
  .gate-card h1{ font-size:21px; font-weight:600; color:var(--cream); margin:6px 0 8px; line-height:1.3; }
  .gate-card .desc{color:#c9c6da; font-size:14px; margin:0 0 18px;}
  .gate-field{margin-bottom:14px;}
  .gate-field label{
    display:block; font-family:'JetBrains Mono',monospace; font-size:11px;
    letter-spacing:.08em; text-transform:uppercase; color:#a9a6c4; margin-bottom:6px;
  }
  .gate-field input, .gate-field select{
    width:100%; background:rgba(255,255,255,.08); border:1px solid rgba(255,255,255,.2);
    border-radius:8px; padding:10px 12px; color:#fff; font-size:16px; font-family:'Inter',sans-serif; outline:none;
  }
  .gate-field select option{ background: var(--navy); color: #fff; }
  .gate-field input::placeholder{color:#8b88a3;}
  .gate-field input:focus, .gate-field select:focus{border-color:var(--t3);background:rgba(255,255,255,.13);}

  /* Confirmation Modal */
  .confirm-modal{
    position:fixed; inset:0; z-index:200; background:rgba(15, 18, 30, 0.75);
    display:none; align-items:center; justify-content:center; padding:20px;
    backdrop-filter: blur(4px);
  }
  .confirm-modal.show{ display:flex; }
  .confirm-card{
    background:var(--paper-card); border:1px solid var(--line); border-radius:16px;
    padding:24px 26px; max-width:420px; width:100%; box-shadow:0 20px 25px -5px rgba(0,0,0,0.2);
    text-align:center;
  }
  .confirm-card h2{ font-size:20px; font-weight:700; color:var(--navy); margin-bottom:10px; }
  .confirm-card p{ font-size:14.5px; color:var(--muted); margin-bottom:20px; line-height:1.5; }
  .confirm-actions{ display:flex; gap:10px; justify-content:center; }
  .confirm-actions button{ flex:1; padding:10px 16px; font-size:14px; border-radius:99px; font-weight:600; cursor:pointer; font-family:'Inter',sans-serif; }
  .btn-cancel{ background:var(--paper); border:1px solid var(--line); color:var(--ink); }
  .btn-cancel:hover{ background:#e8e5dc; }
  .btn-confirm{ background:var(--good); border:none; color:#fff; }
  .btn-confirm:hover{ background:#198256; }

  .gate-error{ color:#ff8c82; font-size:13px; min-height:18px; margin-bottom:6px; font-family:'JetBrains Mono',monospace; }
  .gate-card .primary{width:100%; margin-top:6px;}
</style>
</head>
<body>

<div id="gateScreen" class="gate-screen">
  <div class="gate-card">
    <div class="eyebrow">Descriptive Text · People</div>
    <h1>ENGLISH EXAM, 10TH GRADE - DESCRIPTIVE - PEOPLE</h1>
    <p class="desc">Fill in your name, select class, and enter token to start.</p>
    <div class="gate-field">
      <label for="gateName">Name</label>
      <input id="gateName" type="text" placeholder="Write your full name" autocomplete="off">
    </div>
    <div class="gate-field">
      <label for="gateClass">Select Class</label>
      <select id="gateClass">
        <option value="">-- Choose Class --</option>
        <option value="X-I">X-I</option>
        <option value="X-J">X-J</option>
        <option value="X-K">X-K</option>
      </select>
    </div>
    <div class="gate-field">
      <label for="gateToken">Exam Token</label>
      <input id="gateToken" type="text" placeholder="Enter token (e.g. TK----)" autocomplete="off" style="text-transform:uppercase;">
    </div>
    <div class="gate-error" id="gateError"></div>
    <button class="primary" id="gateSubmitBtn" type="button">Start Exam</button>
  </div>
</div>

<!-- Modal Konfirmasi Submit -->
<div id="confirmModal" class="confirm-modal">
  <div class="confirm-card">
    <h2>Submit Exam Confirmation</h2>
    <p id="confirmMsg">Are you sure you want to submit your answers? You cannot change them after submission.</p>
    <div class="confirm-actions">
      <button type="button" class="btn-cancel" id="cancelSubmitBtn">Cancel</button>
      <button type="button" class="btn-confirm" id="confirmSubmitBtn">Yes, Submit Now</button>
    </div>
  </div>
</div>

<div id="appMain" style="display:none;">

<input type="hidden" id="stuName">
<input type="hidden" id="stuClass">

<div class="progress-shell">
  <div class="wrap progress-inner">
    <button type="button" class="palette-toggle" id="backToLoginBtn"><span>&larr; Login Menu</span></button>
    <div class="online-badge online" id="onlineBadge"><span class="online-dot"></span>Online</div>
    <div class="timer-badge" id="timerBadge">90:00</div>
    <div class="progress-track"><div class="progress-fill" id="progressFill"></div></div>
    <div class="progress-label" id="progressLabel">0 / 30 answered</div>
    <button type="button" class="palette-toggle" id="paletteToggleBtn"><span>Show all numbers</span></button>
  </div>
  <div class="wrap">
    <div class="palette-panel" id="palettePanel">
      <div class="palette-legend">
        <span><span class="legend-dot" style="background:#fff;border:1.5px solid var(--line);"></span>Not answered</span>
        <span><span class="legend-dot" style="background:#eef0fb;border:1.5px solid #c9cdf0;"></span>Answered</span>
        <span><span class="legend-dot" style="background:var(--good-bg);border:1.5px solid var(--good);"></span>Correct (after check)</span>
        <span><span class="legend-dot" style="background:var(--bad-bg);border:1.5px solid var(--bad);"></span>Wrong (after check)</span>
      </div>
      <div class="palette-grid" id="paletteGrid"></div>
    </div>
  </div>
</div>

<div class="wrap">
  <div id="resultsBox" class="results">
    <div class="score-big" id="scoreBig">0%</div>
    <div class="score-sub" id="scoreSub">0 out of 0 points correct</div>
    <div class="score-msg" id="scoreMsg">—</div>
    <div class="submit-row">
      <div class="send-note" id="sendNote"></div>
      <button class="ghost retry-send" id="retrySendBtn" type="button" style="display:none;">Try Sending Again</button>
    </div>
  </div>

  <div class="stage" id="stage"></div>
</div>

<div class="nav-bar">
  <div class="wrap nav-inner">
    <button class="navbtn" id="prevBtn" type="button">&larr; Previous</button>
    <div class="nav-status" id="navStatus">Question 1 / 30</div>
    <div class="nav-btns">
      <button class="ghost" id="resetBtn" type="button">Reshuffle</button>
      <button class="navbtn" id="nextBtn" type="button">Next &rarr;</button>
      <button class="primary" id="submitBtn" type="button">Check &amp; Submit Answers</button>
    </div>
  </div>
</div>

</div>

<script>
const DATA = [
  {
    id:'text1',
    tag:'TEXT 1',
    color:'var(--t1)',
    bg:'var(--t1-bg)',
    title:`My Best Friend, Sarah`,
    meta:`Descriptive Text · People · Questions No. 1-7`,
    passage:[
      `My best friend's name is Sarah Putri. She is fourteen years old, and we have been friends since elementary school. Sarah is not very tall, but she has long, curly black hair and bright brown eyes. She usually wears a pair of round glasses because she is nearsighted. Her smile is warm, and it always makes people around her feel comfortable.`,
      `Sarah is a very kind and patient person. She never gets angry easily, even when her friends make mistakes. She is also extremely diligent; she always finishes her homework on time and studies hard for every test. Besides being hardworking, Sarah is also very creative. She loves drawing comic characters in her notebook during free time, and many of her friends ask her to draw their favorite characters too.`,
      `In her free time, Sarah enjoys reading mystery novels and playing badminton with her older brother. She dreams of becoming an illustrator one day, so she practices drawing almost every day after school. Sarah is also a good listener. Whenever I have a problem, she always takes the time to listen carefully and give helpful advice.`,
      `In my opinion, Sarah is the most amazing friend anyone could ever ask for. I feel very lucky to have her as my best friend, and I hope our friendship will last forever.`
    ],
    questions:[
      { id:'q1', no:1, type:'single', prompt:`According to the text, what does Sarah usually wear?`,
        options:[
          {k:'A',t:`Round glasses`},
          {k:'B',t:`A wide-brim hat`},
          {k:'C',t:`A backpack`},
          {k:'D',t:`Braces`},
          {k:'E',t:`A wristwatch`}
        ], correct:'A' },
      { id:'q2', no:2, type:'single', prompt:`Which word best describes Sarah's personality based on the text?`,
        options:[
          {k:'A',t:`Lazy and careless`},
          {k:'B',t:`Kind, patient, and diligent`},
          {k:'C',t:`Shy and quiet all the time`},
          {k:'D',t:`Rude to her friends`},
          {k:'E',t:`Impatient and easily angered`}
        ], correct:'B' },
      { id:'q3', no:3, type:'multi', prompt:`Which of the following are Sarah's hobbies, according to the text?`, hint:`Choose more than one answer!`,
        options:[
          {k:'A',t:`Reading mystery novels`},
          {k:'B',t:`Playing badminton`},
          {k:'C',t:`Playing the piano`},
          {k:'D',t:`Drawing comic characters`}
        ], correct:['A','B','D'] },
      { id:'q4', no:4, type:'matrix', prompt:`Read the following statements taken from the text. Decide whether each is a FACT or an OPINION.`,
        cols:['FACT','OPINION'],
        statements:[
          {t:`"Sarah is fourteen years old."`, correct:'FACT'},
          {t:`"Sarah is the most amazing friend anyone could ever ask for."`, correct:'OPINION'},
          {t:`"Sarah dreams of becoming an illustrator."`, correct:'FACT'}
        ] },
      { id:'q5', no:5, type:'single', prompt:`The word "diligent" in paragraph 2 is closest in meaning to...`,
        options:[
          {k:'A',t:`Lazy`},
          {k:'B',t:`Hardworking`},
          {k:'C',t:`Careless`},
          {k:'D',t:`Nervous`},
          {k:'E',t:`Forgetful`}
        ], correct:'B' },
      { id:'q6', no:6, type:'single', prompt:`Which outline best shows the order of information in the text?`,
        options:[
          {k:'A',t:`I. Physical appearance II. Personality III. Hobbies and dreams IV. Writer's feelings`},
          {k:'B',t:`I. Hobbies II. Physical appearance III. Personality IV. Writer's feelings`},
          {k:'C',t:`I. Writer's feelings II. Personality III. Physical appearance IV. Hobbies`},
          {k:'D',t:`I. Personality II. Hobbies III. Physical appearance IV. Writer's feelings`},
          {k:'E',t:`I. Physical appearance II. Hobbies III. Writer's feelings IV. Personality`}
        ], correct:'A' },
      { id:'q7', no:7, type:'single', prompt:`What is the writer's purpose in writing this text?`,
        options:[
          {k:'A',t:`To persuade readers to make friends with Sarah`},
          {k:'B',t:`To describe Sarah's physical appearance and personality`},
          {k:'C',t:`To retell a story about Sarah's childhood`},
          {k:'D',t:`To explain how to draw comic characters`},
          {k:'E',t:`To compare Sarah with another friend`}
        ], correct:'B' }
    ]
  },
  {
    id:'text2',
    tag:'TEXT 2',
    color:'var(--t2)',
    bg:'var(--t2-bg)',
    title:`Mr. Rudi, My Favorite Teacher`,
    meta:`Descriptive Text · People · Questions No. 8-15`,
    passage:[
      `Mr. Rudi is my English teacher at school, and he is definitely my favorite teacher. He is a tall man in his early forties, with short black hair that is starting to turn gray at the sides. He always wears neat batik shirts and a pair of dark-framed glasses. His deep voice and calm way of speaking make it easy for students to pay attention in class.`,
      `What I admire most about Mr. Rudi is his patience. He never gets angry when students ask the same question twice, and he always explains difficult grammar rules in a simple, fun way. He often uses games and short videos to make his lessons more interesting. Besides being patient, Mr. Rudi is also very disciplined; he always arrives at class exactly on time and expects his students to do the same.`,
      `Outside the classroom, Mr. Rudi is friendly and easygoing. He often jokes with students during break time, and he is always willing to give extra help to anyone who is struggling with their English. He has been teaching for almost fifteen years, and many former students still visit him to say thank you for his guidance.`,
      `I believe Mr. Rudi is one of the best teachers in our school. His passion for teaching and his caring attitude make every student feel motivated to learn English.`
    ],
    questions:[
      { id:'q8', no:8, type:'single', prompt:`How long has Mr. Rudi been teaching, according to the text?`,
        options:[
          {k:'A',t:`Five years`},
          {k:'B',t:`Ten years`},
          {k:'C',t:`Almost fifteen years`},
          {k:'D',t:`Twenty years`},
          {k:'E',t:`Two years`}
        ], correct:'C' },
      { id:'q9', no:9, type:'single', prompt:`Which of the following best describes Mr. Rudi's appearance?`,
        options:[
          {k:'A',t:`Short with curly red hair`},
          {k:'B',t:`Tall, with short black hair turning gray, and dark-framed glasses`},
          {k:'C',t:`Bald with a long beard`},
          {k:'D',t:`Young with braces on his teeth`},
          {k:'E',t:`Wears a suit and tie every day`}
        ], correct:'B' },
      { id:'q10', no:10, type:'multi', prompt:`According to the text, which of the following are Mr. Rudi's personality traits?`, hint:`Choose more than one answer!`,
        options:[
          {k:'A',t:`Patient`},
          {k:'B',t:`Disciplined`},
          {k:'C',t:`Lazy`},
          {k:'D',t:`Friendly`}
        ], correct:['A','B','D'] },
      { id:'q11', no:11, type:'matrix', prompt:`Read the following statements. Decide whether each is "Stated in the Text" or "Not Stated in the Text."`,
        cols:['STATED','NOT STATED'],
        statements:[
          {t:`Mr. Rudi always arrives at class exactly on time.`, correct:'STATED'},
          {t:`Mr. Rudi was born in Jakarta.`, correct:'NOT STATED'},
          {t:`Mr. Rudi uses games and short videos in his lessons.`, correct:'STATED'}
        ] },
      { id:'q12', no:12, type:'single', prompt:`The word "easygoing" in paragraph 3 most likely means...`,
        options:[
          {k:'A',t:`Strict and serious`},
          {k:'B',t:`Relaxed and friendly`},
          {k:'C',t:`Angry and impatient`},
          {k:'D',t:`Quiet and shy`},
          {k:'E',t:`Careless about rules`}
        ], correct:'B' },
      { id:'q13', no:13, type:'match', prompt:`Match each word from the text (Column A) with its correct meaning (Column B). Choose the correct letter for each word.`,
        items:[
          {t:`Patient`, correct:'b'},
          {t:`Disciplined`, correct:'a'},
          {t:`Easygoing`, correct:'c'}
        ],
        choices:[
          {k:'a', t:`Following rules and schedules strictly`},
          {k:'b', t:`Able to stay calm without complaining`},
          {k:'c', t:`Relaxed, calm, and friendly`}
        ] },
      { id:'q14', no:14, type:'single', prompt:`What is the main idea of the text?`,
        options:[
          {k:'A',t:`Mr. Rudi is strict and unfriendly to his students`},
          {k:'B',t:`Mr. Rudi is a patient, disciplined, and caring English teacher who is loved by his students`},
          {k:'C',t:`Mr. Rudi dislikes using technology in his lessons`},
          {k:'D',t:`Mr. Rudi has only been teaching for two years`},
          {k:'E',t:`Mr. Rudi rarely helps students outside class`}
        ], correct:'B' },
      { id:'q15', no:15, type:'single', prompt:`This text is an example of a descriptive text because it...`,
        options:[
          {k:'A',t:`Tells a chronological story about Mr. Rudi's life`},
          {k:'B',t:`Gives step-by-step instructions on how to teach English`},
          {k:'C',t:`Describes the physical appearance and characteristics of a particular person`},
          {k:'D',t:`Argues for a particular opinion about teaching methods`},
          {k:'E',t:`Retells a past experience with Mr. Rudi`}
        ], correct:'C' }
    ]
  },
  {
    id:'text3',
    tag:'TEXT 3',
    color:'var(--t3)',
    bg:'var(--t3-bg)',
    title:`Rani, the Young Badminton Champion`,
    meta:`Descriptive Text · People · Questions No. 16-23`,
    passage:[
      `Rani Anggraini is a sixteen-year-old badminton player from Surabaya, and she is well known in her school for her amazing skills on the court. She is of medium height, with a slim, athletic body built from years of intense training. Her short ponytail and bright, determined eyes make her easy to recognize during matches.`,
      `Rani started playing badminton when she was only six years old, taught by her father, who used to be a badminton coach. Since then, she has trained almost every single day, waking up at five in the morning before school to practice her footwork and smashes. Her hard work has paid off; she has already won several regional junior championships and hopes to represent Indonesia internationally one day.`,
      `Besides being talented, Rani is also humble and disciplined. She always thanks her coaches and teammates after every match, and she never boasts about her achievements. Her friends describe her as cheerful and supportive, always ready to help her teammates improve their skills.`,
      `Outside of badminton, Rani enjoys listening to music and spending time with her family. She believes that a balanced life, combining hard training with rest and family time, is the secret to her success. Many people in her school consider her a true inspiration, proving that dedication and discipline can help anyone achieve their dreams.`
    ],
    questions:[
      { id:'q16', no:16, type:'single', prompt:`According to the text, at what age did Rani start playing badminton?`,
        options:[
          {k:'A',t:`Four`},
          {k:'B',t:`Five`},
          {k:'C',t:`Six`},
          {k:'D',t:`Ten`},
          {k:'E',t:`Sixteen`}
        ], correct:'C' },
      { id:'q17', no:17, type:'single', prompt:`Who taught Rani how to play badminton?`,
        options:[
          {k:'A',t:`Her mother`},
          {k:'B',t:`Her school teacher`},
          {k:'C',t:`Her father`},
          {k:'D',t:`Her older sister`},
          {k:'E',t:`A professional coach from Jakarta`}
        ], correct:'C' },
      { id:'q18', no:18, type:'multi', prompt:`Which of the following are mentioned as Rani's personality traits?`, hint:`Choose more than one answer!`,
        options:[
          {k:'A',t:`Humble`},
          {k:'B',t:`Disciplined`},
          {k:'C',t:`Arrogant`},
          {k:'D',t:`Cheerful and supportive`}
        ], correct:['A','B','D'] },
      { id:'q19', no:19, type:'matrix', prompt:`Read the following statements taken from the text. Decide whether each is a FACT or an OPINION.`,
        cols:['FACT','OPINION'],
        statements:[
          {t:`"Rani wakes up at five in the morning to practice."`, correct:'FACT'},
          {t:`"Rani is a true inspiration for dedication and discipline."`, correct:'OPINION'},
          {t:`"Rani has won several regional junior championships."`, correct:'FACT'}
        ] },
      { id:'q20', no:20, type:'single', prompt:`The word "humble" in paragraph 3 is closest in meaning to...`,
        options:[
          {k:'A',t:`Proud and boastful`},
          {k:'B',t:`Not proud about one's own achievements`},
          {k:'C',t:`Angry and rude`},
          {k:'D',t:`Confused and nervous`},
          {k:'E',t:`Careless and lazy`}
        ], correct:'B' },
      { id:'q21', no:21, type:'single', prompt:`Which outline best matches the order of ideas in the text?`,
        options:[
          {k:'A',t:`I. Introduction & appearance II. Background & training III. Personality IV. Other interests & closing message`},
          {k:'B',t:`I. Personality II. Introduction III. Training IV. Closing message`},
          {k:'C',t:`I. Closing message II. Training III. Appearance IV. Personality`},
          {k:'D',t:`I. Other interests II. Personality III. Appearance IV. Training`},
          {k:'E',t:`I. Training II. Appearance III. Closing IV. Personality`}
        ], correct:'A' },
      { id:'q22', no:22, type:'single', prompt:`What is the writer's main purpose in writing this text?`,
        options:[
          {k:'A',t:`To criticize Rani for training too much`},
          {k:'B',t:`To describe Rani's appearance, background, and personality as an inspiring young athlete`},
          {k:'C',t:`To give instructions on how to play badminton`},
          {k:'D',t:`To compare Rani with other badminton players`},
          {k:'E',t:`To argue that badminton is better than other sports`}
        ], correct:'B' },
      { id:'q23', no:23, type:'single', prompt:`Based on the text, what can we infer about Rani's daily routine?`,
        options:[
          {k:'A',t:`She rarely wakes up early`},
          {k:'B',t:`She combines intense training with school and rest`},
          {k:'C',t:`She only trains on weekends`},
          {k:'D',t:`She stopped playing badminton after winning her first championship`},
          {k:'E',t:`She trains without her father's guidance`}
        ], correct:'B' }
    ]
  },
  {
    id:'text4',
    tag:'TEXT 4',
    color:'var(--t4)',
    bg:'var(--t4-bg)',
    title:`My Grandfather`,
    meta:`Descriptive Text · People · Questions No. 24-30`,
    passage:[
      `My grandfather, whom I call Kakek, is seventy-two years old, but he is still active and healthy. He is not very tall, and his hair is completely white now, though he still has a thick mustache that makes him look wise and dignified. His hands are rough and strong from years of working as a farmer, and his skin is tanned from spending so much time outdoors.`,
      `Kakek is a very hardworking and generous man. Even though he is retired now, he still enjoys tending his small vegetable garden every morning. He often shares his fresh vegetables with our neighbors, never asking for anything in return. Kakek is also incredibly wise; whenever I have a problem, he always gives me thoughtful advice based on his many years of experience.`,
      `Despite his age, Kakek has a great sense of humor. He loves telling funny stories about his childhood, and his laughter is loud and contagious. Every weekend, my cousins and I visit him, and we all gather around to listen to his stories while enjoying tea and homemade snacks.`,
      `I truly admire my grandfather for his strength, wisdom, and kindness. He has taught me that hard work and generosity are two of the most important values in life, and I hope I can be just like him when I grow old.`
    ],
    questions:[
      { id:'q24', no:24, type:'single', prompt:`How old is the writer's grandfather, according to the text?`,
        options:[
          {k:'A',t:`Sixty`},
          {k:'B',t:`Sixty-five`},
          {k:'C',t:`Seventy`},
          {k:'D',t:`Seventy-two`},
          {k:'E',t:`Eighty`}
        ], correct:'D' },
      { id:'q25', no:25, type:'single', prompt:`Which of the following describes the grandfather's physical appearance?`,
        options:[
          {k:'A',t:`Tall with black hair and a beard`},
          {k:'B',t:`Short with white hair and a thick mustache`},
          {k:'C',t:`Bald with glasses`},
          {k:'D',t:`Tall and thin with curly hair`},
          {k:'E',t:`Short with a shaved head`}
        ], correct:'B' },
      { id:'q26', no:26, type:'multi', prompt:`According to the text, which of the following are the grandfather's characteristics?`, hint:`Choose more than one answer!`,
        options:[
          {k:'A',t:`Hardworking`},
          {k:'B',t:`Generous`},
          {k:'C',t:`Rude to neighbors`},
          {k:'D',t:`Wise`}
        ], correct:['A','B','D'] },
      { id:'q27', no:27, type:'matrix', prompt:`Read the following statements. Decide whether each is "Stated in the Text" or "Not Stated in the Text."`,
        cols:['STATED','NOT STATED'],
        statements:[
          {t:`The grandfather used to work as a farmer.`, correct:'STATED'},
          {t:`The grandfather lives in a big city.`, correct:'NOT STATED'},
          {t:`The grandfather shares vegetables with the neighbors.`, correct:'STATED'}
        ] },
      { id:'q28', no:28, type:'single', prompt:`The word "contagious," used to describe his laughter, most likely means...`,
        options:[
          {k:'A',t:`Dangerous and harmful`},
          {k:'B',t:`Easily making others laugh or feel the same way`},
          {k:'C',t:`Quiet and hard to hear`},
          {k:'D',t:`Sad and serious`},
          {k:'E',t:`Rare and unusual`}
        ], correct:'B' },
      { id:'q29', no:29, type:'single', prompt:`What is the main idea of the text?`,
        options:[
          {k:'A',t:`The writer's grandfather is lazy and unfriendly`},
          {k:'B',t:`The writer admires his/her grandfather for being hardworking, wise, generous, and humorous`},
          {k:'C',t:`The grandfather no longer talks to his grandchildren`},
          {k:'D',t:`The grandfather is a famous farmer known throughout the country`},
          {k:'E',t:`The text mainly describes the grandfather's house`}
        ], correct:'B' },
      { id:'q30', no:30, type:'single', prompt:`Why did the writer include the sentence "I hope I can be just like him when I grow old" at the end of the text?`,
        options:[
          {k:'A',t:`To give a command to the reader`},
          {k:'B',t:`To express the writer's personal feeling and admiration toward the grandfather`},
          {k:'C',t:`To explain the steps of gardening`},
          {k:'D',t:`To argue against getting old`},
          {k:'E',t:`To describe the grandfather's physical appearance`}
        ], correct:'B' }
    ]
  }
];

const VALID_TOKENS = {
  'X-I': ['TK1010', 'TK1011'],
  'X-J': ['TK1012'],
  'X-K': ['TK1013']
};

let FLAT = [];
function buildFlat(){
  FLAT = [];
  DATA.forEach(section=>{
    const qs = shuffle(section.questions.slice());
    qs.forEach(q=>{
      const qCopy = Object.assign({}, q, {_section:section});
      if(Array.isArray(q.options)){
        qCopy.options = shuffle(q.options.slice());
      }
      FLAT.push(qCopy);
    });
  });
}
function shuffle(arr){
  for(let i=arr.length-1;i>0;i--){
    const j = Math.floor(Math.random()*(i+1));
    [arr[i],arr[j]]=[arr[j],arr[i]];
  }
  return arr;
}

let answers = {};
let submitted = false;
let currentIndex = 0;
let paletteOpen = false;

function isAnsweredQ(q){
  if(q.type==='matrix'){
    const a = answers[q.id]||{};
    return Object.keys(a).length===q.statements.length;
  }
  if(q.type==='match'){
    const a = answers[q.id]||{};
    return Object.keys(a).length===q.items.length;
  }
  if(q.type==='multi'){
    return !!(answers[q.id] && answers[q.id].length>0);
  }
  return !!answers[q.id];
}

function arraysEqual(a,b){
  if(a.length!==b.length) return false;
  const sa=[...a].sort(), sb=[...b].sort();
  return sa.every((v,i)=>v===sb[i]);
}

function computeResult(q){
  if(q.type==='single'){
    const correct = answers[q.id]===q.correct;
    return {correct, earned: correct?1:0, total:1};
  }
  if(q.type==='multi'){
    const chosen = answers[q.id]||[];
    const correct = arraysEqual(chosen, q.correct);
    return {correct, earned: correct?1:0, total:1};
  }
  if(q.type==='matrix'){
    const chosenMap = answers[q.id]||{};
    let earned = 0;
    const rowResults = q.statements.map((s,i)=>{
      const ok = chosenMap[i]===s.correct;
      if(ok) earned++;
      return ok;
    });
    return {correct: earned===q.statements.length, earned, total:q.statements.length, rowResults};
  }
  if(q.type==='match'){
    const chosenMap = answers[q.id]||{};
    let earned = 0;
    const rowResults = q.items.map((it,i)=>{
      const ok = chosenMap[i]===it.correct;
      if(ok) earned++;
      return ok;
    });
    return {correct: earned===q.items.length, earned, total:q.items.length, rowResults};
  }
}

const stage = document.getElementById('stage');

function renderStage(){
  const q = FLAT[currentIndex];
  const section = q._section;
  stage.innerHTML = '';
  stage.style.setProperty('--sc', section.color);

  const head = document.createElement('div');
  head.className='stage-head';
  head.innerHTML = `
    <span class="genre-tag" style="background:${section.bg}; color:${section.color};">${section.tag}</span>
    <span class="stage-index">Question ${currentIndex+1} of ${FLAT.length}</span>
  `;
  stage.appendChild(head);

  const passage = document.createElement('div');
  passage.className='passage';
  passage.style.borderLeftColor = section.color;
  passage.innerHTML = `
    <div class="meta">${section.meta}</div>
    <h3>${section.title}</h3>
    ${section.passage.map(p=>`<p>${p}</p>`).join('')}
  `;
  stage.appendChild(passage);

  const card = document.createElement('div');
  card.className='q-card';
  card.id='card-'+q.id;

  const top = document.createElement('div');
  top.className='q-top';
  top.innerHTML = `
    <div class="q-num" style="background:${section.bg}; color:${section.color};">${currentIndex+1}</div>
    <div class="q-prompt">${q.prompt}</div>
  `;
  card.appendChild(top);

  if(q.hint){
    const hint = document.createElement('div');
    hint.className='q-hint';
    hint.textContent = q.hint;
    card.appendChild(hint);
  }

  if(q.type==='single'){
    const opts = document.createElement('div');
    opts.className='options';
    q.options.forEach(o=>{
      const lbl = document.createElement('label');
      lbl.className='opt';
      lbl.dataset.key=o.k;
      const checked = answers[q.id]===o.k ? 'checked' : '';
      lbl.innerHTML = `<input type="radio" name="${q.id}" value="${o.k}" ${checked}> <span>${o.t}</span> <span class="tag"></span>`;
      if(answers[q.id]===o.k) lbl.classList.add('selected');
      lbl.querySelector('input').addEventListener('change', ()=>{
        answers[q.id]=o.k;
        refreshOptionSelection(q, card);
        updateProgress();
        renderPalette();
        saveState();
      });
      opts.appendChild(lbl);
    });
    card.appendChild(opts);
  }

  if(q.type==='multi'){
    const opts = document.createElement('div');
    opts.className='options';
    q.options.forEach(o=>{
      const lbl = document.createElement('label');
      lbl.className='opt';
      lbl.dataset.key=o.k;
      const isChecked = (answers[q.id]||[]).includes(o.k);
      lbl.innerHTML = `<input type="checkbox" name="${q.id}" value="${o.k}" ${isChecked?'checked':''}> <span>${o.t}</span> <span class="tag"></span>`;
      if(isChecked) lbl.classList.add('selected');
      lbl.querySelector('input').addEventListener('change', ()=>{
        const cur = new Set(answers[q.id]||[]);
        if(lbl.querySelector('input').checked) cur.add(o.k); else cur.delete(o.k);
        answers[q.id]=Array.from(cur);
        refreshOptionSelection(q, card);
        updateProgress();
        renderPalette();
        saveState();
      });
      opts.appendChild(lbl);
    });
    card.appendChild(opts);
  }

  if(q.type==='matrix'){
    const box = document.createElement('div');
    box.className='matrix';
    const table = document.createElement('table');
    table.innerHTML = `<thead><tr><th>Statement</th><th>${q.cols[0]}</th><th>${q.cols[1]}</th></tr></thead>`;
    const tbody = document.createElement('tbody');
    q.statements.forEach((s,i)=>{
      const tr = document.createElement('tr');
      const chosenVal = (answers[q.id]||{})[i];
      tr.innerHTML = `
        <td class="stmt">${i+1}. ${s.t}</td>
        <td class="pick" data-col="${q.cols[0]}"><input type="radio" name="${q.id}-${i}" value="${q.cols[0]}" ${chosenVal===q.cols[0]?'checked':''}></td>
        <td class="pick" data-col="${q.cols[1]}"><input type="radio" name="${q.id}-${i}" value="${q.cols[1]}" ${chosenVal===q.cols[1]?'checked':''}></td>
      `;
      tr.querySelectorAll('input').forEach(inp=>{
        inp.addEventListener('change', ()=>{
          if(!answers[q.id]) answers[q.id]={};
          answers[q.id][i]=inp.value;
          updateProgress();
          renderPalette();
          saveState();
        });
      });
      tbody.appendChild(tr);
    });
    table.appendChild(tbody);
    box.appendChild(table);
    card.appendChild(box);
  }

  if(q.type==='match'){
    const box = document.createElement('div');
    box.className='match-box';
    const table = document.createElement('table');
    table.innerHTML = `<thead><tr><th>Word (Column A)</th><th>Meaning (Column B)</th></tr></thead>`;
    const tbody = document.createElement('tbody');
    q.items.forEach((it,i)=>{
      const tr = document.createElement('tr');
      tr.dataset.row = i;
      const chosenVal = (answers[q.id]||{})[i] || '';
      const optionsHtml = `<option value="" ${chosenVal===''?'selected':''}>-- choose --</option>` +
        q.choices.map(c=>`<option value="${c.k}" ${chosenVal===c.k?'selected':''}>${c.k}. ${c.t}</option>`).join('');
      tr.innerHTML = `
        <td class="word">${it.t}</td>
        <td><select data-idx="${i}">${optionsHtml}</select></td>
      `;
      tr.querySelector('select').addEventListener('change', (e)=>{
        if(!answers[q.id]) answers[q.id]={};
        answers[q.id][i]=e.target.value;
        updateProgress();
        renderPalette();
        saveState();
      });
      tbody.appendChild(tr);
    });
    table.appendChild(tbody);
    box.appendChild(table);
    card.appendChild(box);
  }

  const note = document.createElement('div');
  note.className='answer-note';
  note.id='note-'+q.id;
  card.appendChild(note);

  stage.appendChild(card);

  if(submitted){
    applyGradingToCard(q, card, note);
  }

  updateNavButtons();
}

function refreshOptionSelection(q, card){
  card.querySelectorAll('.opt').forEach(lbl=>{
    const key = lbl.dataset.key;
    const sel = q.type==='multi' ? (answers[q.id]||[]).includes(key) : answers[q.id]===key;
    lbl.classList.toggle('selected', !!sel && !submitted);
  });
}

function applyGradingToCard(q, card, note){
  const result = computeResult(q);

  if(q.type==='single' || q.type==='multi'){
    card.classList.add(result.correct?'correct':'incorrect');
    card.querySelectorAll('.opt').forEach(lbl=>{
      const key = lbl.dataset.key;
      lbl.classList.remove('selected');
      lbl.querySelector('input').disabled = true;
      lbl.classList.add('locked');
      const tag = lbl.querySelector('.tag');
      const isCorrectKey = q.type==='single' ? key===q.correct : q.correct.includes(key);
      const wasChosen = q.type==='single' ? key===answers[q.id] : (answers[q.id]||[]).includes(key);
      if(isCorrectKey){
        lbl.classList.add('opt-correct');
        tag.textContent = q.type==='single' ? 'Correct answer' : 'Should be chosen';
      }
      if(wasChosen && !isCorrectKey){
        lbl.classList.add('opt-wrong');
        tag.textContent = q.type==='single' ? 'Your choice' : 'Your choice (wrong)';
      }
    });
    if(!result.correct){
      if(q.type==='single'){
        const correctOpt = q.options.find(o=>o.k===q.correct);
        note.innerHTML = `<b>Not quite.</b> Correct answer: <b>${correctOpt.t}</b>`;
      } else {
        const correctTexts = q.correct.map(k=>q.options.find(o=>o.k===k).t);
        note.innerHTML = `<b>Not quite.</b> Correct answer: <b>${correctTexts.join(' · ')}</b>`;
      }
      note.classList.add('show');
    }
  }

  if(q.type==='matrix'){
    card.classList.add(result.correct?'correct':'incorrect');
    const rows = card.querySelectorAll('.matrix tbody tr');
    q.statements.forEach((s,i)=>{
      const row = rows[i];
      row.querySelectorAll('input').forEach(inp=>{ inp.disabled = true; });
      const chosen = (answers[q.id]||{})[i];
      row.querySelectorAll('.pick').forEach(td=>{
        const col = td.dataset.col;
        if(col===s.correct) td.classList.add('right-cell');
        if(col===chosen && chosen!==s.correct) td.classList.add('wrong-cell');
      });
    });
    if(!result.correct){
      note.innerHTML = `<b>Check the rows marked in red</b> — the green box shows the answer that should have been chosen.`;
      note.classList.add('show');
    }
  }

  if(q.type==='match'){
    card.classList.add(result.correct?'correct':'incorrect');
    const rows = card.querySelectorAll('.match-box tbody tr');
    q.items.forEach((it,i)=>{
      const row = rows[i];
      row.querySelector('select').disabled = true;
      const chosen = (answers[q.id]||{})[i];
      if(chosen===it.correct){ row.classList.add('right-row'); }
      else { row.classList.add('wrong-row'); }
    });
    if(!result.correct){
      const correctList = q.items.map(it=>`${it.t} = ${it.correct}`).join(' · ');
      note.innerHTML = `<b>Not quite.</b> Correct matches: <b>${correctList}</b>`;
      note.classList.add('show');
    }
  }
}

/* ---------- palette ---------- */
const paletteGrid = document.getElementById('paletteGrid');
function renderPalette(){
  paletteGrid.innerHTML='';
  FLAT.forEach((q,i)=>{
    const btn = document.createElement('button');
    btn.type='button';
    btn.className='pnum';
    btn.textContent = i+1;
    if(i===currentIndex) btn.classList.add('pn-current');
    if(submitted){
      const r = computeResult(q);
      btn.classList.add(r.correct ? 'pn-correct' : 'pn-incorrect');
    } else if(isAnsweredQ(q)){
      btn.classList.add('pn-answered');
    }
    btn.addEventListener('click', ()=>{
      currentIndex = i;
      renderStage();
      renderPalette();
      saveState();
      window.scrollTo({top:0, behavior:'smooth'});
    });
    paletteGrid.appendChild(btn);
  });
}

document.getElementById('paletteToggleBtn').addEventListener('click', ()=>{
  paletteOpen = !paletteOpen;
  document.getElementById('palettePanel').classList.toggle('open', paletteOpen);
});

/* ---------- progress ---------- */
function updateProgress(){
  const answered = FLAT.filter(isAnsweredQ).length;
  const pct = Math.round((answered/FLAT.length)*100);
  document.getElementById('progressFill').style.width=pct+'%';
  document.getElementById('progressLabel').textContent = `${answered} / ${FLAT.length} answered`;
  document.getElementById('navStatus').textContent = `Question ${currentIndex+1} / ${FLAT.length}`;
}

/* ---------- nav buttons ---------- */
function updateNavButtons(){
  document.getElementById('prevBtn').disabled = currentIndex===0;
  document.getElementById('nextBtn').disabled = currentIndex===FLAT.length-1;
  const isLast = currentIndex===FLAT.length-1;
  document.getElementById('submitBtn').style.display = isLast ? '' : 'none';
}

document.getElementById('prevBtn').addEventListener('click', ()=>{
  if(currentIndex>0){ currentIndex--; renderStage(); renderPalette(); updateProgress(); saveState(); window.scrollTo({top:0, behavior:'smooth'}); }
});
document.getElementById('nextBtn').addEventListener('click', ()=>{
  if(currentIndex<FLAT.length-1){ currentIndex++; renderStage(); renderPalette(); updateProgress(); saveState(); window.scrollTo({top:0, behavior:'smooth'}); }
});

/* ---------- grading + submit ---------- */
function grade(auto){
  const name = document.getElementById('stuName').value.trim();
  const stuClass = document.getElementById('stuClass').value.trim();
  if(!auto && (!name || !stuClass)){
    const err = document.getElementById('gateError');
    if(err) err.textContent = 'Please fill in Name and Class at the top before checking & submitting.';
    window.scrollTo({top:0, behavior:'smooth'});
    return;
  }
  if(submitted) return;

  stopTimer();
  submitted = true;
  let earned=0, total=0;
  FLAT.forEach(q=>{
    const r = computeResult(q);
    earned += r.earned;
    total += r.total;
  });

  const pct = Math.round((earned/total)*100);
  document.getElementById('scoreBig').textContent = pct+'%';
  document.getElementById('scoreSub').textContent = `${earned} out of ${total} points correct`;
  const msg = document.getElementById('scoreMsg');
  let msgText, msgColor, msgBg;
  if(pct>=90){ msgText='Excellent! ⭐'; msgColor='var(--good)'; msgBg='var(--good-bg)'; }
  else if(pct>=75){ msgText='Great job, almost perfect!'; msgColor='var(--good)'; msgBg='var(--good-bg)'; }
  else if(pct>=60){ msgText='Pretty good, keep practicing.'; msgColor='var(--t3)'; msgBg='var(--t3-bg)'; }
  else { msgText='Please re-read the texts and try again.'; msgColor='var(--bad)'; msgBg='var(--bad-bg)'; }
  msg.textContent = msgText;
  msg.style.color = msgColor;
  msg.style.background = msgBg;

  const resultsBox = document.getElementById('resultsBox');
  resultsBox.classList.add('show');

  document.getElementById('submitBtn').disabled = true;
  document.getElementById('timerBadge').textContent = 'Finished';
  document.getElementById('timerBadge').classList.remove('warn','danger','paused');
  renderStage();
  renderPalette();
  saveState();
  resultsBox.scrollIntoView({behavior:'smooth', block:'start'});

  attemptSend(name, stuClass, {pct, earned, total});
}

/* ---------- build a readable per-question answer report ---------- */
function buildAnswerReport(){
  const sorted = FLAT.slice().sort((a,b)=> a.no - b.no );
  const lines = sorted.map(q=>{
    const r = computeResult(q);
    const mark = r.correct ? 'CORRECT' : 'WRONG';
    let ansText;
    if(q.type==='single'){
      ansText = answers[q.id] || '-';
    } else if(q.type==='multi'){
      ansText = (answers[q.id]||[]).slice().sort().join(',') || '-';
    } else if(q.type==='matrix'){
      const chosenMap = answers[q.id]||{};
      ansText = q.statements.map((s,i)=> `${i+1}:${chosenMap[i]||'-'}`).join(' | ');
    } else if(q.type==='match'){
      const chosenMap = answers[q.id]||{};
      ansText = q.items.map((it,i)=> `${it.t}=${chosenMap[i]||'-'}`).join(' | ');
    }
    return `No.${q.no} [${mark}] ${ansText}`;
  });
  return lines.join('\n');
}

/* ---------- send result to Google Form ---------- */
const GFORM_BASE = 'https://docs.google.com/forms/d/e/1FAIpQLSelRC84_2TymjK6Ewa3zfYIAvmD_2sePEh0-zLdw71EX3yYEg/formResponse';
const GFORM_ENTRY_NAME = 'entry.1215958487';
const GFORM_ENTRY_CLASS = 'entry.928005117';
const GFORM_ENTRY_ANSWER = 'entry.1406651719';
const GFORM_ENTRY_SCORE = 'entry.1591162386';
let pendingSend = null;

function isReallyOnline(){
  return new Promise(resolve=>{
    if(!navigator.onLine){ resolve(false); return; }
    let done = false;
    const finish = (val)=>{ if(!done){ done = true; resolve(val); } };
    const timer = setTimeout(()=>finish(false), 4000);
    const img = new Image();
    img.onload = ()=>{ clearTimeout(timer); finish(true); };
    img.onerror = ()=>{ clearTimeout(timer); finish(true); };
    img.src = 'https://www.google.com/favicon.ico?_=' + Date.now();
  });
}

function attemptSend(name, stuClass, score){
  const note = document.getElementById('sendNote');
  const retryBtn = document.getElementById('retrySendBtn');
  pendingSend = {name, stuClass, score};

  note.textContent = 'Checking internet connection...';
  note.className = 'send-note';
  retryBtn.style.display = 'none';

  isReallyOnline().then(online=>{
    if(!online){
      note.textContent = 'No internet connection. Your answers have NOT been sent.';
      note.className = 'send-note err';
      retryBtn.style.display = 'inline-block';
      return;
    }
    sendResultToForm(pendingSend.name, pendingSend.stuClass, pendingSend.score);
  });
}

document.getElementById('retrySendBtn').addEventListener('click', ()=>{
  if(pendingSend){
    attemptSend(pendingSend.name, pendingSend.stuClass, pendingSend.score);
  }
});

function sendResultToForm(name, stuClass, score){
  const note = document.getElementById('sendNote');
  const retryBtn = document.getElementById('retrySendBtn');
  const answerReport = buildAnswerReport();
  const scoreText = `${score.pct}% (${score.earned}/${score.total})`;

  const iframeName = 'gform-send-target';
  let iframe = document.getElementById(iframeName);
  if(!iframe){
    iframe = document.createElement('iframe');
    iframe.name = iframeName;
    iframe.id = iframeName;
    iframe.style.display = 'none';
    document.body.appendChild(iframe);
  }

  const form = document.createElement('form');
  form.action = GFORM_BASE;
  form.method = 'POST';
  form.target = iframeName;
  form.style.display = 'none';

  const fields = {
    [GFORM_ENTRY_NAME]: name,
    [GFORM_ENTRY_CLASS]: stuClass,
    [GFORM_ENTRY_ANSWER]: answerReport,
    [GFORM_ENTRY_SCORE]: scoreText
  };
  Object.keys(fields).forEach(key=>{
    const input = document.createElement('input');
    input.type = 'hidden';
    input.name = key;
    input.value = fields[key];
    form.appendChild(input);
  });

  document.body.appendChild(form);
  form.submit();
  document.body.removeChild(form);

  pendingSend = null;
  retryBtn.style.display = 'none';
  note.textContent = 'Answers submitted! Thank you.';
  note.className = 'send-note ok';
}

function resetQuiz(){
  answers = {};
  submitted = false;
  currentIndex = 0;
  pendingSend = null;
  document.getElementById('resultsBox').classList.remove('show');
  document.getElementById('submitBtn').disabled = false;
  document.getElementById('sendNote').textContent = '';
  document.getElementById('sendNote').className = 'send-note';
  document.getElementById('retrySendBtn').style.display = 'none';
  buildFlat();
  renderStage();
  renderPalette();
  updateProgress();
  startTimer(Date.now()+TIMER_MS);
  saveState();
  window.scrollTo({top:0, behavior:'smooth'});
}

document.getElementById('submitBtn').addEventListener('click', ()=>{
  if(submitted) return;
  const unanswered = FLAT.length - FLAT.filter(isAnsweredQ).length;
  const msgEl = document.getElementById('confirmMsg');
  if(unanswered > 0){
    msgEl.innerHTML = `You still have <b>${unanswered} unanswered question(s)</b>.<br>Are you sure you want to submit your exam now?`;
  } else {
    msgEl.innerHTML = `You have answered all <b>${FLAT.length} questions</b>.<br>Are you sure you want to submit your exam now?`;
  }
  document.getElementById('confirmModal').classList.add('show');
});

document.getElementById('cancelSubmitBtn').addEventListener('click', ()=>{
  document.getElementById('confirmModal').classList.remove('show');
});

document.getElementById('confirmSubmitBtn').addEventListener('click', ()=>{
  document.getElementById('confirmModal').classList.remove('show');
  grade(false);
});

document.getElementById('resetBtn').addEventListener('click', resetQuiz);

/* ---------- anti copy-paste & anti-select ---------- */
function isEditable(el){
  return el && (el.tagName==='INPUT' || el.tagName==='TEXTAREA' || el.tagName==='SELECT' || el.isContentEditable);
}
['copy','cut','contextmenu','selectstart','dragstart'].forEach(evt=>{
  document.addEventListener(evt, e=>{
    if(isEditable(e.target)) return;
    e.preventDefault();
  });
});
document.addEventListener('keydown', e=>{
  const k = (e.key || '').toLowerCase();
  if(!k) return;
  const blockedCombo = (e.ctrlKey||e.metaKey) && ['c','x','a','s','u','p'].includes(k);
  if((blockedCombo && !isEditable(e.target)) || k==='f12'){
    e.preventDefault();
  }
});

/* ---------- persistence (localStorage) ---------- */
const STORAGE_KEY = 'eng_exam_10_descriptive_people_v1';

function saveState(){
  try{
    const state = {
      name: document.getElementById('stuName').value,
      cls: document.getElementById('stuClass').value,
      gatePassed: true,
      order: FLAT.map(q=>q.id),
      answers: answers,
      currentIndex: currentIndex,
      submitted: submitted,
      endAt: examEndAt,
      remainingTimeMs: isTimerPaused ? remainingTimeMs : (examEndAt ? Math.max(0, examEndAt - Date.now()) : TIMER_MS),
      isTimerPaused: isTimerPaused
    };
    localStorage.setItem(STORAGE_KEY, JSON.stringify(state));
  }catch(e){ /* localStorage unavailable, ignore */ }
}

function clearState(){
  try{ localStorage.removeItem(STORAGE_KEY); }catch(e){}
}

function loadState(){
  try{
    const raw = localStorage.getItem(STORAGE_KEY);
    if(!raw) return null;
    const state = JSON.parse(raw);
    if(!state || !state.gatePassed || !Array.isArray(state.order)) return null;

    const byId = {};
    FLAT.forEach(q=>{ byId[q.id]=q; });
    const allIdsMatch = state.order.length===FLAT.length && state.order.every(id=>byId[id]);
    if(!allIdsMatch) return null;

    return state;
  }catch(e){ return null; }
}

const TIMER_MINUTES = 90;
const TIMER_MS = TIMER_MINUTES*60*1000;
let timerInterval = null;
let examEndAt = null;
let remainingTimeMs = TIMER_MS;
let isTimerPaused = false;

function formatTime(ms){
  if(ms<0) ms=0;
  const totalSec = Math.floor(ms/1000);
  const m = Math.floor(totalSec/60);
  const s = totalSec%60;
  return String(m).padStart(2,'0')+':'+String(s).padStart(2,'0');
}

function renderTimerDisplay(ms){
  const badge = document.getElementById('timerBadge');
  if(!badge) return;
  badge.classList.remove('warn','danger','paused');
  if(isTimerPaused){
    badge.textContent = formatTime(ms) + ' (PAUSED)';
    badge.classList.add('paused');
  } else {
    badge.textContent = formatTime(ms);
    if(ms<=2*60*1000) badge.classList.add('danger');
    else if(ms<=10*60*1000) badge.classList.add('warn');
  }
}

function stopTimer(){
  if(timerInterval){ clearInterval(timerInterval); timerInterval=null; }
}

function tick(){
  if(isTimerPaused) return;
  const remaining = examEndAt - Date.now();
  if(remaining<=0){
    remainingTimeMs = 0;
    renderTimerDisplay(0);
    stopTimer();
    if(!submitted){
      grade(true);
    }
    return;
  }
  remainingTimeMs = remaining;
  renderTimerDisplay(remaining);
}

function startTimer(endAt){
  examEndAt = endAt;
  remainingTimeMs = Math.max(0, examEndAt - Date.now());
  stopTimer();
  if(!navigator.onLine){
    pauseTimer();
  } else {
    isTimerPaused = false;
    tick();
    timerInterval = setInterval(tick, 1000);
  }
}

function pauseTimer(){
  if(submitted) return;
  if(!isTimerPaused && examEndAt){
    remainingTimeMs = Math.max(0, examEndAt - Date.now());
  }
  isTimerPaused = true;
  stopTimer();
  renderTimerDisplay(remainingTimeMs);
}

function resumeTimer(){
  if(submitted) return;
  if(isTimerPaused || !timerInterval){
    isTimerPaused = false;
    if(remainingTimeMs > 0){
      startTimer(Date.now() + remainingTimeMs);
    } else {
      renderTimerDisplay(0);
    }
  }
}

function updateOnlineBadge(){
  const badge = document.getElementById('onlineBadge');
  if(!badge) return;
  if(navigator.onLine){
    badge.classList.remove('offline');
    badge.classList.add('online');
    badge.innerHTML = '<span class="online-dot"></span>Online';
    if(examEndAt && !submitted && isTimerPaused){
      resumeTimer();
      saveState();
    }
  }else{
    badge.classList.remove('online');
    badge.classList.add('offline');
    badge.innerHTML = '<span class="online-dot"></span>Offline';
    if(examEndAt && !submitted){
      pauseTimer();
      saveState();
    }
  }
}
window.addEventListener('online', updateOnlineBadge);
window.addEventListener('offline', updateOnlineBadge);

/* ---------- init ---------- */
buildFlat();

const saved = loadState();
if(saved){
  FLAT = saved.order.map(id=>FLAT.find(q=>q.id===id));
  answers = saved.answers || {};
  currentIndex = Math.min(saved.currentIndex||0, FLAT.length-1);
  submitted = !!saved.submitted;
  document.getElementById('stuName').value = saved.name || '';
  document.getElementById('stuClass').value = saved.cls || '';
  document.getElementById('gateScreen').style.display = 'none';
  document.getElementById('appMain').style.display = 'block';

  if(submitted){
    let earned=0, total=0;
    FLAT.forEach(q=>{ const r=computeResult(q); earned+=r.earned; total+=r.total; });
    const pct = Math.round((earned/total)*100);
    document.getElementById('scoreBig').textContent = pct+'%';
    document.getElementById('scoreSub').textContent = `${earned} out of ${total} points correct`;
    const msg = document.getElementById('scoreMsg');
    let msgText, msgColor, msgBg;
    if(pct>=90){ msgText='Excellent! ⭐'; msgColor='var(--good)'; msgBg='var(--good-bg)'; }
    else if(pct>=75){ msgText='Great job, almost perfect!'; msgColor='var(--good)'; msgBg='var(--good-bg)'; }
    else if(pct>=60){ msgText='Pretty good, keep practicing.'; msgColor='var(--t3)'; msgBg='var(--t3-bg)'; }
    else { msgText='Please re-read the texts and try again.'; msgColor='var(--bad)'; msgBg='var(--bad-bg)'; }
    msg.textContent = msgText;
    msg.style.color = msgColor;
    msg.style.background = msgBg;
    document.getElementById('resultsBox').classList.add('show');
    document.getElementById('submitBtn').disabled = true;
    document.getElementById('timerBadge').textContent = 'Finished';
  } else {
    let rem = saved.remainingTimeMs;
    if(rem === undefined && saved.endAt){
      rem = saved.endAt - Date.now();
    }
    remainingTimeMs = Math.max(0, rem !== undefined ? rem : TIMER_MS);
    if(remainingTimeMs <= 0){
      renderTimerDisplay(0);
      grade(true);
    } else if(!navigator.onLine || saved.isTimerPaused){
      isTimerPaused = true;
      pauseTimer();
    } else {
      startTimer(Date.now() + remainingTimeMs);
    }
  }
}

renderStage();
renderPalette();
updateProgress();
updateOnlineBadge();

if(saved && !saved.submitted && (remainingTimeMs <= 0)){
  grade(true);
}

/* ---------- gate: name + class + token ---------- */
function checkGate(){
  const name = document.getElementById('gateName').value.trim();
  const cls = document.getElementById('gateClass').value.trim();
  const token = document.getElementById('gateToken').value.trim().toUpperCase();
  const err = document.getElementById('gateError');

  if(!name){
    err.textContent = 'Please fill in your Name.';
    return;
  }
  if(!cls){
    err.textContent = 'Please select a Class (X-I, X-J, or X-K).';
    return;
  }
  if(!token){
    err.textContent = 'Please enter the Exam Token.';
    return;
  }

  const allowedTokens = VALID_TOKENS[cls] || [];
  if(!allowedTokens.includes(token)){
    err.textContent = `Invalid token '${token}' for Class ${cls}.`;
    return;
  }

  err.textContent = '';
  document.getElementById('stuName').value = name;
  document.getElementById('stuClass').value = cls;
  document.getElementById('gateScreen').style.display = 'none';
  document.getElementById('appMain').style.display = 'block';
  window.scrollTo({top:0});
  startTimer(Date.now()+TIMER_MS);
  saveState();
}

document.getElementById('backToLoginBtn').addEventListener('click', ()=>{
  saveState();
  stopTimer();
  document.getElementById('gateName').value = document.getElementById('stuName').value || '';
  const currentCls = document.getElementById('stuClass').value || '';
  document.getElementById('gateClass').value = currentCls;
  document.getElementById('gateToken').value = '';
  document.getElementById('gateError').textContent = '';
  document.getElementById('appMain').style.display = 'none';
  document.getElementById('gateScreen').style.display = 'flex';
  window.scrollTo({top:0});
});

document.getElementById('gateSubmitBtn').addEventListener('click', checkGate);
document.getElementById('gateToken').addEventListener('keydown', e=>{
  if(e.key === 'Enter') checkGate();
});
document.getElementById('gateName').addEventListener('keydown', e=>{
  if(e.key === 'Enter') checkGate();
});
</script>
</body>
</html>
