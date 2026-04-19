<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>IPL 2026 Live Dashboard</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Plus+Jakarta+Sans:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
:root {
  --bg:#07090f;--surface:#0e1117;--surface2:#141820;
  --border:rgba(255,255,255,0.06);--border2:rgba(255,255,255,0.11);
  --blue:#4f8ef7;--blue-dim:rgba(79,142,247,0.1);
  --gold:#f5c542;--green:#22c55e;--green-dim:rgba(34,197,94,0.1);
  --red:#ef4444;--red-dim:rgba(239,68,68,0.1);
  --purple:#a855f7;--purple-dim:rgba(168,85,247,0.1);
  --text:#e8ecf5;--muted:#5a6480;--muted2:#8492b0;
}
*{margin:0;padding:0;box-sizing:border-box;}
body{background:var(--bg);color:var(--text);font-family:'Plus Jakarta Sans',sans-serif;font-weight:300;min-height:100vh;overflow-x:hidden;}
body::before{content:'';position:fixed;inset:0;background:radial-gradient(ellipse 60% 40% at 20% 0%,rgba(79,142,247,0.06) 0%,transparent 60%),radial-gradient(ellipse 50% 30% at 80% 100%,rgba(168,85,247,0.05) 0%,transparent 60%);pointer-events:none;z-index:0;}
header{position:sticky;top:0;z-index:100;background:rgba(7,9,15,0.9);backdrop-filter:blur(20px);border-bottom:0.5px solid var(--border);display:flex;align-items:center;justify-content:space-between;padding:0 2rem;height:58px;}
.logo{display:flex;align-items:center;gap:10px;}
.logo-text{font-family:'Bebas Neue',sans-serif;font-size:26px;letter-spacing:0.06em;}
.logo-badge{font-size:10px;font-weight:600;letter-spacing:0.1em;background:var(--gold);color:#07090f;padding:3px 8px;border-radius:4px;}
.header-right{display:flex;align-items:center;gap:12px;}
.live-pill{display:flex;align-items:center;gap:5px;font-size:11px;font-weight:500;letter-spacing:0.08em;color:var(--red);}
.live-pill::before{content:'';width:6px;height:6px;border-radius:50%;background:var(--red);animation:blink 1.4s ease infinite;}
@keyframes blink{0%,100%{opacity:1}50%{opacity:0.3}}
.refresh-btn{background:transparent;border:0.5px solid var(--border2);color:var(--muted2);font-family:'Plus Jakarta Sans',sans-serif;font-size:12px;padding:6px 14px;border-radius:20px;cursor:pointer;transition:all 0.2s;}
.refresh-btn:hover{border-color:var(--blue);color:var(--blue);}
.last-updated{font-size:11px;color:var(--muted);}
nav{position:relative;z-index:1;display:flex;gap:2px;padding:0 2rem;border-bottom:0.5px solid var(--border);background:rgba(7,9,15,0.6);}
.tab{font-family:'Plus Jakarta Sans',sans-serif;font-size:13px;font-weight:500;padding:14px 18px;background:transparent;border:none;color:var(--muted);cursor:pointer;border-bottom:2px solid transparent;margin-bottom:-0.5px;transition:color 0.2s,border-color 0.2s;}
.tab:hover{color:var(--text);}
.tab.active{color:var(--blue);border-bottom-color:var(--blue);}
main{position:relative;z-index:1;max-width:1080px;margin:0 auto;padding:2rem;}
.panel{display:none;animation:fadeUp 0.25s ease;}
.panel.active{display:block;}
@keyframes fadeUp{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:translateY(0)}}
.label{font-size:10px;font-weight:600;letter-spacing:0.12em;text-transform:uppercase;color:var(--muted);margin-bottom:12px;display:block;}
.section-head{font-family:'Bebas Neue',sans-serif;font-size:34px;letter-spacing:0.04em;margin-bottom:1.5rem;line-height:1;}
.section-head span{color:var(--blue);}
.metrics{display:grid;grid-template-columns:repeat(4,minmax(0,1fr));gap:10px;margin-bottom:1.5rem;}
.metric{background:var(--surface);border:0.5px solid var(--border);border-radius:10px;padding:14px 16px;}
.metric-label{font-size:11px;color:var(--muted);margin-bottom:6px;}
.metric-value{font-size:22px;font-weight:600;font-family:'Bebas Neue',sans-serif;letter-spacing:0.04em;}
.metric-sub{font-size:11px;color:var(--muted2);margin-top:2px;}
.matches-grid{display:grid;gap:10px;}
.match-card{background:var(--surface);border:0.5px solid var(--border);border-radius:12px;padding:1.25rem 1.5rem;position:relative;overflow:hidden;transition:border-color 0.2s;}
.match-card:hover{border-color:var(--border2);}
.match-card.live-card{border-color:rgba(239,68,68,0.25);}
.match-card.live-card::after{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:var(--red);border-radius:3px 0 0 3px;}
.match-card.result-card::after{content:'';position:absolute;left:0;top:0;bottom:0;width:3px;background:var(--green);border-radius:3px 0 0 3px;}
.match-meta{display:flex;align-items:center;gap:8px;margin-bottom:14px;}
.match-series-name{font-size:11px;color:var(--muted);flex:1;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.badge{font-size:10px;font-weight:600;letter-spacing:0.08em;padding:3px 9px;border-radius:20px;text-transform:uppercase;white-space:nowrap;}
.badge-live{background:var(--red-dim);color:var(--red);border:0.5px solid rgba(239,68,68,0.3);}
.badge-result{background:var(--green-dim);color:var(--green);border:0.5px solid rgba(34,197,94,0.2);}
.badge-upcoming{background:rgba(255,255,255,0.04);color:var(--muted);border:0.5px solid var(--border);}
.teams-row{display:flex;align-items:center;gap:1rem;}
.team-block{flex:1;}
.team-block.right{text-align:right;}
.team-name-big{font-family:'Bebas Neue',sans-serif;font-size:24px;letter-spacing:0.05em;color:var(--text);line-height:1;}
.team-score-big{font-family:'JetBrains Mono',monospace;font-size:14px;color:var(--blue);margin-top:4px;}
.team-score-big.muted{color:var(--muted);}
.vs-divider{font-family:'Bebas Neue',sans-serif;font-size:14px;color:var(--muted);letter-spacing:0.1em;flex-shrink:0;}
.status-line{font-size:12px;color:var(--muted2);margin-top:10px;line-height:1.5;}
.status-line.winner{color:var(--gold);}
.table-card{background:var(--surface);border:0.5px solid var(--border);border-radius:12px;overflow:hidden;}
.table-head{display:grid;grid-template-columns:28px 1fr 36px 36px 36px 50px 70px 64px;padding:10px 16px;border-bottom:0.5px solid var(--border);background:rgba(255,255,255,0.02);}
.table-head span{font-size:10px;font-weight:600;letter-spacing:0.1em;text-transform:uppercase;color:var(--muted);text-align:center;}
.table-head span:nth-child(2){text-align:left;}
.table-row{display:grid;grid-template-columns:28px 1fr 36px 36px 36px 50px 70px 64px;padding:11px 16px;border-bottom:0.5px solid var(--border);align-items:center;transition:background 0.15s;}
.table-row:last-child{border-bottom:none;}
.table-row:hover{background:rgba(255,255,255,0.02);}
.table-row.qualify{border-left:2px solid var(--blue);padding-left:14px;}
.rank-num{font-size:11px;color:var(--muted);font-family:'JetBrains Mono',monospace;text-align:center;}
.team-info{display:flex;align-items:center;gap:10px;}
.team-dot{width:9px;height:9px;border-radius:50%;flex-shrink:0;}
.team-label{font-size:13px;font-weight:500;}
.qualify-tag{font-size:9px;font-weight:600;padding:2px 5px;border-radius:3px;background:var(--blue-dim);color:var(--blue);letter-spacing:0.06em;margin-left:5px;}
.cell{font-size:12px;font-family:'JetBrains Mono',monospace;text-align:center;color:var(--muted2);}
.cell.pts{font-weight:500;color:var(--text);font-size:13px;}
.nrr-pos{color:var(--green) !important;}
.nrr-neg{color:var(--red) !important;}
.stats-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
.stats-card{background:var(--surface);border:0.5px solid var(--border);border-radius:12px;overflow:hidden;}
.stats-card-head{padding:14px 16px;border-bottom:0.5px solid var(--border);display:flex;align-items:center;justify-content:space-between;}
.stats-card-title{font-family:'Bebas Neue',sans-serif;font-size:18px;letter-spacing:0.04em;}
.cap-badge{font-size:10px;font-weight:600;letter-spacing:0.06em;padding:4px 10px;border-radius:20px;}
.orange-cap{background:rgba(251,146,60,0.15);color:#fb923c;border:0.5px solid rgba(251,146,60,0.3);}
.purple-cap{background:var(--purple-dim);color:var(--purple);border:0.5px solid rgba(168,85,247,0.3);}
.player-row{display:flex;align-items:center;gap:10px;padding:10px 16px;border-bottom:0.5px solid var(--border);}
.player-row:last-child{border-bottom:none;}
.player-rank{font-size:10px;color:var(--muted);font-family:'JetBrains Mono',monospace;width:14px;flex-shrink:0;}
.player-details{flex:1;}
.player-name{font-size:13px;font-weight:500;}
.player-team-tag{font-size:9px;font-weight:600;padding:2px 5px;border-radius:3px;margin-left:6px;letter-spacing:0.05em;}
.player-stat-main{font-family:'Bebas Neue',sans-serif;font-size:20px;letter-spacing:0.04em;color:var(--blue);}
.player-stat-sub{font-size:10px;color:var(--muted);margin-top:1px;}
.bar-track{background:rgba(255,255,255,0.05);border-radius:2px;height:3px;margin-top:5px;}
.bar-fill{height:3px;border-radius:2px;}
.sched-card{display:flex;align-items:center;justify-content:space-between;background:var(--surface);border:0.5px solid var(--border);border-radius:10px;padding:12px 16px;margin-bottom:8px;transition:border-color 0.2s;}
.sched-card:hover{border-color:var(--border2);}
.sched-teams{display:flex;align-items:center;gap:8px;font-size:13px;font-weight:500;}
.sched-vs{font-size:10px;color:var(--muted);}
.sched-right{text-align:right;}
.sched-time{font-size:12px;color:var(--muted2);}
.sched-venue{font-size:11px;color:var(--muted);margin-top:2px;}
.date-divider{font-size:11px;font-weight:600;color:var(--muted2);letter-spacing:0.08em;text-transform:uppercase;padding:10px 0 8px;border-bottom:0.5px solid var(--border);margin-bottom:8px;}
.schedule-group{margin-bottom:1.5rem;}
.state-box{text-align:center;padding:3rem 2rem;color:var(--muted);}
.spinner{width:26px;height:26px;border:2px solid var(--border);border-top-color:var(--blue);border-radius:50%;animation:spin 0.8s linear infinite;margin:0 auto 1rem;}
@keyframes spin{to{transform:rotate(360deg)}}
.no-match-box{background:var(--surface);border:0.5px solid var(--border);border-radius:12px;padding:2rem;text-align:center;}
footer{text-align:center;padding:2rem;font-size:11px;color:var(--muted);border-top:0.5px solid var(--border);position:relative;z-index:1;margin-top:2rem;}
footer a{color:var(--blue);text-decoration:none;}
@media(max-width:700px){
  main{padding:1rem;}header{padding:0 1rem;}nav{padding:0 1rem;overflow-x:auto;}
  .tab{padding:12px 12px;white-space:nowrap;}
  .metrics{grid-template-columns:repeat(2,1fr);}
  .stats-grid{grid-template-columns:1fr;}
  .table-head,.table-row{grid-template-columns:24px 1fr 32px 32px 44px 58px;}
  .table-head span:nth-child(4),.table-row .cell-l{display:none;}
  .section-head{font-size:26px;}
}
</style>
</head>
<body>
<header>
  <div class="logo">
    <div class="logo-text">IPL 2026</div>
    <div class="logo-badge">TATA</div>
  </div>
  <div class="header-right">
    <div class="live-pill" id="livePill" style="display:none;">Live</div>
    <span class="last-updated" id="lastUpdated"></span>
    <button class="refresh-btn" onclick="loadAll()">↻ Refresh</button>
  </div>
</header>
<nav>
  <button class="tab active" onclick="switchTab('scores',this)">Scores</button>
  <button class="tab" onclick="switchTab('table',this)">Points Table</button>
  <button class="tab" onclick="switchTab('stats',this)">Stats</button>
  <button class="tab" onclick="switchTab('schedule',this)">Schedule</button>
</nav>
<main>
  <div id="panel-scores" class="panel active">
    <div class="section-head">Live <span>&amp; Recent</span></div>
    <div id="scores-content"><div class="state-box"><div class="spinner"></div>Fetching live scores...</div></div>
  </div>
  <div id="panel-table" class="panel">
    <div class="section-head">Points <span>Table</span></div>
    <span class="label">Updated after Match 28 · CSK vs KKR · Apr 18, 2026</span>
    <div class="table-card">
      <div class="table-head">
        <span>#</span><span>Team</span><span>M</span><span>W</span><span class="cell-l">L</span><span>NR</span><span>Pts</span><span>NRR</span>
      </div>
      <div id="points-table-body"></div>
    </div>
    <div style="margin-top:10px;font-size:11px;color:var(--muted);display:flex;align-items:center;gap:6px;">
      <div style="width:10px;height:2px;background:var(--blue);border-radius:2px;display:inline-block;"></div>
      Top 4 qualify for playoffs · Finals: May 31, 2026
    </div>
  </div>
  <div id="panel-stats" class="panel">
    <div class="section-head">Season <span>Stats</span></div>
    <span class="label">After Match 28 · Apr 18, 2026</span>
    <div class="stats-grid" id="stats-content"></div>
  </div>
  <div id="panel-schedule" class="panel">
    <div class="section-head">Upcoming <span>Fixtures</span></div>
    <div id="schedule-content"></div>
  </div>
</main>
<footer>
  IPL 2026 Live Dashboard &nbsp;·&nbsp; Live data via <a href="https://cricketdata.org" target="_blank">CricketData.org</a> &nbsp;·&nbsp; Auto-refreshes every 60s
</footer>
<script>
const API_KEY='5631a83f-551f-4e41-ad25-af64f20eee41';
const BASE='https://api.cricapi.com/v1';
const TC={
  'Punjab Kings':'#dc2626','PBKS':'#dc2626',
  'Royal Challengers Bengaluru':'#ef4444','RCB':'#ef4444',
  'Mumbai Indians':'#1d4ed8','MI':'#1d4ed8',
  'Chennai Super Kings':'#f59e0b','CSK':'#f59e0b',
  'Kolkata Knight Riders':'#7c3aed','KKR':'#7c3aed',
  'Rajasthan Royals':'#ec4899','RR':'#ec4899',
  'Gujarat Titans':'#0ea5e9','GT':'#0ea5e9',
  'Sunrisers Hyderabad':'#f97316','SRH':'#f97316',
  'Delhi Capitals':'#3b82f6','DC':'#3b82f6',
  'Lucknow Super Giants':'#06b6d4','LSG':'#06b6d4',
};
function tc(n){return TC[n]||'#8492b0';}

const TABLE=[
  {team:'Royal Challengers Bengaluru',short:'RCB',m:6,w:5,l:1,nr:0,pts:10,nrr:1.503},
  {team:'Punjab Kings',short:'PBKS',m:5,w:4,l:0,nr:1,pts:9,nrr:1.067},
  {team:'Rajasthan Royals',short:'RR',m:5,w:4,l:1,nr:0,pts:8,nrr:0.889},
  {team:'Sunrisers Hyderabad',short:'SRH',m:5,w:2,l:3,nr:0,pts:4,nrr:0.576},
  {team:'Delhi Capitals',short:'DC',m:4,w:2,l:2,nr:0,pts:4,nrr:0.322},
  {team:'Gujarat Titans',short:'GT',m:4,w:2,l:2,nr:0,pts:4,nrr:-0.029},
  {team:'Lucknow Super Giants',short:'LSG',m:5,w:2,l:3,nr:0,pts:4,nrr:-0.804},
  {team:'Chennai Super Kings',short:'CSK',m:6,w:2,l:4,nr:0,pts:4,nrr:-0.846},
  {team:'Mumbai Indians',short:'MI',m:5,w:1,l:4,nr:0,pts:2,nrr:-1.076},
  {team:'Kolkata Knight Riders',short:'KKR',m:6,w:0,l:5,nr:1,pts:1,nrr:-1.383},
];
const BATTERS=[
  {name:'Virat Kohli',team:'RCB',runs:228,avg:45.6,sr:153.0},
  {name:'Heinrich Klaasen',team:'SRH',runs:224,avg:44.8,sr:188.2},
  {name:'Vaibhav Suryavanshi',team:'RR',runs:200,avg:50.0,sr:178.6},
  {name:'Rajat Patidar',team:'RCB',runs:195,avg:65.0,sr:162.5},
  {name:'Shreyas Iyer',team:'PBKS',runs:203,avg:50.7,sr:187.0},
];
const BOWLERS=[
  {name:'Prasidh Krishna',team:'GT',wkts:10,avg:15.2,eco:7.60},
  {name:'Anshul Kamboj',team:'CSK',wkts:10,avg:19.6,eco:9.80},
  {name:'Ravi Bishnoi',team:'RR',wkts:9,avg:12.7,eco:6.35},
  {name:'Prince Yadav',team:'LSG',wkts:9,avg:18.4,eco:8.20},
  {name:'Jofra Archer',team:'MI',wkts:7,avg:21.0,eco:8.75},
];
const FIXTURES=[
  {date:'Sun, Apr 19',match:'PBKS vs LSG',teams:['PBKS','LSG'],venue:'New Chandigarh',time:'7:30 PM IST'},
  {date:'Mon, Apr 21',match:'GT vs MI',teams:['GT','MI'],venue:'Ahmedabad',time:'7:30 PM IST'},
  {date:'Tue, Apr 22',match:'SRH vs DC',teams:['SRH','DC'],venue:'Hyderabad',time:'7:30 PM IST'},
  {date:'Wed, Apr 23',match:'KKR vs RR',teams:['KKR','RR'],venue:'Kolkata',time:'7:30 PM IST'},
  {date:'Thu, Apr 24',match:'CSK vs RCB',teams:['CSK','RCB'],venue:'Chennai',time:'7:30 PM IST'},
  {date:'Fri, Apr 25',match:'MI vs SRH',teams:['MI','SRH'],venue:'Mumbai',time:'7:30 PM IST'},
  {date:'Sat, Apr 26',match:'PBKS vs GT',teams:['PBKS','GT'],venue:'New Chandigarh',time:'7:30 PM IST'},
  {date:'Sun, Apr 27',match:'DC vs LSG',teams:['DC','LSG'],venue:'Delhi',time:'3:30 PM IST'},
  {date:'Sun, Apr 27',match:'RR vs CSK',teams:['RR','CSK'],venue:'Jaipur',time:'7:30 PM IST'},
];

function switchTab(name,btn){
  document.querySelectorAll('.panel').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.tab').forEach(b=>b.classList.remove('active'));
  document.getElementById('panel-'+name).classList.add('active');
  btn.classList.add('active');
}

function fmtScore(scores){
  if(!scores||!scores.length)return'';
  return scores.map(s=>`${s.r}/${s.w} (${parseFloat(s.o).toFixed(1)})`).join(' & ');
}

function matchCard(m){
  const live=m.matchStarted&&!m.matchEnded;
  const ended=m.matchEnded;
  const t1=(m.teams&&m.teams[0])||'TBA';
  const t2=(m.teams&&m.teams[1])||'TBA';
  const sc=m.score||[];
  const s1=fmtScore(sc.filter((_,i)=>i===0));
  const s2=fmtScore(sc.filter((_,i)=>i===1));
  let badge=`<span class="badge badge-upcoming">Upcoming</span>`;
  if(live)badge=`<span class="badge badge-live">Live</span>`;
  if(ended)badge=`<span class="badge badge-result">Result</span>`;
  const status=m.status||'';
  const win=ended&&status.toLowerCase().includes('won');
  return`<div class="match-card ${live?'live-card':ended?'result-card':''}">
    <div class="match-meta"><span class="match-series-name">${m.name||''}</span>${badge}</div>
    <div class="teams-row">
      <div class="team-block"><div class="team-name-big">${t1}</div>${s1?`<div class="team-score-big">${s1}</div>`:''}</div>
      <div class="vs-divider">VS</div>
      <div class="team-block right"><div class="team-name-big">${t2}</div>${s2?`<div class="team-score-big${ended?' muted':''}">${s2}</div>`:''}</div>
    </div>
    ${status?`<div class="status-line${win?' winner':''}">${status}</div>`:''}
  </div>`;
}

async function loadScores(){
  const el=document.getElementById('scores-content');
  const metrics=`<div class="metrics">
    <div class="metric"><div class="metric-label">Season</div><div class="metric-value">IPL 2026</div><div class="metric-sub">19th edition · TATA</div></div>
    <div class="metric"><div class="metric-label">Matches played</div><div class="metric-value">28</div><div class="metric-sub">of 74 total</div></div>
    <div class="metric"><div class="metric-label">Orange cap</div><div class="metric-value">228</div><div class="metric-sub">Virat Kohli · RCB</div></div>
    <div class="metric"><div class="metric-label">Purple cap</div><div class="metric-value">10</div><div class="metric-sub">Prasidh Krishna · GT</div></div>
  </div>`;
  try{
    const res=await fetch(`${BASE}/currentMatches?apikey=${API_KEY}&offset=0`);
    const data=await res.json();
    if(data.status!=='success')throw new Error(data.reason||'API error');
    const all=data.data||[];
    const ipl=all.filter(m=>{
      const n=(m.name||'').toLowerCase();
      return n.includes('ipl')||n.includes('indian premier')||n.includes('t20');
    });
    const matches=ipl.length?ipl:all;
    document.getElementById('livePill').style.display=matches.some(m=>m.matchStarted&&!m.matchEnded)?'flex':'none';
    if(!matches.length){
      el.innerHTML=metrics+`<div class="no-match-box"><div style="font-size:28px;margin-bottom:10px;">🏏</div><div style="font-size:14px;color:var(--muted2);">No live IPL matches right now</div><div style="font-size:12px;color:var(--muted);margin-top:6px;">Next: PBKS vs LSG · Apr 19 · 7:30 PM IST · New Chandigarh</div></div>`;
      return;
    }
    const live=matches.filter(m=>m.matchStarted&&!m.matchEnded);
    const ended=matches.filter(m=>m.matchEnded);
    const upcoming=matches.filter(m=>!m.matchStarted);
    let html=metrics;
    if(live.length)html+=`<span class="label">Live now</span><div class="matches-grid" style="margin-bottom:1.5rem;">${live.map(matchCard).join('')}</div>`;
    if(ended.length)html+=`<span class="label">Recent results</span><div class="matches-grid" style="margin-bottom:1.5rem;">${ended.map(matchCard).join('')}</div>`;
    if(upcoming.length)html+=`<span class="label">Coming up</span><div class="matches-grid">${upcoming.map(matchCard).join('')}</div>`;
    el.innerHTML=html;
  }catch(e){
    el.innerHTML=metrics+`<div class="no-match-box"><div style="font-size:14px;color:var(--muted2);">Live feed unavailable right now</div><div style="font-size:11px;color:var(--red);margin-top:6px;">${e.message}</div><div style="font-size:12px;color:var(--muted);margin-top:8px;">Points table &amp; stats tabs are up to date</div></div>`;
  }
  document.getElementById('lastUpdated').textContent='Updated '+new Date().toLocaleTimeString('en-IN',{hour:'2-digit',minute:'2-digit'});
}

function renderTable(){
  const sorted=[...TABLE].sort((a,b)=>b.pts-a.pts||b.nrr-a.nrr);
  document.getElementById('points-table-body').innerHTML=sorted.map((t,i)=>{
    const q=i<4;
    const nrr=(t.nrr>=0?'+':'')+t.nrr.toFixed(3);
    return`<div class="table-row${q?' qualify':''}">
      <span class="rank-num">${i+1}</span>
      <div class="team-info">
        <div class="team-dot" style="background:${tc(t.short)};"></div>
        <div><div class="team-label">${t.short}${q?`<span class="qualify-tag">Q</span>`:''}</div></div>
      </div>
      <span class="cell">${t.m}</span>
      <span class="cell">${t.w}</span>
      <span class="cell cell-l">${t.l}</span>
      <span class="cell">${t.nr}</span>
      <span class="cell pts">${t.pts}</span>
      <span class="cell ${t.nrr>=0?'nrr-pos':'nrr-neg'}">${nrr}</span>
    </div>`;
  }).join('');
}

function renderStats(){
  const maxR=Math.max(...BATTERS.map(b=>b.runs));
  const maxW=Math.max(...BOWLERS.map(b=>b.wkts));
  const bHTML=BATTERS.sort((a,b)=>b.runs-a.runs).map((b,i)=>`
    <div class="player-row">
      <span class="player-rank">${i+1}</span>
      <div class="player-details">
        <div><span class="player-name">${b.name}</span><span class="player-team-tag" style="background:${tc(b.team)}22;color:${tc(b.team)};">${b.team}</span></div>
        <div style="font-size:10px;color:var(--muted);margin-top:2px;">Avg ${b.avg} &nbsp;·&nbsp; SR ${b.sr}</div>
        <div class="bar-track"><div class="bar-fill" style="width:${Math.round(b.runs/maxR*100)}%;background:${tc(b.team)};"></div></div>
      </div>
      <div style="text-align:right;flex-shrink:0;"><div class="player-stat-main">${b.runs}</div><div class="player-stat-sub">runs</div></div>
    </div>`).join('');
  const wHTML=BOWLERS.sort((a,b)=>b.wkts-a.wkts).map((b,i)=>`
    <div class="player-row">
      <span class="player-rank">${i+1}</span>
      <div class="player-details">
        <div><span class="player-name">${b.name}</span><span class="player-team-tag" style="background:${tc(b.team)}22;color:${tc(b.team)};">${b.team}</span></div>
        <div style="font-size:10px;color:var(--muted);margin-top:2px;">Avg ${b.avg} &nbsp;·&nbsp; Eco ${b.eco}</div>
        <div class="bar-track"><div class="bar-fill" style="width:${Math.round(b.wkts/maxW*100)}%;background:${tc(b.team)};"></div></div>
      </div>
      <div style="text-align:right;flex-shrink:0;"><div class="player-stat-main">${b.wkts}</div><div class="player-stat-sub">wickets</div></div>
    </div>`).join('');
  document.getElementById('stats-content').innerHTML=`
    <div class="stats-card">
      <div class="stats-card-head"><div class="stats-card-title">Top Run Scorers</div><div class="cap-badge orange-cap">Orange Cap</div></div>${bHTML}
    </div>
    <div class="stats-card">
      <div class="stats-card-head"><div class="stats-card-title">Top Wicket Takers</div><div class="cap-badge purple-cap">Purple Cap</div></div>${wHTML}
    </div>`;
}

function renderSchedule(){
  const grouped={};
  FIXTURES.forEach(f=>{if(!grouped[f.date])grouped[f.date]=[];grouped[f.date].push(f);});
  let html='';
  Object.entries(grouped).forEach(([date,ms])=>{
    html+=`<div class="schedule-group"><div class="date-divider">${date}</div>`;
    ms.forEach(m=>{
      const[t1,t2]=m.teams;
      html+=`<div class="sched-card">
        <div class="sched-teams">
          <span style="color:${tc(t1)};font-weight:600;">${t1}</span>
          <span class="sched-vs">vs</span>
          <span style="color:${tc(t2)};font-weight:600;">${t2}</span>
        </div>
        <div class="sched-right"><div class="sched-time">${m.time}</div><div class="sched-venue">${m.venue}</div></div>
      </div>`;
    });
    html+=`</div>`;
  });
  document.getElementById('schedule-content').innerHTML=html;
}

let timer;
function loadAll(){loadScores();renderTable();renderStats();renderSchedule();}
function startTimer(){if(timer)clearInterval(timer);timer=setInterval(loadScores,60000);}
loadAll();startTimer();
</script>
</body>
</html>
