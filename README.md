<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>🌹 Educational Existence | Victor Munisi 🎓</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

/* ========= CINEMATIC PHOTO BACKGROUND ========= */

body{

background:
linear-gradient(
rgba(2,6,23,0.82),
rgba(15,23,42,0.78),
rgba(30,27,75,0.75),
rgba(14,165,233,0.55)
),
url("victor.jpg");

background-size:cover;
background-position:center;
background-attachment:fixed;

animation:bgZoom 20s ease infinite;

color:white;
overflow-x:hidden;

}

@keyframes bgZoom{
0%{
background-size:100%;
}

50%{
background-size:110%;
}

100%{
background-size:100%;
}
}


/* Floating glowing circles */

body::before,
body::after{

content:"";
position:fixed;

width:500px;
height:500px;

border-radius:50%;

filter:blur(120px);

opacity:0.35;

z-index:-1;

animation:float 12s infinite ease-in-out;
}

body::before{

background:#22d3ee;
top:-150px;
left:-150px;

}

body::after{

background:#a855f7;

bottom:-150px;
right:-150px;

}

@keyframes float{

0%,100%{
transform:translateY(0);
}

50%{
transform:translateY(80px);
}

}

/* ========= GLASS EFFECT ========= */

.glass{

background:rgba(255,255,255,0.08);

backdrop-filter:blur(25px);

border:1px solid rgba(255,255,255,0.18);

border-radius:25px;

box-shadow:
0 25px 60px rgba(0,0,0,0.35);

overflow:hidden;

}


/* ========= NAVIGATION ========= */

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

}


.logo{

font-size:1.3rem;

font-weight:700;

letter-spacing:1px;

}


nav a{

color:white;

text-decoration:none;

margin-left:18px;

transition:0.4s;

}


nav a:hover{

color:#22d3ee;

}


nav button{

margin-left:15px;

padding:8px 18px;

border:none;

border-radius:25px;

cursor:pointer;

background:
linear-gradient(135deg,#22d3ee,#a855f7);

color:white;

}


/* ========= SECTIONS ========= */

section{

padding:120px 8%;

}


h2{

font-size:3rem;

text-align:center;

margin-bottom:40px;

}


/* ========= HERO ========= */

.hero{

min-height:100vh;

display:flex;

justify-content:space-between;

align-items:center;

gap:40px;

}


.hero-text{

max-width:50%;

padding:35px;

animation:fadeUp 1.5s ease;

}


@keyframes fadeUp{

from{

opacity:0;

transform:translateY(50px);

}

to{

opacity:1;

transform:translateY(0);

}

}


.hero h1{

font-size:4rem;

line-height:1.2;

background:
linear-gradient(
90deg,
#fff,
#22d3ee,
#a855f7,
#fff);

-webkit-background-clip:text;

-webkit-text-fill-color:transparent;

}


.hero p{

margin-top:20px;

font-size:1.15rem;

line-height:1.8;

}


.btn{

margin-top:25px;

padding:16px 35px;

border:none;

border-radius:50px;

color:white;

cursor:pointer;

font-size:1rem;

background:
linear-gradient(
135deg,
#22d3ee,
#a855f7,
#ec4899);

transition:0.4s;

}


.btn:hover{

transform:scale(1.08);

box-shadow:
0 0 35px #22d3ee;

}

#globe{

width:400px;
height:400px;

}
/* ========= GRIDS & CARDS ========= */

.grid{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:25px;

}


.card{

padding:30px;

transition:0.5s;

}


.card:hover{

transform:
translateY(-10px);

box-shadow:
0 0 35px rgba(34,211,238,0.7);

}


.card h3{

font-size:1.4rem;

margin-bottom:15px;

color:#22d3ee;

}


.card p{

line-height:1.7;

}


/* ========= GALLERY ========= */

.gallery{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:20px;

}


.gallery img{

width:100%;

height:230px;

object-fit:cover;

border-radius:20px;

transition:0.5s;

}


.gallery img:hover{

transform:scale(1.05);

}


/* ========= VIDEOS ========= */

iframe{

width:100%;

height:250px;

border:none;

border-radius:20px;

}


/* ========= FORMS ========= */

form{

display:flex;

flex-direction:column;

gap:15px;

}


input,
textarea{

padding:15px;

border:none;

border-radius:15px;

background:
rgba(255,255,255,0.12);

color:white;

outline:none;

}


input::placeholder,
textarea::placeholder{

color:#ddd;

}


button{

padding:13px;

border:none;

border-radius:15px;

cursor:pointer;

font-weight:600;

}


/* ========= AI CHATBOT ========= */

#chatbot{

position:fixed;

bottom:20px;

right:20px;

width:280px;

padding:15px;

z-index:1000;

}


#chatlog{

height:120px;

overflow-y:auto;

margin-bottom:10px;

font-size:0.9rem;

}


