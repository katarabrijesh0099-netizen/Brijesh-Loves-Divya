<img width="899" height="1599" alt="84eb5af1-af18-4366-9f8e-09b30d5b5913-1_all_22347" src="https://github.com/user-attachments/assets/db814b64-d55b-47fa-93ed-d86c94731d9a" />
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Brijesh ❤️ Divya</title>

<style>
body{
margin:0;
overflow:hidden;
font-family:cursive;
background:linear-gradient(135deg,#ffdde1,#ee9ca7);
color:white;
text-align:center;
}

h1{
font-size:45px;
margin-top:15px;
text-shadow:0 0 20px white;
}

.slider{
width:100%;
height:70vh;
position:relative;
overflow:hidden;
margin-top:10px;
}

.slider img{
width:100%;
height:100%;
object-fit:cover;
position:absolute;
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
animation:float 6s linear infinite;
}

@keyframes float{
0%{transform:translateY(100vh);opacity:0;}
100%{transform:translateY(-100px);opacity:1;}
}

.msg{
font-size:20px;
margin:10px;
}

button{
padding:10px 20px;
border:none;
border-radius:20px;
background:white;
color:black;
font-weight:bold;
cursor:pointer;
}
</style>
</head>

<body>

<h1>💖 Brijesh ❤️ Divya 💖</h1>
<p>11 June 🌹</p>

<div class="slider">
<img src="photo1.jpg">
<img src="photo2.jpg">
<img src="photo3.jpg">
<img src="photo4.jpg">
<img src="photo5.jpg">
<img src="photo6.jpg">
</div>

<p class="msg">YOU ARE MY EVERYTHING ❤️🧿🌏</p>
<p class="msg">Bacccchuuuh 💗🫶🏼</p>

<button onclick="alert('💖 I LOVE YOU FOREVER 💖')">
Open Surprise 💌
</button>

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
