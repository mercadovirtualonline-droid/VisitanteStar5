
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
background:url('data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDAAgGBgcGBQgHBwcJCQgKDBQNDAsLDBkSEw8UHRofHh0aHBwgJC4nICIsIxwcKDcpLDAxNDQ0Hyc5PTgyPC4zNDL/2wBDAQkJCQwLDBgNDRgyIRwhMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjL/wAARCASVAscDASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDwiiiimIKKKKACiiigAooooAuxaksTQkidXjBIaOYjn+me9MlvrWZN0lmzSBFQMZTwAMD+VUpFLYxQqBeTyanlVyuZiou1fenUUVRIUUUqoznCqWPoBmgBKK1bLw1reosFs9Ku5iemyI1Qu7S4sLuW0u4XhuImKSRuMFSOxoAhooooAWinQwy3EyQwRPLK5CoiKWZj6ADrWg/h3W4737C+jail35XnfZ2tXEnl/wB/bjO3g89KAM2kopVVnYKqlmJwABkk0AJRU95ZXenXT2t7azW1wmN0U8ZR1yMjIPI4qCgBKKsmwvF09dQNpOLJpPKW5MZ8svjO0NjGcc461WoAKKKs2theXyzNaWk9wsEZkmMUZcRoOrNgcD3NAFaiilVWdgqqWZjgADJJoASirF5ZXenXT2t9azW1wmN0U8ZR1yMjIPI4qvQAUUUUAFFFFABRRRQAUUUmaAFopM0ZpALRSZozTAWikzRmgBaKTNGaAFopKKEGgtFJRQwuLRSUUBcKKKKACjNFCjmgdgxRQcswA61d1bSb7Q9Rl07UrZ7a8hx5kT4yuQGHT2INAWKdBGOtaei2BvbtAR8tTa3pv2R1wOKylVip8iNI0248zMXIopSMHPakrS5nYKKKKb8gCijFFAgoopKBi0UUUCCiiigAooooAKKKKACiiigAooooAKKKKANbw1/ZP/CS6d/bu7+yvPX7Vtz9zPPTnHrjnHSum+Kn/CHf8JDbf8Id5X2fyB9o8jd5e/JxjPfGM446d81y3h7R5fEPiCx0iKVIpLyZYhI/Rc963viJ4Bl8AavbWT6gl9HcQ+akgi8sjnBBXJx+dAHHUUUUAFFFFADqKKKACiiigAooooAKKKKACiiigAooooAK9h+BA0uBvEuparBFJDY2scxeRA2xRvLED6CvHgMkCvo3S/Aln4M+EniLUFvWnuNS0djKTgICUYgL+LYoA3NP+M3ha+1yy0fTLe5le6nWBHWIIiljjJzjivAPiX/yUrxD/wBfr/zr0b4F6f4WayutT1F4P7Vtpw0fnNjy1ABDD8c815j48vrfU/Hmt3tq4kgmu3ZGHQjPWkBjafYXOqahb2FnEZbm4kWKJB/ExOBXfH4a6ImojRJfHWnpr5Plm0+yyGIS9NhmzjOeOnXtWF8N9TtNI+Imi3t86pbJcbXdui7lKgn2BINat98NPF03jqezj0u7Ilu2dL8IfJ2FsiTzOnTnrn8aYHQfCTw/baT4/vItVvvsutacsyJZm2L/AMBBkD5wMA8DuDVHw+uoan8QLpdD8eXt3IumSsdUmtWLsg+ZotkjZAz3zweRXSaXqVpq37Q+uXdlIrwGzljDqchykKox/NTXHfBn/kcrz/sF3P8A6CKQGP4c8Frq2jXGu6tq0Oj6LDJ5P2qWNpGlkxnaiDljj/PXEms+EYtFg0zWdF8Q2+p6fc3AijuYkMUkUowcNGxyPX/9YzvR6bd+KvgvpltokL3d3o9/M13aQjdJtkyVcKOSO3Hv6GuauvBWsaBp2matqsS2YuroRRWk5K3BAwd+wjhe3PPTjkUwNnxP4Z1jWPi3deH73W4r2+ygk1C6UQJt8pWyVBIGAcYHXHvTZvh7pF5p+pP4b8X22sXunwNcTWn2N4S0a/eKMSQ+Pb+tdZrHh7T/ABL+0HrtlqSPLDHAJ1tUk2NcusEeIw3UZznj0rW8HLqQg8QPN4LsPDdgumXEaMbd0uJn2527nOWUAEnAxkCkB59df8m/WP8A2ML/APok1y/hLQ7fxJ4nstGuL/7Al25jScxeYA+DtBG4dTgde9dRdf8AJv1j/wBjC/8A6JNctf6Jrnhh9Ovru1ls2uUW6s5CQSwGCGGCcHocHmmAtl4Zv7zxjF4Z27L1rz7I/GQhDYZvoME/QV1mh6Le6bqvjbTtD8TPHDp2nTtPMlsP9MWPhkwWOzkkBgSfzruLhrOzN78W4PLUXWkILeMc7dQfMTYH+zt5+prg/hkxaw8csxJY+HbkknqelAGLoeh+FL/TFn1fxg2l3ZYg2w0uSfA7HerAc1peLvBNr4Mn0SWy8QteXN7idEazNvJCmRtcqWJGT0BweK0fh14SZdNn8aahplxqNtZttsbCCFpGu7gdMgA4RT1P+GDzevp4lu/Ea6x4ksL6Ce7uAd9zbvEp5HyruHQDoPSgDa8VeF9f1r4t3Xh6TUjq2qExq15LGIVK+UrZKjIUKD29PU1JH8NtG1G6k0zQ/HFhqGtIDtszavEkrAZKpKSVY8HpXZzXdvB+0X4itZ51gfULI2cErHAWV4I9vPbpj6muP8FeAfFFh4/06a+0u6sLbTbpLi6u50KRJHGdzYc/KcgY4J6+lAGb4W+HcniPSdavp9Uh0z+yZY0nW5j+VVJO8s2eCoB4wcnjil1nwJYW/hSfxD4f8SQ61ZWsqxXeLV7d4Sxwp2sSSCSBnj+ddFJfwal4D+KV/aH/AEe61WCWPHGVa4JH6VjeFP8AkkHxC+unf+jzQB5/1NWLyxvNOuDb31rPazgBjHPGUbB6HB5qFHaN1dGKspBBHUGtHXfEGq+JtR/tDWLtrq62CPzGVV+UdBhQBQB6B8NNWvtC+HXjvUtNnMF5AtmY5QobaS7g8EEdCas+D/Gt54+1uPwr4xSDU7XUFeOK5MCJNbSbSVZWUD0x+Ppwc/wBaXF98L/H9taW8txcSLZBIoULs37xjwByak+GnhDV9J8UQ+I9csrjStI0sPPPPexmLJCkBVDYJJJHT+eKAMzw/wDDddag8QT3euW+mx6JcCGeSWEshXcwZs7sjG3gYOSQOKisPANhq9/fS6d4lgbw/p8SPdavc2rwqjNnCLGSSzfj/TOvYX39pfDD4jX4UqLrULWbae26ctj9ai8I2k3iL4UeIPD2ljzdWjvYr4Wyn55ogAp2jvgjOPp60AZepeArJvD11rfhnxHBrtrZYN5GLZ7eWFT0bYxJK+/+Bq3bfDewXwppHiTVvFNvpthfo5bfatI6uG2hUVWy+QCSeMe+a0PB2ian4V8M+Lda16zn0+zuNJl0+CK7QxtPNJjbhTgnGOuO/saoeNyf+FY/DwZ48i84/wC2q0hmL4u8GN4ZbTprTUI9U07UozJZ3UUZTzMEAgqckEEjj3ra/wCFc6Pp0kNj4h8aWelaxKqsbL7I8oh3DIEkgIVDyOvSrmpXcVh4G+FN7cAmG3ubyWQYz8q3KE/oK63xjdeJG8WTNpnw/wDD2t2V2yy2uof2T9o85GAwXkBxntk46elMDxjxFoF54Y1250m/VRPAw+ZDlXUjIZT3BBBq/wCHvH3ifwtYyWWiam1pbSSmVkEMb5cgDOWUnoo/KrfxJvtYvfGEya5Fp8d/bRJbumnnMQAGQOp5GcEdsVyFAj3D4l/EfxZoOqaLDpusNbx3Gj29zKBBG26Ri25uVPXA46VxFj4Ni1DR18TeKvEUGi22oTOYGe2aaW5bPzMI0xhcnr/9ar3xj/5DXh3/ALF+1/m9XPE2j6h4r8BeEdS0G0m1CGwsjY3UNshkeGVT1KDnnrnHp60DOb8QeBn0YaZd2mpW+p6Pqb+Xb38CkDdnBVlPKsPTPY+hrP8AFfhn/hGPGN34f+1/aTbyInn+Xs3blVs7cnH3vXtXZ6pay+EvhXoeka1mDUrnWv7SW1k/1kECpsyR2yece57g1d+IPgvX9Z+LVxd2emzS2F48M0d6q/uBGEQFmf7oAwep/mKEIwY/hiZPitP4HGr8xJuF59m6/uhJjZv98fe9/asPxR4e0XQFjhsfE0Wq6gshjuYYLVkjiIHOJCcPzxwK9aiyP2qNQI/54n/0kWvAKYHpnwYuZrLVfE13bvsng0C5kjfAO1lZCDz7isqb4veO7iGSCXXnaORSjr9mhGQRgj7lavwYuZrLVfE13bPsng0G5ljfAO1lZCDz7isS++K3jXVNPuLC81t5bW5jaKWM28Q3KRgjIXPSlYZ1XhzxHq3hf4Dz3+jXZtbo6+YzIEVvlMKkjDAjsKs+FfEer/EHRfEtp4tEV9YWumS3Md9JbojW0y424ZVHuce3pVbw54i1Xwx8B57/AEe5FvdHXjGXMSSfKYVJGHBHYdq4zW/iN4s8RWLWOqa1JLasfmijjSJW+oRRn8aBM6TxWf8AhKPhR4b8SD57vS2Ok3p6naOYyfwx ') center center/cover no-repeat;
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
src="

<h1>Bem-vindo ao Wi-Fi</h1>

<p>
Siga nosso Instagram para liberar seu acesso gratuito.
</p>

<button class="instagram" onclick="seguirInstagram()">
“¸ Seguir no Instagram
</button>

<div class="loading" id="loading">
âœ” Liberando Wi-Fi...
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
