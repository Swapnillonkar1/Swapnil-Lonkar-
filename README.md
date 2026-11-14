<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Swapnil Lahu Lonkar | Engineering Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Space+Grotesk:wght@500;600;700&display=swap" rel="stylesheet">

<style>
:root {
    --bg: #07111f;
    --panel: #0d1b2c;
    --panel2: #102238;
    --line: #20364d;
    --cyan: #48d7f4;
    --violet: #a78bfa;
    --white: #edf5ff;
    --muted: #a5b5c8;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 90px;
}

body {
    font-family: "DM Sans", sans-serif;
    background: radial-gradient(ellipse at 75% 0%, #173653 0%, var(--bg) 48%);
    color: var(--white);
    line-height: 1.7;
}

a {
    color: inherit;
    text-decoration: none;
}

.container {
    width: min(1120px, calc(100% - 40px));
    margin: auto;
}

header {
    position: sticky;
    top: 0;
    z-index: 10;
    background: #07111fef;
    backdrop-filter: blur(16px);
    border-bottom: 1px solid var(--line);
}

.nav {
    min-height: 72px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
}

.brand {
    font: 700 23px "Space Grotesk";
    color: var(--cyan);
}

nav {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
}

nav a {
    font-size: 13px;
    color: var(--muted);
}

nav a:hover {
    color: var(--cyan);
}

/* HERO */

.hero {
    display: grid;
    grid-template-columns: 1.45fr .8fr;
    gap: 45px;
    align-items: center;
    padding: 90px 0 55px;
}

.eyebrow {
    color: var(--cyan);
    font-size: 12px;
    font-weight: 700;
    letter-spacing: 2px;
    text-transform: uppercase;
}

h1, h2, h3 {
    font-family: "Space Grotesk", sans-serif;
    line-height: 1.25;
}

h1 {
    font-size: clamp(38px, 6vw, 66px);
    margin: 14px 0;
}

.gradient {
    background: linear-gradient(100deg, var(--cyan), var(--violet));
    -webkit-background-clip: text;
    background-clip: text;
    color: transparent;
}

.role {
    font-size: 19px;
    color: #c5d5e7;
    margin-bottom: 18px;
}

.lead {
    max-width: 680px;
    color: var(--muted);
    font-size: 15px;
}

.tags, .chips {
    display: flex;
    flex-wrap: wrap;
    gap: 9px;
    margin: 22px 0;
}

.tag, .chip {
    font-size: 11px;
    border: 1px solid var(--line);
    border-radius: 30px;
    padding: 6px 11px;
    color: #c9d9e9;
    background: #0b1a2a;
}

.actions {
    display: flex;
    flex-wrap: wrap;
    gap: 12px;
    margin: 25px 0;
}

.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 11px 18px;
    border-radius: 30px;
    font-size: 13px;
    font-weight: 700;
    transition: .2s;
}

