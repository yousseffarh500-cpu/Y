<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>🎊 كل سنة وانت طيب يا إيهاب</title>
<style>
*{margin:0;padding:0;box-sizing:border-box;}
body{
font-family:'Tahoma',sans-serif;
background:linear-gradient(145deg, #1a2f3f 0%, #0f2027 100%);
min-height:100vh;
display:flex;
justify-content:center;
align-items:center;
padding:16px;
position:relative;
overflow-x:hidden;
}
.stars{
position:fixed;
width:100%;
height:100%;
background-image:radial-gradient(white 2px, transparent 2px);
background-size:50px 50px;
animation:starsMove 30s linear infinite;
opacity:0.4;
top:0;
right:0;
}
@keyframes starsMove{
0%{background-position:0 0;}
100%{background-position:100px 100px;}
}
.moon{
position:fixed;
top:20px;
left:50%;
transform:translateX(-50%);
font-size:70px;
filter:drop-shadow(0 0 15px #ffd700);
animation:moonFloat 4s infinite alternate;
z-index:1;
}
@keyframes moonFloat{
0%{transform:translateX(-50%) translateY(0);}
100%{transform:translateX(-50%) translateY(20px);}
}
.lantern{
position:fixed;
font-size:50px;
animation:lanternSwing 2.5s infinite alternate;
filter:drop-shadow(0 0 8px orange);
z-index:1;
}
.l1{top:15px;right:15px;animation-delay:0s;}
.l2{top:25px;left:15px;animation-delay:0.7s;}
.l3{bottom:15px;right:25px;animation-delay:0.3s;}
.l4{bottom:25px;left:20px;animation-delay:1s;}
@keyframes lanternSwing{
0%{transform:rotate(-8deg);}
100%{transform:rotate(8deg);}
}
.card{
background:rgba(10, 25, 35, 0.6);
backdrop-filter:blur(15px);
-webkit-backdrop-filter:blur(15px);
border:2px solid rgba(255,215,0,0.3);
border-radius:40px;
padding:30px 25px;
width:100%;
max-width:430px;
box-shadow:0 25px 50px -8px black, 0 0 0 1px rgba(255,215,0,0.2) inset;
position:relative;
z-index:5;
text-align:center;
}
h1{
font-size:32px;
margin-bottom:20px;
background:linear-gradient(135deg, #fff9e0, #ffd700);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
text-shadow:0 0 10px #ffd70055;
}
h1 i{font-style:normal;display:inline-block;animation:twinkle 1.5s infinite;}
@keyframes twinkle{
0%,100%{opacity:1;}
50%{opacity:0.5;}
}
.sub{
color:#ffffffcc;
font-size:18px;
margin:20px 0 10px;
background:rgba(255,215,0,0.1);
padding:10px 20px;
border-radius:60px;
display:inline-block;
}
.passBox{
background:rgba(0,0,0,0.4);
border-radius:30px;
padding:10px 20px;
margin:20px 0;
border:1px solid #ffd70055;
}
.passBox span{
color:#ffd700;
font-size:22px;
font-weight:bold;
display:block;
margin-top:5px;
letter-spacing:2px;
text-shadow:0 0 8px gold;
}
input{
width:100%;
padding:18px 22px;
font-size:18px;
border:none;
border-radius:60px;
background:rgba(255,255,255,0.1);
border:2px solid #ffd70055;
color:white;
text-align:center;
margin:20px 0 15px;
outline:none;
transition:0.3s;
}
input:focus{border-color:#ffd700;box-shadow:0 0 20px #ffd70055;}
input::placeholder{color:#ffffff80;}
button{
background:linear-gradient(45deg, #ffd700, #fdb931);
border:none;
border-radius:60px;
padding:18px 30px;
width:100%;
font-size:22px;
font-weight:bold;
color:#0f2027;
cursor:pointer;
box-shadow:0 8px 0 #b17e1a, 0 10px 20px black;
transition:0.1s;
border:1px solid #ffe88c;
}
button:active{
transform:translateY(6px);
box-shadow:0 2px 0 #b17e1a, 0 5px 12px black;
}
#error{
color:#ffb3b3;
margin-top:15px;
font-size:16px;
min-height:24px;
text-shadow:0 0 5px red;
}
.messageCard{
background:rgba(10, 25, 35, 0.7);
backdrop-filter:blur(18px);
border:3px solid #ffd700;
padding:35px 25px;
}
.message{
font-size:22px;
line-height:2;
color:#ffffff;
text-shadow:0 2px 5px black;
}
.message span{
color:#ffd700;
font-size:28px;
display:block;
margin:20px 0 10px;
}
.signature{
margin-top:35px;
font-size:25px;
color:#ffd700;
border-top:2px dashed #ffd70055;
padding-top:25px;
}
.hidden{display:none;}
.glow{animation:glowPulse 2s infinite;}
@keyframes glowPulse{
0%,100%{text-shadow:0 0 10px gold;}
50%{text-shadow:0 0 30px gold;}
}
@media(max-width:480px){
h1{font-size:28px;}
.message{font-size:18px;}
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

<div class="card" id="loginBox">
    <h1><i>✨</i> إيهاب ... مرحباً <i>✨</i></h1>
    <div class="sub">🔐 رمضانك مبارك</div>
    <div class="passBox">
        كلمة المرور<br>
        <span>يوسف</span>
    </div>
    <input type="text" id="nameInput" placeholder="اكتب كلمة المرور هنا">
    <button onclick="checkName()">✨ افتح الباب ✨</button>
    <p id="error"></p>
</div>

<div class="card messageCard hidden" id="messageBox">
    <h1 class="glow">⭐ رمضان كريم ⭐</h1>
    <div class="message">
        <span>🎁 لإيهاب الغالي 🎁</span>
        بمناسبة حلول شهر رمضان المبارك 🌙<br>
        أقدم لك أسمى آيات التهاني والتبريكات ✨<br>
        أعاده الله عليك بالخير واليمن والبركات 🤍<br>
        وجعل أيامك كلها نجاح وتوفيق يا بطل 💫
        <div class="signature">
            💙 أخوك يوسف 💙
        </div>
    </div>
</div>

<audio id="ramadanSong" src="song00.mp3" preload="auto"></audio>

<script>
function checkName(){
    let correctName = "يوسف";
    let enteredName = document.getElementById("nameInput").value.trim();
    
    if(enteredName === correctName){
        document.getElementById("loginBox").classList.add("hidden");
        document.getElementById("messageBox").classList.remove("hidden");
        
        // تشغيل الاغنية باحترافية
        let audio = document.getElementById("ramadanSong");
        audio.volume = 0.7;
        
        // محاولة تشغيل الاغنية مع دعم كل المتصفحات
        let playPromise = audio.play();
        
        if (playPromise !== undefined) {
            playPromise.then(() => {
                console.log("🎵 الاغنية شغالة");
            }).catch(error => {
                console.log("المتصفح منع التشغيل التلقائي");
                // طريقة بديلة: رسالة تخبر المستخدم
                alert("اضغط على الصفحة لتشغيل الاغنية");
                
                // تشغيل الاغنية عند اول لمسة على الشاشة
                document.body.addEventListener('touchstart', function playOnce(){
                    audio.play();
                    document.body.removeEventListener('touchstart', playOnce);
                }, {once: true});
            });
        }
    } else {
        document.getElementById("error").innerText = "❌ كلمة المرور غلط، حاول تاني";
    }
}
</script>
</body>
</html>