/* ========= LOGIN ========= */

.login{

position:fixed;

top:85px;

right:20px;

padding:15px;

display:none;

z-index:1000;

}


/* ========= ADMIN PANEL ========= */

#admin{

position:fixed;

top:85px;

left:20px;

padding:15px;

display:none;

z-index:1000;

}


/* ========= RESPONSIVE DESIGN ========= */

@media(max-width:900px){

.hero{

flex-direction:column;

text-align:center;

}


.hero-text{

max-width:100%;

}


.hero h1{

font-size:2.8rem;

}


#globe{

width:300px;

height:300px;

}


nav{

flex-direction:column;

gap:15px;

}

}


/* ========= END OF CSS ========= */

</style>

</head>


<body>


<!-- ========= NAVIGATION ========= -->


<nav class="glass">


<div class="logo">

🌹 Educational Existence 🎓

</div>


<div>

<a href="#about">About</a>

<a href="#history">
History
</a>

<a href="#courses">
Courses
</a>


<a href="#gallery">
Gallery
</a>


<a href="#videos">
Videos
</a>


<a href="#contact">
Inquiry
</a>


<button onclick="showLogin()">

Login

</button>


<button onclick="showAdmin()">

Admin

</button>


</div>


</nav>



<!-- ========= HERO SECTION ========= -->


<section class="hero">


<div class="hero-text glass">


<h1>

🎓 Educational Existence ✨

</h1>


<p>

🌹 Welcome to Victor Munisi's world where 
knowledge becomes power,
technology meets creativity,
and every student can shine.
He is the creator of this website
Email : victorbob025@gmail.com
Phone number : +255613306940

Explore AI 🤖, coding 💻,
science 🔬, mathematics 📐,
and limitless opportunities 🌍✨.

</p>


<button class="btn">

🚀 Start Learning Journey

</button>


</div>


<div id="globe">

</div>


</section>


<!-- ========= ABOUT SECTION ========= -->


<section id="about">


<h2>

📚 About Education

</h2>


<div class="grid">
<div class="glass card">

<h3>
🌱 What is Education?
</h3>

<p>
Education is the journey of gaining knowledge, skills,
values and wisdom that helps individuals grow and
contribute positively to the world.
</p>

</div>


<div class="glass card">

<h3>
🌍 Why Education Matters
</h3>

<p>
Education fights poverty, encourages innovation,
creates leaders and builds a better future for humanity.
</p>

</div>


<div class="glass card">

<h3>
🚀 Future of Learning
</h3>

<p>
Artificial Intelligence 🤖, Virtual Reality 🥽,
online classes 💻 and advanced technology are changing
how students learn across the globe.
</p>

</div>


</div>

</section>



<!-- ========= STATISTICS ========= -->


<section>

<h2>
📊 Educational Statistics
</h2>


<div class="grid">


<div class="glass card">

<h3>
5000+
</h3>

<p>
Happy Students 👨‍🎓👩‍🎓
</p>

</div>


<div class="glass card">

<h3>
100+
</h3>

<p>
Professional Courses 📚
</p>

</div>


<div class="glass card">

<h3>
50+
</h3>

<p>
Learning Resources 📖
</p>

</div>


<div class="glass card">

<h3>
20+
</h3>

<p>
Academic Subjects 🧪
</p>

</div>


</div>

</section>



<!-- ========= HISTORY ========= -->


<section id="history">


<h2>
🏛 History of Education
</h2>


<div class="glass card">


<p>

Education has evolved from ancient civilizations such as
Egypt, Mesopotamia and Greece to today's digital era.
Modern technology now connects millions of learners
through online platforms, AI and interactive experiences.

</p>


</div>


</section>



<!-- ========= COURSES ========= -->


<section id="courses">


<h2>
🎯 Our Courses
</h2>


<div class="grid">


<div class="glass card">

<h3>
📐 Mathematics
</h3>

<p>
Algebra, Geometry, Calculus and problem-solving skills.
</p>

</div>



<div class="glass card">

<h3>
🔬 Science
</h3>

<p>
Physics, Chemistry, Biology and scientific discovery.
</p>

</div>



<div class="glass card">

<h3>
💻 Technology
</h3>

<p>
Programming, Artificial Intelligence and digital skills.
</p>

</div>



<div class="glass card">

<h3>
💼 Business
</h3>

