<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Educational Existence | Victor Munisi</title><link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet"><style>

:root{
--primary:#00c6ff;
--secondary:#0072ff;
--glass:rgba(255,255,255,0.08);
--border:rgba(255,255,255,0.15);
--text:#ffffff;
}

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
scroll-behavior:smooth;
}

body{
background:linear-gradient(135deg,#020617,#0f172a,#0ea5e9);
color:white;
overflow-x:hidden;
}

.video-bg{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
object-fit:cover;
z-index:-2;
opacity:.25;
}

.overlay{
position:fixed;
width:100%;
height:100%;
background:rgba(0,0,0,.55);
z-index:-1;
}

nav{
position:fixed;
width:100%;
padding:20px 8%;
display:flex;
justify-content:space-between;
align-items:center;
backdrop-filter:blur(20px);
background:rgba(255,255,255,.05);
border-bottom:1px solid rgba(255,255,255,.08);
z-index:999;
}

.logo{
font-size:30px;
font-weight:800;
}

nav ul{
display:flex;
gap:25px;
list-style:none;
}

nav a{
text-decoration:none;
color:white;
font-weight:500;
}

section{
padding:120px 8%;
}

.glass{
background:var(--glass);
backdrop-filter:blur(20px);
border:1px solid var(--border);
border-radius:30px;
box-shadow:0 25px 45px rgba(0,0,0,.25);
}

.hero{
min-height:100vh;
display:flex;
align-items:center;
justify-content:center;
text-align:center;
}

.hero-content{
padding:60px;
max-width:1000px;
}

.hero h1{
font-size:5rem;
margin-bottom:20px;
}

.hero p{
font-size:1.2rem;
line-height:1.8;
}

.btn{
display:inline-block;
margin-top:30px;
padding:15px 35px;
border-radius:50px;
background:linear-gradient(45deg,var(--primary),var(--secondary));
text-decoration:none;
color:white;
font-weight:600;
}

h2{
text-align:center;
font-size:3rem;
margin-bottom:50px;
}

.grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:30px;
}

.card{
padding:30px;
transition:.4s;
transform-style:preserve-3d;
}

.card:hover{
transform:translateY(-10px) rotateX(8deg);
}

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
}

.video-grid{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(400px,1fr));
gap:20px;
}

iframe{
width:100%;
height:280px;
border:none;
border-radius:20px;
}

.stats{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
gap:20px;
text-align:center;
}

.stat{
padding:30px;
}

.stat h3{
font-size:3rem;
}

.timeline{
border-left:3px solid white;
padding-left:25px;
}

.timeline div{
margin-bottom:40px;
}

form{
display:flex;
flex-direction:column;
gap:15px;
}

input,textarea{
padding:15px;
border:none;
border-radius:15px;
background:rgba(255,255,255,.08);
color:white;
}

