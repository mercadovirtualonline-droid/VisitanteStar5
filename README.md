<script>

function seguirInstagram(){

document.getElementById('loading').style.display='block';

window.open(
'https://www.instagram.com/star.festaseeventos?igsh=ejByMXRoNTlmdmR2&utm_source=qr',
'_blank'
);

setTimeout(() => {

liberarWifi();

}, 4000);

}

function liberarWifi(){

const currentUrl = window.location.href;

if(currentUrl.includes("userurl=")){

const url = new URL(currentUrl);

const userurl = url.searchParams.get("userurl");
const uamip = url.searchParams.get("uamip");
const uamport = url.searchParams.get("uamport");
const challenge = url.searchParams.get("challenge");

if(uamip && uamport){

window.location.href =
"http://" + uamip + ":" + uamport +
"/logon?username=star&password=star";

}else{

window.location.href = userurl || "https://google.com";

}

}else{

window.location.href = "https://google.com";

}

}

</script>