.primary {
    background: linear-gradient(110deg, var(--cyan), #9b9cfb);
    color: #07111f;
}

.secondary {
    border: 1px solid #3d6683;
    color: var(--cyan);
}

.btn:hover {
    transform: translateY(-3px);
}

/* PROFILE CARD */

.hero-card, .card {
    background: linear-gradient(145deg, #10243a, #0b1727);
    border: 1px solid var(--line);
    border-radius: 20px;
    box-shadow: 0 18px 50px #0003;
}

.hero-card {
    padding: 28px;
    text-align: center;
}

.avatar {
    height: 112px;
    width: 112px;
    margin: 0 auto 17px;
    border-radius: 50%;
    display: grid;
    place-items: center;
    background: linear-gradient(135deg, var(--cyan), var(--violet));
    color: #081321;
    font: 700 38px "Space Grotesk";
    border: 5px solid #1b3852;
}

.hero-card h2 {
    font-size: 20px;
}

.hero-card p {
    color: var(--muted);
    font-size: 12px;
    margin: 5px 0 20px;
}

.stats {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
}

.stat {
    background: #081625;
    border: 1px solid var(--line);
    border-radius: 14px;
    padding: 13px;
}

.stat strong {
    display: block;
    color: var(--cyan);
    font: 700 24px "Space Grotesk";
}

.stat span {
    font-size: 11px;
    color: var(--muted);
}

/* SECTIONS */

section {
    padding: 48px 0 8px;
}

.section-head {
    margin-bottom: 22px;
}

.section-head h2 {
    font-size: 30px;
    margin-bottom: 5px;
}

.section-head h2 span {
    color: var(--cyan);
}

.section-head p, .muted {
    font-size: 13px;
    color: var(--muted);
}

.card {
    padding: 22px;
    transition: .25s;
}

.card:hover {
    transform: translateY(-4px);
    border-color: #3b7796;
}

.card h3 {
    font-size: 17px;
    margin-bottom: 5px;
}

.meta {
    font-size: 12px;
    color: var(--cyan);
    margin-bottom: 11px;
}

.card p {
    font-size: 13px;
    color: var(--muted);
}

.card ul {
    padding-left: 18px;
    margin-top: 9px;
}

.card li {
    font-size: 13px;
    color: var(--muted);
    margin: 4px 0;
}

.grid2 {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 17px;
}

.grid3 {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 17px;
}

.pill {
    display: inline-block;
    margin-top: 13px;
    padding: 4px 10px;
    border: 1px solid #2f627d;
    border-radius: 30px;
    color: var(--cyan);
    font-size: 10px;
}

/* SKILLS */

.skill-card h3 {
    font-size: 15px;
}

.skill-card .chips {
    margin-bottom: 0;
}

/* CERTIFICATIONS */

.cert-list {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 12px;
}

.cert {
    padding: 16px 18px;
    border-radius: 14px;
    background: var(--panel);
    border: 1px solid var(--line);
}

.cert strong {
    display: block;
    font-size: 13px;
}

.cert span {
    font-size: 11px;
    color: var(--muted);
}

/* CONTACT */

.contact-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
}

.contact-line {
    margin: 12px 0;
    color: var(--muted);
    font-size: 13px;
    overflow-wrap: anywhere;
}

.contact-line b {
    color: var(--cyan);
    display: block;
    font-size: 11px;
    text-transform: uppercase;
    letter-spacing: 1px;
}

.socials {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 18px;
}

.socials a {
    border: 1px solid var(--line);
    border-radius: 30px;
    padding: 8px 13px;
    color: var(--cyan);
    font-size: 12px;
}

footer {
    margin-top: 65px;
    padding: 25px 0;
    border-top: 1px solid var(--line);
    text-align: center;
    color: var(--muted);
    font-size: 12px;
}

/* RESPONSIVE */

@media(max-width:800px) {
    .hero {
        grid-template-columns: 1fr;
        padding-top: 55px;
    }

    .hero-card {
        max-width: 420px;
        width: 100%;
        margin: auto;
    }

    .grid3 {
        grid-template-columns: repeat(2, minmax(0, 1fr));
    }
}

@media(max-width:620px) {
    .nav {
        padding: 14px 0;
        align-items: flex-start;
        flex-direction: column;
    }

    nav {
        gap: 12px;
    }

    .grid2, .grid3, .cert-list, .contact-grid {
        grid-template-columns: 1fr;
    }

    .section-head h2 {
        font-size: 25px;
    }

    .container {
        width: min(100% - 28px, 1120px);
    }
}
</style>
</head>

<body>

<header>
<div class="container nav">

<a class="brand" href="#home">SL.</a>

<nav>
<a href="#about">About</a>
<a href="#education">Education</a>
<a href="#internships">Internships</a>
<a href="#skills">Skills</a>
<a href="#projects">Projects</a>
<a href="#certifications">Certifications</a>
<a href="#contact">Contact</a>
</nav>

</div>
</header>

<main class="container">

<!-- HERO SECTION -->

<section class="hero" id="home">

<div>

<div class="eyebrow">Electronics • Embedded • Hardware</div>

<h1>
Hi, I'm
<span class="gradient">Swapnil Lahu Lonkar</span>
</h1>

<div class="role">
B.Tech – Electronics & Telecommunication Engineering
</div>

<p class="lead">
Motivated Electronics and Telecommunication Engineering student
with knowledge of Embedded Systems, STM32, C programming and
Edge AI. Seeking opportunities in hardware and embedded domains
to apply technical skills in firmware development, circuit design
and real-time system applications.
</p>

<div class="tags">
<span class="tag">B.Tech 2023–2027</span>
<span class="tag">Embedded Systems</span>
<span class="tag">STM32</span>
<span class="tag">Embedded C</span>
<span class="tag">PCB Basics</span>
<span class="tag">Sensors & Interfacing</span>
</div>

<div class="actions">

<a class="btn primary" href="#projects">
Explore My Projects ↗
</a>

<a class="btn secondary"
href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
target="_blank">
Connect on LinkedIn
</a>

<a class="btn secondary"
href="mailto:swapnillonkar0606@gmail.com">
Email Me
</a>

</div>

<p class="muted">
Ahilyanagar, Maharashtra, India · +91 84830 40612
</p>

</div>

<aside class="hero-card">

<div class="avatar">SL</div>

<h2>Swapnil Lahu Lonkar</h2>

<p>MIT Academy of Engineering, Pune</p>

<div class="stats">

<div class="stat">
<strong>7.31</strong>
<span>CGPA / 10</span>
</div>

<div class="stat">
<strong>03</strong>
<span>Internship Programs</span>
</div>

<div class="stat">
<strong>04</strong>
<span>Academic Projects</span>
</div>

<div class="stat">
<strong>2027</strong>
<span>Expected Graduation</span>
</div>

</div>

</aside>

</section>

<!-- ABOUT -->

<section id="about">

<div class="section-head">
<h2>About <span>Me</span></h2>
<p>Professional profile and areas of interest</p>
</div>

<div class="card">

<h3>Building practical solutions with electronics and embedded technology</h3>

<p>
I am pursuing a B.Tech in Electronics and Telecommunication
Engineering at MIT Academy of Engineering, Pune. My technical
interests include embedded systems, microcontroller programming,
hardware development, circuit design and sensor interfacing.
Through academic projects, workshops and internship programs,
I continue to develop my technical foundation, teamwork and
problem-solving skills.
</p>

<span class="pill">
Interested in Hardware & Embedded Opportunities
</span>

</div>

</section>

<!-- EDUCATION -->

<section id="education">

<div class="section-head">
<h2>My <span>Education</span></h2>
<p>Academic qualifications</p>
</div>

<div class="grid2">

<article class="card">

<h3>MIT Academy of Engineering, Pune</h3>

<div class="meta">2023 – 2027 · B.Tech</div>

<p>Electronics and Telecommunication Engineering</p>

<p><b>CGPA: 7.31 / 10</b></p>

<span class="pill">Currently Pursuing</span>

</article>

<article class="card">

<h3>Sahyadri International Junior College, Ahilyanagar</h3>

<div class="meta">2023 · 12th Standard · MSBSHSE</div>

<p><b>Percentage: 71.67 / 100</b></p>

</article>

<article class="card">

<h3>Residential High School, Ahilyanagar</h3>

<div class="meta">2021 · 10th Standard · MSBSHSE</div>

<p><b>Percentage: 86.40 / 100</b></p>

</article>

</div>

</section>

<!-- INTERNSHIPS -->

<section id="internships">

<div class="section-head">
<h2>Internships & <span>Programs</span></h2>
<p>Internship and technology learning experience</p>
</div>

<div class="grid2">

<article class="card">

<h3>Cisco Networking Academy</h3>

<div class="meta">01 June 2025 – 30 August 2025</div>

<p><b>Cisco AICTE Virtual Internship Program 2025</b></p>

<p>
Developed knowledge of computer networking, networking
fundamentals, network security and LAN/WAN technologies.
</p>

<div class="chips">
<span class="chip">Computer Networking</span>
<span class="chip">Network Security</span>
<span class="chip">LAN & WAN</span>
</div>

</article>

<article class="card">

<h3>Edunet Foundation</h3>

<div class="meta">15 July 2025 – 07 August 2025</div>

<p>
<b>SkillsBuild & IBM Cloud Platform in Emerging Technologies
(AI & Cloud)</b>
</p>

<p>
Explored data analytics, cloud computing, IBM Cloud and
artificial intelligence.
</p>

<div class="chips">
<span class="chip">Data Analytics</span>
<span class="chip">Cloud Computing</span>
<span class="chip">IBM Cloud</span>
<span class="chip">AI</span>
</div>

</article>

<article class="card">

<h3>Eduskills</h3>

<div class="meta">01 July 2024 – 30 September 2024</div>

<p><b>Android Developer</b></p>

<p>
Built foundational knowledge in Android and mobile application
development, UI/UX design for mobile apps and problem solving.
</p>

<div class="chips">
<span class="chip">Android Development</span>
<span class="chip">Mobile Apps</span>
<span class="chip">UI/UX</span>
</div>

</article>

</div>

</section>

<!-- SKILLS -->

<section id="skills">

<div class="section-head">
<h2>Technical <span>Expertise</span></h2>
<p>Skills and technologies</p>
</div>

<div class="grid3">

<article class="card skill-card">

<h3>Programming</h3>

<div class="chips">
<span class="chip">C Programming</span>
<span class="chip">C++ Programming</span>
<span class="chip">Python Programming</span>
<span class="chip">Embedded C</span>
</div>

</article>

<article class="card skill-card">

<h3>Embedded & Electronics</h3>

<div class="chips">
<span class="chip">STM32</span>
<span class="chip">PCB Basics</span>
<span class="chip">Sensors & Interfacing</span>
<span class="chip">Microcontrollers</span>
</div>

</article>

<article class="card skill-card">

<h3>Communication Systems</h3>

<div class="chips">
<span class="chip">Digital Communication</span>
<span class="chip">Satellite Communication</span>
<span class="chip">Wireless Communication</span>
</div>

</article>

<article class="card skill-card">

<h3>Networking & Security</h3>

<div class="chips">
<span class="chip">Computer Networking</span>
<span class="chip">Network Security</span>
<span class="chip">LAN & WAN</span>
</div>

</article>

<article class="card skill-card">

<h3>Tools & Platforms</h3>

<div class="chips">
<span class="chip">MATLAB</span>
<span class="chip">Simulink</span>
<span class="chip">Arduino</span>
<span class="chip">IBM Cloud</span>
</div>

</article>

<article class="card skill-card">

<h3>Professional Skills</h3>

<div class="chips">
<span class="chip">Problem Solving</span>
<span class="chip">Teamwork</span>
<span class="chip">Communication</span>
<span class="chip">Interview Preparation</span>
</div>

</article>

</div>

</section>

<!-- PROJECTS -->

<section id="projects">

<div class="section-head">
<h2>Academic <span>Projects</span></h2>
<p>Projects included in my updated resume</p>
</div>

<div class="grid2">

<article class="card">

<h3>01 · Digital Wireless Communication Link over Satellite Using Simulink</h3>

<div class="meta">01 March 2025 – 30 April 2025</div>

<p>
Simulation-based project focused on a digital wireless
communication link over the GSAT-31 satellite and communication
system performance evaluation.
</p>

<p style="margin-top:9px">
Mentor: Prof. Vipin Yadav · Team size: 4
</p>

<div class="chips">
<span class="chip">MATLAB</span>
<span class="chip">Simulink</span>
<span class="chip">Digital Communication</span>
<span class="chip">GSAT-31</span>
</div>

<a class="project-link"
href="https://drive.google.com/file/d/1jTvDosoLyYf_YAJYFBIQHs1KAvqEODDz/view?usp=drivesdk"
target="_blank">
View Project Documentation ↗
</a>

</article>

<article class="card">

<h3>02 · Automatic Wiper for Automobiles Using Rain Sensor and Arduino</h3>

<div class="meta">15 February 2025 – 01 April 2025</div>

<p>
Project focused on automatic automobile wiper operation using
a rain sensor and Arduino, with emphasis on sensor integration,
microcontroller programming and real-time system design.
</p>

<p style="margin-top:9px">
Mentor: Prof. Nutan Bansode · Team size: 4
</p>

<div class="chips">
<span class="chip">Arduino</span>
<span class="chip">Sensor Integration</span>
<span class="chip">Real-Time Systems</span>
<span class="chip">Signal Processing</span>
</div>

<a class="project-link"
href="https://drive.google.com/drive/folders/1ZFIdEfJZ6wqCUmMwtMJo1w4aWWWvq-w5"
target="_blank">
View Project Files ↗
</a>

</article>

<article class="card">

<h3>03 · Smart Traffic Management System</h3>

<div class="meta">30 August 2024 – 25 December 2024</div>

<p>
Project involving IoT systems, smart traffic management,
microcontroller programming and real-time data processing.
</p>

<p style="margin-top:9px">
Mentor: Prof. Nutan Bansode · Team size: 4
</p>

<div class="chips">
<span class="chip">IoT Systems</span>
<span class="chip">Traffic Management</span>
<span class="chip">Microcontrollers</span>
<span class="chip">Real-Time Data</span>
</div>

<a class="project-link"
href="https://drive.google.com/drive/folders/1Fej62i8V13O6EB6N0vvMSRivDZDA1XJ4"
target="_blank">
View Project Files ↗
</a>

</article>

<article class="card">

<h3>04 · Automatic Plant Watering System</h3>

<div class="meta">10 January 2024 – 21 May 2024</div>

<p>
Project focused on Arduino programming, microcontroller
programming, automation systems and circuit design for an
automatic plant watering application.
</p>

<p style="margin-top:9px">
Mentor: Dr. Mahesh Gouder · Team size: 3
</p>

<div class="chips">
<span class="chip">Arduino</span>
<span class="chip">Microcontrollers</span>
<span class="chip">Automation</span>
<span class="chip">Circuit Design</span>
</div>

<a class="project-link"
href="https://drive.google.com/drive/folders/1d2wSnKWCJ7j3pSnfPgo4NNGKGXvYk50k"
target="_blank">
View Project Files ↗
</a>

</article>

</div>

</section>

<!-- CERTIFICATIONS -->

<section id="certifications">

<div class="section-head">
<h2>Certifications & <span>Training</span></h2>
<p>Assessments, workshops and professional development</p>
</div>

<div class="cert-list">

<div class="cert">
<strong>AI Fluency For Nonprofits</strong>
<span>ANTHROP/C</span>
</div>

<div class="cert">
<strong>AI Fluency: Framework & Foundations</strong>
<span>ANTHROP/C</span>
</div>

<div class="cert">
<strong>AI Fluency for Students</strong>
<span>ANTHROP/C</span>
</div>

<div class="cert">
<strong>Claude 101</strong>
<span>ANTHROP/C</span>
</div>

</div>

<div class="grid2" style="margin-top:17px">

<article class="card">

<h3>Electronic Workshop</h3>

<div class="meta">28 August 2023 – 30 November 2023</div>

<p>MIT Academy of Engineering, Pune</p>

<p>
Key skills: Basic Electronics, Circuit Prototyping,
Microcontroller Basics and Sensor Interfacing.
</p>

</article>

<article class="card">

<h3>CRPC Corporation</h3>

<div class="meta">20 September 2023 – 20 October 2023</div>

<p>MIT Academy of Engineering, Pune</p>

<p>
Key skills: Career Planning, Resume Building,
Interview Preparation and Professional Communication.
</p>

</article>

</div>

</section>

<!-- CONTACT -->

<section id="contact">

<div class="section-head">
<h2>Let's <span>Connect</span></h2>
<p>Open to connecting about engineering, hardware and embedded systems opportunities</p>
</div>

<div class="contact-grid">

<article class="card">

<h3>Contact Information</h3>

<div class="contact-line">
<b>Email</b>
<a href="mailto:swapnillonkar0606@gmail.com">
swapnillonkar0606@gmail.com
</a>
</div>

<div class="contact-line">
<b>College Email</b>
<a href="mailto:202301070187@mitaoe.ac.in">
202301070187@mitaoe.ac.in
</a>
</div>

<div class="contact-line">
<b>Phone</b>
<a href="tel:+918483040612">
+91 84830 40612
</a>
</div>

<div class="contact-line">
<b>Location</b>
Ahilyanagar, Maharashtra, India – 414604
</div>

</article>

<article class="card">

<h3>Professional Profiles</h3>

<p>
Explore my professional and project profiles or get in touch
by email.
</p>

<div class="socials">

<a href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
target="_blank">
LinkedIn ↗
</a>

<a href="https://github.com/Swapnillonkar1"
target="_blank">
GitHub ↗
</a>

<a href="https://x.com/LonkarSwapnil1"
target="_blank">
X / Twitter ↗
</a>

</div>

<div class="actions">
<a class="btn primary"
href="mailto:swapnillonkar0606@gmail.com">
Send an Email
</a>
</div>

</article>

</div>

</section>

<!-- PERSONAL INTERESTS -->

<section>

<div class="section-head">
<h2>Beyond <span>Engineering</span></h2>
</div>

<div class="card">

<p>
Personal interests: Reading, listening to music, playing sports,
exploring new technologies and travelling.
Languages: English, Marathi and Hindi.
</p>

</div>

</section>

</main>

<footer>
<div class="container">
© <span id="year"></span> Swapnil Lahu Lonkar · Electronics & Telecommunication Engineering
</div>
</footer>

<script>
document.getElementById("year").textContent =
new Date().getFullYear();
</script>

</body>
</html>
