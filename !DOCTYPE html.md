<!DOCTYPE html>  
<html lang="ar" dir="rtl">  
<head>  
<meta charset="utf-8">  
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">  
<meta name="description" content="تقاطع: منصة ذكاء اصطناعي لاكتشاف التعارضات وتحويل المعلومات المتضاربة إلى قرارات موثوقة">  
<title>تقاطع | TAQATOA</title>  
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 44 30'%3E%3Ccircle cx='16' cy='15' r='12' fill='%232563D6'/%3E%3Ccircle cx='28' cy='15' r='12' fill='%230E9F7E'/%3E%3Cpath d='M22 5.2a12 12 0 0 1 0 19.6a12 12 0 0 1 0-19.6z' fill='%23E8A100'/%3E%3C/svg%3E">  
<link href="https://fonts.googleapis.com/css2?family=Readex+Pro:wght@300;400;600;700&display=swap" rel="stylesheet">  
<style>  
:root{--bg:#EEF2F7;--card:#fff;--ink:#0B1F3A;--mut:#5A6B80;--line:#DCE3EC;--a:#2563D6;--b:#0E9F7E;--x:#E8A100;--red:#D43D2E;--vio:#6F52C9;--hero:#0B1F3A;--soft:#F6F8FB;  
box-sizing:border-box;padding-top:env(safe-area-inset-top,0px);padding-bottom:env(safe-area-inset-bottom,0px)}  
@media(prefers-color-scheme:dark){:root:not([data-theme="light"]){--bg:#08121F;--card:#111E2F;--ink:#E8EEF6;--mut:#9DAEC2;--line:#233449;--a:#6C9CFF;--b:#3FD3A8;--x:#F5BE45;--red:#FF7C6C;--vio:#AD98F5;--hero:#0D2342;--soft:#0D1928}}  
:root[data-theme="dark"]{--bg:#08121F;--card:#111E2F;--ink:#E8EEF6;--mut:#9DAEC2;--line:#233449;--a:#6C9CFF;--b:#3FD3A8;--x:#F5BE45;--red:#FF7C6C;--vio:#AD98F5;--hero:#0D2342;--soft:#0D1928}  
html{scroll-padding-top:env(safe-area-inset-top,0px)}  
*{box-sizing:border-box}  
body{margin:0;background:var(--bg);color:var(--ink);font:400 15px/1.85 "Readex Pro",Tahoma,sans-serif}  
button{font:inherit;color:inherit;cursor:pointer}  
button:focus-visible,label:focus-within,.chip:focus-visible{outline:3px solid var(--x);outline-offset:2px}  
.wrap{max-width:980px;margin:0 auto;padding:0 16px 56px}  
.top{background:var(--hero);color:#fff;position:relative;overflow:hidden}  
.top .wrap{padding-bottom:0}  
.bg{position:absolute;inset-inline-start:-40px;top:-30px;width:420px;opacity:.35;pointer-events:none}  
header{position:relative;display:flex;align-items:center;justify-content:space-between;gap:12px;padding:16px 0;flex-wrap:wrap}  
.logo{display:flex;align-items:center;gap:10px;font-weight:700;font-size:24px}  
.logo small{display:block;font-size:10.5px;font-weight:300;letter-spacing:.2em;direction:ltr;opacity:.7;line-height:1.2}  
.hero{position:relative;padding:20px 0 60px}  
.hero h1{font-size:clamp(26px,5.2vw,42px);line-height:1.45;margin:0 0 10px;font-weight:700;max-width:18em}  
.hero p{margin:0;max-width:56ch;opacity:.8;font-weight:300}  
nav{position:relative;display:flex;gap:4px;margin-top:-26px;background:var(--card);border:1px solid var(--line);border-radius:16px;padding:5px;box-shadow:0 8px 24px rgba(11,31,58,.14);overflow-x:auto}  
nav button{flex:1;border:0;background:none;padding:10px 14px;border-radius:12px;white-space:nowrap;color:var(--mut);font-weight:600}  
nav button[aria-selected=true]{background:var(--ink);color:var(--card)}  
.note{border-radius:12px;background:var(--soft);border:1px solid var(--line);border-inline-start:4px solid var(--x);padding:10px 14px;font-size:13px;color:var(--mut);margin:16px 0}  
.card{background:var(--card);border:1px solid var(--line);border-radius:18px;padding:18px}  
.grid{display:grid;gap:12px}.g3{grid-template-columns:repeat(auto-fit,minmax(250px,1fr))}  
h2{font-size:20px;margin:26px 0 12px}  
h3{font-size:16px;margin:0 0 2px}  
.src{display:flex;gap:12px;align-items:flex-start;position:relative;overflow:hidden}  
.src:before{content:"";position:absolute;inset-block:0;inset-inline-start:0;width:5px;background:var(--c)}  
.ico{width:40px;height:40px;border-radius:12px;background:var(--c);color:#fff;display:grid;place-items:center;font-weight:700;flex:none}  
.meta{font-size:12.5px;color:var(--mut)}  
.btn{border:0;background:var(--a);color:#fff;padding:12px 24px;border-radius:12px;font-weight:600;display:inline-block}  
.btn.alt{background:var(--card);border:1px solid var(--line);color:var(--ink)}  
.btn:disabled{opacity:.5}  
.steps{list-style:none;padding:0;margin:16px 0 0;display:grid;gap:8px;grid-template-columns:repeat(auto-fit,minmax(220px,1fr))}  
.steps li{display:flex;gap:10px;align-items:center;color:var(--mut);font-size:14px;background:var(--card);border:1px solid var(--line);border-radius:12px;padding:8px 12px}  
.steps li i{width:22px;height:22px;border-radius:50%;border:2px solid var(--line);flex:none;display:grid;place-items:center;font-size:12px;font-style:normal}  
.steps li.on{color:var(--ink)}  
.steps li.on i{background:var(--b);border-color:var(--b);color:#fff}  
.chips{display:flex;gap:6px;flex-wrap:wrap;margin:0 0 14px}  
.chip{border:1px solid var(--line);background:var(--card);border-radius:99px;padding:4px 14px;font-size:13px}  
.chip[aria-pressed=true]{background:var(--ink);color:var(--card);border-color:var(--ink)}  
.tag{display:inline-block;border-radius:8px;padding:0 10px;font-size:12.5px;font-weight:600;color:#fff;background:var(--k)}  
.t-conf{--k:var(--red)}.t-poss{--k:var(--x);color:#1b1200}.t-expl{--k:var(--b);color:#00241a}.t-unr{--k:var(--vio)}.t-ok{--k:var(--a)}  
.item{width:100%;text-align:start;display:block;margin-bottom:10px;position:relative;overflow:hidden}  
.item:before{content:"";position:absolute;inset-block:0;inset-inline-start:0;width:5px;background:var(--k)}  
.item[aria-expanded=true]{border-color:var(--ink)}  
.row{display:flex;align-items:center;gap:12px;justify-content:space-between}  
.ring{--p:0;width:54px;height:54px;border-radius:50%;background:conic-gradient(var(--k) calc(var(--p)*1%),var(--line) 0);display:grid;place-items:center;flex:none}  
.ring b{width:42px;height:42px;border-radius:50%;background:var(--card);display:grid;place-items:center;font-size:13px}  
.cmp{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin:14px 0}  
.q{border-radius:14px;padding:12px;background:var(--soft);border-top:4px solid var(--c)}  
.q small{display:block;color:var(--mut);font-size:12px}  
.q b{font-size:20px}  
.six{display:grid;gap:0;margin:8px 0}  
.six div{padding:10px 0;border-top:1px solid var(--line)}  
.six b{display:block;font-size:12.5px;color:var(--mut);font-weight:600}  
.why{background:var(--soft);border:1px solid var(--line);border-radius:14px;padding:14px;margin-top:12px}  
.why h4{margin:0 0 6px;font-size:15px;display:flex;gap:8px;align-items:center;flex-wrap:wrap}  
.lvl{font-size:12.5px;border-radius:8px;padding:0 10px;background:var(--k);color:#fff}  
.fx{list-style:none;margin:8px 0;padding:0;display:grid;gap:6px;font-size:14px}  
.fx li{display:flex;gap:8px}  
.fx li span{width:20px;height:20px;border-radius:6px;display:grid;place-items:center;flex:none;font-size:13px;font-weight:700;color:#fff;margin-top:4px}  
.pl{background:var(--b)}.mi{background:var(--red)}  
.ev{display:flex;gap:6px;flex-wrap:wrap}  
.ev span{border:1px solid var(--line);background:var(--card);border-radius:8px;padding:2px 10px;font-size:12.5px}  
.bar{height:8px;background:var(--line);border-radius:9px;overflow:hidden;margin:4px 0 8px}  
.bar span{display:block;height:100%;background:var(--k)}  
.stat{font-size:34px;font-weight:700;line-height:1.3}  
.hid{display:none}  
table{border-collapse:collapse;width:100%;font-size:13.5px;min-width:640px}  
td,th{border-bottom:1px solid var(--line);padding:8px;text-align:start;vertical-align:top}  
th{color:var(--mut);font-weight:600}  
.scroll{overflow-x:auto}  
@media(max-width:520px){.cmp{grid-template-columns:1fr}.bg{width:300px}}  
@media print{.top,nav,.noprint{display:none!important}.hid.pr{display:block!important}}  
</style>  
</head>  
<body>  
<div class="top">  
<svg class="bg" viewBox="0 0 420 260" aria-hidden="true"><circle cx="150" cy="130" r="115" fill="var(--a)"/><circle cx="270" cy="130" r="115" fill="var(--b)"/><path d="M210 30a115 115 0 0 1 0 200a115 115 0 0 1 0-200z" fill="var(--x)"/></svg>  
<div class="wrap">  
<header>  
 <div class="logo">  
  <svg width="48" height="32" viewBox="0 0 44 30" aria-hidden="true"><circle cx="16" cy="15" r="12" fill="#6C9CFF"/><circle cx="28" cy="15" r="12" fill="#3FD3A8"/><path d="M22 5.2a12 12 0 0 1 0 19.6a12 12 0 0 1 0-19.6z" fill="#F5BE45"/></svg>  
  <div>تقاطع<small>TAQATOA</small></div>  
 </div>  
</header>  
<section class="hero">  
 <h1>اعرف أي معلومة تثق بها، وأي معلومة تحتاج إلى تحقق</h1>  
 <p>ارفع مصادر عن موضوع واحد، ويكشف «تقاطع» التعارضات بينها، ويشرح أثرها، ويذكر سبب كل درجة ثقة ومصدرها.</p>  
</section>  
</div>  
</div>  
  
<div class="wrap">  
<nav role="tablist" aria-label="أقسام النموذج">  
 <button role="tab" data-t="work" aria-selected="true">مساحة العمل</button>  
 <button role="tab" data-t="res" aria-selected="false">النتائج</button>  
 <button role="tab" data-t="rep" aria-selected="false">التقرير</button>  
</nav>  
<div class="note">نموذج أولي تفاعلي: التحليل محاكى على بيانات توضيحية، وليست معلومات فعلية عن جهة أو برنامج حقيقي.</div>  
  
<main id="work" class="panel">  
 <h2>المصادر · موضوع: القبول في «برنامج س» (وهمي)</h2>  
 <div class="grid g3" id="srcs"></div>  
 <div style="margin-top:16px;display:flex;gap:8px;flex-wrap:wrap" class="noprint">  
  <label class="btn alt" for="up">إضافة ملف PDF</label>  
  <input id="up" type="file" accept=".pdf" class="hid">  
  <button class="btn" id="go">حلّل المصادر</button>  
 </div>  
 <ul class="steps" id="steps" aria-live="polite"></ul>  
</main>  
  
<main id="res" class="panel hid">  
 <h2>التعارضات المكتشفة</h2>  
 <div class="chips" id="chips" role="group" aria-label="تصفية النتائج"></div>  
 <div id="list"></div>  
</main>  
  
<main id="rep" class="panel hid pr">  
 <h2>التقرير القابل للمراجعة</h2>  
 <div class="grid g3" id="sum"></div>  
 <div class="card scroll" style="margin-top:12px"><table id="tbl"></table></div>  
 <div style="margin-top:14px;display:flex;gap:8px" class="noprint">  
  <button class="btn" id="copy">نسخ الملخص</button>  
  <button class="btn alt" onclick="window.print()">طباعة / حفظ PDF</button>  
 </div>  
</main>  
</div>  
  
<script>  
const S=[  
 {n:"دليل القبول 2026",o:"عمادة القبول (جهة وهمية)",d:"2026-08-01",k:"دليل",p:12,c:"var(--a)"},  
 {n:"الأسئلة الشائعة",o:"عمادة القبول (جهة وهمية)",d:"2026-09-10",k:"أسئلة شائعة",p:3,c:"var(--b)"},  
 {n:"تعميم تحديث الرسوم",o:"الشؤون المالية (جهة وهمية)",d:"2026-09-22",k:"تعميم",p:1,c:"var(--vio)"}];  
const C={conf:["تعارض مؤكد","t-conf"],poss:["تعارض محتمل","t-poss"],expl:["اختلاف مفسّر","t-expl"],unr:["غير محسوم","t-unr"],ok:["متفق عليه","t-ok"]};  
const L=c=>c>=90?["ثقة عالية","var(--b)"]:c>=75?["ثقة جيدة","var(--a)"]:c>=60?["ثقة متوسطة","var(--x)"]:["غير متأكد","var(--red)"];  
const F=[  
{id:1,cl:"unr",ti:"موعد إغلاق التقديم",a:["20 نوفمبر","دليل القبول، ص4"],b:["25 نوفمبر","الأسئلة الشائعة، ص2"],cf:62,  
 what:"تاريخ إغلاق التقديم: 20 نوفمبر في الدليل و25 نوفمبر في الأسئلة الشائعة.",  
 real:"المصدران عن البرنامج والفئة والفترة نفسها، فلا يوجد تفسير يزيل الاختلاف.",  
 time:"الأسئلة الشائعة أحدث (10 سبتمبر)، لكن الأحدث ليس بالضرورة الأعلى سلطة.",  
 imp:"أثر محتمل: قد يفوّت المتقدم الموعد إن اعتمد التاريخ المتأخر.",  
 act:"اسأل عمادة القبول: «ما موعد إغلاق التقديم المعتمد لبرنامج س؟»",  
 why:"النصان مستخرجان حرفيًا وهما متعارضان فعلًا، لكن لا يوجد نص رسمي يحدد أيهما يسري.",  
 fx:[[1,"الاقتباسان حرفيان من وثيقتين صادرتين عن الجهة نفسها"],[1,"البرنامج والفئة والفترة متطابقة في المصدرين"],[0,"لا يوجد تعميم أو نص ينص على إلغاء أحد التاريخين"],[0,"الأحدث تاريخًا لا يعني الأعلى اعتمادًا"]],  
 ev:["دليل القبول 2026 · ص4","الأسئلة الشائعة · ص2"]},  
{id:2,cl:"expl",ti:"الحد الأدنى للنسبة الموزونة",a:["85%","دليل القبول، ص6 (خريجو الثانوية)"],b:["80%","الأسئلة الشائعة، ص1 (حملة الدبلوم)"],cf:91,  
 what:"نسبتان مختلفتان: 85% و80%.",  
 real:"ليس تعارضًا: كل نسبة تخص فئة مختلفة من المتقدمين.",  
 time:"لا يوجد تغيير زمني بين النسختين.",  
 imp:"أثر مثبت: على المتقدم أن يطابق فئته قبل قراءة الشرط.",  
 act:"اعرض الشرطين مقسّمين حسب الفئة في الدليل.",  
 why:"الفئة مذكورة صراحة بجوار كل نسبة في المصدرين، فالتفسير مدعوم بنص مباشر.",  
 fx:[[1,"كل نسبة مقرونة بفئتها في النص نفسه"],[1,"لا يوجد في أي مصدر ما يوحي بأن النسبتين لفئة واحدة"],[0,"التحقق من الفئات اعتمد على صياغة الأسئلة الشائعة المختصرة"]],  
 ev:["دليل القبول 2026 · ص6","الأسئلة الشائعة · ص1"]},  
{id:3,cl:"conf",ti:"رسوم اختبار القبول",a:["100 ريال","دليل القبول، ص3"],b:["150 ريال","تعميم تحديث الرسوم، ص1"],cf:96,  
 what:"رسوم الاختبار: 100 ريال في الدليل و150 ريالًا في التعميم.",  
 real:"تعارض مؤكد: التعميم ينص صراحة على تعديل الرسوم لنفس الاختبار والفترة.",  
 time:"التعميم (22 سبتمبر) أحدث من الدليل (1 أغسطس) ويحل محله بنص صريح.",  
 imp:"أثر مثبت: الدليل المتداول يعرض رسمًا قديمًا.",  
 act:"حدّث الدليل، وراجع النص الأصلي للتعميم قبل الاعتماد.",  
 why:"التعميم صادر عن جهة مالية مختصة، ويذكر صراحة أنه يعدّل الرسم السابق.",  
 fx:[[1,"نص التعميم يصرّح بتعديل الرسم الوارد في الدليل"],[1,"التعميم أحدث من الدليل وصادر عن جهة الاختصاص"],[1,"الاختبار والفترة متطابقان في المصدرين"],[0,"التحقق البشري من النص الأصلي ما زال مطلوبًا"]],  
 ev:["دليل القبول 2026 · ص3","تعميم تحديث الرسوم · ص1"]},  
{id:4,cl:"poss",ti:"شرط شهادة اللغة",a:["مطلوبة","دليل القبول، ص7"],b:["غير مذكورة","الأسئلة الشائعة، ص2"],cf:70,  
 what:"الدليل يشترط شهادة لغة، والأسئلة الشائعة تعدّد الوثائق دون ذكرها.",  
 real:"قد يكون شرطًا ناقصًا لا تعارضًا: الصمت لا يعني الإلغاء.",  
 time:"الأسئلة الشائعة أحدث، لكنها لا تذكر إلغاءً صريحًا.",  
 imp:"أثر محتمل: قد يقدّم الطالب ملفًا ناقصًا.",  
 act:"أضف الشرط إلى قائمة الأسئلة الشائعة بعد تأكيده.",  
 why:"الشرط موجود في مصدر واحد فقط، والمصدر الآخر لا يتناوله بالنفي، فالدليل غير كافٍ للجزم.",  
 fx:[[1,"الدليل يذكر الشرط بنص صريح"],[0,"الأسئلة الشائعة قائمة وثائق مختصرة وليست قائمة شاملة"],[0,"لا يوجد نص ينفي الشرط أو يلغيه"]],  
 ev:["دليل القبول 2026 · ص7","الأسئلة الشائعة · ص2"]},  
{id:5,cl:"ok",ti:"موعد إعلان النتائج",a:["1 ديسمبر","دليل القبول، ص5"],b:["1 ديسمبر","الأسئلة الشائعة، ص3"],cf:100,  
 what:"لا اختلاف: التاريخ نفسه في المصدرين.",  
 real:"لا يوجد تعارض.",  
 time:"لم يتغير بين النسختين.",  
 imp:"لا أثر: يمكن الاعتماد عليه مع مراجعة روتينية.",  
 act:"لا إجراء مطلوب.",  
 why:"تاريخ متطابق نصًا في مصدرين صادرين عن الجهة نفسها، دون أي استثناء.",  
 fx:[[1,"التاريخ والصياغة متطابقان في المصدرين"],[1,"لا يوجد تعميم لاحق يعدّله"],[1,"المصدران من الجهة نفسها وللفترة نفسها"]],  
 ev:["دليل القبول 2026 · ص5","الأسئلة الشائعة · ص3"]}];  
const $=s=>document.querySelector(s),H=(el,h)=>el.innerHTML=h;  
const st={};F.forEach(f=>st[f.id]="جديد");  
let flt="all",done=false;  
const srcs=()=>H($("#srcs"),S.map(s=>`<div class="card src" style="--c:${s.c}"><div class="ico">${s.n[0]}</div><div><h3>${s.n}</h3><div class="meta">${s.k} · ${s.o}<br>نُشر ${s.d} · ${s.p} صفحة</div></div></div>`).join(""));  
srcs();  
document.querySelectorAll("nav button").forEach(b=>b.onclick=()=>show(b.dataset.t));  
function show(t){document.querySelectorAll(".panel").forEach(p=>p.classList.toggle("hid",p.id!==t));  
 document.querySelectorAll("nav button").forEach(b=>b.setAttribute("aria-selected",b.dataset.t===t));  
 if(t==="res")renderList();if(t==="rep")renderRep()}  
$("#up").onchange=e=>{const f=e.target.files[0];if(!f)return;S.push({n:f.name.replace(/\.pdf$/i,""),o:"ملف مرفوع",d:new Date().toISOString().slice(0,10),k:"مستند",p:"؟",c:"var(--x)"});srcs();  
 $("#steps").insertAdjacentHTML("beforeend",`<li class="on"><i>!</i>أُضيف الملف للقائمة، لكن العرض التجريبي يحلل البيانات التوضيحية فقط.</li>`)};  
$("#go").onclick=async()=>{const P=["جمع المصادر وتسجيل بياناتها","استخراج الشروط والتواريخ والأرقام","ربط العلاقات بين الادعاءات","كشف التعارضات","حساب الثقة وتوثيق أسبابها","إعداد التقرير بالأدلة"];  
 $("#go").disabled=true;H($("#steps"),P.map(l=>`<li><i></i>${l}</li>`).join(""));  
 for(const x of document.querySelectorAll("#steps li")){await new Promise(r=>setTimeout(r,matchMedia("(prefers-reduced-motion:reduce)").matches?0:450));x.classList.add("on");x.firstChild.textContent="✓"}  
 done=true;$("#go").disabled=false;show("res")};  
function chips(){const k=[["all","الكل"],...Object.entries(C).map(([a,b])=>[a,b[0]])];  
 H($("#chips"),k.map(([a,b])=>`<button class="chip" aria-pressed="${flt===a}" data-f="${a}">${b}</button>`).join(""));  
 document.querySelectorAll(".chip").forEach(c=>c.onclick=()=>{flt=c.dataset.f;renderList()})}  
const col={conf:"var(--red)",poss:"var(--x)",expl:"var(--b)",unr:"var(--vio)",ok:"var(--a)"};  
function renderList(){chips();  
 if(!done){H($("#list"),`<div class="card">لا توجد نتائج بعد. افتح «مساحة العمل» ثم اضغط «حلّل المصادر».</div>`);return}  
 H($("#list"),F.filter(f=>flt==="all"||f.cl===flt).map(f=>{const l=L(f.cf);return `<div class="card item" style="--k:${col[f.cl]}"><button class="row" style="all:unset;display:flex;width:100%;gap:12px;align-items:center;justify-content:space-between;cursor:pointer" data-i="${f.id}" aria-expanded="false"><span><span class="tag ${C[f.cl][1]}">${C[f.cl][0]}</span> <b>${f.ti}</b><br><span class="meta">${f.a[0]} ⟷ ${f.b[0]} · ${st[f.id]}</span></span><span class="ring" style="--p:${f.cf};--k:${l[1]}"><b>${f.cf}%</b></span></button><div class="d hid"></div></div>`}).join(""));  
 document.querySelectorAll(".item button").forEach(b=>b.onclick=()=>open(b))}  
function open(b){const f=F.find(x=>x.id==b.dataset.i),d=b.parentNode.querySelector(".d"),o=b.getAttribute("aria-expanded")==="true",l=L(f.cf);  
 b.setAttribute("aria-expanded",!o);d.classList.toggle("hid",o);if(o)return;  
 H(d,`<div class="cmp"><div class="q" style="--c:var(--a)"><small>المصدر الأول</small><b>${f.a[0]}</b><small>${f.a[1]}</small></div><div class="q" style="--c:var(--b)"><small>المصدر الثاني</small><b>${f.b[0]}</b><small>${f.b[1]}</small></div></div>  
 <div class="six"><div><b>ما الذي اختلف؟</b>${f.what}</div><div><b>أين ظهر الاختلاف؟</b>${f.a[1]}، و${f.b[1]}</div><div><b>هل هو تعارض حقيقي؟</b>${f.real}</div><div><b>هل تغيرت المعلومة مع الزمن؟</b>${f.time}</div><div><b>ما أثر الاختلاف؟</b>${f.imp}</div><div><b>ما الذي يمكن فعله؟</b>${f.act}</div></div>  
 <div class="why" style="--k:${l[1]}"><h4>درجة الثقة ${f.cf}% <span class="lvl">${l[0]}</span></h4><div class="bar"><span style="width:${f.cf}%"></span></div>  
 <b>السبب:</b> ${f.why}  
 <ul class="fx">${f.fx.map(x=>`<li><span class="${x[0]?"pl":"mi"}">${x[0]?"+":"−"}</span>${x[1]}</li>`).join("")}</ul>  
 <b>المصادر المعتمدة:</b><div class="ev" style="margin-top:6px">${f.ev.map(e=>`<span>${e}</span>`).join("")}</div></div>  
 <div style="margin-top:12px;display:flex;gap:6px;flex-wrap:wrap">${["قيد المراجعة","حُسم بتوضيح رسمي"].map(s=>`<button class="chip" data-s="${s}" aria-pressed="${st[f.id]===s}">${s}</button>`).join("")}</div>`);  
 d.querySelectorAll("[data-s]").forEach(c=>c.onclick=()=>{st[f.id]=c.dataset.s;renderList();document.querySelector(`[data-i="${f.id}"]`).click()})}  
function renderRep(){  
 if(!done){H($("#sum"),"");H($("#tbl"),"<tr><td>حلّل المصادر أولًا من مساحة العمل.</td></tr>");return}  
 H($("#sum"),Object.entries(C).map(([k,v])=>`<div class="card" style="--k:${col[k]}"><span class="tag ${v[1]}">${v[0]}</span><div class="stat">${F.filter(f=>f.cl===k).length}</div></div>`).join(""));  
 H($("#tbl"),`<tr><th>البند</th><th>التصنيف</th><th>الثقة وسببها</th><th>المصادر</th><th>المتابعة</th><th>الإجراء</th></tr>`+F.map(f=>`<tr><td>${f.ti}</td><td>${C[f.cl][0]}</td><td><b>${f.cf}% · ${L(f.cf)[0]}</b><br>${f.why}</td><td>${f.ev.join("<br>")}</td><td>${st[f.id]}</td><td>${f.act}</td></tr>`).join(""))}  
$("#copy").onclick=async()=>{const t="تقرير تقاطع (بيانات توضيحية)\n"+F.map(f=>`- ${f.ti}: ${C[f.cl][0]} | ثقة ${f.cf}% (${L(f.cf)[0]}) | السبب: ${f.why} | المصادر: ${f.ev.join("، ")} | ${f.act}`).join("\n");  
 try{await navigator.clipboard.writeText(t);$("#copy").textContent="تم النسخ"}catch(e){$("#copy").textContent="تعذّر النسخ"}};  
</script>  
</body>  
</html>  
