<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
<title>يوسف → إيهاب | رمضان 2026</title>
<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', 'Tahoma', sans-serif;
}

body {
    min-height: 100vh;
    background: linear-gradient(145deg, #0c1c28 0%, #1d3e52 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 16px;
    position: relative;
    overflow-x: hidden;
}

/* نجوم احترافية */
.stars {
    position: fixed;
    width: 100%;
    height: 100%;
    background: transparent;
    z-index: 0;
}

.stars::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background-image: 
        radial-gradient(2px 2px at 10px 50px, #fff, transparent),
        radial-gradient(3px 3px at 150px 200px, #ffd700, transparent),
        radial-gradient(2px 2px at 300px 80px, #fff, transparent),
        radial-gradient(4px 4px at 450px 600px, #fffacd, transparent),
        radial-gradient(2px 2px at 600px 350px, #ffd700, transparent),
        radial-gradient(3px 3px at 750px 150px, #fff, transparent),
        radial-gradient(2px 2px at 850px 700px, #ffd700, transparent),
        radial-gradient(3px 3px at 200px 800px, #fff, transparent),
        radial-gradient(2px 2px at 500px 900px, #fffacd, transparent);
    background-size: 300px 300px;
    opacity: 0.7;
    animation: starTwinkle 3s infinite alternate;
}

@keyframes starTwinkle {
    0% { opacity: 0.4; }
    100% { opacity: 0.9; }
}

/* قمر مضيء */
.moon {
    position: fixed;
    top: 20px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 90px;
    filter: drop-shadow(0 0 40px #ffefb0);
    animation: moonDance 6s infinite alternate;
    z-index: 1;
    text-shadow: 0 0 40px #ffeb99;
}

@keyframes moonDance {
    0% { transform: translateX(-50%) translateY(0) rotate(0deg); }
    100% { transform: translateX(-50%) translateY(-20px) rotate(5deg); }
}

/* فوانيس متنوعة */
.lantern {
    position: fixed;
    font-size: 55px;
    filter: drop-shadow(0 0 20px #ffaa33);
    animation: lanternGlow 3s infinite alternate;
    z-index: 2;
}

.l1 { top: 15px; right: 15px; animation-delay: 0s; }
.l2 { top: 25px; left: 15px; animation-delay: 0.4s; font-size: 50px; }
.l3 { bottom: 20px; right: 25px; animation-delay: 0.8s; font-size: 60px; }
.l4 { bottom: 30px; left: 20px; animation-delay: 1.2s; font-size: 48px; }
.l5 { top: 45%; left: 8px; animation-delay: 0.6s; font-size: 42px; }
.l6 { top: 40%; right: 10px; animation-delay: 1s; font-size: 65px; }
.l7 { top: 70%; left: 12px; animation-delay: 1.4s; font-size: 45px; }
.l8 { top: 15%; right: 8px; animation-delay: 0.2s; font-size: 52px; }

@keyframes lanternGlow {
    0% { transform: rotate(-6deg) scale(1); filter: drop-shadow(0 0 15px #ff8c00); }
    100% { transform: rotate(6deg) scale(1.08); filter: drop-shadow(0 0 35px #ffaa33); }
}

/* البطاقة الرئيسية - فاخرة جداً */
.card {
    position: relative;
    z-index: 10;
    width: 100%;
    max-width: 460px;
    background: rgba(8, 28, 40, 0.35);
    backdrop-filter: blur(18px);
    -webkit-backdrop-filter: blur(18px);
    border: 2px solid rgba(255, 215, 0, 0.4);
    border-radius: 60px;
    padding: 35px 28px;
    box-shadow: 
        0 40px 70px -20px black,
        0 0 0 1px rgba(255, 215, 0, 0.3) inset,
        0 0 50px rgba(255, 215, 0, 0.25);
    overflow: hidden;
}

/* الصورة في الخلفية - مضبوطة ومثالية */
.card::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: url('image00.jpg');
    background-size: cover;
    background-position: center 30%;
    background-repeat: no-repeat;
    opacity: 0.3;
    z-index: -1;
    filter: blur(3px) brightness(0.8) contrast(1.1);
    transition: opacity 0.5s;
}

/* طبقة ذهبية متلألئة */
.card::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 70% 20%, rgba(255,215,0,0.15), transparent 70%);
    z-index: -1;
}

/* توقيع يوسف في الخلفية */
.signature-bg {
    position: absolute;
    bottom: 10px;
    left: 20px;
    font-size: 14px;
    color: rgba(255, 215, 0, 0.2);
    transform: rotate(-5deg);
    z-index: 0;
    font-style: italic;
}

/* محتوى البطاقة */
.content {
    position: relative;
    z-index: 5;
}

/* عنوان مع تأثير */
.main-title {
    text-align: center;
    margin-bottom: 20px;
}

.main-title h1 {
    font-size: 42px;
    background: linear-gradient(135deg, #fffbf0, #ffd700, #fff0b5);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 30px #ffd700cc;
    animation: titlePulse 2.5s infinite alternate;
}

@keyframes titlePulse {
    0% { text-shadow: 0 0 20px #ffd700; }
    100% { text-shadow: 0 0 45px #ffaa00, 0 0 15px white; }
}

.sub-title {
    color: #ffffffdd;
    font-size: 20px;
    letter-spacing: 2px;
    margin: 10px 0;
}

/* صورة مصغرة في الزاوية */
.corner-img {
    position: absolute;
    top: -25px;
    left: -25px;
    width: 100px;
    height: 100px;
    background: url('image00.jpg') center/cover;
    border-radius: 50%;
    border: 4px solid #ffd700;
    opacity: 0.5;
    transform: rotate(-10deg);
    box-shadow: 0 0 40px gold;
    z-index: 3;
}

/* صورة في الزاوية الأخرى */
.corner-img2 {
    position: absolute;
    bottom: -25px;
    right: -25px;
    width: 90px;
    height: 90px;
    background: url('image00.jpg') center/cover;
    border-radius: 50%;
    border: 4px solid #ffd700;
    opacity: 0.4;
    transform: rotate(15deg);
    box-shadow: 0 0 40px #ffbb00;
    z-index: 3;
}

/* صندوق كلمة المرور */
.pass-showcase {
    background: rgba(0, 0, 0, 0.45);
    border-radius: 100px;
    padding: 20px;
    margin: 25px 0;
    border: 1px solid rgba(255, 215, 0, 0.5);
    backdrop-filter: blur(5px);
    text-align: center;
}

.pass-label {
    color: #fff;
    font-size: 20px;
    margin-bottom: 10px;
    opacity: 0.9;
}

.pass-value {
    background: linear-gradient(145deg, #ffd700, #e5b81b);
    display: inline-block;
    padding: 15px 40px;
    border-radius: 60px;
    color: #0a1a24;
    font-size: 42px;
    font-weight: 900;
    letter-spacing: 5px;
    box-shadow: 0 6px 0 #a07800, 0 15px 30px black;
    border: 2px solid #fff2b5;
    text-shadow: 0 2px 5px white;
    margin: 5px 0;
}

/* حقل الإدخال */
.glass-input {
    width: 100%;
    padding: 18px 25px;
    font-size: 18px;
    background: rgba(255, 255, 255, 0.1);
    border: 2px solid rgba(255, 215, 0, 0.4);
    border-radius: 60px;
    color: white;
    text-align: center;
    margin: 20px 0 15px;
    outline: none;
    transition: 0.4s;
    backdrop-filter: blur(5px);
}

.glass-input:focus {
    border-color: #ffd700;
    box-shadow: 0 0 40px rgba(255, 215, 0, 0.6);
    background: rgba(255, 255, 255, 0.18);
    transform: scale(1.02);
}

.glass-input::placeholder {
    color: #ffffffcc;
    font-size: 16px;
}

/* زر الدخول السحري */
.magic-btn {
    width: 100%;
    padding: 18px 25px;
    background: linear-gradient(145deg, #ffd700, #f0b81b);
    border: none;
    border-radius: 60px;
    color: #0b1f2c;
    font-size: 28px;
    font-weight: bold;
    cursor: pointer;
    box-shadow: 0 8px 0 #b17e1a, 0 15px 40px black;
    transition: 0.15s;
    border: 2px solid #fff5cc;
    text-shadow: 0 1px 3px white;
    margin: 5px 0 10px;
    position: relative;
    overflow: hidden;
}

.magic-btn::before {
    content: "✨";
    position: absolute;
    left: -20px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 28px;
    animation: sparkleLeft 2s infinite;
}

.magic-btn::after {
    content: "✨";
    position: absolute;
    right: -20px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 28px;
    animation: sparkleRight 2s infinite 1s;
}

@keyframes sparkleLeft {
    0%, 100% { left: -20px; opacity: 0.3; }
    50% { left: 10px; opacity: 1; }
}

@keyframes sparkleRight {
    0%, 100% { right: -20px; opacity: 0.3; }
    50% { right: 10px; opacity: 1; }
}

.magic-btn:active {
    transform: translateY(6px);
    box-shadow: 0 2px 0 #b17e1a, 0 10px 30px black;
}

/* رسالة الخطأ */
.error-msg {
    color: #ffb3b3;
    text-align: center;
    min-height: 28px;
    font-size: 18px;
    text-shadow: 0 0 10px #ff0000aa;
    margin: 10px 0 0;
    font-weight: bold;
}

/* بطاقة التهاني - فاخرة جداً */
.greeting-card {
    background: rgba(10, 30, 45, 0.7);
    border: 3px solid #ffd700;
    padding: 30px 25px;
    text-align: center;
    position: relative;
}

/* صورة مركزية كبيرة */
.profile-large {
    width: 160px;
    height: 160px;
    border-radius: 50%;
    border: 6px solid #ffd700;
    margin: 10px auto 25px;
    background: url('image00.jpg') center/cover;
    box-shadow: 0 0 60px #ffd700;
    animation: profilePulse 3s infinite alternate;
}

@keyframes profilePulse {
    0% { box-shadow: 0 0 30px #ffd700; transform: scale(1); }
    100% { box-shadow: 0 0 80px #ffaa00, 0 0 30px white; transform: scale(1.05); }
}

/* نص التهنئة */
.greeting-title {
    font-size: 44px;
    background: linear-gradient(135deg, #fffacd, #ffd700, #fff0b5);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 20px;
    text-shadow: 0 0 20px gold;
}

.greeting-message {
    background: rgba(0, 0, 0, 0.4);
    border-radius: 50px;
    padding: 30px 20px;
    border: 1px solid rgba(255, 215, 0, 0.4);
    backdrop-filter: blur(8px);
    color: #fff;
    font-size: 22px;
    line-height: 2;
    margin: 20px 0;
}

.greeting-message span {
    color: #ffd700;
    font-size: 26px;
    display: block;
    margin: 15px 0 5px;
    text-shadow: 0 0 10px gold;
}

/* توقيع يوسف */
.final-signature {
    margin-top: 30px;
    font-size: 32px;
    color: #ffd700;
    border-top: 3px dashed #ffd70080;
    padding-top: 25px;
    font-weight: bold;
    text-shadow: 0 0 15px gold;
}

/* رسالة خاصة من يوسف */
.from-youss {
    position: absolute;
    bottom: 10px;
    right: 20px;
    color: rgba(255, 215, 0, 0.3);
    font-size: 14px;
    font-style: italic;
}

.hidden {
    display: none;
}

.fade-scale {
    animation: fadeScale 0.8s ease-out;
}

@keyframes fadeScale {
    0% { opacity: 0; transform: scale(0.8); }
    100% { opacity: 1; transform: scale(1); }
}

/* اهتزاز للغلط */
@keyframes shake {
    0%, 100% { transform: translateX(0); }
    20%, 60% { transform: translateX(-12px); }
    40%, 80% { transform: translateX(12px); }
}

.shake-effect {
    animation: shake 0.4s ease-in-out;
}

/* للموبايل */
@media (max-width: 480px) {
    .moon { font-size: 70px; }
    .lantern { font-size: 45px; }
    .main-title h1 { font-size: 36px; }
    .pass-value { font-size: 34px; padding: 12px 30px; }
    .greeting-title { font-size: 36px; }
    .greeting-message { font-size: 18px; }
    .final-signature { font-size: 26px; }
}
</style>
</head>
<body>
<div class="stars"></div>
<div class="moon">🌙</div>

<!-- فوانيس كثيرة -->
<div class="lantern l1">🏮</div>
<div class="lantern l2">🏮</div>
<div class="lantern l3">🏮</div>
<div class="lantern l4">🏮</div>
<div class="lantern l5">🏮</div>
<div class="lantern l6">🏮</div>
<div class="lantern l7">🏮</div>
<div class="lantern l8">🏮</div>

<!-- صفحة الدخول -->
<div class="card" id="loginBox">
    <div class="corner-img"></div>
    <div class="corner-img2"></div>
    <div class="signature-bg">✍️ من يوسف</div>
    
    <div class="content">
        <div class="main-title">
            <h1>🌙 إيـهـاب 🌙</h1>
            <div class="sub-title">✨ من يوسف إلى إيهاب ✨</div>
        </div>
        
        <div class="pass-showcase">
            <div class="pass-label">🔐 كلمة المرور</div>
            <div class="pass-value">يوسف</div>
        </div>
        
        <input type="text" id="nameInput" class="glass-input" placeholder="اكتب كلمة المرور ..." autocomplete="off">
        
        <button class="magic-btn" onclick="checkName()">ادخل عالمي</button>
        <p id="error" class="error-msg"></p>
    </div>
</div>

<!-- صفحة التهاني -->
<div class="card greeting-card hidden" id="messageBox">
    <div class="profile-large"></div>
    
    <h2 class="greeting-title">⭐ رمضان كريم ⭐</h2>
    
    <div class="greeting-message">
        <span>💌 إلى إيهاب الغالي 💌</span>
        
        بمناسبة حلول شهر رمضان المبارك 🌙<br>
        أهديك هذه المفاجأة من القلب ✨<br>
        أعاده الله عليك بالخير واليمن والبركات 🤍<br>
        وجعل أيامك كلها فرح ونجاح يا غالي 💫
        
        <span>💙 كل سنة وانت طيب 💙</span>
    </div>
    
    <div class="final-signature">
        أخوك: يوسف
    </div>
    
    <div class="from-youss">✍️ صممها لك يوسف بحب</div>
</div>

<audio id="ramadanSong" src="song00.mp3" preload="auto"></audio>

<script>
function checkName() {
    let correctName = "يوسف";
    let enteredName = document.getElementById("nameInput").value.trim();
    let loginBox = document.getElementById("loginBox");
    
    if (enteredName === correctName) {
        // إخفاء صفحة الدخول وإظهار التهاني
        loginBox.classList.add("hidden");
        let msgBox = document.getElementById("messageBox");
        msgBox.classList.remove("hidden");
        msgBox.classList.add("fade-scale");
        
        // تشغيل الأغنية
        let audio = document.getElementById("ramadanSong");
        audio.volume = 0.6;
        audio.currentTime = 0;
        
        let playPromise = audio.play();
        
        if (playPromise !== undefined) {
            playPromise.catch(error => {
                console.log("منع التشغيل التلقائي");
                
                // إضافة رسالة للمس
                const tapMsg = document.createElement("p");
                tapMsg.style.color = "#ffd700";
                tapMsg.style.marginTop = "20px";
                tapMsg.style.fontSize = "18px";
                tapMsg.style.animation = "fadeScale 1s";
                tapMsg.innerText = "👆 اضغط على الشاشة لتشغيل الأغنية";
                msgBox.appendChild(tapMsg);
                
                // تشغيل عند اللمس
                let touchHandler = function() {
                    audio.play();
                    if (tapMsg) tapMsg.remove();
                    document.body.removeEventListener('touchstart', touchHandler);
                };
                document.body.addEventListener('touchstart', touchHandler, { once: true });
            });
        }
    } else {
        // رسالة خطأ
        document.getElementById("error").innerText = "❌ غلط! كلمة المرور هي يوسف";
        
        // تأثير اهتزاز
        loginBox.classList.add("shake-effect");
        setTimeout(() => {
            loginBox.classList.remove("shake-effect");
        }, 400);
    }
}
</script>
</body>
</html>
