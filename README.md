<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Wi-Fi Free</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
background:#000;
overflow:hidden;
}

.video-bg{
position:fixed;
right:0;
bottom:0;
min-width:100%;
min-height:100%;
object-fit:cover;
z-index:-1;
}

.box{
width:90%;
max-width:350px;
background:rgba(0,0,0,0.75);
padding:30px;
border-radius:20px;
text-align:center;
backdrop-filter:blur(5px);
}

.logo{
width:90px;
margin-bottom:20px;
}

h1{
color:#fff;
margin-bottom:10px;
font-size:24px;
}

p{
color:#ddd;
margin-bottom:25px;
font-size:15px;
}

button{
width:100%;
padding:15px;
border:none;
border-radius:12px;
background:#E1306C;
color:#fff;
font-size:18px;
font-weight:bold;
cursor:pointer;
transition:0.3s;
}

button:hover{
transform:scale(1.03);
background:#ff2c75;
}

.loading{
display:none;
margin-top:20px;
color:#fff;
font-size:14px;
}

</style>
</head>

<body>

<video autoplay muted loop class="video-bg">
<source src="https://cdn.coverr.co/videos/coverr-night-city-1567843181086?download=1080p" type="video/mp4">
</video>

<div class="box">

<img class="logo"
src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png">

<h1>Wi-Fi Liberado</h1>

<p>
Clique abaixo para acessar o Instagram e liberar sua internet.
</p>

<button onclick="liberarWifi()">
ENTRAR COM INSTAGRAM
</button>

<div class="loading" id="loading">
Conectando...
</div>

</div>

<script>

function liberarWifi(){

document.getElementById("loading").style.display="block";

fetch("http://10.0.0.1/auth", {
method: "POST",
mode: "no-cors"
});

setTimeout(() => {

window.location.href = "https://instagram.com";

}, 1500);

setTimeout(() => {

window.location.href = "https://www.google.com.br";

}, 7000);

}

</script>

</body>
</html>
