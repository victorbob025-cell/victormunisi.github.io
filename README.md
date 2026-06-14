<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Educational Existence | Victor Munisi</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

/* =========================
   LIQUID GLASS UPGRADED UI
========================= */

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
color:white;
overflow-x:hidden;

/* Animated futuristic background */
background:linear-gradient(135deg,#020617,#0f172a,#1e1b4b,#0ea5e9);
background-size:400% 400%;
animation:moveBG 18s ease infinite;
}

@keyframes moveBG{
0%{background-position:0% 50%;}
50%{background-position:100% 50%;}
100%{background-position:0% 50%;}
}

/* Floating glowing blobs */
body::before,
body::after{
content:"";
position:fixed;
width:500px;
height:500px;
border-radius:50%;
filter:blur(120px);
opacity:.5;
z-index:-1;
animation:float 12s ease-in-out infinite;
}

body::before{background:#22d3ee;top:-150px;left:-150px;}
body::after{background:#a855f7;bottom:-150px;right:-150px;}

@keyframes float{
0%,100%{transform:translateY(0);}
50%{transform:translateY(80px);}
}

/* =========================
   GLASS EFFECT CORE
========================= */

.glass{
background:rgba(255,255,255,0.06);
backdrop-filter:blur(25px) saturate(180%);
-webkit-backdrop-filter:blur(25px) saturate(180%);
border:1px solid rgba(255,255,255,0.15);
border-radius:25px;
box-shadow:0 25px 60px rgba(0,0,0,0.3);
position:relative;
overflow:hidden;
}

.glass::before{
content:"";
position:absolute;
top:-50%;
left:-60%;
width:40%;
height:200%;
background:linear-gradient(90deg,transparent,rgba(255,255,255,0.25),transparent);
transform:rotate(20deg);
animation:shine 7s infinite;
}

@keyframes shine{
0%{left:-60%;}
100%{left:160%;}
}

/* =========================
   NAVBAR
========================= */

nav{
position:fixed;
top:0;
width:100%;
display:flex;
justify-content:space-between;
align-items:center;
padding:18px 8%;
z-index:1000;

background:rgba(255,255,255,0.05);
backdrop-filter:blur(30px);
border-bottom:1px solid rgba(255,255,255,0.1);
}

.logo{font-size:26px;font-weight:800;}

nav ul{display:flex;gap:25px;list-style:none;}

nav a{
text-decoration:none;
color:white;
transition:.3s;
}

nav a:hover{
color:#22d3ee;
text-shadow:0 0 10px #22d3ee;
}

/* =========================
   SECTIONS
========================= */

section{padding:120px 8%;}

h2{
text-align:center;
font-size:3rem;
margin-bottom:50px;
}

/* =========================
   HERO
========================= */

.hero{
min-height:100vh;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
}

.hero-content{
padding:60px;
max-width:900px;
}

.hero h1{
font-size:4.5rem;
background:linear-gradient(90deg,#fff,#22d3ee,#a855f7,#fff);
background-size:300%;
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
animation:textFlow 8s linear infinite;
}

@keyframes textFlow{
0%{background-position:0%;}
100%{background-position:300%;}
}

.hero p{margin-top:20px;font-size:1.1rem;opacity:.9;}

.btn{
display:inline-block;
margin-top:30px;
padding:15px 35px;
border-radius:50px;
background:linear-gradient(135deg,#22d3ee,#a855f7,#ec4899);
color:white;
text-decoration:none;
font-weight:600;
}

/* =========================
   GRID + CARDS
========================= */

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:25px;
}

.card{
padding:30px;
transition:.4s;
}

.card:hover{
transform:translateY(-10px) rotateX(8deg);
}

/* =========================
   GALLERY
========================= */

.gallery{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:20px;
}

.gallery img{
width:100%;
height:250px;
object-fit:cover;
border-radius:20px;
transition:.4s;
}

.gallery img:hover{transform:scale(1.08);}

/* =========================
   VIDEO
========================= */

.video-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(350px,1fr));
gap:20px;
}

iframe{
width:100%;
height:280px;
border:none;
border-radius:20px;
}

/* =========================
   STATS
========================= */

.stats{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px;
text-align:center;
}

.stat h3{
font-size:3rem;
color:#22d3ee;
text-shadow:0 0 15px #22d3ee;
}

/* =========================
   FAQ
========================= */

.faq details{
padding:20px;
cursor:pointer;
}

/* =========================
   FORM
========================= */

form{
display:flex;
flex-direction:column;
gap:15px;
}

input,textarea{
padding:15px;
border:none;
border-radius:15px;
background:rgba(255,255,255,0.08);
color:white;
}

button{
padding:15px;
border:none;
border-radius:15px;
background:linear-gradient(135deg,#22d3ee,#a855f7,#ec4899);
color:white;
font-weight:600;
cursor:pointer;
}

/* =========================
   FOOTER
========================= */

footer{
text-align:center;
padding:50px;
margin-top:50px;
}

/* =========================
   MOBILE
========================= */

@media(max-width:768px){
.hero h1{font-size:2.5rem;}
nav ul{display:none;}
}

</style>
</head>

<body>

<!-- NAV -->
<nav class="glass">
<div class="logo">Educational Existence</div>
<ul>
<li><a href="#about">About</a></li>
<li><a href="#history">History</a></li>
<li><a href="#courses">Courses</a></li>
<li><a href="#gallery">Gallery</a></li>
<li><a href="#videos">Videos</a></li>
<li><a href="#contact">Inquiry</a></li>
</ul>
</nav>

<!-- HERO -->
<section class="hero">
<div class="glass hero-content">
<h1>Educational Existence</h1>
<p>
A modern educational platform dedicated to knowledge, innovation,
research, and academic excellence worldwide.
</p>
<a class="btn" href="#contact">Start Learning</a>
</div>
</section>

<!-- ABOUT -->
<section id="about">
<h2>About Education</h2>

<div class="grid">

<div class="glass card">
<h3>What is Education?</h3>
<p>Education is acquiring knowledge, skills, values, and habits through learning and experience.</p>
</div>

<div class="glass card">
<h3>Why Education Matters</h3>
<p>It reduces poverty, builds innovation, and improves society.</p>
</div>

<div class="glass card">
<h3>Future of Learning</h3>
<p>AI, VR, and online platforms are transforming education globally.</p>
</div>

</div>
</section>

<!-- STATS -->
<section>
<h2>Statistics</h2>

<div class="stats">
<div class="glass card"><h3>5000+</h3><p>Students</p></div>
<div class="glass card"><h3>100+</h3><p>Courses</p></div>
<div class="glass card"><h3>50+</h3><p>Resources</p></div>
<div class="glass card"><h3>20+</h3><p>Subjects</p></div>
</div>

</section>

<!-- HISTORY -->
<section id="history">
<h2>History of Education</h2>

<div class="glass card">
<p><b>Ancient Egypt:</b> Writing, math, and administration.</p>
<p><b>Mesopotamia:</b> Early schools and cuneiform writing.</p>
<p><b>Ancient Greece:</b> Philosophy by Socrates, Plato, Aristotle.</p>
<p><b>Modern Era:</b> Digital and online learning systems.</p>
</div>

</section>

<!-- COURSES -->
<section id="courses">
<h2>Courses</h2>

<div class="grid">

<div class="glass card"><h3>Mathematics</h3><p>Algebra, Calculus, Geometry</p></div>
<div class="glass card"><h3>Science</h3><p>Physics, Chemistry, Biology</p></div>
<div class="glass card"><h3>Technology</h3><p>Programming, AI, Cybersecurity</p></div>
<div class="glass card"><h3>Business</h3><p>Finance, Marketing, Entrepreneurship</p></div>

</div>
</section>

<!-- GALLERY -->
<section id="gallery">
<h2>Gallery</h2>

<div class="gallery">
<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<img src="https://images.unsplash.com/photo-1513258496099-48168024aec0">
<img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b">
</div>

</section>

<!-- VIDEOS -->
<section id="videos">
<h2>Videos</h2>

<div class="video-grid">
<iframe src="https://www.youtube.com/embed/WXuK6gekU1Y"></iframe>
<iframe src="https://www.youtube.com/embed/pJ0auP7dbcY"></iframe>
</div>

</section>

<!-- FAQ -->
<section>
<h2>FAQ</h2>

<div class="glass faq">
<details>
<summary>What is education?</summary>
<p>Education is learning knowledge and skills.</p>
</details>
</div>

<div class="glass faq">
<details>
<summary>Why is education important?</summary>
<p>It improves opportunities and development.</p>
</details>
</div>

</section>

<!-- INQUIRY -->
<section id="contact">
<h2>Inquiry Form</h2>

<div class="glass card">

<form action="https://formsubmit.co/victorbob025@gmail.com" method="POST">

<input type="text" name="name" placeholder="Full Name" required>
<input type="email" name="email" placeholder="Email" required>
<textarea name="message" placeholder="Write your inquiry..." required></textarea>

<button type="submit">Submit Inquiry</button>

</form>

</div>
</section>

<!-- FOOTER -->
<footer class="glass">
<p><b>Educational Existence</b></p>
<p>Creator: Victor Munisi</p>
<p>Email: victorbob025@gmail.com</p>
<p>© 2026 All Rights Reserved</p>
</footer>

</body>
