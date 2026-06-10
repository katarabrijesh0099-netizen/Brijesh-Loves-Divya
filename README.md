<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Love Reel 💖</title>

<link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Poppins:wght@300;600&display=swap" rel="stylesheet">

<style>
body{
margin:0;
overflow:hidden;
background:black;
color:white;
font-family:Poppins;
}

/* FULL VERTICAL REEL */
.container{
position:relative;
width:100vw;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
text-align:center;
}

/* DARK CINEMA OVERLAY */
.overlay{
position:absolute;
width:100%;
height:100%;
background: radial-gradient(circle at center, rgba(255,0,100,0.25), black 70%);
animation: glow 3s infinite alternate;
}

@keyframes glow{
from{filter:brightness(1);}
to{filter:brightness(1.5);}
}

/* INTRO TEXT */
h1{
font-family:'Great Vibes', cursive;
font-size:48px;
color:#ff4d6d;
text-shadow:0 0 20px #ff4d6d;
}

p{
font-size:16px;
opacity:0.85;
}

/* IMAGE */
img{
max-width:85%;
max-height:70%;
border-radius:20px;
box-shadow:0 0 40px rgba(255,0,100,0.6);
animation:zoom 3s ease-in-out;
}

@keyframes zoom{
0%{transform:scale(1.2);opacity:0;}
100%{transform:scale(1);opacity:1;}
}

/* HEARTS */
.heart{
position:absolute;
color:#ff4d6d;
font-size:18px;
animation: float 5s linear infinite;
}

@keyframes float{
from{transform:translateY(100vh);}
to{transform:translateY(-10vh);}
}

/* PETALS */
.petal{
position:absolute;
font-size:18px;
animation: fall 6s linear infinite;
opacity:0.7;
}

@keyframes fall{
from{transform:translateY(-10vh) rotate(0deg);}
to{transform:translateY(110vh) rotate(360deg);}
}

/* END INFINITY */
.infinity{
font-size:80px;
color:#00ffe5;
text-shadow:0 0 30px #00ffe5;
animation:pulse 1.5s infinite;
}

@keyframes pulse{
0%{transform:scale(1);}
50%{transform:scale(1.2);}
100%{transform:scale(1);}
}

/* SCREENS */
.screen{
position:absolute;
width:100%;
height:100%;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
opacity:0;
animation:fade 1.5s forwards;
}

@keyframes fade{to{opacity:1;}}
</style>
</head>

<body>

<audio id="song" loop>
<source src="song.mp3">
</audio>

<!-- INTRO -->
<div id="intro" class="screen">
<div class="container">
<div class="overlay"></div>
<h1>💖 OUR LOVE STORY 💖</h1>
<p>“A cinematic reel of forever…”</p>
</div>
</div>

<!-- SLIDES -->
<div id="slide" class="screen" style="display:none;">
<img id="img">
<p id="cap"></p>
</div>

<!-- END -->
<div id="end" class="screen" style="display:none;">
<h1>💞 Forever & Infinity 💞</h1>
<p>
Tum meri duniya ho ❤️<br>
Tum meri rooh ho ♾️
</p>
<div class="infinity">∞ 💖 ∞</div>
</div>

<script>

let photos=["1.jpg","2.jpg","3.jpg","4.jpg"];
let captions=[
"First moment ❤️",
"Endless memories 💕",
"My soulmate 💍",
"Forever & always ♾️"
];

let i=0;

/* petals */
for(let p=0;p<25;p++){
let d=document.createElement("div");
d.className="petal";
d.innerHTML="🌹";
d.style.left=Math.random()*100+"vw";
d.style.animationDuration=(4+Math.random()*3)+"s";
document.body.appendChild(d);
}

/* hearts */
setInterval(()=>{
let h=document.createElement("div");
h.className="heart";
h.innerHTML="❤";
h.style.left=Math.random()*100+"vw";
document.body.appendChild(h);
setTimeout(()=>h.remove(),5000);
},200);

/* flow */
setTimeout(()=>{
document.getElementById("intro").style.display="none";
document.getElementById("slide").style.display="flex";
document.getElementById("song").play();

let s=setInterval(()=>{
document.getElementById("img").src=photos[i];
document.getElementById("cap").innerText=captions[i];
i++;

if(i===photos.length){
clearInterval(s);
document.getElementById("slide").style.display="none";
document.getElementById("end").style.display="flex";
}
},2500);

},4000);

</script>

</body>
</html><img width="736" height="1308" alt="1000158117" src="https://github.com/user-attachments/assets/55c6e13b-b103-41a5-90c0-e45ae8dd651d" />

