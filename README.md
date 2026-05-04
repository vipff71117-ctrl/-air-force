# -air-force
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>كتيبة الطيران</title>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box}
body{
    font-family:'Cairo',sans-serif;
    background: linear-gradient(135deg,#0b1a2b,#050d18);
    color:white;
}
header{
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:20px 40px;
    background:rgba(255,255,255,0.05);
    backdrop-filter: blur(10px);
    position:sticky;
    top:0;
}
nav a{
    color:white;
    margin:0 10px;
    text-decoration:none;
    transition:0.3s;
}
nav a:hover{color:#00c3ff}
.hero{
    text-align:center;
    padding:100px 20px;
}
.hero h1{
    font-size:40px;
}
.hero p{opacity:0.7;margin-top:10px}
section{padding:60px 20px;max-width:1100px;margin:auto}
.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}
.card{
    background:rgba(255,255,255,0.05);
    padding:20px;
    border-radius:15px;
    backdrop-filter: blur(8px);
    transition:0.3s;
}
.card:hover{
    transform:translateY(-5px);
    background:rgba(255,255,255,0.08);
}
img{
    width:100%;
    border-radius:15px;
}
button{
    background:#00c3ff;
    border:none;
    padding:12px;
    border-radius:8px;
    color:white;
    cursor:pointer;
    width:100%;
}
input,textarea{
    width:100%;
    padding:10px;
    margin:5px 0;
    border:none;
    border-radius:8px;
}
footer{
    text-align:center;
    padding:30px;
    opacity:0.6;
}
</style>
</head>
<body>

<header>
<h2>✈️ كتيبة الطيران</h2>
<nav>
<a href="#about">نبذة</a>
<a href="#rules">القوانين</a>
<a href="#tasks">المهام</a>
<a href="#gallery">الصور</a>
<a href="#apply">التقديم</a>
</nav>
</header>

<div class="hero">
<h1>Air Force Elite</h1>
<p>نخبة العمليات الجوية - قوة، انضباط، احتراف</p>
</div>

<section id="about">
<h2>📌 نبذة</h2>
<div class="card">كتيبة الطيران وحدة نخبة متخصصة في السيطرة الجوية وتنفيذ المهام العسكرية بدقة عالية.</div>
</section>

<section id="rules">
<h2>📜 القوانين</h2>
<div class="grid">
<div class="card">احترام الجميع</div>
<div class="card">تنفيذ الأوامر</div>
<div class="card">عدم الغياب</div>
<div class="card">التواصل الرسمي فقط</div>
</div>

<h2 style="margin-top:30px">📖 اللائحة</h2>
<div class="grid">
<div class="card">الترقية حسب الأداء</div>
<div class="card">إنذار ثم عقوبة</div>
<div class="card">فصل عند التكرار</div>
</div>
</section>

<section id="tasks">
<h2>🎯 المهام</h2>
<div class="grid">
<div class="card">دعم جوي</div>
<div class="card">استطلاع</div>
<div class="card">نقل القوات</div>
<div class="card">إنزال سريع</div>
</div>
</section>

<section id="gallery">
<h2>🖼️ الصور</h2>
<div class="grid">
<img src="https://images.unsplash.com/photo-1508614999368-9260051292e5">
<img src="https://images.unsplash.com/photo-1474302770737-173ee21bab63">
</div>
</section>

<section id="apply">
<h2>📝 التقديم</h2>
<div class="card">
<form onsubmit="send(event)">
<input type="text" placeholder="الاسم" required>
<input type="number" placeholder="العمر" required>
<textarea placeholder="خبراتك"></textarea>
<button>إرسال</button>
</form>
<p id="msg"></p>
</div>
</section>

<footer>© 2026 Air Force</footer>

<script>
function send(e){
e.preventDefault();
document.getElementById('msg').innerText='تم الإرسال بنجاح ✈️';
}
</script>

</body>
</html>