button{
padding:15px;
border:none;
border-radius:15px;
background:linear-gradient(45deg,#00c6ff,#0072ff);
color:white;
font-size:16px;
cursor:pointer;
}

footer{
padding:50px;
text-align:center;
margin-top:50px;
}

.faq{
margin-bottom:20px;
padding:25px;
}

details{
cursor:pointer;
}

summary{
font-size:18px;
font-weight:600;
}

@media(max-width:768px){

.hero h1{
font-size:2.8rem;
}

nav ul{
display:none;
}

.video-grid{
grid-template-columns:1fr;
}

}

</style></head><body><video autoplay muted loop class="video-bg">
<source src="education.mp4" type="video/mp4">
</video><div class="overlay"></div><nav>
<div class="logo">Educational Existence</div><ul>
<li><a href="#about">About</a></li>
<li><a href="#history">History</a></li>
<li><a href="#courses">Courses</a></li>
<li><a href="#gallery">Gallery</a></li>
<li><a href="#videos">Videos</a></li>
<li><a href="#contact">Inquiry</a></li>
</ul>
</nav><section class="hero"><div class="glass hero-content"><h1>Educational Existence</h1><p>
Educational Existence is a modern educational platform dedicated to promoting
knowledge, learning, innovation, research, and academic excellence.
Explore the history of education, learning resources, educational videos,
courses, and future learning technologies.
</p><a href="#contact" class="btn">Start Learning</a>

</div></section><section id="about"><h2>About Education</h2><div class="grid"><div class="glass card">
<h3>What is Education?</h3>
<p>
Education is the process of acquiring knowledge, skills, values,
beliefs, and habits through teaching, training, research,
or practical experience.
</p>
</div><div class="glass card">
<h3>Why Education Matters</h3>
<p>
Education empowers individuals, reduces poverty, drives innovation,
and contributes to social and economic development.
</p>
</div><div class="glass card">
<h3>Future of Learning</h3>
<p>
Artificial Intelligence, online learning, virtual reality,
and personalized education are transforming the future.
</p>
</div></div></section><section><h2>Educational Statistics</h2><div class="stats"><div class="glass stat">
<h3>5000+</h3>
<p>Students</p>
</div><div class="glass stat">
<h3>100+</h3>
<p>Courses</p>
</div><div class="glass stat">
<h3>50+</h3>
<p>Resources</p>
</div><div class="glass stat">
<h3>20+</h3>
<p>Subjects</p>
</div></div></section><section id="history"><h2>History of Education</h2><div class="glass card timeline"><div>
<h3>Ancient Egypt</h3>
<p>
Education focused on writing, mathematics,
administration, and religious studies.
</p>
</div><div>
<h3>Mesopotamia</h3>
<p>
Schools taught reading, writing,
and record keeping using cuneiform scripts.
</p>
</div><div>
<h3>Ancient Greece</h3>
<p>
Philosophers such as Socrates, Plato,
and Aristotle shaped educational thinking.
</p>
</div><div>
<h3>Modern Education</h3>
<p>
Technology, online learning,
and global connectivity have transformed education.
</p>
</div></div></section><section id="courses"><h2>Popular Courses</h2><div class="grid"><div class="glass card">
<h3>Mathematics</h3>
<p>Algebra, Calculus, Geometry.</p>
</div><div class="glass card">
<h3>Science</h3>
<p>Physics, Chemistry, Biology.</p>
</div><div class="glass card">
<h3>Technology</h3>
<p>Programming, AI, Cybersecurity.</p>
</div><div class="glass card">
<h3>Business</h3>
<p>Entrepreneurship, Finance, Marketing.</p>
</div></div></section><section id="gallery"><h2>Educational Gallery</h2><div class="gallery"><img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f">
<img src="https://images.unsplash.com/photo-1513258496099-48168024aec0">
<img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b">
<img src="https://images.unsplash.com/photo-1541339907198-e08756dedf3f">
<img src="https://images.unsplash.com/photo-1524995997946-a1c2e315a42f">
<img src="https://images.unsplash.com/photo-1523580494863-6f3031224c94"></div></section><section id="videos"><h2>Educational Videos</h2><div class="video-grid"><iframe src="https://www.youtube.com/embed/WXuK6gekU1Y"></iframe><iframe src="https://www.youtube.com/embed/pJ0auP7dbcY"></iframe></div></section><section><h2>Frequently Asked Questions</h2><div class="glass faq">
<details>
<summary>What is education?</summary>
<p>Education is the acquisition of knowledge and skills.</p>
</details>
</div><div class="glass faq">
<details>
<summary>Why is education important?</summary>
<p>It improves opportunities, knowledge, and development.</p>
</details>
</div><div class="glass faq">
<details>
<summary>Can learning happen online?</summary>
<p>Yes. Modern technology enables learning from anywhere.</p>
</details>
</div></section><section id="contact"><h2>Inquiry Form</h2><div class="glass card"><form action="https://formsubmit.co/victorbob025@gmail.com" method="POST"><input type="text" name="name" placeholder="Full Name" required><input type="email" name="email" placeholder="Email Address" required><input type="tel" name="phone" placeholder="Phone Number"><input type="text" name="country" placeholder="Country"><input type="text" name="subject" placeholder="Subject"><textarea name="message" rows="6" placeholder="Write your inquiry..." required></textarea><button type="submit">Submit Inquiry</button>

</form></div></section><footer class="glass"><h3>Educational Existence</h3><p><strong>Creator:</strong> Victor Munisi</p><p><strong>Phone:</strong> +255 613 306 940</p><p><strong>Email:</strong> victorbob025@gmail.com</p><p>© 2026 Educational Existence. All Rights Reserved.</p></footer></body>
</html>