<p>
Finance, Entrepreneurship and Marketing strategies.
</p>

</div>


</div>


</section>



<!-- ========= GALLERY ========= -->


<section id="gallery">


<h2>
🖼 Student Gallery
</h2>


<div class="gallery">


<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">


<img src="https://images.unsplash.com/photo-1513258496099-48168024aec0">


<img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b">


</div>


</section>



<!-- ========= VIDEOS ========= -->


<section id="videos">


<h2>
🎥 Educational Videos
</h2>


<div class="grid">


<iframe
src="https://www.youtube.com/embed/WXuK6gekU1Y">
</iframe>


<iframe
src="https://www.youtube.com/embed/pJ0auP7dbcY">
</iframe>


</div>


</section>



<!-- ========= INQUIRY FORM ========= -->


<section id="contact">


<h2>
📩 Contact & Inquiry
</h2>


<div class="glass card">


<form action="https://formsubmit.co/victorbob025@gmail.com"
method="POST">


<input
type="text"
placeholder="👤 Your Name"
required>


<input
type="email"
placeholder="📧 Your Email"
required>


<textarea
placeholder="💬 Write your message..."
required>
</textarea>


<button type="submit">

🚀 Send Message

</button>


</form>


</div>


</section>
<!-- ========= AI CHATBOT ========= -->

<div class="glass" id="chatbot">

<h4>
🤖 AI Learning Assistant
</h4>

<div id="chatlog">

🌟 Hello learner! Ask me about education, AI, science, or history.

</div>


<input 
id="chatInput"
placeholder="💬 Ask me anything...">


<button onclick="chat()">

📨 Send

</button>


</div>



<!-- ========= LOGIN PANEL ========= -->

<div class="glass login" id="loginBox">


<h3>
🔐 Student Login
</h3>


<input 
id="user"
placeholder="👤 Enter your name">


<button onclick="login()">

✨ Login

</button>


</div>



<!-- ========= ADMIN PANEL ========= -->


<div class="glass" id="admin">


<h3>
👨‍💻 Admin Dashboard
</h3>


<p>
Registered Users:
</p>


<p id="count">

0

</p>


</div>



<!-- ========= JAVASCRIPT ========= -->


<script>


/* ===== 3D ROTATING GLOBE ===== */


const scene = new THREE.Scene();


const camera = new THREE.PerspectiveCamera(
75,
1,
0.1,
1000
);


const renderer = new THREE.WebGLRenderer({
alpha:true
});


renderer.setSize(400,400);


document
.getElementById("globe")
.appendChild(renderer.domElement);



const sphere = new THREE.Mesh(

new THREE.SphereGeometry(
2,
32,
32
),


new THREE.MeshBasicMaterial({

wireframe:true,
color:0x22d3ee

})

);


scene.add(sphere);


camera.position.z = 5;



function animate(){

requestAnimationFrame(animate);


sphere.rotation.y += 0.01;


sphere.rotation.x += 0.003;


renderer.render(
scene,
camera
);

}


animate();



/* ===== AI CHATBOT ===== */


function chat(){


let input =
document.getElementById("chatInput")
.value.toLowerCase();


let log =
document.getElementById("chatlog");


let reply =
"🤖 I am your AI educational assistant. Ask me about learning!";


if(input.includes("history")){

reply =
"🏛 Education started in ancient civilizations like Egypt, Greece and Mesopotamia.";

}


else if(input.includes("ai")){

reply =
"🤖 Artificial Intelligence helps students learn through smart tools and personalized education.";

}


else if(input.includes("science")){

reply =
"🔬 Science helps us understand nature through observation and experiments.";

}


else if(input.includes("math")){

reply =
"📐 Mathematics is the language of logic, numbers and problem solving.";

}



log.innerHTML += 
"<br><br>👤 You: " 
+ input +
"<br>🤖 AI: "
+ reply;


document.getElementById("chatInput")
.value = "";


}



/* ===== LOGIN SYSTEM ===== */


function login(){


let username =
document.getElementById("user")
.value;


localStorage.setItem(
"user",
username
);


alert(
"🌹 Welcome " +
username +
" to Educational Existence 🎓✨"
);


}



/* ===== ADMIN PANEL ===== */


function showAdmin(){


document
.getElementById("admin")
.style.display =
"block";


let users =
localStorage.getItem("user")
? 1 : 0;


document.getElementById("count")
.innerHTML =
"👥 " + users + " Student(s)";


}



/* ===== SHOW LOGIN ===== */


function showLogin(){


document
.getElementById("loginBox")
.style.display =
"block";


}


</script>



</body>
