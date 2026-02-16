<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>مفاجأة رمضان 🌙✨</title>
<style>
body{
    margin:0;
    font-family: 'Tahoma', sans-serif;
    background: radial-gradient(circle at top, #0f2027, #203a43, #2c5364);
    display:flex;
    justify-content:center;
    align-items:center;
    min-height:100vh;
    color:white;
    padding:15px;
    box-sizing:border-box;
}
.stars{
    position:fixed;
    width:100%;
    height:100%;
    background: radial-gradient(white 1px, transparent 1px);
    background-size: 40px 40px;
    animation: moveStars 20s linear infinite;
    opacity:0.5;
    top:0;
    left:0;
    z-index:0;
}
@keyframes moveStars{
    from {background-position: 0 0;}
    to {background-position: 1000px 1000px;}
}
.moon{
    position:fixed;
    top:20px;
    left:50%;
    transform:translateX(-50%);
    font-size:60px;
    animation: float 5s ease-in-out infinite;
    z-index:1;
}
@keyframes float{
    0%{transform:translate(-50%,0px);}
    50%{transform:translate(-50%,15px);}
    100%{transform:translate(-50%,0px);}
}
.lantern{
    position:fixed;
    font-size:40px;
    animation: swing 3s infinite alternate ease-in-out;
    z-index:1;
}
.l1{ left:5%; top:10%; }
.l2{ left:20%; top:15%; }
.l3{ right:20%; top:12%; }
.l4{ right:5%; top:8%; }
@keyframes swing{
    from{ transform:rotate(-10deg);}
    to{ transform:rotate(10deg);}
}
.card{
    background: rgba(255,255,255,0.1);
    backdrop-filter: blur(12px);
    width:100%;
    max-width:400px;
    padding:25px;
    border-radius:25px;
    box-shadow:0 20px 50px rgba(0,0,0,0.6);
    text-align:center;
    border:1px solid rgba(255,255,255,0.3);
    position:relative;
    z-index:2;
    margin:20px auto;
}
h1{ color:#ffd700; font-size:24px; }
input{
    width:100%;
    padding:12px;
    border-radius:12px;
    border:none;
    margin:15px 0;
    font-size:16px;
    text-align:center;
    box-sizing:border-box;
}
button{
    background:#ffd700;
    color:#000;
    border:none;
    padding:12px 25px;
    border-radius:12px;
    font-size:16px;
    cursor:pointer;
    font-weight:bold;
    width:100%;
}
button:hover{
    transform:scale(1.05);
    transition:0.3s;
}
.hidden{ display:none; }
.message{
    line-height:1.8;
    font-size:16px;
}
#error{ color:#ff6b6b; margin:10px 0 0; }
</style>
</head>
<body>
<div class="stars"></div>
<div class="moon">🌙</div>
<div class="lantern l1">🏮</div>
<div class="lantern l2">🏮</div>
<div class="lantern l3">🏮</div>
<div class="lantern l4">🏮</div>

<div class="card" id="loginBox">
    <h1>مرحبًا إيهاب</h1>
    <p>🔐 كلمة المرور: <strong>يوسف</strong></p>
    <input type="text" id="nameInput" placeholder="اكتب كلمة المرور">
    <button onclick="checkName()">دخول ✨</button>
    <p id="error"></p>
</div>

<div class="card hidden" id="messageBox">
    <h1>⭐ رمضان كريم ⭐</h1>
    <div class="message">
        بمناسبة حلول شهر رمضان المبارك 🌙<br>
        أقدم لك أسمى آيات التهاني والتبريكات ✨<br>
        أعاده الله عليك بالخير واليمن والبركات 🤍<br>
        وجعل أيامك كلها نجاح وتوفيق يا بطل 💫
        <br><br>
        مع خالص التقدير<br>
        أخوك يوسف 💙
    </div>
</div>

<audio id="ramadanSong" src="song00.mp3"></audio>

<script>
function checkName(){
    var correctName = "يوسف";
    var enteredName = document.getElementById("nameInput").value.trim();
    if(enteredName === correctName){
        document.getElementById("loginBox").classList.add("hidden");
        document.getElementById("messageBox").classList.remove("hidden");
        var audio = document.getElementById("ramadanSong");
        audio.play().catch(e => console.log("المتصفح منع التشغيل التلقائي"));
    } else {
        document.getElementById("error").innerText = "كلمة المرور غير صحيحة";
    }
}
</script>
</body>
</html>
