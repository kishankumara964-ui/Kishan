<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Happy Birthday My Love ❤️</title>

<style>
body{
margin:0;
font-family:Arial;
background:linear-gradient(135deg,#ff9ecf,#ffd1dc);
display:flex;
justify-content:center;
align-items:center;
height:100vh;
overflow:hidden;
text-align:center;
}

.box{
background:white;
padding:40px;
border-radius:20px;
box-shadow:0 0 20px rgba(0,0,0,.2);
width:80%;
max-width:500px;
}

button{
padding:12px 25px;
margin:10px;
font-size:18px;
border:none;
border-radius:10px;
cursor:pointer;
background:#ff4081;
color:white;
}

#celebration{
display:none;
}

.balloon{
position:absolute;
bottom:-150px;
font-size:50px;
animation:float 8s linear infinite;
}

@keyframes float{
0%{transform:translateY(0);}
100%{transform:translateY(-120vh);}
}

h1{
color:#ff0066;
}

.hearts{
font-size:30px;
animation:pulse 1s infinite;
}

@keyframes pulse{
50%{transform:scale(1.2);}
}
</style>

</head>

<body>

<div class="box" id="questionBox">

<h2 id="question"> my dear wifeeee do u want to marry me ❤️</h2>

<button onclick="yes()">Yes</button>

<button onclick="no()">No</button>

</div>

<div class="box" id="celebration">

<h1>🎉 Happy Birthday My darling wifeeeeee queennnnnnnn 🎉</h1>

<h2>❤️ I Love You Forever my cutie pie ❤️</h2>

<p>

May your smile never fade.<br>

Thank you for making my life beautiful.<br><br>

You are my happiness, my peace and my forever.

</p>

<div class="hearts">

❤️ 💖 💕 💗 💝 💘 ❤️

</div>

</div>

<script>

let count=0;

function no(){

count++;

if(count<3){

document.getElementById("question").innerHTML="Are you sure? 🥺";

}

else{

document.getElementById("questionBox").innerHTML=`

<h2>🧸 Teddy Says...</h2>

<div style="font-size:90px;">🧸</div>

<h3>The only correct answer is YES ❤️</h3>

<button onclick="restart()">Okay ❤️</button>

`;

}

}

function restart(){

document.getElementById("questionBox").innerHTML=`

<h2>Do you love me? ❤️</h2>

<button onclick="yes()">Yes</button>

`;

}

function yes(){

document.getElementById("questionBox").style.display="none";

document.getElementById("celebration").style.display="block";

for(let i=0;i<60;i++){

let b=document.createElement("div");

b.className="balloon";

b.innerHTML=Math.random()>0.5?"🎈":"❤️";

b.style.left=Math.random()*100+"vw";

b.style.animationDuration=(5+Math.random()*5)+"s";

document.body.appendChild(b);

}

}

</script>

</body>

</html>
