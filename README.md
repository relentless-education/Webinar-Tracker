<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Relentless Education — Webinar & Events Tracker</title>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Helvetica,Arial,sans-serif;background:#111;color:#f0ede8;min-height:100vh}
.nav{display:flex;align-items:center;background:#0d0d0f;border-bottom:1px solid #252528;position:sticky;top:0;z-index:100;flex-wrap:wrap}
.brand{display:flex;align-items:center;gap:10px;padding:12px 20px;border-right:1px solid #252528;flex-shrink:0}
.bi{width:34px;height:34px;background:#F5E500;border-radius:7px;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:800;color:#111}
.bn{font-size:13px;font-weight:700;color:#F5E500;white-space:nowrap}
.nav-tabs{display:flex;overflow-x:auto;flex:1}
.nav-tabs::-webkit-scrollbar{height:2px}
.nt{padding:14px 16px;font-size:12px;font-weight:600;color:#666663;cursor:pointer;border-bottom:2px solid transparent;white-space:nowrap;background:none;border-top:none;border-left:none;border-right:none;font-family:inherit;transition:color 0.15s,border-color 0.15s}
.nt:hover{color:#c0bdb8}
.nt.active{color:#F5E500;border-bottom-color:#F5E500}
.pg{display:none;padding:28px 20px;max-width:1200px;margin:0 auto}
.pg.active{display:block}
.ph h1{font-size:24px;font-weight:700;color:#fff;letter-spacing:-0.025em;margin-bottom:6px}
.ph h1 em{color:#F5E500;font-style:normal}
.ph p{font-size:13px;color:#888885;line-height:1.5;margin-bottom:24px}
.sl{font-size:10px;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;color:#F5E500;margin-bottom:12px;margin-top:24px;opacity:0.85;display:block}

/* INPUTS */
.fi{width:100%;background:#141416;border:1px solid #2e2e32;border-radius:8px;padding:9px 12px;font-size:14px;font-weight:600;color:#fff;font-family:inherit;outline:none;transition:border-color 0.15s}
.fi:focus{border-color:#F5E500}
.fi::placeholder{color:#333331;font-weight:400}
.fi[type=number]::-webkit-inner-spin-button{-webkit-appearance:none}
select.fi{cursor:pointer}
.fl{font-size:12px;font-weight:500;color:#c0bdb8;margin-bottom:5px;display:block}
.fg{margin-bottom:14px}
.frow{display:flex;align-items:center;gap:6px}
.fpfx{font-size:14px;font-weight:600;color:#555552}

/* METRIC CARDS */
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:10px;margin-bottom:24px}
.mc{background:#1a1a1c;border:1px solid #2a2a2e;border-radius:12px;padding:14px}
.mc.y{background:#1a1900;border-color:#F5E500}
.mc.g{background:#0d1f0d;border-color:#1e4d1e}
.mc.r{background:#1f0d0d;border-color:#6d2424}
.mlb{font-size:10px;font-weight:700;letter-spacing:0.07em;text-transform:uppercase;color:#444442;margin-bottom:5px}
.mc.y .mlb{color:#b8a800}.mc.g .mlb{color:#3a6a3a}.mc.r .mlb{color:#8a4040}
.mv{font-size:20px;font-weight:800;letter-spacing:-0.02em;color:#666663}
.mc.y .mv{color:#F5E500}.mc.g .mv{color:#6dcf6d}.mc.r .mv{color:#e88080}
.ms{font-size:11px;color:#444442;margin-top:2px}

/* DATA ENTRY GRID */
.entry-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:8px;margin-bottom:20px}
.ebox{background:#141418;border:1px solid #252528;border-radius:10px;padding:12px 10px;display:flex;flex-direction:column;align-items:center;gap:5px;transition:border-color 0.15s}
.ebox:focus-within{border-color:#F5E500}
.ebox.ad{border-top:2px solid #8a7000}
.ebox.org{border-top:2px solid #2a5a2a}
.ebox.web{border-top:2px solid #2a2a8a}
.ebox.app{border-top:2px solid #6a2a8a}
.ebox.sale{border-top:2px solid #8a2a2a}
.ebox-grp{font-size:8px;font-weight:700;letter-spacing:0.08em;text-transform:uppercase;opacity:0.7}
.ebox.ad .ebox-grp{color:#c8a800}
.ebox.org .ebox-grp{color:#4a8a4a}
.ebox.web .ebox-grp{color:#5a6adf}
.ebox.app .ebox-grp{color:#8a5adf}
.ebox.sale .ebox-grp{color:#df5a5a}
.ebox-label{font-size:9px;font-weight:600;color:#888885;text-align:center;line-height:1.3}
.ebox input{background:transparent;border:none;outline:none;font-size:22px;font-weight:800;color:#fff;text-align:center;width:100%;font-family:inherit}
.ebox input::placeholder{color:#2a2a28;font-size:16px;font-weight:400}
.ebox input[type=number]::-webkit-inner-spin-button{-webkit-appearance:none}

/* RESULTS */
.res-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:10px;margin-bottom:20px}
.ri{background:#141418;border:1px solid #252528;border-radius:10px;padding:12px 14px}
.ri-lb{font-size:10px;font-weight:700;letter-spacing:0.07em;text-transform:uppercase;color:#444442;margin-bottom:4px}
.ri-v{font-size:18px;font-weight:800;color:#888885}
.ri-bm{font-size:11px;color:#444442;margin-top:2px}
.good{color:#6dcf6d!important}.ok{color:#F5E500!important}.bad{color:#e88080!important}.hi{color:#F5E500!important}

/* FUNNEL */
.funnel{display:grid;grid-template-columns:repeat(auto-fit,minmax(75px,1fr));gap:1px;border-radius:10px;overflow:hidden;border:1px solid #252528;margin-bottom:20px}
.fs{background:#141416;padding:12px 6px;text-align:center;border-right:1px solid #1c1c1e}
.fs:last-child{border-right:none;background:#1a1900}
.fs-lb{font-size:8px;font-weight:700;letter-spacing:0.06em;text-transform:uppercase;color:#555552;margin-bottom:4px}
.fs-v{font-size:18px;font-weight:800;color:#888885}
.fs:last-child .fs-v{color:#F5E500}
.fs-bar{height:3px;background:#252528;border-radius:2px;margin-top:5px;overflow:hidden}
.fs-fill{height:100%;background:#2e2e40;border-radius:2px}
.fs:last-child .fs-fill{background:#F5E500}

/* TABLE */
.tw{overflow-x:auto;border-radius:12px;border:1px solid #252528;margin-bottom:20px}
table{width:100%;border-collapse:collapse;font-size:12px}
thead th{background:#141416;color:#888885;font-weight:700;padding:9px 12px;text-align:center;white-space:nowrap;border-bottom:1px solid #252528;font-size:10px;letter-spacing:0.05em;text-transform:uppercase}
thead th.tl{text-align:left}
tbody td{padding:8px 12px;border-bottom:1px solid #1c1c1e;color:#c0bdb8;text-align:center;white-space:nowrap}
tbody td.tl{text-align:left;color:#f0ede8;font-weight:600}
tbody tr:last-child td{border-bottom:none}
tbody tr:hover td{background:rgba(255,255,255,0.02)}

/* BUTTONS */
.btn{display:inline-flex;align-items:center;gap:6px;padding:9px 16px;border-radius:8px;font-size:13px;font-weight:600;font-family:inherit;cursor:pointer;transition:all 0.15s;border:1px solid #2e2e32;background:transparent;color:#c0bdb8}
.btn:hover{border-color:#F5E500;color:#F5E500}
.btnp{background:#F5E500;color:#111;border-color:#F5E500}
.btnp:hover{background:#e0d100;color:#111}
.btns{padding:6px 12px;font-size:12px}
.btn:active{transform:scale(0.98)}
.btnr{color:#e88080;border-color:#6d2424}
.btnr:hover{color:#e88080;border-color:#e88080}

/* EVENT TABS */
.ev-tabs{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:20px}
.ev-tab{padding:7px 14px;font-size:12px;font-weight:600;border-radius:8px;border:1px solid #2e2e32;background:transparent;color:#666663;cursor:pointer;font-family:inherit;transition:all 0.15s}
.ev-tab:hover{border-color:#383838;color:#c0bdb8}
.ev-tab.active{background:#1a1900;border-color:#F5E500;color:#F5E500}

/* EVENT CARDS */
.ev-card{background:#141418;border:1px solid #2a2a2e;border-radius:12px;padding:18px 20px;margin-bottom:14px}
.badge{display:inline-flex;padding:3px 9px;border-radius:5px;font-size:10px;font-weight:700;letter-spacing:0.05em;text-transform:uppercase}
.bl{background:#0d1f0d;color:#6dcf6d;border:1px solid #1e4d1e}
.bu{background:#1a1900;color:#F5E500;border:1px solid #3a3600}
.bc{background:#1a1a1c;color:#666663;border:1px solid #2a2a2e}

.g2{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.card{background:#1a1a1c;border:1px solid #2a2a2e;border-radius:12px;padding:16px 18px;margin-bottom:12px}
.card-title{font-size:13px;font-weight:600;color:#c0bdb8;margin-bottom:12px}
.tip{font-size:12px;color:#555552;margin-top:4px;line-height:1.5}
.ibox{background:#1a1900;border:1px solid #2e2b00;border-left:3px solid #F5E500;border-radius:8px;padding:12px 16px;margin-bottom:16px}
.ibox p{font-size:13px;color:#c0bdb8;line-height:1.6}
.ibox strong{color:#F5E500}
</style>
</head>
<body>

<nav class="nav">
  <div class="brand">
    <div class="bi">RE</div>
    <span class="bn">Webinar & Events Tracker</span>
  </div>
  <div class="nav-tabs">
    <button class="nt active" onclick="gp('events',this)">Events</button>
    <button class="nt" onclick="gp('log',this)">Event Log</button>
    <button class="nt" onclick="gp('summary',this)">Summary</button>
    <button class="nt" onclick="gp('benchmarks',this)">Benchmarks</button>
  </div>
</nav>

<!-- EVENTS -->
<div class="pg active" id="pg-events">
  <div class="ph">
    <h1>Webinar & <em>Events</em></h1>
    <p>Add each webinar or event then click "Enter Data" to log your numbers.</p>
  </div>
  <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:16px">
    <span class="sl" style="margin:0">Your Events</span>
    <button class="btn btnp btns" onclick="addEvent()">+ New Event</button>
  </div>
  <div id="ev-list"></div>
  <div id="ev-empty" style="display:none;text-align:center;padding:60px 20px;color:#555552">
    <div style="font-size:36px;margin-bottom:12px">📅</div>
    <div style="font-size:15px;font-weight:600;color:#888885;margin-bottom:16px">No events yet</div>
    <button class="btn btnp" onclick="addEvent()">+ Add Your First Event</button>
  </div>
</div>

<!-- LOG -->
<div class="pg" id="pg-log">
  <div class="ph">
    <h1>Event <em>Log</em></h1>
    <p>Select an event and enter your numbers. All conversion rates calculate instantly.</p>
  </div>
  <div class="ev-tabs" id="log-tabs"></div>
  <!-- Each event gets a persistent panel built once and shown/hidden -->
  <div id="log-panels"></div>
</div>

<!-- SUMMARY -->
<div class="pg" id="pg-summary">
  <div class="ph">
    <h1>All Events <em>Summary</em></h1>
    <p>Aggregated results across all your webinars and events.</p>
  </div>
  <div class="cards" id="sum-cards"></div>
  <span class="sl" style="margin-top:0">Conversion Funnel — All Events Combined</span>
  <div class="funnel" id="sum-funnel"></div>
  <span class="sl">All Events Comparison</span>
  <div class="tw" id="sum-table"></div>
</div>

<!-- BENCHMARKS -->
<div class="pg" id="pg-benchmarks">
  <div class="ph">
    <h1>Benchmarks &amp; <em>ROI Calculator</em></h1>
    <p>Plan your webinar ROI before you run it, and set conversion targets that colour-code your actuals in the Event Log.</p>
  </div>

  <div class="ibox"><p><strong>Green</strong> = on or above target &nbsp;·&nbsp; <strong>Yellow</strong> = within 80% of target &nbsp;·&nbsp; <strong>Red</strong> = below target. Changes here instantly update colour-coding in all event logs.</p></div>

  <!-- PRE-EVENT ROI CALCULATOR -->
  <span class="sl" style="margin-top:0">Pre-Event ROI Calculator</span>
  <p style="font-size:13px;color:#888885;margin-bottom:16px;line-height:1.6">Enter your targets to project your funnel, revenue and ROI before running the event.</p>

  <div class="g2" style="margin-bottom:8px">
    <div>
      <div class="card">
        <div class="card-title">📢 Ad Spend</div>
        <div class="fg"><label class="fl">Ad Budget (ex. GST)</label><div class="frow"><span class="fpfx">$</span><input class="fi" id="rc-adspend" type="number" placeholder="0" oninput="calcRC()"/></div></div>
        <div class="fg"><label class="fl">Target Cost Per Lead ($)</label><div class="frow"><span class="fpfx">$</span><input class="fi" id="rc-cpl" type="number" placeholder="0" oninput="calcRC()"/></div><p class="tip">Projected registrations = Budget ÷ CPL</p></div>
        <div class="fg"><label class="fl">Management Fee (if applicable)</label><div class="frow"><span class="fpfx">$</span><input class="fi" id="rc-mgmt" type="number" placeholder="0" oninput="calcRC()"/></div></div>
      </div>
      <div class="card">
        <div class="card-title">🎙 Webinar Funnel</div>
        <div class="fg"><label class="fl">Expected Attend Rate (%)</label><div class="frow"><input class="fi" id="rc-att" type="number" placeholder="30" oninput="calcRC()"/><span class="fpfx">%</span></div></div>
        <div class="fg"><label class="fl">Expected Application Rate (%)</label><div class="frow"><input class="fi" id="rc-app" type="number" placeholder="20" oninput="calcRC()"/><span class="fpfx">%</span></div></div>
        <div class="fg"><label class="fl">Expected Booking Rate (%)</label><div class="frow"><input class="fi" id="rc-bk" type="number" placeholder="60" oninput="calcRC()"/><span class="fpfx">%</span></div></div>
      </div>
      <div class="card">
        <div class="card-title">💰 Sales</div>
        <div class="fg"><label class="fl">Expected Show Rate (%)</label><div class="frow"><input class="fi" id="rc-sh" type="number" placeholder="80" oninput="calcRC()"/><span class="fpfx">%</span></div></div>
        <div class="fg"><label class="fl">Expected Close Rate (%)</label><div class="frow"><input class="fi" id="rc-cl" type="number" placeholder="30" oninput="calcRC()"/><span class="fpfx">%</span></div></div>
        <div class="fg"><label class="fl">Avg. Program Sale Value (ex. GST)</label><div class="frow"><span class="fpfx">$</span><input class="fi" id="rc-sale" type="number" placeholder="0" oninput="calcRC()"/></div></div>
      </div>
    </div>

    <div>
      <span class="sl" style="margin-top:0">Projected Funnel</span>
      <div id="rc-funnel" style="display:flex;flex-direction:column;gap:6px;margin-bottom:20px"></div>

      <span class="sl">Projected Results</span>
      <div id="rc-results" style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:16px"></div>

      <div id="rc-tip" style="display:none;background:#161600;border:1px solid #2e2b00;border-left:3px solid #F5E500;border-radius:8px;padding:14px 16px;margin-bottom:16px">
        <p id="rc-tip-text" style="font-size:13px;color:#c0bdb8;line-height:1.7"></p>
      </div>

      <button class="btn btns" onclick="resetRC()">Reset calculator</button>
    </div>
  </div>

  <hr style="border:none;border-top:1px solid #252528;margin:28px 0"/>

  <!-- CONVERSION BENCHMARKS -->
  <span class="sl" style="margin-top:0">Conversion Rate Benchmarks</span>
  <p style="font-size:13px;color:#888885;margin-bottom:16px;line-height:1.6">These targets colour-code your actuals across all event logs.</p>

  <div class="g2">
    <div class="card">
      <div class="card-title">Advertising & Webinar</div>
      <div class="fg"><label class="fl">Target Ad CPL ($)</label><div class="frow"><span class="fpfx">$</span><input class="fi" id="bm-cpl" type="number" placeholder="15" onchange="saveBM()"/></div><p class="tip">Cost per lead from paid ads</p></div>
      <div class="fg"><label class="fl">Target Attended Rate (%)</label><div class="frow"><input class="fi" id="bm-att" type="number" placeholder="30" onchange="saveBM()"/><span class="fpfx">%</span></div><p class="tip">% of registrants who show up</p></div>
      <div class="fg"><label class="fl">Target Application Rate (%)</label><div class="frow"><input class="fi" id="bm-app" type="number" placeholder="20" onchange="saveBM()"/><span class="fpfx">%</span></div><p class="tip">% of attendees who apply</p></div>
      <div class="fg"><label class="fl">Target Booking Rate (%)</label><div class="frow"><input class="fi" id="bm-bk" type="number" placeholder="60" onchange="saveBM()"/><span class="fpfx">%</span></div><p class="tip">% of applicants who book a call</p></div>
    </div>
    <div class="card">
      <div class="card-title">Sales & Returns</div>
      <div class="fg"><label class="fl">Target Show Rate (%)</label><div class="frow"><input class="fi" id="bm-sh" type="number" placeholder="80" onchange="saveBM()"/><span class="fpfx">%</span></div><p class="tip">% of booked calls that attend</p></div>
      <div class="fg"><label class="fl">Target Close Rate (%)</label><div class="frow"><input class="fi" id="bm-cl" type="number" placeholder="30" onchange="saveBM()"/><span class="fpfx">%</span></div><p class="tip">% of attended calls that buy</p></div>
      <div class="fg"><label class="fl">Target CPA ($)</label><div class="frow"><span class="fpfx">$</span><input class="fi" id="bm-cpa" type="number" placeholder="500" onchange="saveBM()"/></div><p class="tip">Target cost per acquisition</p></div>
      <div class="fg"><label class="fl">Target ROI (%)</label><div class="frow"><input class="fi" id="bm-roi" type="number" placeholder="200" onchange="saveBM()"/><span class="fpfx">%</span></div><p class="tip">Min return on ad spend %</p></div>
      <div class="fg"><label class="fl">Target ROAS (x)</label><div class="frow"><input class="fi" id="bm-roas" type="number" placeholder="3" step="0.1" onchange="saveBM()"/><span class="fpfx">x</span></div><p class="tip">Revenue ÷ ad spend target</p></div>
    </div>
  </div>

  <span class="sl">Current Benchmarks at a Glance</span>
  <div class="cards" id="bm-summary-cards"></div>
</div>
<script>
// ====== STATE ======
let S = {
  events: [],
  bm: {cpl:15,att:30,app:20,bk:60,sh:80,cl:30,cpa:500,roi:200,roas:3},
  activeLog: null
};

// Key insight: we store which panels have been built so we never rebuild them
const builtPanels = new Set();

function save(){ localStorage.setItem('re-wbt4', JSON.stringify(S)); }
function load(){
  try{
    ['re-webinar','re-webinar2','re-wb3'].forEach(k=>localStorage.removeItem(k));
    const d = localStorage.getItem('re-wbt4');
    if(d) S = JSON.parse(d);
  }catch(e){}
}

// ====== NAV ======
function gp(id, btn){
  document.querySelectorAll('.pg').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nt').forEach(t=>t.classList.remove('active'));
  document.getElementById('pg-'+id).classList.add('active');
  if(btn) btn.classList.add('active');
  if(id==='log'){ rebuildLogTabs(); showActivePanel(); }
  if(id==='summary') rSummary();
  if(id==='benchmarks'){ loadBMInputs(); renderBMCards(); }
}

// ====== FORMATTING ======
function fD(n){ if(n===null||n===undefined||!isFinite(n)||n===0)return '—'; return '$'+Math.round(Math.abs(n)).toLocaleString('en-AU'); }
function fP(n){ if(n===null||n===undefined||!isFinite(n))return '—'; return (n*100).toFixed(1)+'%'; }
function fN(n){ if(n===null||n===undefined)return '—'; const r=Math.round(n); return r===0?'0':r.toLocaleString('en-AU'); }
function safe(a,b){ return (b&&b>0) ? a/b : null; }

function rCls(actual, target, lower=false){
  if(actual===null||actual===undefined||!isFinite(actual)||!target) return '';
  const r = actual/target;
  if(lower) return r<=1?'good':r<=1.3?'ok':'bad';
  return r>=1?'good':r>=0.8?'ok':'bad';
}

// ====== CALC ======
function calc(ev){
  const d = ev.data||{};
  const totalReg = (d.adReg||0)+(d.orgReg||0);
  const m = {
    totalReg,
    adCPL:    safe(d.adSpend, d.adReg),
    attRate:  safe(d.attended, totalReg),
    appRate:  safe(d.appFilled, d.attended),
    bkRate:   safe(d.bookedCall, d.appFilled),
    shRate:   safe(d.attendedCall, d.bookedCall),
    depRate:  safe(d.deposit, d.attendedCall),
    closeRate:safe(d.purchased, d.attendedCall),
    l2s:      safe(d.purchased, totalReg),
    cpa:      safe(d.adSpend, d.purchased),
    revenue:  (d.purchased||0)*(d.avgSaleValue||0),
  };
  m.roi  = d.adSpend>0 ? (m.revenue - d.adSpend)/d.adSpend : null;
  m.roas = safe(m.revenue, d.adSpend);
  return m;
}

// ====== EVENTS PAGE ======
function addEvent(){
  const ev = {
    id: Date.now(),
    name: 'New Webinar',
    date: new Date().toISOString().split('T')[0],
    type: 'webinar',
    status: 'upcoming',
    data: {
      adSpend:0,adReg:0,dms:0,emails:0,content:0,orgReg:0,
      registered:0,attended:0,appFilled:0,saidYes:0,saidNo:0,
      bookedCall:0,attendedCall:0,deposit:0,purchased:0,avgSaleValue:0
    }
  };
  S.events.unshift(ev);
  S.activeLog = ev.id;
  save();
  rEventList();
  // Open the log for this event
  gp('log', document.querySelectorAll('.nt')[1]);
}

function deleteEvent(id){
  if(!confirm('Delete this event? Cannot be undone.')) return;
  S.events = S.events.filter(e=>e.id!==id);
  builtPanels.delete(id);
  const panel = document.getElementById('panel-'+id);
  if(panel) panel.remove();
  if(S.activeLog===id) S.activeLog = S.events.length ? S.events[0].id : null;
  save();
  rEventList();
  rebuildLogTabs();
}

function setMeta(id, field, val){
  const ev = S.events.find(e=>e.id===id);
  if(!ev) return;
  ev[field] = val;
  save();
  // Update the name shown in the panel header if it exists
  const hdr = document.getElementById('panel-hdr-'+id);
  if(hdr && field==='name') hdr.textContent = val;
  // Update tab label
  const tab = document.getElementById('tab-'+id);
  if(tab && field==='name') tab.textContent = val;
  // Refresh the event card summary stats
  refreshEvCardStats(id);
}

function refreshEvCardStats(id){
  const ev = S.events.find(e=>e.id===id);
  if(!ev) return;
  const m = calc(ev);
  const el = document.getElementById('evstats-'+id);
  if(el) el.innerHTML = evStatsHTML(ev, m);
}

function evStatsHTML(ev, m){
  const d = ev.data;
  return [
    {l:'Total Regs', v:fN(m.totalReg)},
    {l:'Attended',   v:fN(d.attended)},
    {l:'Applied',    v:fN(d.appFilled)},
    {l:'Sales',      v:fN(d.purchased), y:true},
    {l:'Revenue',    v:fD(m.revenue), g:true},
    {l:'Ad Spend',   v:fD(d.adSpend)},
    {l:'ROI', v:m.roi!==null?(m.roi*100).toFixed(0)+'%':'—', g:m.roi>0, r:m.roi!==null&&m.roi<=0},
    {l:'Close Rate', v:fP(m.closeRate)},
  ].map(x=>`
    <div style="background:#1a1a1c;border:1px solid #252528;border-radius:8px;padding:10px 12px">
      <div style="font-size:9px;font-weight:700;letter-spacing:.07em;text-transform:uppercase;color:#444442;margin-bottom:3px">${x.l}</div>
      <div style="font-size:15px;font-weight:800;color:${x.y?'#F5E500':x.g?'#6dcf6d':x.r?'#e88080':'#c0bdb8'}">${x.v}</div>
    </div>`).join('');
}

function rEventList(){
  const el = document.getElementById('ev-list');
  const empty = document.getElementById('ev-empty');
  if(!S.events.length){ el.innerHTML=''; empty.style.display='block'; return; }
  empty.style.display='none';

  el.innerHTML = S.events.map(ev=>{
    const m = calc(ev);
    const bCls = ev.status==='live'?'bl':ev.status==='completed'?'bc':'bu';
    const bLbl = ev.status==='live'?'Live':ev.status==='completed'?'Completed':'Upcoming';
    return `
    <div class="ev-card">
      <div style="display:flex;justify-content:space-between;align-items:flex-start;margin-bottom:14px;flex-wrap:wrap;gap:10px">
        <div>
          <div style="font-size:16px;font-weight:700;color:#fff">${ev.name}</div>
          <div style="font-size:12px;color:#888885;margin-top:3px">${ev.date} · ${ev.type}</div>
        </div>
        <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap">
          <span class="badge ${bCls}">${bLbl}</span>
          <button class="btn btns" onclick="openLog(${ev.id})" style="border-color:#F5E500;color:#F5E500">Enter Data ↗</button>
          <button class="btn btns btnr" onclick="deleteEvent(${ev.id})">Delete</button>
        </div>
      </div>
      <div class="g2" style="margin-bottom:14px">
        <div style="display:flex;flex-direction:column;gap:8px">
          <div><label class="fl">Event Name</label>
            <input class="fi" value="${ev.name}" placeholder="Event name" style="font-size:13px"
              onchange="setMeta(${ev.id},'name',this.value)"/>
          </div>
          <div><label class="fl">Date</label>
            <input class="fi" type="date" value="${ev.date}" onchange="setMeta(${ev.id},'date',this.value)"/>
          </div>
        </div>
        <div style="display:flex;flex-direction:column;gap:8px">
          <div><label class="fl">Type</label>
            <select class="fi" onchange="setMeta(${ev.id},'type',this.value)">
              <option value="webinar" ${ev.type==='webinar'?'selected':''}>Webinar</option>
              <option value="live" ${ev.type==='live'?'selected':''}>Live Event</option>
              <option value="workshop" ${ev.type==='workshop'?'selected':''}>Workshop</option>
              <option value="challenge" ${ev.type==='challenge'?'selected':''}>Challenge</option>
            </select>
          </div>
          <div><label class="fl">Status</label>
            <select class="fi" onchange="setMeta(${ev.id},'status',this.value)">
              <option value="upcoming" ${ev.status==='upcoming'?'selected':''}>Upcoming</option>
              <option value="live" ${ev.status==='live'?'selected':''}>Live</option>
              <option value="completed" ${ev.status==='completed'?'selected':''}>Completed</option>
            </select>
          </div>
        </div>
      </div>
      <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(110px,1fr));gap:8px" id="evstats-${ev.id}">
        ${evStatsHTML(ev,m)}
      </div>
    </div>`;
  }).join('');
}

// ====== LOG PAGE — persistent panels ======
function openLog(id){
  S.activeLog = id;
  save();
  gp('log', document.querySelectorAll('.nt')[1]);
}

function rebuildLogTabs(){
  const el = document.getElementById('log-tabs');
  if(!S.events.length){ el.innerHTML='<div style="color:#555552;font-size:13px">No events yet — add one on the Events tab.</div>'; return; }
  el.innerHTML = S.events.map(ev=>
    `<button class="ev-tab ${S.activeLog===ev.id?'active':''}" id="tab-${ev.id}"
      onclick="switchLogPanel(${ev.id})">${ev.name}</button>`
  ).join('');
}

function switchLogPanel(id){
  S.activeLog = id;
  save();
  // Update tab highlights
  document.querySelectorAll('.ev-tab').forEach(t=>t.classList.remove('active'));
  const tab = document.getElementById('tab-'+id);
  if(tab) tab.classList.add('active');
  showActivePanel();
}

function showActivePanel(){
  if(!S.activeLog && S.events.length) S.activeLog = S.events[0].id;
  // Hide all panels
  document.querySelectorAll('.log-panel').forEach(p=>p.style.display='none');
  if(!S.activeLog) return;

  // Build panel if not yet built
  if(!builtPanels.has(S.activeLog)){
    buildPanel(S.activeLog);
  }

  const panel = document.getElementById('panel-'+S.activeLog);
  if(panel) panel.style.display='block';
}

const FIELDS = [
  {key:'adSpend',   label:'Ad Spend ($)',           grp:'ad',   dollar:true},
  {key:'adReg',     label:'Ad Registrations',        grp:'ad'},
  {key:'dms',       label:'DMs Sent',                grp:'org'},
  {key:'emails',    label:'Emails Sent',             grp:'org'},
  {key:'content',   label:'Content Posts',           grp:'org'},
  {key:'orgReg',    label:'Organic Registrations',   grp:'org'},
  {key:'registered',label:'Registered on GHL',       grp:'web'},
  {key:'attended',  label:'Attended Webinar',        grp:'web'},
  {key:'appFilled', label:'Filled Application',      grp:'app'},
  {key:'saidYes',   label:'Said Yes',                grp:'app'},
  {key:'saidNo',    label:'Said No',                 grp:'app'},
  {key:'bookedCall',label:'Booked a Call',           grp:'app'},
  {key:'attendedCall',label:'Attended Call',         grp:'sale'},
  {key:'deposit',   label:'Deposit Paid',            grp:'sale'},
  {key:'purchased', label:'Purchased',               grp:'sale'},
];

const GRP_LABELS = {ad:'📢 Ad',org:'🌱 Organic',web:'🎙 Webinar',app:'📋 Application',sale:'💰 Sale'};

// Build a panel once using real DOM elements — never innerHTML for inputs
function buildPanel(id){
  const ev = S.events.find(e=>e.id===id);
  if(!ev) return;
  builtPanels.add(id);

  const container = document.getElementById('log-panels');
  const panel = document.createElement('div');
  panel.className = 'log-panel';
  panel.id = 'panel-'+id;
  panel.style.display = 'none';

  // Header
  const hdr = document.createElement('div');
  hdr.style.cssText = 'margin-bottom:20px';
  hdr.innerHTML = `<div style="font-size:18px;font-weight:700;color:#fff" id="panel-hdr-${id}">${ev.name}</div>
    <div style="font-size:12px;color:#888885;margin-top:3px">${ev.date} · ${ev.type}</div>`;
  panel.appendChild(hdr);

  // Section: Enter Numbers
  const s1lbl = document.createElement('span');
  s1lbl.className = 'sl';
  s1lbl.style.marginTop = '0';
  s1lbl.textContent = 'Enter Your Numbers';
  panel.appendChild(s1lbl);

  // Entry grid — built with real DOM elements so they never get wiped
  const grid = document.createElement('div');
  grid.className = 'entry-grid';
  FIELDS.forEach(f=>{
    const box = document.createElement('div');
    box.className = `ebox ${f.grp}`;

    const grpLabel = document.createElement('div');
    grpLabel.className = 'ebox-grp';
    grpLabel.textContent = GRP_LABELS[f.grp];
    box.appendChild(grpLabel);

    const fLabel = document.createElement('div');
    fLabel.className = 'ebox-label';
    fLabel.textContent = f.label;
    box.appendChild(fLabel);

    const inp = document.createElement('input');
    inp.type = 'number';
    inp.min = '0';
    inp.placeholder = '0';
    inp.value = ev.data[f.key] || '';
    // oninput: update state and refresh ONLY the calculated outputs (not inputs)
    inp.addEventListener('input', function(){
      const evLive = S.events.find(e=>e.id===id);
      if(!evLive) return;
      evLive.data[f.key] = parseFloat(this.value)||0;
      save();
      refreshPanelOutputs(id);
      refreshEvCardStats(id);
    });
    box.appendChild(inp);
    grid.appendChild(box);
  });
  panel.appendChild(grid);

  // Avg sale value
  const avgWrap = document.createElement('div');
  avgWrap.style.cssText = 'max-width:280px;margin-bottom:20px';
  avgWrap.innerHTML = `<label class="fl">Average Sale Value — ex. GST ($)</label>`;
  const avgRow = document.createElement('div');
  avgRow.className = 'frow';
  const avgPfx = document.createElement('span');
  avgPfx.className = 'fpfx';
  avgPfx.textContent = '$';
  const avgInp = document.createElement('input');
  avgInp.className = 'fi';
  avgInp.type = 'number';
  avgInp.placeholder = '0';
  avgInp.value = ev.data.avgSaleValue || '';
  avgInp.addEventListener('input', function(){
    const evLive = S.events.find(e=>e.id===id);
    if(!evLive) return;
    evLive.data.avgSaleValue = parseFloat(this.value)||0;
    save();
    refreshPanelOutputs(id);
    refreshEvCardStats(id);
  });
  avgRow.appendChild(avgPfx);
  avgRow.appendChild(avgInp);
  avgWrap.appendChild(avgRow);
  panel.appendChild(avgWrap);

  // Output sections — these get innerHTML-replaced on every update (safe because no inputs)
  const funnelLbl = document.createElement('span');
  funnelLbl.className = 'sl';
  funnelLbl.textContent = 'Conversion Funnel';
  panel.appendChild(funnelLbl);

  const funnelEl = document.createElement('div');
  funnelEl.className = 'funnel';
  funnelEl.id = `funnel-${id}`;
  panel.appendChild(funnelEl);

  const resLbl = document.createElement('span');
  resLbl.className = 'sl';
  resLbl.textContent = 'Calculated Results';
  panel.appendChild(resLbl);

  const resEl = document.createElement('div');
  resEl.className = 'res-grid';
  resEl.id = `res-${id}`;
  panel.appendChild(resEl);

  const bmLbl = document.createElement('span');
  bmLbl.className = 'sl';
  bmLbl.textContent = 'Metrics vs Your Benchmarks';
  panel.appendChild(bmLbl);

  const bmWrap = document.createElement('div');
  bmWrap.className = 'tw';
  bmWrap.innerHTML = `<table><thead><tr>
    <th class="tl">Metric</th>
    <th>Your Result</th>
    <th>Benchmark</th>
    <th>Status</th>
  </tr></thead><tbody id="bmt-${id}"></tbody></table>`;
  panel.appendChild(bmWrap);

  container.appendChild(panel);

  // Initial render of outputs
  refreshPanelOutputs(id);
}

// Refresh ONLY the calculated output sections — inputs are untouched
function refreshPanelOutputs(id){
  const ev = S.events.find(e=>e.id===id);
  if(!ev) return;
  const d = ev.data;
  const m = calc(ev);
  const bm = S.bm;

  // Funnel
  const fEl = document.getElementById(`funnel-${id}`);
  if(fEl){
    const steps=[
      {l:'Ad Regs',v:d.adReg||0},
      {l:'Org Regs',v:d.orgReg||0},
      {l:'Total Regs',v:m.totalReg},
      {l:'Attended',v:d.attended||0},
      {l:'Applied',v:d.appFilled||0},
      {l:'Booked',v:d.bookedCall||0},
      {l:'Showed',v:d.attendedCall||0},
      {l:'Purchased',v:d.purchased||0},
    ];
    const maxV = Math.max(...steps.map(s=>s.v), 1);
    fEl.innerHTML = steps.map(s=>`
      <div class="fs">
        <div class="fs-lb">${s.l}</div>
        <div class="fs-v">${s.v}</div>
        <div class="fs-bar"><div class="fs-fill" style="width:${(s.v/maxV*100).toFixed(1)}%"></div></div>
      </div>`).join('');
  }

  // Results cards
  const rEl = document.getElementById(`res-${id}`);
  if(rEl){
    const items=[
      {l:'Total Registrations', v:fN(m.totalReg), c:''},
      {l:'Ad CPL',  v:m.adCPL!==null?fD(m.adCPL):'—',   c:rCls(m.adCPL,bm.cpl,true),  bm:'Target: $'+bm.cpl},
      {l:'Attended Rate', v:fP(m.attRate),  c:rCls(m.attRate&&m.attRate*100,bm.att),  bm:'Target: '+bm.att+'%'},
      {l:'Application Rate', v:fP(m.appRate), c:rCls(m.appRate&&m.appRate*100,bm.app), bm:'Target: '+bm.app+'%'},
      {l:'Booking Rate',   v:fP(m.bkRate),   c:rCls(m.bkRate&&m.bkRate*100,bm.bk),   bm:'Target: '+bm.bk+'%'},
      {l:'Show Rate',      v:fP(m.shRate),   c:rCls(m.shRate&&m.shRate*100,bm.sh),   bm:'Target: '+bm.sh+'%'},
      {l:'Close Rate',     v:fP(m.closeRate),c:rCls(m.closeRate&&m.closeRate*100,bm.cl),bm:'Target: '+bm.cl+'%'},
      {l:'Lead → Sale',  v:fP(m.l2s),   c:'', bm:''},
      {l:'CPA',            v:m.cpa!==null?fD(m.cpa):'—', c:rCls(m.cpa,bm.cpa,true),  bm:'Target: $'+bm.cpa},
      {l:'Revenue',        v:fD(m.revenue),  c:'hi',  bm:''},
      {l:'ROAS',           v:m.roas!==null?m.roas.toFixed(2)+'x':'—', c:m.roas>=1?'good':'bad', bm:''},
      {l:'ROI',            v:m.roi!==null?(m.roi*100).toFixed(1)+'%':'—', c:m.roi>0?'good':'bad', bm:''},
    ];
    rEl.innerHTML = items.map(x=>`
      <div class="ri">
        <div class="ri-lb">${x.l}</div>
        <div class="ri-v ${x.c}">${x.v}</div>
        ${x.bm?`<div class="ri-bm">${x.bm}</div>`:''}
      </div>`).join('');
  }

  // Benchmarks table
  const btEl = document.getElementById(`bmt-${id}`);
  if(btEl){
    const rows=[
      {l:'Ad CPL',         a:m.adCPL,                          bm:bm.cpl,  fmt:'$',lower:true},
      {l:'Attended Rate',  a:m.attRate!==null?m.attRate*100:null,   bm:bm.att,  fmt:'%'},
      {l:'Application Rate',a:m.appRate!==null?m.appRate*100:null,  bm:bm.app,  fmt:'%'},
      {l:'Booking Rate',   a:m.bkRate!==null?m.bkRate*100:null,   bm:bm.bk,   fmt:'%'},
      {l:'Show Rate',      a:m.shRate!==null?m.shRate*100:null,    bm:bm.sh,   fmt:'%'},
      {l:'Close Rate',     a:m.closeRate!==null?m.closeRate*100:null,bm:bm.cl, fmt:'%'},
      {l:'Lead → Sale',    a:m.l2s!==null?m.l2s*100:null,         bm:null,    fmt:'%'},
      {l:'CPA',            a:m.cpa,                              bm:bm.cpa,  fmt:'$',lower:true},
      {l:'Revenue',        a:m.revenue,                          bm:null,    fmt:'$'},
      {l:'ROI',            a:m.roi!==null?m.roi*100:null,         bm:null,    fmt:'%'},
    ];
    const fmtV=(v,fmt)=>{
      if(v===null||v===undefined||!isFinite(v))return '—';
      if(fmt==='$')return '$'+Math.round(Math.abs(v)).toLocaleString('en-AU');
      if(fmt==='%')return v.toFixed(1)+'%';
      return v;
    };
    btEl.innerHTML = rows.map(r=>{
      const cls = r.bm!==null ? rCls(r.a,r.bm,r.lower||false) : '';
      const status = !r.bm||r.a===null||!isFinite(r.a)?'—':
        cls==='good'?'✅ On target':cls==='ok'?'⚠️ Close':'❌ Off target';
      const sc = cls==='good'?'color:#6dcf6d':cls==='ok'?'color:#F5E500':cls==='bad'?'color:#e88080':'color:#888885';
      const bmStr = r.bm!==null&&r.bm!==undefined ? (r.fmt==='$'?'$'+r.bm:r.bm+'%') : '—';
      return `<tr>
        <td class="tl">${r.l}</td>
        <td style="font-weight:700;color:#fff">${fmtV(r.a,r.fmt)}</td>
        <td style="color:#666663">${bmStr}</td>
        <td style="${sc}">${status}</td>
      </tr>`;
    }).join('');
  }
}

// ====== SUMMARY ======
function rSummary(){
  if(!S.events.length){
    document.getElementById('sum-cards').innerHTML='<div style="color:#555552;font-size:13px;padding:20px 0">No events yet.</div>';
    document.getElementById('sum-funnel').innerHTML='';
    document.getElementById('sum-table').innerHTML='';
    return;
  }

  let tot={adSpend:0,adReg:0,orgReg:0,attended:0,appFilled:0,bookedCall:0,attendedCall:0,deposit:0,purchased:0,revenue:0};
  S.events.forEach(ev=>{
    const m=calc(ev);const d=ev.data;
    Object.keys(tot).forEach(k=>{ tot[k]+= k==='revenue'?m.revenue:(d[k]||0); });
  });
  const tr=tot.adReg+tot.orgReg;
  const tROI=tot.adSpend>0?(tot.revenue-tot.adSpend)/tot.adSpend:null;
  const tClose=safe(tot.purchased,tot.attendedCall);

  // Cards
  document.getElementById('sum-cards').innerHTML=[
    {l:'Total Events',         v:S.events.length,         c:'',  s:'tracked'},
    {l:'Total Registrations',  v:fN(tr),                  c:'',  s:'all sources'},
    {l:'Total Ad Spend',       v:fD(tot.adSpend),          c:'',  s:'paid advertising'},
    {l:'Total Sales',          v:fN(tot.purchased),        c:'y', s:'purchases made'},
    {l:'Total Revenue',        v:fD(tot.revenue),          c:'g', s:'generated'},
    {l:'Overall ROI',          v:tROI!==null?(tROI*100).toFixed(0)+'%':'—', c:tROI>0?'g':'r', s:'on ad spend'},
    {l:'Avg Close Rate',       v:fP(tClose),               c:'',  s:''},
    {l:'Overall CPA',          v:tot.purchased>0?fD(tot.adSpend/tot.purchased):'—', c:'', s:'cost per acquisition'},
  ].map(x=>`<div class="mc ${x.c}"><div class="mlb">${x.l}</div><div class="mv">${x.v}</div>${x.s?`<div class="ms">${x.s}</div>`:''}</div>`).join('');

  // Funnel
  const fSteps=[
    {l:'Ad Regs',v:tot.adReg},{l:'Org Regs',v:tot.orgReg},
    {l:'Total Regs',v:tr},{l:'Attended',v:tot.attended},
    {l:'Applied',v:tot.appFilled},{l:'Booked',v:tot.bookedCall},
    {l:'Showed',v:tot.attendedCall},{l:'Deposited',v:tot.deposit},
    {l:'Purchased',v:tot.purchased},
  ];
  const maxV=Math.max(...fSteps.map(s=>s.v),1);
  document.getElementById('sum-funnel').innerHTML=fSteps.map(s=>`
    <div class="fs">
      <div class="fs-lb">${s.l}</div>
      <div class="fs-v">${s.v}</div>
      <div class="fs-bar"><div class="fs-fill" style="width:${(s.v/maxV*100).toFixed(1)}%"></div></div>
    </div>`).join('');

  // Table
  let trows='';
  S.events.forEach(ev=>{
    const m=calc(ev);const d=ev.data;
    const cOk=v=>v!==null&&isFinite(v);
    trows+=`<tr>
      <td class="tl">${ev.name}</td>
      <td>${ev.date}</td>
      <td>${fD(d.adSpend)}</td>
      <td>${fN(d.adReg)}</td>
      <td>${fN(d.orgReg)}</td>
      <td style="font-weight:700">${fN(m.totalReg)}</td>
      <td>${fN(d.attended)}</td>
      <td style="color:${cOk(m.attRate)?m.attRate>=0.3?'#6dcf6d':m.attRate>=0.2?'#F5E500':'#e88080':'#888885'};font-weight:700">${fP(m.attRate)}</td>
      <td>${fN(d.appFilled)}</td>
      <td style="color:${cOk(m.appRate)?m.appRate>=0.2?'#6dcf6d':m.appRate>=0.15?'#F5E500':'#e88080':'#888885'};font-weight:700">${fP(m.appRate)}</td>
      <td>${fN(d.bookedCall)}</td>
      <td>${fN(d.attendedCall)}</td>
      <td style="color:${cOk(m.closeRate)?m.closeRate>=0.3?'#6dcf6d':m.closeRate>=0.2?'#F5E500':'#e88080':'#888885'};font-weight:700">${fP(m.closeRate)}</td>
      <td style="color:#F5E500;font-weight:700">${fN(d.purchased)}</td>
      <td style="color:#6dcf6d;font-weight:700">${fD(m.revenue)}</td>
      <td style="color:${m.roi>0?'#6dcf6d':m.roi!==null?'#e88080':'#888885'};font-weight:700">${m.roi!==null?(m.roi*100).toFixed(0)+'%':'—'}</td>
      <td>${fD(m.cpa)}</td>
    </tr>`;
  });
  // Totals
  trows+=`<tr style="background:#141416">
    <td class="tl" style="color:#F5E500;font-weight:700">TOTALS</td>
    <td style="color:#888885">—</td>
    <td style="color:#fff;font-weight:700">${fD(tot.adSpend)}</td>
    <td style="color:#fff;font-weight:700">${fN(tot.adReg)}</td>
    <td style="color:#fff;font-weight:700">${fN(tot.orgReg)}</td>
    <td style="color:#F5E500;font-weight:700">${fN(tr)}</td>
    <td style="color:#fff;font-weight:700">${fN(tot.attended)}</td>
    <td style="color:#fff;font-weight:700">${fP(safe(tot.attended,tr))}</td>
    <td style="color:#fff;font-weight:700">${fN(tot.appFilled)}</td>
    <td style="color:#fff;font-weight:700">${fP(safe(tot.appFilled,tot.attended))}</td>
    <td style="color:#fff;font-weight:700">${fN(tot.bookedCall)}</td>
    <td style="color:#fff;font-weight:700">${fN(tot.attendedCall)}</td>
    <td style="color:#fff;font-weight:700">${fP(safe(tot.purchased,tot.attendedCall))}</td>
    <td style="color:#F5E500;font-weight:700">${fN(tot.purchased)}</td>
    <td style="color:#6dcf6d;font-weight:700">${fD(tot.revenue)}</td>
    <td style="color:${tROI>0?'#6dcf6d':tROI!==null?'#e88080':'#888885'};font-weight:700">${tROI!==null?(tROI*100).toFixed(0)+'%':'—'}</td>
    <td style="color:#fff;font-weight:700">${tot.purchased>0?fD(tot.adSpend/tot.purchased):'—'}</td>
  </tr>`;

  document.getElementById('sum-table').innerHTML=`<table>
    <thead><tr>
      <th class="tl" style="min-width:140px">Event</th><th>Date</th>
      <th>Ad Spend</th><th>Ad Regs</th><th>Org Regs</th><th>Total Regs</th>
      <th>Attended</th><th>Att. Rate</th>
      <th>Applied</th><th>App Rate</th>
      <th>Booked</th><th>Showed</th><th>Close Rate</th>
      <th>Sales</th><th>Revenue</th><th>ROI</th><th>CPA</th>
    </tr></thead>
    <tbody>${trows}</tbody>
  </table>`;
}

// ====== PRE-EVENT ROI CALCULATOR ======
function calcRC(){
  const adSpend = parseFloat(document.getElementById('rc-adspend').value)||0;
  const cpl     = parseFloat(document.getElementById('rc-cpl').value)||0;
  const mgmt    = parseFloat(document.getElementById('rc-mgmt').value)||0;
  const att     = parseFloat(document.getElementById('rc-att').value)||0;
  const app     = parseFloat(document.getElementById('rc-app').value)||0;
  const bk      = parseFloat(document.getElementById('rc-bk').value)||0;
  const sh      = parseFloat(document.getElementById('rc-sh').value)||0;
  const cl      = parseFloat(document.getElementById('rc-cl').value)||0;
  const sale    = parseFloat(document.getElementById('rc-sale').value)||0;

  const totalSpend = adSpend + mgmt;
  const regs       = cpl>0 ? adSpend/cpl : 0;
  const attended   = regs * (att/100);
  const applied    = attended * (app/100);
  const booked     = applied * (bk/100);
  const showed     = booked * (sh/100);
  const sales      = showed * (cl/100);
  const revenue    = sales * sale;
  const roi        = totalSpend>0 ? (revenue-totalSpend)/totalSpend : null;
  const roas       = totalSpend>0 ? revenue/totalSpend : null;
  const cpa        = sales>0 ? totalSpend/sales : null;
  const hasData    = adSpend>0 && cpl>0 && att>0 && cl>0 && sale>0;

  // Funnel
  const fSteps=[
    {l:'Ad Budget',      v:'$'+Math.round(adSpend).toLocaleString('en-AU'), raw:adSpend, isD:true},
    {l:'Registrations',  v:Math.ceil(regs).toLocaleString('en-AU'),         raw:regs},
    {l:'Attended',       v:Math.ceil(attended).toLocaleString('en-AU'),     raw:attended},
    {l:'Applied',        v:Math.ceil(applied).toLocaleString('en-AU'),      raw:applied},
    {l:'Booked Call',    v:Math.ceil(booked).toLocaleString('en-AU'),       raw:booked},
    {l:'Showed Up',      v:Math.ceil(showed).toLocaleString('en-AU'),       raw:showed},
    {l:'Sales',          v:Math.ceil(sales).toLocaleString('en-AU'),        raw:sales, hi:true},
  ];
  const maxV = Math.max(...fSteps.map(s=>s.raw),1);
  document.getElementById('rc-funnel').innerHTML = fSteps.map(s=>`
    <div style="background:#141418;border:1px solid #252528;border-radius:8px;padding:10px 14px;display:flex;align-items:center;gap:12px">
      <div style="flex:1">
        <div style="font-size:10px;font-weight:700;letter-spacing:.07em;text-transform:uppercase;color:#444442;margin-bottom:3px">${s.l}</div>
        <div style="font-size:18px;font-weight:800;color:${s.hi?'#F5E500':'#c0bdb8'}">${regs>0||s.isD ? s.v : '—'}</div>
      </div>
      <div style="width:80px;height:6px;background:#252528;border-radius:3px;overflow:hidden;flex-shrink:0">
        <div style="height:100%;width:${maxV>0&&s.raw>0?(s.raw/maxV*100).toFixed(1):0}%;background:${s.hi?'#F5E500':'#3a3a60'};border-radius:3px"></div>
      </div>
    </div>`).join('');

  // Results
  const roiOk = roi!==null&&roi>0;
  const items=[
    {l:'Total Ad Spend',  v:totalSpend>0?'$'+Math.round(totalSpend).toLocaleString('en-AU'):'—', c:''},
    {l:'Projected Sales', v:sales>0?Math.ceil(sales)+'':'—', c:'hi'},
    {l:'Projected Revenue',v:revenue>0?'$'+Math.round(revenue).toLocaleString('en-AU'):'—', c:revenue>0?'good':''},
    {l:'Projected CPA',   v:cpa!==null?'$'+Math.round(cpa).toLocaleString('en-AU'):'—', c:''},
    {l:'ROI',             v:roi!==null?(roi*100).toFixed(1)+'%':'—', c:roiOk?'good':'bad'},
    {l:'ROAS',            v:roas!==null?roas.toFixed(2)+'x':'—', c:roas>=1?'good':roas!==null?'bad':''},
  ];
  document.getElementById('rc-results').innerHTML = items.map(x=>`
    <div class="ri">
      <div class="ri-lb">${x.l}</div>
      <div class="ri-v ${x.c}">${x.v}</div>
    </div>`).join('');

  // Tip
  const tipEl = document.getElementById('rc-tip');
  const tipTxt = document.getElementById('rc-tip-text');
  if(hasData){
    tipEl.style.display='block';
    if(roi>=2) tipTxt.innerHTML=`<strong>Excellent projected ROI.</strong> At ${(roi*100).toFixed(0)}% ROI, every $1 spent returns $${(roas).toFixed(2)}. For ${Math.ceil(sales)} sales you need ${Math.ceil(showed)} calls to show — book ${Math.ceil(booked)} to hit that.`;
    else if(roi>0) tipTxt.innerHTML=`<strong>Profitable but slim.</strong> At ${(roi*100).toFixed(0)}% ROI you make $${Math.round(revenue-totalSpend).toLocaleString('en-AU')} profit. To hit 200% ROI you need either a higher close rate (${((totalSpend*3/showed/sale)*100).toFixed(0)}%+) or raise your avg. sale value to $${Math.round(totalSpend*3/Math.max(sales,0.01)).toLocaleString('en-AU')}.`;
    else if(roi<=0) { const salesNeeded=Math.ceil(totalSpend/sale); tipTxt.innerHTML=`<strong>Currently loss-making at these rates.</strong> You need <strong>${salesNeeded} sales</strong> to break even (projected: ${Math.ceil(sales)}). Try increasing close rate, attendance rate, or reducing your CPL below $${(totalSpend/Math.ceil(salesNeeded/Math.max(cl/100*sh/100*bk/100*app/100*att/100,0.001))).toFixed(0)}.`;}
  } else {
    tipEl.style.display='none';
  }
}

function resetRC(){
  ['rc-adspend','rc-cpl','rc-mgmt','rc-att','rc-app','rc-bk','rc-sh','rc-cl','rc-sale'].forEach(id=>{
    const el=document.getElementById(id); if(el) el.value='';
  });
  document.getElementById('rc-funnel').innerHTML='';
  document.getElementById('rc-results').innerHTML='';
  document.getElementById('rc-tip').style.display='none';
}

// ====== BENCHMARKS ======
function saveBM(){
  S.bm={
    cpl:  parseFloat(document.getElementById('bm-cpl').value)||15,
    att:  parseFloat(document.getElementById('bm-att').value)||30,
    app:  parseFloat(document.getElementById('bm-app').value)||20,
    bk:   parseFloat(document.getElementById('bm-bk').value)||60,
    sh:   parseFloat(document.getElementById('bm-sh').value)||80,
    cl:   parseFloat(document.getElementById('bm-cl').value)||30,
    cpa:  parseFloat(document.getElementById('bm-cpa').value)||500,
    roi:  parseFloat(document.getElementById('bm-roi').value)||200,
    roas: parseFloat(document.getElementById('bm-roas').value)||3,
  };
  save();
  builtPanels.forEach(id=>refreshPanelOutputs(id));
  renderBMCards();
}

function renderBMCards(){
  const bm=S.bm;
  const el=document.getElementById('bm-summary-cards');
  if(!el)return;
  el.innerHTML=[
    {l:'Target CPL',        v:'$'+bm.cpl,       c:''},
    {l:'Attended Rate',     v:bm.att+'%',        c:''},
    {l:'Application Rate',  v:bm.app+'%',        c:''},
    {l:'Booking Rate',      v:bm.bk+'%',         c:''},
    {l:'Show Rate',         v:bm.sh+'%',         c:''},
    {l:'Close Rate',        v:bm.cl+'%',         c:'y'},
    {l:'Target CPA',        v:'$'+bm.cpa,        c:''},
    {l:'Target ROI',        v:bm.roi+'%',        c:'g'},
    {l:'Target ROAS',       v:bm.roas+'x',       c:'g'},
  ].map(x=>`<div class="mc ${x.c}"><div class="mlb">${x.l}</div><div class="mv" style="font-size:18px">${x.v}</div></div>`).join('');
}

function loadBMInputs(){
  const bm=S.bm;
  document.getElementById('bm-cpl').value  = bm.cpl||'';
  document.getElementById('bm-att').value  = bm.att||'';
  document.getElementById('bm-app').value  = bm.app||'';
  document.getElementById('bm-bk').value   = bm.bk||'';
  document.getElementById('bm-sh').value   = bm.sh||'';
  document.getElementById('bm-cl').value   = bm.cl||'';
  document.getElementById('bm-cpa').value  = bm.cpa||'';
  document.getElementById('bm-roi').value  = bm.roi||'';
  document.getElementById('bm-roas').value = bm.roas||'';
  renderBMCards();
}

// ====== INIT ======
function init(){
  load();
  if(!S.activeLog && S.events.length) S.activeLog = S.events[0].id;
  rEventList();
  rebuildLogTabs();
  loadBMInputs();
}
init();
</script>
</body>
</html>

