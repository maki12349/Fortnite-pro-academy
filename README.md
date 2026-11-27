# Fortnite-pro-academy
Learn how to play like a pro in fortnite

<!DOCTYPE html>
<html lang="en">
<head><!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Fortnite Pro Academy</title>
<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #101426;
  color: white;
  text-align: center;
}
header {
  background: #713cff;
  padding: 25px;
}
h1 { font-size: 32px; }
section { padding: 20px; }
.lesson {
  background: #202a46;
  padding: 20px;
  margin: 15px auto;
  max-width: 500px;
  border-radius: 15px;
}
button {
  background: #ffb800;
  border: none;
  padding: 12px 22px;
  border-radius: 8px;
  font-weight: bold;
  cursor: pointer;
}
#target {
  width: 65px;
  height: 65px;
  border-radius: 50%;
  background: red;
  position: relative;
  margin: 20px auto;
  cursor: pointer;
}
</style>
</head>
<body>

<header>
<h1>🎮 FORTNITE PRO ACADEMY</h1>
<p>Train Like a Pro. Become a Champion.</p>
</header>

<section>
<h2>🔥 Choose Your Training</h2>

<div class="lesson">
<h3>🎯 Aim Training</h3>
<p>Click the target as fast as possible!</p>
<button onclick="startAim()">Start Aim Training</button>
<p id="score">Score: 0</p>
<div id="target" onclick="hitTarget()"></div>
</div>

<div class="lesson">
<h3>🏗️ Building Skills</h3>
<p>Learn the basic Fortnite builds:</p>
<p>Wall • Ramp • Floor • Cone</p>
<button onclick="alert('Practice building walls, ramps and 90s!')">
Learn Building
</button>
</div>

<div class="lesson">
<h3>⚡ Editing Skills</h3>
<p>Learn how to edit walls, floors and ramps.</p>
<button onclick="alert('Practice wall edits and reset edits!')">
Learn Editing
</button>
</div>

<div class="lesson">
<h3>🧠 Pro Tips</h3>
<p>1. Always keep moving.</p>
<p>2. Learn to aim before shooting.</p>
<p>3. Build to protect yourself.</p>
<p>4. Practice every day.</p>
</div>
</section>

<script>
let score = 0;
let playing = false;

function startAim() {
  score = 0;
  playing = true;
  document.getElementById("score").innerText = "Score: 0";
  moveTarget();
}

function hitTarget() {
  if (!playing) return;
  score++;
  document.getElementById("score").innerText =
    "Score: " + score;
  moveTarget();
}

function moveTarget() {
  let target = document.getElementById("target");
  target.style.left = (Math.random() * 100 - 50) + "px";
  target.style.top = (Math.random() * 100 - 50) + "px";
}
</script>

