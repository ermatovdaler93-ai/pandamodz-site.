<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>PANDA MODZ</title>
<style>
:root{--bg:#07070d;--card:rgba(255,255,255,.05);--bd:rgba(255,255,255,.1);--tx:#f2f2f8;--mu:#8b8ba3;--c1:#39ff88;--c2:#ff3d9a;--c3:#2de2ff;--c4:#a259ff;--c5:#ffb830;box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}
@media(prefers-color-scheme:dark){:root{color-scheme:dark}}
*{box-sizing:border-box}html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--tx);font-family:system-ui,-apple-system,"Segoe UI",Roboto,sans-serif;min-height:100vh;overflow-x:hidden}
body:before{content:"";position:fixed;inset:0;background:radial-gradient(600px 400px at 10% 0,rgba(162,89,255,.25),transparent),radial-gradient(600px 400px at 90% 10%,rgba(255,61,154,.2),transparent),radial-gradient(700px 500px at 50% 110%,rgba(45,226,255,.18),transparent);pointer-events:none;z-index:0}
.w{position:relative;z-index:1;max-width:980px;margin:0 auto;padding:18px 16px 60px}
header{display:flex;align-items:center;justify-content:space-between;gap:10px;flex-wrap:wrap;margin-bottom:18px}
.logo{display:flex;align-items:center;gap:10px;font-weight:900;font-size:24px;letter-spacing:2px}
.logo i{font-style:normal;font-size:34px;filter:drop-shadow(0 0 10px var(--c1))}
.logo b{background:linear-gradient(90deg,var(--c1),var(--c3),var(--c4),var(--c2));-webkit-background-clip:text;background-clip:text;color:transparent}
.tabs{display:flex;gap:6px;background:var(--card);border:1px solid var(--bd);border-radius:14px;padding:4px}
.tabs button{border:0;background:none;color:var(--mu);padding:9px 16px;border-radius:10px;font-weight:700;cursor:pointer;font-size:14px}
.tabs button.on{background:linear-gradient(135deg,var(--c4),var(--c2));color:#fff;box-shadow:0 0 18px rgba(255,61,154,.4)}
.card{background:var(--card);border:1px solid var(--bd);border-radius:20px;padding:20px;backdrop-filter:blur(12px);margin-bottom:16px}
h2{margin:0 0 14px;font-size:15px;text-transform:uppercase;letter-spacing:2px;color:var(--mu)}
.prods{display:grid;grid-template-columns:repeat(auto-fit,minmax(150px,1fr));gap:10px}
.p{border:2px solid var(--bd);border-radius:16px;padding:14px;cursor:pointer;background:rgba(0,0,0,.25);transition:.2s;text-align:left;color:var(--tx)}
.p .e{font-size:26px}.p .n{font-weight:800;margin-top:4px}.p .d{font-size:12px;color:var(--mu)}
.p.on{border-color:var(--pc);box-shadow:0 0 22px -4px var(--pc),inset 0 0 20px -12px var(--pc)}
.row{display:flex;gap:8px;flex-wrap:wrap}
.chip{border:1px solid var(--bd);background:rgba(0,0,0,.3);color:var(--tx);padding:9px 14px;border-radius:12px;cursor:pointer;font-weight:600;font-size:14px}
.chip.on{background:var(--c3);color:#001;border-color:var(--c3);box-shadow:0 0 16px rgba(45,226,255,.5)}
.btn{border:0;border-radius:14px;padding:14px 22px;font-weight:900;font-size:16px;cursor:pointer;color:#001;background:linear-gradient(135deg,var(--c1),var(--c3));box-shadow:0 0 26px rgba(57,255,136,.4);width:100%;margin-top:16px;letter-spacing:1px}
.btn:active{transform:scale(.98)}.btn[disabled]{opacity:.5}
.btn.pk{background:linear-gradient(135deg,var(--c2),var(--c4));color:#fff;box-shadow:0 0 26px rgba(255,61,154,.4)}
.key{font-family:ui-monospace,Menlo,Consolas,monospace;font-size:clamp(17px,5vw,26px);font-weight:800;text-align:center;padding:18px;border-radius:16px;margin-top:16px;border:1px dashed var(--c1);color:var(--c1);text-shadow:0 0 12px var(--c1);word-break:break-all;cursor:pointer;background:rgba(57,255,136,.06)}
input,select{width:100%;background:rgba(0,0,0,.35);border:1px solid var(--bd);border-radius:12px;padding:13px;color:var(--tx);font-size:15px;font-family:ui-monospace,Menlo,monospace;outline:none}
input:focus{border-color:var(--c4);box-shadow:0 0 14px rgba(162,89,255,.4)}
.msg{margin-top:12px;padding:11px 14px;border-radius:12px;font-size:14px;font-weight:600}
.ok{background:rgba(57,255,136,.12);color:var(--c1)}.er{background:rgba(255,61,154,.12);color:var(--c2)}.wr{background:rgba(255,184,48,.12);color:var(--c5)}
.stats{display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:10px;margin-bottom:16px}
.st{border-radius:16px;padding:14px;border:1px solid var(--bd);background:var(--card)}
.st b{display:block;font-size:28px;font-weight:900}.st span{font-size:12px;color:var(--mu);text-transform:uppercase;letter-spacing:1px}
.tw{overflow-x:auto;border-radius:12px}
table{width:100%;border-collapse:collapse;font-size:13px;min-width:640px}
th{text-align:left;color:var(--mu);font-size:11px;text-transform:uppercase;letter-spacing:1px;padding:8px}
td{padding:9px 8px;border-top:1px solid var(--bd);font-family:ui-monospace,Menlo,monospace}
.tag{padding:3px 9px;border-radius:99px;font-size:11px;font-weight:800;font-family:system-ui}
.t-new{background:rgba(45,226,255,.15);color:var(--c3)}.t-used{background:rgba(57,255,136,.15);color:var(--c1)}.t-ban{background:rgba(255,61,154,.15);color:var(--c2)}.t-exp{background:rgba(255,184,48,.15);color:var(--c5)}
.ib{border:1px solid var(--bd);background:rgba(0,0,0,.3);color:var(--tx);border-radius:8px;padding:5px 9px;cursor:pointer;margin-right:4px;font-size:12px}
.g2{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.lock{text-align:center;padding:30px 10px}.lock .big{font-size:56px}
.live{display:inline-flex;align-items:center;gap:6px;font-size:12px;color:var(--mu)}.live:before{content:"";width:8px;height:8px;border-radius:50%;background:var(--c1);box-shadow:0 0 10px var(--c1)}
.hide{display:none}
</style>
</head>
<body>
<div class="w">
<header>
  <div class="logo"><i>🐼</i><b>PANDA MODZ</b></div>
  <div class="tabs"><button id="tg" class="on">⚡ Генератор</button><button id="ta">🛡 Админ</button></div>
</header>

<section id="vg">
  <div class="card"><h2>1 · Выбери продукт</h2><div class="prods" id="prods"></div></div>
  <div class="card"><h2>2 · Срок действия</h2><div class="row" id="durs"></div>
    <button class="btn" id="gen">⚡ СГЕНЕРИРОВАТЬ КЛЮЧ</button>
    <div id="out"></div>
  </div>
  <div class="card"><h2>🔑 Активировать ключ</h2>
    <input id="act" placeholder="PANDA-XXXX-XXXX-XXXX" autocapitalize="characters">
    <button class="btn pk" id="actb">АКТИВИРОВАТЬ</button>
    <div id="actm"></div>
  </div>
</section>

<section id="va" class="hide"></section>
</div>

<script>
const PRODS=[
 {id:"vip",n:"VIP Menu",e:"👑",c:"#39ff88",d:"Полный доступ"},
 {id:"aim",n:"Aim Pro",e:"🎯",c:"#ff3d9a",d:"Точность и скорость"},
 {id:"esp",n:"ESP Vision",e:"👁",c:"#2de2ff",d:"Подсветка целей"},
 {id:"ult",n:"Ultimate",e:"💎",c:"#a259ff",d:"Всё включено"},
 {id:"fps",n:"FPS Boost",e:"🚀",c:"#ffb830",d:"Плавная игра"}];
const DURS=[{d:1,l:"1 день"},{d:7,l:"7 дней"},{d:30,l:"30 дней"},{d:0,l:"Навсегда"}];
let sel=PRODS[0].id,dur=7,keys=[],db=null,isAdmin=false,tab="g",lastGen=0;
const $=s=>document.querySelector(s);
const esc=s=>String(s).replace(/[&<>"]/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;"}[c]));
const pr=id=>PRODS.find(p=>p.id===id)||PRODS[0];
const fmt=t=>t?new Date(t).toLocaleString("ru-RU",{day:"2-digit",month:"2-digit",hour:"2-digit",minute:"2-digit"}):"—";

/* ---------- storage: shared db with local fallback ---------- */
function loadLocal(){try{keys=JSON.parse(localStorage.getItem("pm_keys")||"[]")}catch(e){keys=[]}}
function saveLocal(){try{localStorage.setItem("pm_keys",JSON.stringify(keys))}catch(e){}}
async function put(k){
  if(db){try{await db.collection("keys").doc(k.id).set(k);return}catch(e){}}
  const i=keys.findIndex(x=>x.id===k.id);i<0?keys.unshift(k):keys[i]=k;saveLocal();render();
}
async function del(id){
  if(db){try{await db.collection("keys").doc(id).delete();return}catch(e){}}
  keys=keys.filter(x=>x.id!==id);saveLocal();render();
}
function genKey(){
  const A="ABCDEFGHJKLMNPQRSTUVWXYZ23456789",r=new Uint32Array(12);crypto.getRandomValues(r);
  const s=[...r].map(n=>A[n%A.length]).join("");
  return "PANDA-"+s.slice(0,4)+"-"+s.slice(4,8)+"-"+s.slice(8,12);
}
function status(k){
  if(k.status==="banned")return"ban";
  if(k.status==="used")return(k.expiresAt&&k.expiresAt<Date.now())?"exp":"used";
  return"new";
}
async function make(p,d){
  const key=genKey();
  await put({id:key.replace(/-/g,""),key,product:p,days:d,created:Date.now(),status:"new",usedAt:0,expiresAt:0});
  return key;
}

/* ---------- generator view ---------- */
function drawGen(){
  $("#prods").innerHTML=PRODS.map(p=>`<button class="p ${p.id===sel?"on":""}" data-p="${p.id}" style="--pc:${p.c}"><div class="e">${p.e}</div><div class="n" style="color:${p.c}">${p.n}</div><div class="d">${p.d}</div></button>`).join("");
  $("#durs").innerHTML=DURS.map(x=>`<button class="chip ${x.d===dur?"on":""}" data-d="${x.d}">${x.l}</button>`).join("");
}
$("#prods").onclick=e=>{const b=e.target.closest(".p");if(b){sel=b.dataset.p;drawGen()}};
$("#durs").onclick=e=>{const b=e.target.closest(".chip");if(b){dur=+b.dataset.d;drawGen()}};
$("#gen").onclick=async()=>{
  const wait=isAdmin?0:15000-(Date.now()-lastGen);
  if(wait>0){$("#out").innerHTML=`<div class="msg wr">Подожди ${Math.ceil(wait/1000)} сек.</div>`;return}
  lastGen=Date.now();
  const k=await make(sel,dur),p=pr(sel);
  $("#out").innerHTML=`<div class="key" style="border-color:${p.c};color:${p.c};text-shadow:0 0 12px ${p.c}" id="kk">${k}</div><div class="msg ok">Ключ создан и сразу появился в админ-панели. Нажми на ключ, чтобы скопировать.</div>`;
  $("#kk").onclick=()=>{navigator.clipboard&&navigator.clipboard.writeText(k).catch(()=>{});$("#kk").style.opacity=.5;setTimeout(()=>$("#kk").style.opacity=1,300)};
};
$("#actb").onclick=async()=>{
  const v=$("#act").value.trim().toUpperCase(),id=v.replace(/-/g,""),k=keys.find(x=>x.id===id),m=$("#actm");
  if(!k)return m.innerHTML=`<div class="msg er">❌ Ключ не найден</div>`;
  const s=status(k);
  if(s==="ban")return m.innerHTML=`<div class="msg er">🚫 Ключ заблокирован</div>`;
  if(s==="used"||s==="exp")return m.innerHTML=`<div class="msg ${s==="exp"?"wr":"er"}">${s==="exp"?"⏰ Срок ключа истёк":"Ключ уже активирован"}</div>`;
  const now=Date.now();
  await put({...k,status:"used",usedAt:now,expiresAt:k.days?now+k.days*864e5:0});
  m.innerHTML=`<div class="msg ok">✅ ${pr(k.product).e} ${pr(k.product).n} активирован · ${k.days?k.days+" дн.":"навсегда"}</div>`;
};

/* ---------- admin view ---------- */
function drawAdmin(){
  const v=$("#va");
  if(!isAdmin){v.innerHTML=`<div class="card lock"><div class="big">🔒</div><h2 style="margin-top:12px">Доступ только для админа</h2><p style="color:var(--mu)">Войди в claude.ai под аккаунтом владельца или редактора этого сайта.</p></div>`;return}
  const c={new:0,used:0,ban:0,exp:0};keys.forEach(k=>c[status(k)]++);
  const q=(window._q||"").toUpperCase(),list=keys.filter(k=>!q||k.key.includes(q)||pr(k.product).n.toUpperCase().includes(q));
  v.innerHTML=`
  <div class="stats">
   <div class="st" style="border-color:var(--c3)"><b style="color:var(--c3)">${keys.length}</b><span>Всего</span></div>
   <div class="st" style="border-color:var(--c1)"><b style="color:var(--c1)">${c.used}</b><span>Активно</span></div>
   <div class="st" style="border-color:var(--c4)"><b style="color:var(--c4)">${c.new}</b><span>Свободно</span></div>
   <div class="st" style="border-color:var(--c5)"><b style="color:var(--c5)">${c.exp}</b><span>Истекло</span></div>
   <div class="st" style="border-color:var(--c2)"><b style="color:var(--c2)">${c.ban}</b><span>Бан</span></div>
  </div>
  <div class="card"><h2>Массовая генерация <span class="live" style="margin-left:8px">live</span></h2>
   <div class="g2"><select id="bp">${PRODS.map(p=>`<option value="${p.id}">${p.e} ${p.n}</option>`).join("")}</select>
   <select id="bd">${DURS.map(x=>`<option value="${x.d}">${x.l}</option>`).join("")}</select></div>
   <div class="g2" style="margin-top:10px"><input id="bn" type="number" min="1" max="50" value="10"><button class="btn pk" id="bg" style="margin:0;padding:12px">+ СОЗДАТЬ</button></div>
  </div>
  <div class="card"><h2>Ключи</h2>
   <input id="sq" placeholder="🔍 Поиск по ключу или продукту" value="${esc(window._q||"")}" style="margin-bottom:12px">
   <div class="tw"><table><tr><th>Ключ</th><th>Продукт</th><th>Срок</th><th>Статус</th><th>Создан</th><th>Действия</th></tr>
   ${list.slice(0,200).map(k=>{const p=pr(k.product),s=status(k),lb={new:"СВОБОДЕН",used:"АКТИВЕН",ban:"БАН",exp:"ИСТЁК"}[s];
    return`<tr><td>${k.key}</td><td style="color:${p.c};font-family:system-ui;font-weight:700">${p.e} ${p.n}</td><td>${k.days?k.days+"д":"∞"}</td><td><span class="tag t-${s==="ban"?"ban":s}">${lb}</span></td><td>${fmt(k.created)}</td>
    <td><button class="ib" data-a="cp" data-i="${k.id}">📋</button><button class="ib" data-a="bn" data-i="${k.id}">${k.status==="banned"?"♻️":"🚫"}</button><button class="ib" data-a="dl" data-i="${k.id}">🗑</button></td></tr>`}).join("")||`<tr><td colspan="6" style="color:var(--mu);text-align:center;padding:24px">Пока нет ключей</td></tr>`}
   </table></div>
   <div class="row" style="margin-top:12px"><button class="chip" id="ex">⬇ Экспорт TXT</button><button class="chip" id="cl" style="color:var(--c2)">Удалить все истёкшие</button></div>
  </div>`;
  $("#bg").onclick=async()=>{const n=Math.min(50,Math.max(1,+$("#bn").value||1));for(let i=0;i<n;i++)await make($("#bp").value,+$("#bd").value)};
  $("#sq").oninput=e=>{window._q=e.target.value;const p=e.target.selectionStart;drawAdmin();const s=$("#sq");s.focus();s.setSelectionRange(p,p)};
  $("#ex").onclick=async()=>{const txt=list.map(k=>`${k.key} | ${pr(k.product).n} | ${k.days||"forever"} | ${status(k)}`).join("\n");
    try{const d=await claude.use("downloads");if(d){await d.save({filename:"panda-modz-keys.txt",data:txt});return}}catch(e){}
    navigator.clipboard&&navigator.clipboard.writeText(txt)};
  $("#cl").onclick=()=>keys.filter(k=>status(k)==="exp").forEach(k=>del(k.id));
}
$("#va").onclick=e=>{
  const b=e.target.closest("[data-a]");if(!b)return;const k=keys.find(x=>x.id===b.dataset.i);if(!k)return;
  if(b.dataset.a==="cp")navigator.clipboard&&navigator.clipboard.writeText(k.key);
  if(b.dataset.a==="bn")put({...k,status:k.status==="banned"?(k.usedAt?"used":"new"):"banned"});
  if(b.dataset.a==="dl")del(k.id);
};

/* ---------- tabs / render ---------- */
function render(){if(tab==="a")drawAdmin()}
function show(t){tab=t;$("#vg").classList.toggle("hide",t!=="g");$("#va").classList.toggle("hide",t!=="a");$("#tg").classList.toggle("on",t==="g");$("#ta").classList.toggle("on",t==="a");if(t==="a")drawAdmin()}
$("#tg").onclick=()=>show("g");$("#ta").onclick=()=>show("a");

/* ---------- boot ---------- */
drawGen();loadLocal();
(async()=>{
  try{const u=await claude.use("user");isAdmin=!!(u&&u.canEdit());}catch(e){}
  try{db=await claude.use("db")}catch(e){}
  if(db){
    db.collection("keys").orderBy("created","desc").onSnapshot(s=>{keys=s.docs.map(d=>d.data());render()},()=>{db=null;loadLocal();render()});
  }
  render();
})();
</script>
</body>
</html>
