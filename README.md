<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Relentless Education — Financial Forecast</title>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Helvetica,Arial,sans-serif;background:#111;color:#f0ede8;min-height:100vh}
.nav{display:flex;align-items:center;background:#0d0d0f;border-bottom:1px solid #252528;position:sticky;top:0;z-index:100;flex-wrap:wrap}
.brand{display:flex;align-items:center;gap:10px;padding:12px 20px;border-right:1px solid #252528;flex-shrink:0}
.bi{width:34px;height:34px;background:#F5E500;border-radius:7px;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:800;color:#111}
.bn{font-size:13px;font-weight:700;color:#F5E500}
.nav-tabs{display:flex;overflow-x:auto;flex:1}
.nav-tabs::-webkit-scrollbar{height:2px}
.nt{padding:14px 16px;font-size:12px;font-weight:600;color:#666663;cursor:pointer;border-bottom:2px solid transparent;white-space:nowrap;background:none;border-top:none;border-left:none;border-right:none;font-family:inherit;transition:color 0.15s,border-color 0.15s}
.nt:hover{color:#c0bdb8}
.nt.active{color:#F5E500;border-bottom-color:#F5E500}
.pg{display:none;padding:28px 20px;max-width:1200px;margin:0 auto}
.pg.active{display:block}
.ph{margin-bottom:28px}
.ph h1{font-size:24px;font-weight:700;color:#fff;letter-spacing:-0.025em}
.ph h1 em{color:#F5E500;font-style:normal}
.ph p{font-size:13px;color:#888885;margin-top:6px;line-height:1.5}
.year-bar{display:flex;align-items:center;gap:8px;margin-bottom:24px;flex-wrap:wrap}
.year-btn{padding:8px 18px;font-size:12px;font-weight:700;border-radius:8px;border:1px solid #2a2a2e;background:transparent;color:#666663;cursor:pointer;font-family:inherit;transition:all 0.15s;letter-spacing:0.04em}
.year-btn:hover{border-color:#383838;color:#c0bdb8}
.year-btn.active{background:#F5E500;color:#111;border-color:#F5E500}
.year-label{font-size:11px;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;color:#444442;margin-right:4px}
.scards{display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:12px;margin-bottom:28px}
.sc{background:#1a1a1c;border:1px solid #2a2a2e;border-radius:12px;padding:16px}
.sc.yellow{background:#1a1900;border-color:#F5E500}
.sc.green{background:#0d1f0d;border-color:#1e4d1e}
.sc.red{background:#1f0d0d;border-color:#6d2424}
.sc-label{font-size:10px;font-weight:700;letter-spacing:0.08em;text-transform:uppercase;color:#444442;margin-bottom:6px}
.sc.yellow .sc-label{color:#b8a800}
.sc.green .sc-label{color:#3a6a3a}
.sc.red .sc-label{color:#8a4040}
.sc-val{font-size:22px;font-weight:800;letter-spacing:-0.025em;color:#666663}
.sc.yellow .sc-val{color:#F5E500}
.sc.green .sc-val{color:#6dcf6d}
.sc.red .sc-val{color:#e88080}
.sc-sub{font-size:11px;color:#444442;margin-top:3px}
.sc.yellow .sc-sub{color:#8a7800}
.sc.green .sc-sub{color:#3a6a3a}
.slabel{font-size:10px;font-weight:700;letter-spacing:0.1em;text-transform:uppercase;color:#F5E500;margin-bottom:12px;margin-top:28px;opacity:0.8}
.tw{overflow-x:auto;border-radius:12px;border:1px solid #252528;margin-bottom:24px}
table{width:100%;border-collapse:collapse;font-size:12px;min-width:900px}
thead th{background:#141416;color:#888885;font-weight:700;padding:10px 14px;text-align:right;white-space:nowrap;border-bottom:1px solid #252528;font-size:10px;letter-spacing:0.06em;text-transform:uppercase}
thead th:first-child{text-align:left;min-width:220px}
thead th:nth-child(2){text-align:right;min-width:80px}
tbody td{padding:9px 14px;border-bottom:1px solid #1c1c1e;color:#c0bdb8;text-align:right;vertical-align:middle;white-space:nowrap}
tbody td:first-child{text-align:left;color:#f0ede8;font-weight:500}
tbody tr:last-child td{border-bottom:none}
tbody tr:hover td{background:rgba(255,255,255,0.015)}
tfoot td{padding:10px 14px;border-top:1px solid #2a2a2e;background:#141416;text-align:right;font-size:12px;font-weight:700;color:#f0ede8;white-space:nowrap}
tfoot td:first-child{text-align:left}
.ei{background:transparent;border:none;outline:none;color:#fff;font-family:inherit;font-size:12px;font-weight:600;width:100%;min-width:60px;text-align:right;padding:0}
.ei:focus{background:rgba(245,229,0,0.07);border-radius:4px;padding:2px 5px;margin:-2px -5px}
.ei[type=number]::-webkit-inner-spin-button{-webkit-appearance:none}
.row-header td{background:#1a1a1c!important;color:#F5E500!important;font-size:11px!important;font-weight:700!important;letter-spacing:0.06em;text-transform:uppercase;padding:12px 14px!important}
.row-subtotal td{background:#161618!important;color:#c0bdb8!important;font-weight:700!important;border-top:1px solid #2a2a2e!important}
.row-total td{background:#1a1900!important;color:#F5E500!important;font-weight:800!important;border-top:1px solid #F5E500!important}
.row-profit td{background:#0d1f0d!important;color:#6dcf6d!important;font-weight:800!important;border-top:1px solid #1e4d1e!important}
.row-loss td{background:#1f0d0d!important;color:#e88080!important;font-weight:800!important}
.row-ytd td{background:#111115!important;color:#888885!important;font-style:italic}
.row-pct td{color:#777774!important;font-size:11px!important}
.row-spacer td{height:8px;background:#0f0f11!important;border:none!important}
.row-member td{background:#13131a!important;color:#aaa9a4!important}
.row-member td:first-child{padding-left:32px!important;color:#c0bdb8!important}
.fi{width:100%;background:#141416;border:1px solid #2e2e32;border-radius:8px;padding:9px 12px;font-size:14px;font-weight:600;color:#fff;font-family:inherit;outline:none;transition:border-color 0.15s}
.fi:focus{border-color:#F5E500}
.fi::placeholder{color:#333331;font-weight:400}
.fi[type=number]::-webkit-inner-spin-button{-webkit-appearance:none}
select.fi{cursor:pointer}
.fg{margin-bottom:14px}
.fl{font-size:12px;font-weight:500;color:#c0bdb8;margin-bottom:6px;display:block}
.frow{display:flex;align-items:center;gap:6px}
.fpfx{font-size:14px;font-weight:600;color:#555552}
.g2{display:grid;grid-template-columns:1fr 1fr;gap:16px}
.g3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:16px}
@media(max-width:700px){.g2,.g3{grid-template-columns:1fr}}
.card{background:#1a1a1c;border:1px solid #2a2a2e;border-radius:12px;padding:18px 20px;margin-bottom:14px}
.card-title{font-size:13px;font-weight:600;color:#c0bdb8;margin-bottom:14px}
.tip{font-size:12px;color:#555552;margin-top:4px;line-height:1.5}
.btn{display:inline-flex;align-items:center;gap:6px;padding:9px 16px;border-radius:8px;font-size:13px;font-weight:600;font-family:inherit;cursor:pointer;transition:all 0.15s;border:1px solid #2e2e32;background:transparent;color:#c0bdb8}
.btn:hover{border-color:#F5E500;color:#F5E500}
.btnp{background:#F5E500;color:#111;border-color:#F5E500}
.btnp:hover{background:#e0d100;color:#111}
.btns{padding:6px 12px;font-size:12px}
.btn:active{transform:scale(0.98)}
hr.dv{border:none;border-top:1px solid #252528;margin:20px 0}
.pos{color:#6dcf6d!important}
.neg{color:#e88080!important}
.neutral{color:#c0bdb8!important}
.member-card{background:#141418;border:1px solid #2a2a2e;border-radius:10px;padding:16px 18px;margin-bottom:10px}
.member-header{display:flex;align-items:center;gap:10px;margin-bottom:12px}
.member-avatar{width:32px;height:32px;border-radius:50%;background:#1a1900;border:1px solid #F5E500;display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;color:#F5E500;flex-shrink:0}
.role-badge{display:inline-flex;padding:3px 8px;border-radius:4px;font-size:10px;font-weight:700;letter-spacing:0.05em;text-transform:uppercase}
.badge-salary{background:#0d1f0d;color:#6dcf6d;border:1px solid #1e4d1e}
.badge-commission{background:#1a1900;color:#F5E500;border:1px solid #3a3600}
.badge-both{background:#0d0d20;color:#6d9fff;border:1px solid #1e1e4d}
.total-people-bar{background:#1a1900;border:1px solid #3a3600;border-radius:8px;padding:12px 16px;margin-top:12px;display:flex;justify-content:space-between;align-items:center}
.total-people-bar span:first-child{font-size:12px;font-weight:600;color:#888885;letter-spacing:0.05em;text-transform:uppercase}
.total-people-bar span:last-child{font-size:18px;font-weight:800;color:#F5E500}
</style>
</head>
<body>

<nav class="nav">
  <div class="brand">
    <div class="bi">RE</div>
    <span class="bn">Relentless Education</span>
  </div>
  <div class="nav-tabs">
    <button class="nt active" onclick="gp('setup',this)">Setup</button>
    <button class="nt" onclick="gp('forecast',this)">P&amp;L Forecast</button>
    <button class="nt" onclick="gp('people',this)">People Costs</button>
    <button class="nt" onclick="gp('summary',this)">5-Year Summary</button>
  </div>
</nav>

<!-- ===== SETUP ===== -->
<div class="pg active" id="pg-setup">
  <div class="ph"><h1>Business <em>Setup</em></h1><p>Configure revenue programs, expenses, and your team. All figures flow automatically into the P&L and 5-Year Summary.</p></div>

  <div class="slabel" style="margin-top:0">Revenue Programs</div>
  <div id="prog-list"></div>
  <button class="btn btns" onclick="addProg()">+ Add Program</button>

  <div class="slabel">Team Members & People Costs</div>
  <p style="font-size:13px;color:#c0bdb8;margin-bottom:16px;line-height:1.6">Add each team member with their name, role, and pay structure. Costs flow automatically into the P&L (as a total) and the <strong style="color:#F5E500">People Costs</strong> tab (full breakdown).</p>
  <div id="team-list" style="min-height:10px"></div>
  <button class="btn btns btnp" onclick="addMember()" style="margin-top:4px;margin-bottom:16px">+ Add Team Member</button>

  <div class="total-people-bar" id="setup-people-total">
    <span>Total Monthly People Cost (base salary + super)</span>
    <span id="setup-total-val">$0 / month</span>
  </div>

  <div class="slabel">Fixed Monthly Expenses</div>
  <div id="exp-list"></div>
  <button class="btn btns" onclick="addExp()">+ Add Expense</button>

  <div class="slabel">Other Assumptions</div>
  <div class="g3">
    <div class="card">
      <div class="card-title">Annual Growth Rate (Year 2+)</div>
      <div class="frow"><input class="fi" id="growth-rate" type="number" placeholder="20" oninput="save();rAll()"/><span class="fpfx">%</span></div>
      <p class="tip" style="margin-top:8px">Applied to customer numbers each year</p>
    </div>
    <div class="card">
      <div class="card-title">Tax Rate</div>
      <div class="frow"><input class="fi" id="tax-pct" type="number" placeholder="25" oninput="save();rAll()"/><span class="fpfx">%</span></div>
      <p class="tip" style="margin-top:8px">Applied to gross profit when positive</p>
    </div>
    <div class="card">
      <div class="card-title">Superannuation Rate</div>
      <div class="frow"><input class="fi" id="super-pct" type="number" placeholder="11" oninput="save();rAll()"/><span class="fpfx">%</span></div>
      <p class="tip" style="margin-top:8px">Applied to salaried team members only</p>
    </div>
  </div>
</div>

<!-- ===== FORECAST ===== -->
<div class="pg" id="pg-forecast">
  <div class="ph"><h1>P&amp;L <em>Forecast</em></h1><p>Edit customer numbers directly in the table. All totals, gross profit and YTD figures update instantly. People costs show as a single total — see the People Costs tab for the full breakdown.</p></div>
  <div class="year-bar">
    <span class="year-label">Year</span>
    <button class="year-btn active" onclick="swYear(1,this)">Year 1</button>
    <button class="year-btn" onclick="swYear(2,this)">Year 2</button>
    <button class="year-btn" onclick="swYear(3,this)">Year 3</button>
    <button class="year-btn" onclick="swYear(4,this)">Year 4</button>
    <button class="year-btn" onclick="swYear(5,this)">Year 5</button>
  </div>
  <div class="scards" id="summary-cards"></div>
  <div id="forecast-table"></div>
</div>

<!-- ===== PEOPLE ===== -->
<div class="pg" id="pg-people">
  <div class="ph"><h1>People <em>Costs</em></h1><p>Full breakdown of every team member's cost month by month. These totals feed directly into the P&L Cost of Sales line.</p></div>
  <div class="year-bar">
    <span class="year-label">Year</span>
    <button class="year-btn active" onclick="swPeopleYear(1,this)">Year 1</button>
    <button class="year-btn" onclick="swPeopleYear(2,this)">Year 2</button>
    <button class="year-btn" onclick="swPeopleYear(3,this)">Year 3</button>
    <button class="year-btn" onclick="swPeopleYear(4,this)">Year 4</button>
    <button class="year-btn" onclick="swPeopleYear(5,this)">Year 5</button>
  </div>
  <div id="people-table"></div>
</div>

<!-- ===== 5-YEAR SUMMARY ===== -->
<div class="pg" id="pg-summary">
  <div class="ph"><h1>5-Year <em>Summary</em></h1><p>Consolidated view of revenue, profit and key metrics across all 5 years.</p></div>
  <div class="scards" id="five-yr-cards"></div>
  <div id="five-yr-table"></div>
</div>

<script>
const MONTHS=['January','February','March','April','May','June','July','August','September','October','November','December'];
const MS=['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];

let S = {
  programs:[
    {name:'MVP Program',price:25000,attrition:0,customers:[0,0,0,10,10,10,10,10,10,10,10,10]},
    {name:'AI Master Coach',price:2500,attrition:0,customers:[0,0,20,20,20,20,20,20,20,20,20,20]},
    {name:'100k Accelerator (MVP Group)',price:9997,attrition:0,customers:[0,2,5,5,10,10,10,10,10,10,10,10]},
    {name:'DFY Agency',price:50000,attrition:0,customers:[0,0,0,0,0,1,0,1,0,1,0,1]},
    {name:'$497 Monthly Program',price:497,attrition:3,customers:[0,0,0,0,0,0,0,0,0,0,0,0]},
  ],
  // Team members: name, role, type=salary|commission|both, salary(monthly), commissionPct, commissionBase=revenue|grossProfit, superEligible
  team:[
    {name:'Owner / Director',role:'Leadership',type:'salary',salary:20135,commissionPct:0,commissionBase:'revenue',superEligible:true},
  ],
  expenses:[
    {name:'Accounting / ASIC',monthly:[650,650,650,650,650,726,726,726,726,726,726,726]},
    {name:'Ads Spend',monthly:[15000,15000,15000,15000,15000,15000,15000,15000,15000,15000,15000,15000]},
    {name:'Software Expenses',monthly:[200,200,200,200,200,300,300,300,300,300,300,300]},
    {name:'Descript + Opus + Bigspy',monthly:[0,119,119,119,119,119,119,119,119,119,119,119]},
    {name:'Rent',monthly:[0,4000,4000,4000,4000,4000,4000,4000,4000,4000,4000,4000]},
    {name:'Software (Platform)',monthly:[2000,2000,2000,2000,2000,2000,1000,1000,1000,1000,1000,1000]},
    {name:'Event Space Costs',monthly:[2500,2500,2500,2500,2500,2500,2500,2500,2500,2500,2500,2500]},
    {name:'Telephone & Internet',monthly:[250,250,250,250,250,500,500,500,500,500,500,500]},
    {name:'Mentoring Costs',monthly:[2880,0,0,0,0,0,0,0,0,0,0,0]},
  ],
  superPct:11, taxPct:0, growthRate:20,
  yearData:{}
};

let curYear=1, curPeopleYear=1;

function save(){
  S.superPct=parseFloat(document.getElementById('super-pct').value)||11;
  S.taxPct=parseFloat(document.getElementById('tax-pct').value)||0;
  S.growthRate=parseFloat(document.getElementById('growth-rate').value)||20;
  localStorage.setItem('re-fc4',JSON.stringify(S));
}
function load(){
  // Clear any old incompatible saved data
  localStorage.removeItem('re-fc3');
  localStorage.removeItem('re-forecast');
  try{
    const d=localStorage.getItem('re-fc4');
    if(d){
      const parsed=JSON.parse(d);
      // Ensure team array exists and each member has required fields
      if(!parsed.team||!Array.isArray(parsed.team)){
        parsed.team=S.team;
      }
      parsed.team=parsed.team.map(m=>({
        name:m.name||'Team Member',
        role:m.role||'',
        type:m.type||'salary',
        salary:m.salary||0,
        commissionPct:m.commissionPct||0,
        commissionBase:m.commissionBase||'revenue',
        superEligible:m.superEligible!==undefined?m.superEligible:true,
      }));
      S=parsed;
    }
  }catch(e){}
}

function gp(id,btn){
  document.querySelectorAll('.pg').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nt').forEach(t=>t.classList.remove('active'));
  document.getElementById('pg-'+id).classList.add('active');
  btn.classList.add('active');
  if(id==='forecast')rForecast();
  if(id==='people')rPeople();
  if(id==='summary')rFiveYear();
}

function fD(n){
  if(n===0||n===null||n===undefined)return '—';
  const a=Math.abs(n),s=Math.round(a).toLocaleString('en-AU');
  return n<0?'('+s+')':''+s;
}
function fDollar(n){return (n<0?'-$':'$')+Math.round(Math.abs(n)).toLocaleString('en-AU');}

// ---- TEAM COST CALCULATION ----
// Returns per-member cost for a given month and year
function getMemberCost(mi, grossRevenue, yr){
  return S.team.map(m=>{
    let salary = 0, commission = 0, superAmt = 0;
    // Scale salary for yr 2+
    const salaryBase = m.salary||0;
    if(m.type==='salary'||m.type==='both'){
      salary = yr===1 ? salaryBase : Math.round(salaryBase*(1+(S.growthRate/100*0.1*(yr-1))));
    }
    if(m.type==='commission'||m.type==='both'){
      const base = m.commissionBase==='grossProfit' ? Math.max(0,grossRevenue*0.85) : grossRevenue;
      commission = base*(m.commissionPct||0)/100;
    }
    if(m.superEligible && (m.type==='salary'||m.type==='both')){
      superAmt = salary*(S.superPct/100);
    }
    return {salary, commission, superAmt, total:salary+commission+superAmt};
  });
}

function getTotalPeopleCost(mi, grossRevenue, yr){
  return getMemberCost(mi, grossRevenue, yr).reduce((s,m)=>s+m.total,0);
}

// ---- MONTH CALC ----
function getCustomers(yr,pi,mi){
  if(yr===1)return S.programs[pi].customers[mi]||0;
  const key=`${yr}-${pi}-${mi}`;
  if(S.yearData[key]!==undefined)return S.yearData[key];
  const base=S.programs[pi].customers[mi]||0;
  return Math.round(base*Math.pow(1+(S.growthRate/100),yr-1));
}
function setCustomers(yr,pi,mi,val){
  if(yr===1){S.programs[pi].customers[mi]=val;}
  else{S.yearData[`${yr}-${pi}-${mi}`]=val;}
  save();rForecast();
}

function calcMonth(yr,mi){
  let grossRevenue=0;
  const progRev=S.programs.map((p,pi)=>{
    const r=getCustomers(yr,pi,mi)*p.price;
    grossRevenue+=r;return r;
  });
  const memberCosts=getMemberCost(mi,grossRevenue,yr);
  const totalPeople=memberCosts.reduce((s,m)=>s+m.total,0);
  const grossProfit=grossRevenue-totalPeople;
  let totalExp=0;
  const expVals=S.expenses.map(e=>{
    let base=e.monthly[mi]||0;
    if(yr>1)base=Math.round(base*(1+(S.growthRate/100*0.25*(yr-1))));
    totalExp+=base;return base;
  });
  const tax=grossProfit>0?grossProfit*(S.taxPct/100):0;
  totalExp+=tax;
  const profit=grossRevenue-totalPeople-totalExp;
  return{grossRevenue,progRev,totalPeople,memberCosts,grossProfit,totalExp,expVals,tax,profit};
}

function calcYear(yr){
  const months=MONTHS.map((_,mi)=>calcMonth(yr,mi));
  const totals={
    grossRevenue:months.reduce((s,m)=>s+m.grossRevenue,0),
    totalPeople:months.reduce((s,m)=>s+m.totalPeople,0),
    grossProfit:months.reduce((s,m)=>s+m.grossProfit,0),
    totalExp:months.reduce((s,m)=>s+m.totalExp,0),
    profit:months.reduce((s,m)=>s+m.profit,0),
    progRev:S.programs.map((_,pi)=>months.reduce((s,m)=>s+m.progRev[pi],0)),
    expVals:S.expenses.map((_,ei)=>months.reduce((s,m)=>s+m.expVals[ei],0)),
    memberTotals:S.team.map((_,ti)=>({
      salary:months.reduce((s,m)=>s+m.memberCosts[ti].salary,0),
      commission:months.reduce((s,m)=>s+m.memberCosts[ti].commission,0),
      superAmt:months.reduce((s,m)=>s+m.memberCosts[ti].superAmt,0),
      total:months.reduce((s,m)=>s+m.memberCosts[ti].total,0),
    })),
  };
  return{months,totals};
}

// ---- RENDER FORECAST ----
function swYear(yr,btn){
  curYear=yr;
  document.querySelectorAll('#pg-forecast .year-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');rForecast();
}

function rForecast(){
  const yr=curYear;
  const{months,totals}=calcYear(yr);
  const ytdArr=months.reduce((acc,m,i)=>{acc.push((acc[i-1]||0)+m.profit);return acc;},[]);
  const peakI=months.reduce((bi,m,i)=>m.profit>months[bi].profit?i:bi,0);

  document.getElementById('summary-cards').innerHTML=[
    {l:'Gross Revenue',v:'$'+Math.round(totals.grossRevenue).toLocaleString(),s:'Year '+yr+' total',c:'yellow'},
    {l:'Net Profit',v:(totals.profit<0?'-':'')+'$'+Math.round(Math.abs(totals.profit)).toLocaleString(),s:totals.profit>=0?'profit for year':'loss for year',c:totals.profit>=0?'green':'red'},
    {l:'Gross Profit %',v:totals.grossRevenue>0?((totals.grossProfit/totals.grossRevenue)*100).toFixed(1)+'%':'—',s:'after people costs',c:''},
    {l:'Total People Costs',v:'$'+Math.round(totals.totalPeople).toLocaleString(),s:S.team.length+' team member'+(S.team.length!==1?'s':''),c:''},
    {l:'Total Expenses',v:'$'+Math.round(totals.totalExp).toLocaleString(),s:'all operating costs',c:''},
    {l:'Best Month',v:MS[peakI],s:'$'+Math.round(months[peakI].profit).toLocaleString()+' profit',c:months[peakI].profit>=0?'green':'red'},
  ].map(c=>`<div class="sc ${c.c}"><div class="sc-label">${c.l}</div><div class="sc-val">${c.v}</div><div class="sc-sub">${c.s}</div></div>`).join('');

  const mHdr=MS.map(m=>`<th>${m}</th>`).join('')+`<th style="color:#F5E500">TOTAL</th>`;
  let rows='';

  // Revenue
  rows+=`<tr class="row-header"><td colspan="14">REVENUE</td></tr>`;
  S.programs.forEach((prog,pi)=>{
    rows+=`<tr class="row-header" style="opacity:0.65"><td style="padding-left:20px;color:#c0bdb8;font-size:11px;text-transform:none;letter-spacing:0">${prog.name} <span style="color:#555552">— $${prog.price.toLocaleString()}/client</span></td>${MS.map(()=>'<td></td>').join('')}<td></td></tr>`;
    rows+=`<tr><td style="padding-left:32px;color:#888885;font-size:11px">Net Customers</td>
      ${MONTHS.map((_,mi)=>`<td><input class="ei" type="number" value="${getCustomers(yr,pi,mi)||''}" placeholder="0" oninput="setCustomers(${yr},${pi},${mi},parseFloat(this.value)||0)"/></td>`).join('')}
      <td style="font-weight:700;color:#c0bdb8">${MONTHS.reduce((s,_,mi)=>s+getCustomers(yr,pi,mi),0)}</td>
    </tr>`;
    rows+=`<tr class="row-pct"><td style="padding-left:32px">Revenue</td>
      ${months.map(m=>`<td>${m.progRev[pi]>0?'$'+Math.round(m.progRev[pi]).toLocaleString():'—'}</td>`).join('')}
      <td style="color:#c0bdb8;font-weight:700">${totals.progRev[pi]>0?'$'+Math.round(totals.progRev[pi]).toLocaleString():'—'}</td>
    </tr>`;
    rows+=`<tr class="row-spacer"><td colspan="14"></td></tr>`;
  });
  rows+=`<tr class="row-total"><td>GROSS SALES REVENUE</td>
    ${months.map(m=>`<td>${m.grossRevenue>0?'$'+Math.round(m.grossRevenue).toLocaleString():'—'}</td>`).join('')}
    <td>$${Math.round(totals.grossRevenue).toLocaleString()}</td>
  </tr>`;
  rows+=`<tr class="row-spacer"><td colspan="14"></td></tr>`;

  // Cost of Sales — single total line (detail in People Costs tab)
  rows+=`<tr class="row-header"><td colspan="14">COST OF SALES — PEOPLE <span style="font-size:9px;opacity:0.6;font-weight:400;text-transform:none;letter-spacing:0"> (see People Costs tab for full breakdown)</span></td></tr>`;
  rows+=`<tr class="row-subtotal"><td>Total People Costs <span style="font-size:10px;font-weight:400;color:#555552">(${S.team.length} members)</span></td>
    ${months.map(m=>`<td>$${Math.round(m.totalPeople).toLocaleString()}</td>`).join('')}
    <td>$${Math.round(totals.totalPeople).toLocaleString()}</td>
  </tr>`;

  // Gross Profit
  rows+=`<tr class="${totals.grossProfit>=0?'row-profit':'row-loss'}"><td>GROSS PROFIT</td>
    ${months.map(m=>`<td>${fD(m.grossProfit)}</td>`).join('')}
    <td>${fD(totals.grossProfit)}</td>
  </tr>`;
  rows+=`<tr class="row-pct"><td>Gross Profit %</td>
    ${months.map(m=>`<td>${m.grossRevenue>0?((m.grossProfit/m.grossRevenue)*100).toFixed(1)+'%':'—'}</td>`).join('')}
    <td>${totals.grossRevenue>0?((totals.grossProfit/totals.grossRevenue)*100).toFixed(1)+'%':'—'}</td>
  </tr>`;
  rows+=`<tr class="row-spacer"><td colspan="14"></td></tr>`;

  // Expenses
  rows+=`<tr class="row-header"><td colspan="14">OPERATING EXPENSES</td></tr>`;
  S.expenses.forEach((exp,ei)=>{
    rows+=`<tr><td style="padding-left:24px">${exp.name}</td>
      ${months.map((m,mi)=>`<td>${m.expVals[ei]>0?'$'+Math.round(m.expVals[ei]).toLocaleString():'—'}</td>`).join('')}
      <td style="font-weight:700">${totals.expVals[ei]>0?'$'+Math.round(totals.expVals[ei]).toLocaleString():'—'}</td>
    </tr>`;
  });
  if(S.taxPct>0){
    rows+=`<tr><td style="padding-left:24px">Tax (${S.taxPct}%)</td>
      ${months.map(m=>`<td>${m.tax>0?'$'+Math.round(m.tax).toLocaleString():'—'}</td>`).join('')}
      <td style="font-weight:700">${months.reduce((s,m)=>s+m.tax,0)>0?'$'+Math.round(months.reduce((s,m)=>s+m.tax,0)).toLocaleString():'—'}</td>
    </tr>`;
  }
  rows+=`<tr class="row-subtotal"><td>TOTAL EXPENSES</td>
    ${months.map(m=>`<td>$${Math.round(m.totalExp).toLocaleString()}</td>`).join('')}
    <td>$${Math.round(totals.totalExp).toLocaleString()}</td>
  </tr>`;
  rows+=`<tr class="row-spacer"><td colspan="14"></td></tr>`;

  // Net Profit
  rows+=`<tr class="${totals.profit>=0?'row-profit':'row-loss'}"><td>NET PROFIT / (LOSS)</td>
    ${months.map(m=>`<td>${fD(m.profit)}</td>`).join('')}
    <td>${fD(totals.profit)}</td>
  </tr>`;
  let ytdR=0;
  rows+=`<tr class="row-ytd"><td>YTD PROFIT / (LOSS)</td>
    ${months.map(m=>{ytdR+=m.profit;return `<td>${fD(ytdR)}</td>`;}).join('')}
    <td>${fD(ytdR)}</td>
  </tr>`;

  // Ratios
  rows+=`<tr class="row-spacer"><td colspan="14"></td></tr>`;
  let ytdRev=0,ytdProf=0;
  rows+=`<tr class="row-pct"><td>Net Profit % YTD</td>
    ${months.map(m=>{ytdRev+=m.grossRevenue;ytdProf+=m.profit;return `<td>${ytdRev>0?((ytdProf/ytdRev)*100).toFixed(1)+'%':'—'}</td>`;}).join('')}
    <td>${totals.grossRevenue>0?((totals.profit/totals.grossRevenue)*100).toFixed(1)+'%':'—'}</td>
  </tr>`;
  let ytdSales=0;
  rows+=`<tr class="row-pct"><td>YTD Sales Revenue</td>
    ${months.map(m=>{ytdSales+=m.grossRevenue;return `<td>$${Math.round(ytdSales).toLocaleString()}</td>`;}).join('')}
    <td>$${Math.round(totals.grossRevenue).toLocaleString()}</td>
  </tr>`;

  document.getElementById('forecast-table').innerHTML=`<div class="tw"><table><thead><tr><th>Description</th>${mHdr}</tr></thead><tbody>${rows}</tbody></table></div>`;
}

// ---- RENDER PEOPLE ----
function swPeopleYear(yr,btn){
  curPeopleYear=yr;
  document.querySelectorAll('#pg-people .year-btn').forEach(b=>b.classList.remove('active'));
  btn.classList.add('active');rPeople();
}

function rPeople(){
  const yr=curPeopleYear;
  const{months,totals}=calcYear(yr);
  const mHdr=MS.map(m=>`<th>${m}</th>`).join('')+`<th style="color:#F5E500">TOTAL</th>`;
  let rows='';

  S.team.forEach((member,ti)=>{
    const mt=totals.memberTotals[ti];
    // Member header row
    rows+=`<tr class="row-header" style="opacity:0.8"><td colspan="14" style="padding-left:14px">
      ${member.name} <span style="font-size:9px;font-weight:400;color:#888885;text-transform:none;letter-spacing:0;margin-left:8px">${member.role}</span>
      <span style="margin-left:8px;font-size:9px;padding:2px 6px;border-radius:3px;background:${member.type==='salary'?'#0d1f0d':member.type==='commission'?'#1a1900':'#0d0d20'};color:${member.type==='salary'?'#6dcf6d':member.type==='commission'?'#F5E500':'#6d9fff'}">${member.type.toUpperCase()}</span>
    </td></tr>`;
    // Salary row
    if(member.type==='salary'||member.type==='both'){
      rows+=`<tr class="row-member"><td style="padding-left:32px">Base Salary</td>
        ${months.map((m,mi)=>`<td>${m.memberCosts[ti].salary>0?'$'+Math.round(m.memberCosts[ti].salary).toLocaleString():'—'}</td>`).join('')}
        <td style="font-weight:700">$${Math.round(mt.salary).toLocaleString()}</td>
      </tr>`;
      if(S.superPct>0&&member.superEligible){
        rows+=`<tr class="row-member"><td style="padding-left:32px;color:#666663">Super (${S.superPct}%)</td>
          ${months.map((m,mi)=>`<td style="color:#666663">${m.memberCosts[ti].superAmt>0?'$'+Math.round(m.memberCosts[ti].superAmt).toLocaleString():'—'}</td>`).join('')}
          <td style="font-weight:700;color:#888885">$${Math.round(mt.superAmt).toLocaleString()}</td>
        </tr>`;
      }
    }
    // Commission row
    if(member.type==='commission'||member.type==='both'){
      rows+=`<tr class="row-member"><td style="padding-left:32px">Commission (${member.commissionPct||0}% of ${member.commissionBase==='grossProfit'?'gross profit':'revenue'})</td>
        ${months.map((m,mi)=>`<td>${m.memberCosts[ti].commission>0?'$'+Math.round(m.memberCosts[ti].commission).toLocaleString():'—'}</td>`).join('')}
        <td style="font-weight:700">$${Math.round(mt.commission).toLocaleString()}</td>
      </tr>`;
    }
    // Member subtotal
    rows+=`<tr class="row-subtotal"><td style="padding-left:24px">Total — ${member.name}</td>
      ${months.map((m,mi)=>`<td>$${Math.round(m.memberCosts[ti].total).toLocaleString()}</td>`).join('')}
      <td style="color:#F5E500">$${Math.round(mt.total).toLocaleString()}</td>
    </tr>`;
    rows+=`<tr class="row-spacer"><td colspan="14"></td></tr>`;
  });

  // Grand total people
  rows+=`<tr class="row-total"><td>TOTAL PEOPLE COSTS → P&amp;L</td>
    ${months.map(m=>`<td>$${Math.round(m.totalPeople).toLocaleString()}</td>`).join('')}
    <td>$${Math.round(totals.totalPeople).toLocaleString()}</td>
  </tr>`;
  rows+=`<tr class="row-pct"><td>People Costs / Revenue %</td>
    ${months.map(m=>`<td>${m.grossRevenue>0?((m.totalPeople/m.grossRevenue)*100).toFixed(1)+'%':'—'}</td>`).join('')}
    <td>${totals.grossRevenue>0?((totals.totalPeople/totals.grossRevenue)*100).toFixed(1)+'%':'—'}</td>
  </tr>`;

  document.getElementById('people-table').innerHTML=`<div class="tw"><table><thead><tr><th>Team Member / Cost</th>${mHdr}</tr></thead><tbody>${rows}</tbody></table></div>`;
}

// ---- 5-YEAR SUMMARY ----
function rFiveYear(){
  const years=[1,2,3,4,5].map(yr=>calcYear(yr).totals);
  const totalProfit=years.reduce((s,y)=>s+y.profit,0);
  const totalRev=years.reduce((s,y)=>s+y.grossRevenue,0);

  document.getElementById('five-yr-cards').innerHTML=[
    {l:'5-Year Revenue',v:'$'+Math.round(totalRev).toLocaleString(),s:'cumulative gross',c:'yellow'},
    {l:'5-Year Net Profit',v:(totalProfit<0?'-':'')+'$'+Math.round(Math.abs(totalProfit)).toLocaleString(),s:'cumulative profit',c:totalProfit>=0?'green':'red'},
    {l:'Peak Year Revenue',v:'$'+Math.round(Math.max(...years.map(y=>y.grossRevenue))).toLocaleString(),s:'Year '+(years.findIndex(y=>y.grossRevenue===Math.max(...years.map(y=>y.grossRevenue)))+1),c:''},
    {l:'Peak Year Profit',v:'$'+Math.round(Math.max(...years.map(y=>y.profit))).toLocaleString(),s:'Year '+(years.findIndex(y=>y.profit===Math.max(...years.map(y=>y.profit)))+1),c:'green'},
  ].map(c=>`<div class="sc ${c.c}"><div class="sc-label">${c.l}</div><div class="sc-val">${c.v}</div><div class="sc-sub">${c.s}</div></div>`).join('');

  const rows=[
    ['Gross Revenue',...years.map(y=>y.grossRevenue>0?'$'+Math.round(y.grossRevenue).toLocaleString():'—'),'yellow'],
    ['Total People Costs',...years.map(y=>'$'+Math.round(y.totalPeople).toLocaleString()),''],
    ['Gross Profit',...years.map(y=>fD(y.grossProfit)),''],
    ['Gross Profit %',...years.map(y=>y.grossRevenue>0?((y.grossProfit/y.grossRevenue)*100).toFixed(1)+'%':'—'),'pct'],
    ['Total Expenses',...years.map(y=>'$'+Math.round(y.totalExp).toLocaleString()),''],
    ['NET PROFIT / (LOSS)',...years.map(y=>fD(y.profit)),'profit'],
    ['Net Profit %',...years.map(y=>y.grossRevenue>0?((y.profit/y.grossRevenue)*100).toFixed(1)+'%':'—'),'pct'],
    ['People / Revenue %',...years.map(y=>y.grossRevenue>0?((y.totalPeople/y.grossRevenue)*100).toFixed(1)+'%':'—'),'pct'],
  ];

  document.getElementById('five-yr-table').innerHTML=`<div class="tw"><table style="min-width:600px">
    <thead><tr><th>Metric</th><th>Year 1</th><th>Year 2</th><th>Year 3</th><th>Year 4</th><th>Year 5</th></tr></thead>
    <tbody>${rows.map(([label,...rest])=>{
      const cls=rest.pop();
      const rowCls=cls==='profit'?'row-profit':cls==='pct'?'row-pct':'';
      const lStyle=cls==='yellow'?'style="color:#F5E500;font-weight:800"':'';
      return `<tr class="${rowCls}"><td ${lStyle}>${label}</td>${rest.map(v=>`<td>${v}</td>`).join('')}</tr>`;
    }).join('')}</tbody>
  </table></div>`;
}

// ---- SETUP RENDER ----
function rProgs(){
  document.getElementById('prog-list').innerHTML=S.programs.map((p,pi)=>`
    <div class="card" style="margin-bottom:10px">
      <div style="display:flex;align-items:center;gap:10px;margin-bottom:14px;flex-wrap:wrap">
        <input class="fi" value="${p.name}" oninput="S.programs[${pi}].name=this.value;save()" style="flex:2;min-width:160px;font-size:13px"/>
        <div class="frow" style="flex:1;min-width:120px"><span class="fpfx">$</span><input class="fi" type="number" value="${p.price}" oninput="S.programs[${pi}].price=parseFloat(this.value)||0;save()" placeholder="Price per client"/></div>
        <div class="frow" style="flex:1;min-width:100px"><input class="fi" type="number" value="${p.attrition}" oninput="S.programs[${pi}].attrition=parseFloat(this.value)||0;save()" placeholder="0"/><span class="fpfx">% attrition</span></div>
        <button class="btn btns" style="color:#e88080;border-color:#6d2424;flex-shrink:0" onclick="S.programs.splice(${pi},1);rProgs();save()">Remove</button>
      </div>
      <div style="font-size:10px;font-weight:700;color:#444442;letter-spacing:0.08em;text-transform:uppercase;margin-bottom:8px">Year 1 Monthly Customers</div>
      <div style="display:grid;grid-template-columns:repeat(12,1fr);gap:4px">
        ${MS.map((m,mi)=>`<div><div style="font-size:9px;color:#444442;text-align:center;margin-bottom:3px">${m}</div><input class="fi" type="number" value="${p.customers[mi]||''}" placeholder="0" oninput="S.programs[${pi}].customers[${mi}]=parseFloat(this.value)||0;save()" style="font-size:12px;padding:6px;text-align:center"/></div>`).join('')}
      </div>
    </div>`).join('');
}
function addProg(){S.programs.push({name:'New Program',price:0,attrition:0,customers:Array(12).fill(0)});rProgs();save();}

function rTeam(){
  const totalMonthly=S.team.reduce((s,m)=>{
    const sal=m.salary||0;
    const sup=m.superEligible?(sal*(S.superPct/100)):0;
    return s+sal+sup;
  },0);

  document.getElementById('team-list').innerHTML=S.team.map((m,ti)=>`
    <div class="member-card">
      <div class="member-header">
        <div class="member-avatar">${(m.name||'?').split(' ').map(w=>w[0]).join('').slice(0,2).toUpperCase()}</div>
        <div style="flex:1">
          <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap">
            <input class="fi" value="${m.name}" oninput="S.team[${ti}].name=this.value;rTeam();save()" style="flex:1;min-width:140px;font-size:13px;font-weight:700" placeholder="Team member name"/>
            <input class="fi" value="${m.role||''}" oninput="S.team[${ti}].role=this.value;save()" style="flex:1;min-width:120px;font-size:12px" placeholder="Role / title"/>
          </div>
        </div>
        <button class="btn btns" style="color:#e88080;border-color:#6d2424;flex-shrink:0" onclick="S.team.splice(${ti},1);rTeam();rAll();save()">Remove</button>
      </div>
      <div style="display:grid;grid-template-columns:1fr 1fr 1fr;gap:12px;margin-bottom:12px">
        <div>
          <label class="fl">Pay Type</label>
          <select class="fi" onchange="S.team[${ti}].type=this.value;rTeam();save()">
            <option value="salary" ${m.type==='salary'?'selected':''}>Salary Only</option>
            <option value="commission" ${m.type==='commission'?'selected':''}>Commission Only</option>
            <option value="both" ${m.type==='both'?'selected':''}>Salary + Commission</option>
          </select>
        </div>
        ${(m.type==='salary'||m.type==='both')?`
        <div>
          <label class="fl">Monthly Salary ($)</label>
          <div class="frow"><span class="fpfx">$</span><input class="fi" type="number" value="${m.salary||''}" oninput="S.team[${ti}].salary=parseFloat(this.value)||0;rTeam();rAll();save()" placeholder="0"/></div>
        </div>
        <div>
          <label class="fl">Super Eligible?</label>
          <select class="fi" onchange="S.team[${ti}].superEligible=this.value==='true';rTeam();rAll();save()">
            <option value="true" ${m.superEligible?'selected':''}>Yes — ${S.superPct||11}% super</option>
            <option value="false" ${!m.superEligible?'selected':''}>No</option>
          </select>
        </div>`:`<div></div><div></div>`}
      </div>
      ${(m.type==='commission'||m.type==='both')?`
      <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px">
        <div>
          <label class="fl">Commission Rate (%)</label>
          <div class="frow"><input class="fi" type="number" value="${m.commissionPct||''}" oninput="S.team[${ti}].commissionPct=parseFloat(this.value)||0;rAll();save()" placeholder="0"/><span class="fpfx">%</span></div>
        </div>
        <div>
          <label class="fl">Commission Based On</label>
          <select class="fi" onchange="S.team[${ti}].commissionBase=this.value;rAll();save()">
            <option value="revenue" ${m.commissionBase==='revenue'?'selected':''}>Gross Revenue</option>
            <option value="grossProfit" ${m.commissionBase==='grossProfit'?'selected':''}>Gross Profit</option>
          </select>
        </div>
      </div>`:''}
      <div style="margin-top:12px;padding-top:10px;border-top:1px solid #252528;display:flex;justify-content:space-between;align-items:center">
        <span style="font-size:11px;color:#555552;letter-spacing:0.05em;text-transform:uppercase">Estimated Monthly Cost (Year 1)</span>
        <span style="font-size:15px;font-weight:700;color:#F5E500">$${Math.round((m.salary||0)+(m.superEligible?((m.salary||0)*(S.superPct/100)):0)).toLocaleString()}</span>
      </div>
    </div>`).join('');

  document.getElementById('setup-total-val').textContent='$'+Math.round(totalMonthly).toLocaleString()+' / month';
}

function addMember(){
  S.team.push({name:'New Team Member',role:'',type:'salary',salary:0,commissionPct:0,commissionBase:'revenue',superEligible:true});
  rTeam();save();
}

function rExps(){
  document.getElementById('exp-list').innerHTML=S.expenses.map((e,ei)=>`
    <div class="card" style="margin-bottom:10px">
      <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px">
        <input class="fi" value="${e.name}" oninput="S.expenses[${ei}].name=this.value;save()" style="flex:1;font-size:13px"/>
        <button class="btn btns" style="margin-left:10px;color:#e88080;border-color:#6d2424;flex-shrink:0" onclick="S.expenses.splice(${ei},1);rExps();save()">Remove</button>
      </div>
      <div style="font-size:10px;font-weight:700;color:#444442;letter-spacing:0.08em;text-transform:uppercase;margin-bottom:8px">Monthly Amounts ($)</div>
      <div style="display:grid;grid-template-columns:repeat(12,1fr);gap:4px">
        ${MS.map((m,mi)=>`<div><div style="font-size:9px;color:#444442;text-align:center;margin-bottom:3px">${m}</div><input class="fi" type="number" value="${e.monthly[mi]||''}" placeholder="0" oninput="S.expenses[${ei}].monthly[${mi}]=parseFloat(this.value)||0;save()" style="font-size:12px;padding:6px;text-align:center"/></div>`).join('')}
      </div>
    </div>`).join('');
}
function addExp(){S.expenses.push({name:'New Expense',monthly:Array(12).fill(0)});rExps();save();}

function rAll(){
  if(document.getElementById('pg-forecast').classList.contains('active'))rForecast();
  if(document.getElementById('pg-people').classList.contains('active'))rPeople();
  if(document.getElementById('pg-summary').classList.contains('active'))rFiveYear();
  rTeam();
}

function init(){
  load();
  document.getElementById('super-pct').value=S.superPct||11;
  document.getElementById('tax-pct').value=S.taxPct||0;
  document.getElementById('growth-rate').value=S.growthRate||20;
  rProgs();
  rTeam();
  rExps();
  rForecast();
}
init();
</script>
</body>
</html>

