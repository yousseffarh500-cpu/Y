<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>مفاجأة رمضانيه 🌙✨</title>

<style>
body{
    margin:0;
    font-family: 'Tahoma', sans-serif;
    background: radial-gradient(circle at top, #0f2027, #203a43, #2c5364);
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    overflow:hidden;
    color:white;
}

/* Stars */
.stars{
    position:absolute;
    width:100%;
    height:100%;
    background: radial-gradient(white 1px, transparent 1px);
    background-size: 40px 40px;
    animation: moveStars 20s linear infinite;
    opacity:0.5;
}
@keyframes moveStars{
    from {background-position: 0 0;}
    to {background-position: 1000px 1000px;}
}

/* Moon */
.moon{
    position:absolute;
    top:40px;
    left:50%;
    transform:translateX(-50%);
    font-size:75px;
    animation: float 5s ease-in-out infinite;
}
@keyframes float{
    0%{transform:translate(-50%,0px);}
    50%{transform:translate(-50%,25px);}
    100%{transform:translate(-50%,0px);}
}

/* Lanterns */
.lantern{
    position:absolute;
    font-size:45px;
    animation: swing 3s infinite alternate ease-in-out;
}
.l1{ left:8%; top:5%; }
.l2{ left:25%; top:10%; }
.l3{ left:42%; top:6%; }
.l4{ right:42%; top:6%; }
.l5{ right:25%; top:10%; }
.l6{ right:8%; top:5%; }

@keyframes swing{
    from{ transform:rotate(-15deg);}
    to{ transform:rotate(15deg);}
}

/* Card */
.card{
    background: rgba(255,255,255,0.1);
    backdrop-filter: blur(12px);
    width:90%;
    max-width:420px;
    padding:30px;
    border-radius:25px;
    box-shadow:0 20px 50px rgba(0,0,0,0.6);
    text-align:center;
    border:1px solid rgba(255,255,255,0.3);
    z-index:2;
}

h1{ color:#ffd700; }
input{
    width:100%;
    padding:12px;
    border-radius:12px;
    border:none;
    margin-top:15px;
    font-size:16px;
    text-align:center;
}
button{
    margin-top:20px;
    background:#ffd700;
    color:#000;
    border:none;
    padding:12px 25px;
    border-radius:12px;
    font-size:16px;
    cursor:pointer;
    font-weight:bold;
}
button:hover{
    transform:scale(1.08);
    transition:0.3s;
}

.hidden{ display:none; }
.message{
    line-height:1.9;
    font-size:18px;
}
</style>
</head>

<body>

<div class="stars"></div>
<div class="moon">🌙</div>

<div class="lantern l1">🏮</div>
<div class="lantern l2">🏮</div>
<div class="lantern l3">🏮</div>
<div class="lantern l4">🏮</div>
<div class="lantern l5">🏮</div>
<div class="lantern l6">🏮</div>

<div class="card" id="loginBox">
    <h1>مرحبًا إيهاب</h1>
    <p>🔐 كلمة المرور: <strong>يوسف</strong></p>
    <input type="text" id="nameInput" placeholder="اكتب كلمة المرور">
    <button onclick="checkName()">دخول ✨</button>
    <p id="error" style="color:#ff6b6b;"></p>
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

<!-- Direct MP3 audio for Ramadan song -->
<audio id="ramadanSong" src="https://archive.org/download/ramadan-jana/ramadan_jana.mp3"></audio>

<script>
function checkName(){
    var correctName = "يوسف";
    var enteredName = document.getElementById("nameInput").value.trim();
    if(enteredName === correctName){
        document.getElementById("loginBox").classList.add("hidden");
        document.getElementById("messageBox").classList.remove("hidden");
        var audio = document.getElementById("ramadanSong");
        audio.play();
    } else {
        document.getElementById("error").innerText = "كلمة المرور غير صحيحة";
    }
}
</script>

</body>
</html>
