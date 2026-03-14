# my-suprise-box
my suprise box
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Haziya</title>

<style>

body{
margin:0;
font-family: 'Poppins', sans-serif;
background: linear-gradient(135deg,#ff9a9e,#fad0c4,#fad0c4,#fbc2eb);
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
color:white;
overflow:hidden;
}

.card{
background:rgba(255,255,255,0.15);
padding:30px;
border-radius:20px;
width:90%;
max-width:400px;
backdrop-filter: blur(10px);
animation: muncul 2s ease;
}

img{
width:160px;
border-radius:20px;
margin-bottom:15px;
box-shadow:0 10px 25px rgba(0,0,0,0.3);
}

h1{
font-size:26px;
margin-bottom:10px;
}

p{
font-size:14px;
line-height:1.6;
}

button{
margin-top:15px;
padding:10px 25px;
border:none;
border-radius:25px;
background:white;
color:#ff4b7d;
font-weight:bold;
cursor:pointer;
}

button:hover{
transform:scale(1.1);
}

@keyframes muncul{
from{
opacity:0;
transform:translateY(30px);
}
to{
opacity:1;
transform:translateY(0);
}
}

/* animasi hati */

.heart{
position:absolute;
color:#ff4b7d;
animation: naik 6s linear infinite;
}

@keyframes naik{
0%{
transform:translateY(100vh);
opacity:0;
}
100%{
transform:translateY(-10vh);
opacity:1;
}
}

</style>
</head>

<body>

<div class="card">

<img src="haziya.jpg">

<h1>🎉 Happy Birthday 🎂</h1>
<h2>Haziya Raihana Cantika</h2>

<p>

Happy birthday ya Haziya Raihana Cantika 🤍  

perasaan kita baru aja ketemu kok kamu udah ultah aja sih hihihi🥹  

semoga kamu panjang umur sehat selalu dan impianmu terwujud semua, AAMIN.  

bahagia terus ya, jangan suka marah-marah dan cemberut nanti cantiknya kurang lohh 😼  

oiya kamu jangan suka insecure ya, soalnya kamu cantik banget  
(MAA SYAA ALLAH TABARAKALLAH) 😽  

kamu juga gabole dengerin ucapan orang orang yang ga suka sama kamu.  

tetap fokus sama tujuanmu ya.  

jangan lupa kamu harus berbakti sama orang tua dan belajar yang rajin 🤍  

aku juga mau minta maaf kalau sering offline tiba tiba pas kita lagi chatan.  

maaf ya aku ga ngasih kado 🤪  

dan maaf juga ngucapinnya terlambat hihihi 😸  

</p>

<button onclick="surprise()">Klik Surprise 🎁</button>

</div>

<script>

function surprise(){
alert("Semoga hari kamu selalu penuh kebahagiaan 🎉");
}

function hearts(){
const heart = document.createElement("div");
heart.className="heart";
heart.innerHTML="❤";
heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=Math.random()*20+20+"px";
document.body.appendChild(heart);

setTimeout(()=>{
heart.remove();
},6000)
}

setInterval(hearts,500);

</script>

</body>
</html>
