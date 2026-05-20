<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">

<title>Star Festas Wi-Fi</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial;
}

body{
height:100vh;
background:url('https://kommodo.ai/i/KjOO3wjf11A4XHTCAZQH') center center/cover no-repeat;
display:flex;
justify-content:center;
align-items:center;
position:relative;
}

body::before{
content:'';
position:absolute;
inset:0;
background:rgba(0,0,0,.65);
}

.container{
position:relative;
z-index:2;
width:90%;
max-width:420px;
background:rgba(0,0,0,.55);
backdrop-filter:blur(5px);
border:2px solid #FFD700;
border-radius:25px;
padding:30px;
text-align:center;
color:#fff;
box-shadow:0 0 25px rgba(255,215,0,.4);
}

.logo{
width:180px;
margin-bottom:20px;
}

h1{
font-size:34px;
margin-bottom:20px;
}

p{
font-size:18px;
margin-bottom:30px;
line-height:1.5;
}

button{
width:100%;
padding:18px;
border:none;
border-radius:15px;
font-size:24px;
font-weight:bold;
cursor:pointer;
margin-top:15px;
transition:.3s;
}

.instagram{
background:#FFD700;
color:#000;
}

.instagram:hover{
transform:scale(1.03);
}

.loading{
display:none;
margin-top:20px;
font-size:18px;
color:#00ff88;
}

</style>
</head>

<body>

<div class="container">

<img class="logo"
src="https://kommodo.ai/i/KjOO3wjf11A4XHTCAZQH">

<h1>Bem-vindo ao Wi-Fi</h1>

<p>
Siga nosso Instagram para liberar seu acesso gratuito.
</p>

<button class="instagram" onclick="seguirInstagram()">
📸 Seguir no Instagram
</button>

<div class="loading" id="loading">
✔ Liberando Wi-Fi...
</div>

</div>

<script>

function getParam(name){
const urlParams = new URLSearchParams(window.location.search);
return urlParams.get(name);
}

function seguirInstagram(){

document.getElementById('loading').style.display='block';

window.open(
'https://www.instagram.com/star.festaseeventos?igsh=ejByMXRoNTlmdmR2&utm_source=qr',
'_blank'
);

setTimeout(() => {

const redirect = getParam('redirect_uri');

if(redirect){

window.location.href =
redirect +
'?auth_user=star&auth_pass=star';

}else{

alert('Erro ao liberar acesso');

}

}, 5000);

}

</script>

</body>
</html>