</body>
</html>


  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fortnite Pro Academy</title>
  <style>
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #100d20;
      color: white;
    }
    header {
      background: #21163e;
      padding: 20px;
      text-align: center;
      border-bottom: 3px solid #a855f7;
    }
    header h1 { color: #d8a4ff; margin: 0; }
    nav { margin-top: 15px; }
    nav a {
      color: white;
      margin: 8px;
      text-decoration: none;
    }
    .hero {
      padding: 65px 20px;
      text-align: center;
      background: linear-gradient(135deg,#5124a8,#17112d);
    }
    .hero h2 { font-size: 38px; }
    .hero p { font-size: 18px; }
    .button {
      display: inline-block;
      background: #a855f7;
      color: white;
      padding: 13px 24px;
      border-radius: 10px;
      text-decoration: none;
      font-weight: bold;
      margin-top: 12px;
    }
    main { max-width: 1000px; margin: auto; padding: 25px; }
    h2 { color: #d8a4ff; }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
      gap: 18px;
    }
    .card {
      background: #211a37;
      padding: 22px;
      border-radius: 15px;
      border: 1px solid #7140a5;
    }
    .card h3 { color: #d8a4ff; }
    .lesson {
      background: #211a37;
      padding: 16px;
      border-radius: 10px;
      margin: 12px 0;
    }
    footer {
      text-align: center;
      padding: 25px;
      color: #b9a9ce;
    }
  </style>
</head>
<body>
  <header>
    <h1>🎮 FORTNITE PRO ACADEMY</h1>
    <nav>
      <a href="#training">Training</a>
      <a href="#lessons">Lessons</a>
      <a href="#tips">Pro Tips</a>
    </nav>
  </header>

  <section class="hero">
    <h2>Become a Fortnite Pro!</h2>
    <p>Train your aim, master your builds and dominate every match.</p>
    <a class="button" href="#training">START TRAINING</a>
  </section>

  <main>
    <section id="training">
      <h2>🔥 Your Training Academy</h2>
      <div class="cards">
        <div class="card">
          <h3>🎯 Aim Training</h3>
          <p>Improve your accuracy and learn to hit your shots.</p>
        </div>
        <div class="card">
          <h3>🏗️ Building</h3>
          <p>Practice walls, ramps, edits and fast building.</p>
        </div>
        <div class="card">
          <h3>⚡ Editing</h3>
          <p>Learn quick edits and surprise your opponents.</p>
        </div>
        <div class="card">
          <h3>🧠 Game Sense</h3>
          <p>Learn positioning, rotations and smart decisions.</p>
        </div>
      </div>
    </section>

    <section id="lessons">
      <h2>📚 Pro Lessons</h2>
      <div class="lesson">Lesson 1 — Practice your aim every day.</div>
      <div class="lesson">Lesson 2 — Learn to build protective walls.</div>
      <div class="lesson">Lesson 3 — Master editing and movement.</div>
      <div class="lesson">Lesson 4 — Choose smart fights and rotations.</div>
    </section>

    <section id="tips">
      <h2>💡 Pro Tips</h2>
      <div class="card">
        <p>✅ Keep your crosshair at enemy height.</p>
        <p>✅ Use headphones to hear footsteps.</p>
        <p>✅ Practice in Creative mode.</p>
        <p>✅ Learn from every match.</p>
        <p>✅ Have fun and keep improving!</p>
      </div>
    </section>
  </main>

  <footer>
    <p>Fortnite Pro Academy — Train. Improve. Win!</p>
    <p>Fan-made learning website. Not affiliated with Epic Games.</p>
  </footer>
</body>
</html>
!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Fortnite Pro Academy</title>
<style>
body{background:#101426;color:white;font-family:Arial;text-align:center;margin:0}
header{background:#713cff;padding:20px}
.card{background:#202d4c;margin:15px;padding:20px;border-radius:15px}
button{background:#ffbd00;border:0;padding:13px;margin:6px;border-radius:9px;font-weight:bold}
#arena{height:300px;background:#080d19;position:relative;overflow:hidden}
.target{position:absolute;background:red;width:50px;height:50px;border-radius:50%}
.hidden{display:none}
#buildarea{height:280px;background:#18243a;display:grid;grid-template-columns:repeat(3,1fr);gap:5px;padding:5px}
.block{background:#3c75c9;border:2px solid white;display:grid;place-items:center;font-size:25px}
</style>
</head>
<body>
<header>
<h1>🎮 FORTNITE PRO ACADEMY</h1>
<p>XP: <span id="xp">0</span> ⭐</p>
</header>

<div id="home">
<div class="card">
<h2>🎯 AIM TRAINER</h2>
<p>Train your aim and hit the targets!</p>
<button onclick="show('aim')">PLAY NOW</button>
</div>
<div class="card">
<h2>🏗️ BUILDING SIMULATOR</h2>
<p>Learn to build your structures!</p>
<button onclick="show('build')">PLAY NOW</button>
</div>
<div class="card">
<h2>⚡ EDITING CHALLENGE</h2>
<p>Practice selecting tiles to make edits.</p>
<button onclick="show('edit')">PLAY NOW</button>
</div>
</div>

<div id="aim" class="hidden card">
<h2>🎯 AIM TRAINER</h2>
<p>Score: <span id="score">0</span></p>
<p>Time: <span id="time">30</span></p>
<div id="arena"></div>
<button onclick="startAim()">START</button>
<button onclick="show('home')">BACK</button>
</div>

<div id="build" class="hidden card">
<h2>🏗️ BUILDING SIMULATOR</h2>
<p>Choose a structure to place!</p>
<div id="buildarea">
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
<div class="block" onclick="place(this)">+</div>
</div>
<button onclick="choose('🧱 WALL')">WALL</button>
<button onclick="choose('⬆️ RAMP')">RAMP</button>
<button onclick="choose('🟦 FLOOR')">FLOOR</button>
<button onclick="choose('🔺 CONE')">CONE</button>
<p id="message">Choose a structure, then tap a square!</p>
<button onclick="show('home')">BACK</button>
</div>

<div id="edit" class="hidden card">
<h2>⚡ EDITING CHALLENGE</h2>
<p>Tap the highlighted tiles to complete a window edit!</p>
<div id="tiles" style="display:grid;grid-template-columns:repeat(3,1fr);gap:5px"></div>
<p id="editmsg">Select the middle tile!</p>
<button onclick="resetEdit()">TRY AGAIN</button>
<button onclick="show('home')">BACK</button>
</div>

<script>
let xp=0,score=0,time=30,active=false;
let timer,chosen="🧱 WALL";
function show(id){
 document.querySelectorAll("#home,#aim,#build,#edit").forEach(x=>x.classList.add("hidden"));
 document.getElementById(id).classList.remove("hidden");
 active=false;clearInterval(timer);
}
function addXP(n){
 xp+=n;document.getElementById("xp").textContent=xp;
}
function startAim(){
 clearInterval(timer);
 score=0;time=30;active=true;
 document.getElementById("score").textContent=0;
 document.getElementById("time").textContent=30;
 target();
 timer=setInterval(()=>{
 time--;
 document.getElementById("time").textContent=time;
 if(time<=0){
 active=false;clearInterval(timer);
 document.getElementById("arena").innerHTML="GAME OVER!";
 addXP(score*5);
 alert("Great job! You earned "+score*5+" XP!");
 }
 },1000);
}
function target(){
 if(!active)return;
 let a=document.getElementById("arena");
 a.innerHTML="";
 let t=document.createElement("button");
 t.className="target";
 t.style.left=Math.random()*(a.clientWidth-50)+"px";
 t.style.top=Math.random()*(a.clientHeight-50)+"px";
 t.onclick=()=>{
 if(!active)return;
 score++;
 document.getElementById("score").textContent=score;
 target();
 };
 a.appendChild(t);
}
function choose(x){
 chosen=x;
 document.getElementById("message").textContent="Selected "+x+". Now tap a square!";
}
let built=0;
function place(el){
 if(el.textContent!=="+")return;
 el.textContent=chosen;
 built++;
 document.getElementById("message").textContent="Structures placed: "+built;
 if(built===9){
 addXP(50);
 alert("Great building! +50 XP");
 }
}
function resetEdit(){
 let tiles=document.getElementById("tiles");
 tiles.innerHTML="";
 for(let i=0;i<9;i++){
 let b=document.createElement("button");
 b.textContent="⬜";
 b.style.height="75px";
 b.onclick=()=>{
 if(i===4){
 b.textContent="🟦";
 document.getElementById("editmsg").textContent="Perfect edit! +25 XP";
 addXP(25);
 }else{
 document.getElementById("editmsg").textContent="Try the middle tile!";
 }
 };
 tiles.appendChild(b);
 }
}
resetEdit();
</script>
</body>
</html>
