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
