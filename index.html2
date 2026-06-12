<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Uma Pergunta Importante 💜</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Segoe UI',sans-serif;
}

body{
background:#121212;
color:white;
display:flex;
justify-content:center;
align-items:center;
height:100vh;
overflow:hidden;
}

.container{
background:#1e1e1e;
padding:35px;
border-radius:25px;
width:90%;
max-width:450px;
text-align:center;
box-shadow:0 0 20px rgba(157,78,221,.5);
}

h1{
color:#FFD60A;
margin-bottom:15px;
}

p{
margin-bottom:20px;
}

button{
padding:12px 20px;
border:none;
border-radius:15px;
margin:8px;
cursor:pointer;
font-size:16px;
font-weight:bold;
transition:.3s;
}

.sim{
background:#9D4EDD;
color:white;
}

.nao{
background:#FFD60A;
color:black;
position:relative;
}

.proximo{
background:#7B2CBF;
color:white;
}

input, select{
width:100%;
padding:12px;
margin:10px 0;
border:none;
border-radius:12px;
}

.heart{
position:absolute;
font-size:20px;
animation:subir 8s linear infinite;
opacity:.4;
}

@keyframes subir{
0%{
transform:translateY(100vh);
opacity:0;
}
20%{
opacity:.4;
}
100%{
transform:translateY(-100vh);
opacity:0;
}
}
</style>
</head>

<body>

<div class="container" id="app">
<h1>💜 Oi 💜</h1>
<p>Tenho uma pergunta importante...</p>
<button class="proximo" onclick="tela2()">Continuar</button>
</div>

<script>

for(let i=0;i<20;i++){
let heart=document.createElement("div");
heart.className="heart";
heart.innerHTML=Math.random()>0.5?"💜":"💛";
heart.style.left=Math.random()*100+"vw";
heart.style.animationDuration=(5+Math.random()*5)+"s";
document.body.appendChild(heart);
}

let dataEscolhida="";
let horaEscolhida="";
let atividadeEscolhida="";

function tela2(){
document.getElementById("app").innerHTML=`
<h1>💛 Pergunta 💛</h1>
<p>Você aceitaria sair comigo?</p>

<button class="sim" onclick="tela3()">SIM</button>
<button class="nao" id="nao">NÃO</button>
`;

const nao=document.getElementById("nao");

nao.addEventListener("mouseover",()=>{
nao.style.position="absolute";
nao.style.left=Math.random()*80+"%";
nao.style.top=Math.random()*80+"%";
});
}

function tela3(){
document.getElementById("app").innerHTML=`
<h1>🥺</h1>
<p>Sério? Você disse sim?</p>
<button class="proximo" onclick="tela4()">Continuar</button>
`;
}

function tela4(){
document.getElementById("app").innerHTML=`
<h1>📅</h1>
<p>Quando você está livre?</p>

<input type="date" id="data">

<input type="time" id="hora">

<button class="proximo" onclick="salvarData()">Próximo</button>
`;
}

function salvarData(){
dataEscolhida=document.getElementById("data").value;
horaEscolhida=document.getElementById("hora").value;
tela5();
}

function tela5(){
document.getElementById("app").innerHTML=`
<h1>🌙</h1>
<p>O que você gostaria de fazer?</p>

<select id="atividade">
<option>Caminhar juntos</option>
<option>Ir ao bosque</option>
<option>Ver um filme</option>
<option>Tomar alguma coisa</option>
<option>Fazer algo que você goste</option>
<option>Qualquer coisa, desde que seja com você</option>
</select>

<button class="proximo" onclick="finalizar()">Confirmar</button>
`;
}

function finalizar(){

atividadeEscolhida=
document.getElementById("atividade").value;

document.getElementById("app").innerHTML=`
<h1>💜 Encontro Confirmado 💛</h1>

<div style="
background:#2b2b2b;
padding:20px;
border-radius:20px;
margin-top:15px;
">

<h2>📅 COMPROMISSO AGENDADO</h2>

<br>

<p><b>👤 Participantes:</b><br>
Sheldon & Amy</p>

<p><b>📅 Data:</b><br>
${dataEscolhida}</p>

<p><b>🕒 Horário:</b><br>
${horaEscolhida}</p>

<p><b>📍 Programa:</b><br>
${atividadeEscolhida}</p>

<p><b>💜 Status:</b><br>
Confirmado</p>

</div>

<br>

<p>
Talvez não sejamos Sheldon e Amy,
mas achei que valia a pena tentar criar
nossa própria história. 💛
</p>
`;
}

</script>

</body>
</html>
