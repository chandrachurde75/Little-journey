<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Our Little Universe ❤️</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:Arial,sans-serif;min-height:100vh;color:#fff;background:radial-gradient(circle at 15% 15%,#5b164f 0,transparent 30%),radial-gradient(circle at 85% 20%,#30205e 0,transparent 30%),linear-gradient(135deg,#0b0615,#1d0c30,#090615);overflow-x:hidden}
nav{position:sticky;top:0;z-index:10;padding:12px;background:#0b0615dd;backdrop-filter:blur(15px);border-bottom:1px solid #ffffff22}
.nav{max-width:900px;margin:auto;display:flex;gap:12px;align-items:center;justify-content:space-between}.logo{font-weight:800}
select{padding:11px 14px;border-radius:14px;background:#ffffff18;color:#fff;border:1px solid #ffffff30;font-weight:700}option{color:#111}
.page{display:none;min-height:calc(100vh - 65px);padding:35px 16px;align-items:center;justify-content:center}.page.active{display:flex;animation:in .55s ease}
@keyframes in{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:none}}
.card{max-width:820px;width:100%;padding:38px 22px;text-align:center;border-radius:30px;background:#ffffff10;border:1px solid #ffffff20;box-shadow:0 25px 70px #0008;backdrop-filter:blur(18px)}
h1{font-size:clamp(40px,10vw,72px);margin:15px 0}h2{font-size:clamp(30px,7vw,48px);margin:12px 0 22px}h3{margin-bottom:7px}p{line-height:1.8;font-size:17px;color:#ffffffdd}
.gradient{background:linear-gradient(90deg,#fff,#ffadd8,#c9b6ff,#fff);background-size:250%;-webkit-background-clip:text;color:transparent;animation:shine 5s linear infinite}
@keyframes shine{to{background-position:250%}}
.big{font-size:100px;display:inline-block;animation:pulse 1.25s infinite;filter:drop-shadow(0 0 25px #ff69b4)}
@keyframes pulse{50%{transform:scale(1.13)}}
.btn{border:0;border-radius:50px;padding:14px 22px;margin:7px;background:linear-gradient(135deg,#fff,#ffd1e6);color:#28102f;font-weight:800;font-size:15px}
.story{text-align:left;margin:25px 0}.item,.loveitem,.memory,.answer{padding:18px;margin:11px 0;border-radius:18px;background:#ffffff0d;border:1px solid #ffffff12}
.loveitem{transition:.2s}.loveitem:hover{transform:translateY(-3px)}
.options{display:grid;gap:11px;text-align:left}.option{padding:17px;border-radius:17px;background:#ffffff0d;border:1px solid #ffffff18;cursor:pointer}.option.selected{background:#ff6eaf33;border-color:#ffacd4}.check{float:right;opacity:0}.selected .check{opacity:1}
.progress{height:7px;background:#ffffff18;border-radius:20px;margin:15px 0 25px}.bar{height:100%;width:10%;background:linear-gradient(90deg,#ff6eaf,#c5a7ff);border-radius:20px}
.memorygrid{display:grid;grid-template-columns:1fr 1fr;gap:12px}.memory{margin:0}.icon{font-size:38px}
input{padding:14px;border:0;border-radius:14px;text-align:center;font-size:17px;outline:0;max-width:260px;width:100%;margin:18px auto}
#hearts{position:fixed;inset:0;pointer-events:none;overflow:hidden;z-index:1}.heart{position:absolute;bottom:-40px;animation:float 9s linear infinite;opacity:0}
@keyframes float{15%{opacity:.7}100%{transform:translateY(-110vh) rotate(360deg);opacity:0}}
.content{position:relative;z-index:2}
@media(max-width:650px){.nav{flex-direction:column}.nav select{width:100%}.card{padding:30px 16px}}
</style>
</head>
<body>
<div id="hearts"></div>
<nav><div class="nav"><div class="logo">💗 Our Little Universe</div>
<select id="nav" onchange="go(this.value)">
<option value="home">✨ Welcome</option><option value="story">🌸 Our Story</option><option value="message">💌 A Little Message</option><option value="love">❤️ How Much I Love You</option><option value="questions">💖 Love Questions</option><option value="little">🌷 Little Things</option><option value="vault">🔐 Answer Vault</option><option value="final">🎁 Final Surprise</option>
</select></div></nav>

<div class="content">
<section id="home" class="page active"><div class="card"><div class="big">💗</div><p>A tiny universe made especially for you</p><h1>Our<br><span class="gradient">Little World</span></h1><p>Sometimes normal messages aren't enough, so I made a little place where some feelings can live. ✨</p><button class="btn" onclick="go('story')">Begin the Journey 🌸</button></div></section>

<section id="story" class="page"><div class="card"><div class="big">🌸</div><h2>Our Little Story</h2><p>Every story has a beginning. Ours is made from conversations, little moments and memories.</p><div class="story">
<div class="item"><h3>🌱 The Beginning</h3><p>Two people started talking without knowing how meaningful those conversations could become.</p></div>
<div class="item"><h3>💬 The Conversations</h3><p>Random messages slowly became conversations that felt special.</p></div>
<div class="item"><h3>🌙 The Little Moments</h3><p>Funny moments, meaningful moments and quiet moments.</p></div>
<div class="item"><h3>❤️ Today</h3><p>And here we are, still making memories.</p></div></div>
<button class="btn" onclick="go('message')">Continue 💌</button></div></section>

<section id="message" class="page"><div class="card"><div class="big">💌</div><h2>A Little Message</h2><p style="font-size:24px;font-weight:700">Some people become special without even trying.</p><br><p>It's in the little things. A random message. A silly conversation. A laugh. Someone asking how your day was.</p><br><p>Those little things can make someone feel incredibly special.</p><button class="btn" onclick="go('love')">There's Something Else ❤️</button></div></section>

<section id="love" class="page"><div class="card"><div class="big">❤️</div><p>If you ever wondered...</p><h1 class="gradient">I Love You<br>More Than Words Can Say</h1>
<p>I don't think there is one perfect sentence that can explain how much someone can mean to another person.</p><div style="margin:22px auto;max-width:620px">
<div class="loveitem">💗 I love the little moments we share.</div><div class="loveitem">🌸 I love the conversations that make me smile.</div><div class="loveitem">✨ I love the memories we create.</div><div class="loveitem">🌙 I love having someone who feels special to me.</div><div class="loveitem">❤️ And most importantly, I care about you deeply.</div></div>
<p>No fancy explanation. No complicated words. Just one simple feeling:</p><h2 class="gradient">I love you. ❤️</h2><button class="btn" onclick="go('questions')">Answer My Questions 💖</button></div></section>

<section id="questions" class="page"><div class="card"><div id="qn">Question 1 of 10</div><div class="progress"><div class="bar" id="bar"></div></div><h2 id="qt" style="font-size:24px"></h2><div class="options" id="opts"></div><p id="saved" style="margin:15px 0;min-height:25px"></p><button class="btn" onclick="prev()">← Back</button><button class="btn" onclick="next()">Next →</button></div></section>

<section id="little" class="page"><div class="card"><div class="big">🌷</div><h2>Little Things</h2><p>Sometimes the smallest things become the biggest memories.</p><div class="memorygrid" style="margin-top:25px">
<div class="memory"><div class="icon">💬</div><h3>Conversations</h3><p>Even the random ones.</p></div><div class="memory"><div class="icon">😂</div><h3>Laughter</h3><p>The moments that make us smile.</p></div><div class="memory"><div class="icon">🌙</div><h3>Late Talks</h3><p>When time disappears.</p></div><div class="memory"><div class="icon">❤️</div><h3>Little Care</h3><p>Small things that matter.</p></div></div><button class="btn" onclick="go('vault')">See Answer Vault 🔐</button></div></section>

<section id="vault" class="page"><div class="card"><div class="big">🔐</div><h2>Answer Vault</h2><p>Enter the private PIN to see the answers chosen during this visit.</p><input id="pin" type="password" placeholder="Enter PIN"><button class="btn" onclick="unlock()">Unlock 🔓</button><p id="pinmsg"></p><div id="answers"></div></div></section>

<section id="final" class="page"><div class="card"><div class="big">💖</div><p>And finally...</p><h1>Thank You</h1><p>Thank you for every conversation, every laugh, every little moment and every memory still waiting to be created.</p><br><h2 class="gradient">Keep Smiling. 🌸</h2><p>Made with code, creativity and a lot of care. ❤️</p></div></section>
</div>

<script>
const qs=[
["What kind of moment with me would make you happiest?",["A long conversation 💬","A peaceful walk 🌸","Laughing together 😂","Just spending time together ❤️"]],
["Which word describes our connection best?",["Comfort 🌷","Fun 😂","Understanding 💕","Something special ✨"]],
["If we had a whole day together, what would you choose?",["Movie and snacks 🍿","Explore somewhere new 🌍","Talk for hours 💬","Just relax together 🥰"]],
["What makes a conversation really special?",["Feeling comfortable 💗","Laughing a lot 😂","Deep talks 🌙","Feeling understood 🤝"]],
["What can instantly make you smile?",["A sweet message 💌","A funny joke 😂","A surprise ✨","Someone remembering little details 🌸"]],
["Which kind of memory would you love to make?",["A funny memory 😂","A peaceful memory 🌙","An adventurous memory 🌍","A meaningful memory ❤️"]],
["What matters most between two people?",["Trust 🤝","Communication 💬","Understanding 💕","Making each other happy 🌸"]],
["What's your favourite kind of evening?",["Movie night 🎬","Long conversations 🌙","Going somewhere ✨","Quiet time together ❤️"]],
["If you could choose one little surprise, what would you pick?",["A sweet message 💌","A handwritten note 📝","A cute little gift 🎁","A surprise day out 🌸"]],
["What would you choose for our next little adventure?",["Discover a new place 🌍","Food adventure 🍕","Movie day 🎬","Just spend time together ❤️"]]
];
let i=0, answers={};

function showQ(){
 const q=qs[i]; qn.textContent=`Question ${i+1} of ${qs.length}`; qt.textContent=q[0]; bar.style.width=((i+1)*10)+"%"; opts.innerHTML="";
 q[1].forEach(a=>{
  const d=document.createElement("div"); d.className="option"+(answers[i]===a?" selected":""); d.innerHTML=`<span>${a}</span><span class="check">✓</span>`;
  d.onclick=()=>{answers[i]=a;document.querySelectorAll(".option").forEach(x=>x.classList.remove("selected"));d.classList.add("selected");saved.textContent="💗 Answer saved for this visit.";};opts.appendChild(d);
 });
 saved.textContent=answers[i]?"💗 Your answer is selected.":"";
}
function next(){if(i<qs.length-1){i++;showQ()}else go("little")}
function prev(){if(i>0){i--;showQ()}}
function go(id){document.querySelectorAll(".page").forEach(x=>x.classList.remove("active"));document.getElementById(id).classList.add("active");nav.value=id;scrollTo(0,0);if(id==="questions")showQ()}
const PIN="1432";
function unlock(){
 if(pin.value!==PIN){pinmsg.textContent="❌ Incorrect PIN.";pinmsg.style.color="#ffb6d5";answersDiv("");return}
 pinmsg.textContent="🔓 Vault unlocked.";pinmsg.style.color="#caffea";answersDiv();
}
function answersDiv(){
 const box=document.getElementById("answers");box.innerHTML="";
 let found=false;
 qs.forEach((q,n)=>{if(answers[n]){found=true;const d=document.createElement("div");d.className="answer";d.innerHTML=`<b>Question ${n+1}:</b><br>${q[0]}<br><br>💗 <b>Selected answer:</b><br>${answers[n]}`;box.appendChild(d)}});
 if(!found)box.innerHTML='<div class="answer">No answers have been selected yet. 🌸</div>';
}
for(let n=0;n<45;n++){let h=document.createElement("div");h.className="heart";h.textContent=["❤️","💗","💕","💖","🌸","✨"][Math.floor(Math.random()*6)];h.style.left=Math.random()*100+"%";h.style.fontSize=14+Math.random()*20+"px";h.style.animationDelay=Math.random()*9+"s";document.getElementById("hearts").appendChild(h)}
showQ();
</script>
</body>
</html>
