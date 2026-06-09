<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Brijesh ❤️ Divya</title>

<style>
body{
margin:0;
height:100vh;
overflow:hidden;
background:linear-gradient(135deg,#ffdde1,#ee9ca7);
display:flex;
justify-content:center;
align-items:center;
font-family:cursive;
color:white;
text-align:center;
}

.container{
animation:fade 2s;
z-index:2;
}

h1{font-size:55px;}
p{font-size:22px;}

.heart{
position:absolute;
color:white;
animation:float linear infinite;
}

@keyframes float{
0%{transform:translateY(100vh);opacity:0;}
100%{transform:translateY(-100px);opacity:1;}
}

@keyframes fade{
from{opacity:0;}
to{opacity:1;}
}
</style>
</head>

<body>

<div class="container">
<h1>Brijesh ❤️ Divya</h1>
<h2>11 June 🌹</h2>

<p>YOU ARE MY EVERYTHING ❤️🧿🌏</p>
<p>Bacccchuuuh 💗🫶🏼</p>
<h3>Happy Anniversary ❤️</h3>
</div>

<script>
for(let i=0;i<60;i++){
let h=document.createElement("div");
h.innerHTML="❤";
h.className="heart";
h.style.left=Math.random()*100+"%";
h.style.fontSize=(12+Math.random()*25)+"px";
h.style.animationDuration=(4+Math.random()*6)+"s";
document.body.appendChild(h);
}
</script>

</body>
</html>
