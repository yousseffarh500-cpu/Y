<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
<title>🎊 إيهاب .. رمضانك أحلى</title>
<style>
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', Tahoma, sans-serif;
}

body {
    min-height: 100vh;
    background: linear-gradient(135deg, #0b1a24 0%, #1c3a4f 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 16px;
    position: relative;
    overflow-x: hidden;
}

/* خلفية نجوم متحركة */
.stars {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: transparent;
    animation: starsMove 60s linear infinite;
    z-index: 0;
}

.stars::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background-image: 
        radial-gradient(2px 2px at 15px 80px, #fff, rgba(0,0,0,0)),
        radial-gradient(2px 2px at 72px 430px, #ffd700, rgba(0,0,0,0)),
        radial-gradient(3px 3px at 550px 210px, #fff, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 890px 620px, #fffacd, rgba(0,0,0,0)),
        radial-gradient(2px 2px at 250px 920px, #ffd700, rgba(0,0,0,0)),
        radial-gradient(2px 2px at 120px 250px, #fff, rgba(0,0,0,0)),
        radial-gradient(3px 3px at 720px 540px, #fff, rgba(0,0,0,0)),
        radial-gradient(1px 1px at 400px 750px, #ffd700, rgba(0,0,0,0)),
        radial-gradient(2px 2px at 880px 330px, #fff, rgba(0,0,0,0)),
        radial-gradient(2px 2px at 520px 180px, #fffacd, rgba(0,0,0,0));
    background-repeat: repeat;
    background-size: 200px 200px;
    opacity: 0.6;
    animation: twinkle 4s infinite alternate;
}

@keyframes starsMove {
    0% { transform: translate(0, 0); }
    100% { transform: translate(-30px, -30px); }
}

@keyframes twinkle {
    0% { opacity: 0.4; }
    100% { opacity: 0.9; }
}

/* القمر */
.moon {
    position: fixed;
    top: 25px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 85px;
    filter: drop-shadow(0 0 30px #fffbc2);
    animation: moonGlow 4s infinite alternate;
    z-index: 1;
    text-shadow: 0 0 30px #ffeb99;
}

@keyframes moonGlow {
    0% { transform: translateX(-50%) translateY(0) scale(1); filter: drop-shadow(0 0 20px #fffbc2); }
    100% { transform: translateX(-50%) translateY(-15px) scale(1.05); filter: drop-shadow(0 0 40px #fff2b5); }
}

/* الفوانيس - تصميم جديد احترافي */
.lantern {
    position: fixed;
    font-size: 60px;
    filter: drop-shadow(0 0 15px #ffb347);
    animation: lanternLight 2.5s infinite alternate;
    z-index: 2;
    text-shadow: 0 0 20px orange;
}

.l1 { top: 10px; right: 10px; animation-delay: 0s; }
.l2 { top: 20px; left: 10px; animation-delay: 0.5s; font-size: 55px; }
.l3 { bottom: 10px; right: 20px; animation-delay: 1s; font-size: 65px; }
.l4 { bottom: 20px; left: 15px; animation-delay: 1.5s; font-size: 50px; }
.l5 { top: 45%; left: 5px; animation-delay: 0.8s; font-size: 45px; }
.l6 { top: 40%; right: 5px; animation-delay: 1.2s; font-size: 70px; }

@keyframes lanternLight {
    0% { transform: rotate(-5deg) scale(1); filter: drop-shadow(0 0 10px #ff8c00); }
    100% { transform: rotate(5deg) scale(1.1); filter: drop-shadow(0 0 30px #ffaa33); }
}

/* البطاقة الرئيسية - احترافية 2026 */
.card {
    position: relative;
    z-index: 10;
    width: 100%;
    max-width: 440px;
    background: rgba(10, 30, 45, 0.3);
    backdrop-filter: blur(16px);
    -webkit-backdrop-filter: blur(16px);
    border: 2px solid rgba(255, 215, 0, 0.3);
    border-radius: 48px;
    padding: 30px 24px;
    box-shadow: 
        0 30px 60px -15px rgba(0, 0, 0, 0.8),
        0 0 0 1px rgba(255, 215, 0, 0.2) inset,
        0 0 30px rgba(255, 215, 0, 0.2);
    overflow: hidden;
}

/* الصورة في الخلفية بشكل احترافي */
.card::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-image: url('image00.jpg');
    background-size: cover;
    background-position: center;
    opacity: 0.25;
    z-index: -1;
    filter: blur(2px) brightness(0.7);
    transition: opacity 0.3s;
}

/* طبقة زخرفية */
.card::after {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(circle at 30% 30%, rgba(255,215,0,0.1), transparent 70%);
    z-index: -1;
}

/* صورة مصغرة زخرفية في الزاوية */
.decoration-img {
    position: absolute;
    top: -20px;
    right: -20px;
    width: 120px;
    height: 120px;
    background: url('image00.jpg') center/cover;
    border-radius: 50%;
    border: 3px solid #ffd700;
    opacity: 0.4;
    transform: rotate(15deg);
    box-shadow: 0 0 30px gold;
    z-index: 0;
}

/* محتوى البطاقة */
.content {
    position: relative;
    z-index: 5;
}

h1 {
    font-size: 36px;
    margin-bottom: 15px;
    text-align: center;
}

.glowing-text {
    background: linear-gradient(135deg, #fff6d5, #ffd700, #fff6d5);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 20px #ffd70099;
    animation: textGlow 2.5s infinite alternate;
}

@keyframes textGlow {
    0% { text-shadow: 0 0 15px #ffd700; }
    100% { text-shadow: 0 0 35px #ffaa00, 0 0 10px white; }
}

.welcome-box {
    background: rgba(0, 0, 0, 0.5);
    border-radius: 100px;
    padding: 16px 20px;
    margin: 20px 0;
    border: 1px solid rgba(255, 215, 0, 0.4);
    box-shadow: 0 8px 20px rgba(0,0,0,0.4);
    backdrop-filter: blur(5px);
    text-align: center;
}

.welcome-box p {
    color: #ffffffdd;
    font-size: 22px;
    margin-bottom: 8px;
}

.password-highlight {
    background: linear-gradient(145deg, #ffd700, #f5b81b);
    display: inline-block;
    padding: 12px 35px;
    border-radius: 60px;
    color: #0a1e2d;
    font-size: 32px;
    font-weight: 900;
    letter-spacing: 3px;
    box-shadow: 0 5px 0 #a07800, 0 10px 20px black;
    border: 1px solid #fff2b5;
    margin: 8px 0;
    text-shadow: 0 1px 2px white;
}

.input-field {
    width: 100%;
    padding: 18px 25px;
    font-size: 18px;
    background: rgba(255, 255, 255, 0.08);
    border: 2px solid rgba(255, 215, 0, 0.3);
    border-radius: 60px;
    color: white;
    text-align: center;
    margin: 20px 0 18px;
    outline: none;
    transition: 0.3s;
    backdrop-filter: blur(5px);
}

.input-field:focus {
    border-color: #ffd700;
    box-shadow: 0 0 30px rgba(255, 215, 0, 0.5);
    background: rgba(255, 255, 255, 0.15);
}

.input-field::placeholder {
    color: #ffffffb3;
    font-size: 16px;
}

.btn {
    width: 100%;
    padding: 18px 25px;
    background: linear-gradient(145deg, #ffd700, #f5b81b);
    border: none;
    border-radius: 60px;
    color: #0b1f2c;
    font-size: 26px;
    font-weight: bold;
    cursor: pointer;
    box-shadow: 0 7px 0 #b17e1a, 0 10px 30px black;
    transition: 0.1s;
    border: 1px solid #fff5cc;
    text-shadow: 0 1px 2px white;
    margin-bottom: 10px;
    position: relative;
    overflow: hidden;
}

.btn::before {
    content: "✨";
    position: absolute;
    left: -30px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 24px;
    animation: sparkle 2s infinite;
}

.btn::after {
    content: "✨";
    position: absolute;
    right: -30px;
    top: 50%;
    transform: translateY(-50%);
    font-size: 24px;
    animation: sparkle 2s infinite 1s;
}

@keyframes sparkle {
    0% { opacity: 0; transform: translateY(-50%) scale(0.5); }
    50% { opacity: 1; transform: translateY(-50%) scale(1.2); }
    100% { opacity: 0; transform: translateY(-50%) scale(0.5); }
}

.btn:active {
    transform: translateY(5px);
    box-shadow: 0 2px 0 #b17e1a, 0 8px 20px black;
}

.error-msg {
    color: #ffb3b3;
    text-align: center;
    min-height: 24px;
    font-size: 16px;
    text-shadow: 0 0 8px #ff0000aa;
    margin: 10px 0 0;
}

/* رسالة التهنئة - تصميم فاخر */
.message-card {
    background: rgba(8, 25, 38, 0.7);
    border: 3px solid #ffd700;
    padding: 35px 25px;
    text-align: center;
}

.profile-img {
    width: 120px;
    height: 120px;
    border-radius: 50%;
    border: 5px solid #ffd700;
    margin: 10px auto 20px;
    background: url('image00.jpg') center/cover;
    box-shadow: 0 0 40px #ffd700;
    animation: profileGlow 3s infinite alternate;
}

@keyframes profileGlow {
    0% { box-shadow: 0 0 20px #ffd700; }
    100% { box-shadow: 0 0 50px #ffaa00, 0 0 20px white; }
}

.message-title {
    font-size: 38px;
    background: linear-gradient(135deg, #fff6bf, #ffd700);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 20px;
    text-shadow: 0 0 15px gold;
}

.message-text {
    color: #ffffff;
    font-size: 22px;
    line-height: 2;
    background: rgba(0, 0, 0, 0.3);
    border-radius: 40px;
    padding: 25px;
    border: 1px solid rgba(255, 215, 0, 0.3);
    backdrop-filter: blur(5px);
}

.signature-area {
    margin-top: 30px;
    font-size: 28px;
    color: #ffd700;
    border-top: 2px dashed #ffd70080;
    padding-top: 25px;
    font-weight: bold;
}

.hidden {
    display: none;
}

.fade-in {
    animation: fadeIn 1s ease-in-out;
}

@keyframes fadeIn {
    0% { opacity: 0; transform: scale(0.9); }
    100% { opacity: 1; transform: scale(1); }
}

/* للشاشات الصغيرة */
@media (max-width: 480px) {
    .moon { font-size: 65px; }
    .lantern { font-size: 45px; }
    h1 { font-size: 30px; }
    .password-highlight { font-size: 28px; padding: 10px 20px; }
    .btn { font-size: 22px; }
    .message-text { font-size: 18px; padding: 20px; }
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

<!-- صفحة الدخول -->
<div class="card" id="loginBox">
    <div class="decoration-img"></div>
    <div class="content">
        <h1 class="glowing-text">🌙 إيهاب اهلاً 🌙</h1>
        
        <div class="welcome-box">
            <p>🔐 رمضانك أجمل مع</p>
            <div class="password-highlight">يوسف</div>
        </div>
        
        <input type="text" id="nameInput" class="input-field" placeholder="اكتب كلمة المرور هنا..." autocomplete="off">
        
        <button class="btn" onclick="checkName()">افتح الباب</button>
        <p id="error" class="error-msg"></p>
    </div>
</div>

<!-- صفحة التهاني بالصورة -->
<div class="card message-card hidden" id="messageBox">
    <div class="profile-img"></div>
    <h2 class="message-title">⭐ رمضان كريم ⭐</h2>
    
    <div class="message-text">
        <p>✨ باقة أزهار ورسالة عطرة ✨</p><br>
        <p>إلى إيهاب الغالي... 💙</p><br>
        بمناسبة حلول شهر رمضان المبارك 🌙<br>
        أقدم لك أسمى آيات التهاني والتبريكات ✨<br>
        أعاده الله عليك بالخير واليمن والبركات 🤍<br>
        وجعل أيامك كلها نجاح وتوفيق يا بطل 💫
    </div>
    
    <div class="signature-area">
        💙 أخوك يوسف 💙
    </div>
</div>

<audio id="ramadanSong" src="song00.mp3" preload="auto"></audio>

<script>
function checkName() {
    let correctName = "يوسف";
    let enteredName = document.getElementById("nameInput").value.trim();
    
    if (enteredName === correctName) {
        // إخفاء صفحة الدخول وإظهار صفحة التهاني
        document.getElementById("loginBox").classList.add("hidden");
        document.getElementById("messageBox").classList.remove("hidden");
        document.getElementById("messageBox").classList.add("fade-in");
        
        // تشغيل الأغنية
        let audio = document.getElementById("ramadanSong");
        audio.volume = 0.6;
        
        let playPromise = audio.play();
        
        if (playPromise !== undefined) {
            playPromise.catch(error => {
                console.log("التشغيل التلقائي محظور");
                
                // رسالة للمستخدم
                const msgBox = document.getElementById("messageBox");
                const tapMsg = document.createElement("p");
                tapMsg.style.color = "#ffd700";
                tapMsg.style.marginTop = "20px";
                tapMsg.style.fontSize = "18px";
                tapMsg.innerText = "👆 اضغط على الشاشة لتشغيل الأغنية";
                msgBox.appendChild(tapMsg);
                
                // تشغيل الأغنية عند أول لمسة
                document.body.addEventListener('touchstart', function playOnce() {
                    audio.play();
                    if (tapMsg) tapMsg.remove();
                    document.body.removeEventListener('touchstart', playOnce);
                }, { once: true });
            });
        }
    } else {
        document.getElementById("error").innerText = "❌ كلمة المرور غير صحيحة!";
        
        // تأثير اهتزاز
        document.getElementById("loginBox").style.animation = "shake 0.3s";
        setTimeout(() => {
            document.getElementById("loginBox").style.animation = "";
        }, 300);
    }
}

// إضافة تأثير اهتزاز للغلط
const style = document.createElement('style');
style.innerHTML = `
@keyframes shake {
    0%, 100% { transform: translateX(0); }
    25% { transform: translateX(-10px); }
    75% { transform: translateX(10px); }
}`;
document.head.appendChild(style);
</script>
</body>
</html>
