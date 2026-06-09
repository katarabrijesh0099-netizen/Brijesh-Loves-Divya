<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Brijesh ❤️ Divya</title>

<style>
body{
margin:0;
overflow:hidden;
background:linear-gradient(135deg,#ffdde1,#ee9ca7);
font-family:cursive;
text-align:center;
color:white;
}

h1{
font-size:45px;
margin-top:20px;
text-shadow:0 0 20px white;
}

p{
font-size:20px;
}

.slider{
width:320px;
height:420px;
margin:auto;
position:relative;
overflow:hidden;
border-radius:25px;
box-shadow:0 0 30px white;
}

.slider img{
position:absolute;
width:100%;
height:100%;
object-fit:cover;
opacity:0;
animation:fade 18s infinite;
}

.slider img:nth-child(1){animation-delay:0s;}
.slider img:nth-child(2){animation-delay:3s;}
.slider img:nth-child(3){animation-delay:6s;}
.slider img:nth-child(4){animation-delay:9s;}
.slider img:nth-child(5){animation-delay:12s;}
.slider img:nth-child(6){animation-delay:15s;}

@keyframes fade{
0%{opacity:0;}
10%{opacity:1;}
20%{opacity:1;}
30%{opacity:0;}
100%{opacity:0;}
}

.heart{
position:absolute;
color:white;
animation:float linear infinite;
}

@keyframes float{
0%{transform:translateY(100vh);opacity:0;}
100%{transform:translateY(-100px);opacity:1;}
}

.music{
display:none;
}
</style>
</head>

<body>

<audio class="music" autoplay loop>
<source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mp3">
</audio>

<h1>💖 Brijesh ❤️ Divya 💖</h1>
<p>11 June 🌹</p>

<div class="slider">
<img src="file_00000000acd87209b662616f8f114c53">
<img src="file_000000007c107207bab493f27d76526e">
<img src="file_0000000034a47207ac4ee65dfe4d7301">
<img src="file_000000005e98720992f7cda01bc57806">
<img src="file_0000000008707209a2ab71a8f72dff40">
<img src="file_0000000034ec7207a7300fb2096aefbb">
</div>

<p>YOU ARE MY EVERYTHING ❤️🧿🌏</p>
<p>Bacccchuuuh 💗🫶🏼</p>

<script>
for(let i=0;i<60;i++){
let h=document.createElement("div");
h.innerHTML="❤";
h.className="heart";
h.style.left=Math.random()*100+"%";
h.style.fontSize=(10+Math.random()*25)+"px";
h.style.animationDuration=(4+Math.random()*6)+"s";
document.body.appendChild(h);
}
</script>

</body>
</html>
