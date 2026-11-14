<DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Swapnil Lonkar | Electronics & Embedded Systems Portfolio</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

<style>
:root {
  --bg: #050816;
  --bg-alt: #0b1020;
  --card: #111827;
  --accent: #38bdf8;
  --purple: #a855f7;
  --text: #e5e7eb;
  --muted: #9ca3af;
  --border: #263449;
  --radius: 18px;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  font-family: 'Poppins', sans-serif;
  background: radial-gradient(circle at top, #17243a, #050816 55%, #02040a);
  color: var(--text);
  line-height: 1.7;
}

a {
  text-decoration: none;
  color: inherit;
}

.container {
  max-width: 1150px;
  margin: auto;
  padding: 25px 20px;
}

/* NAVBAR */

.navbar {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(5,8,22,0.92);
  backdrop-filter: blur(15px);
  border-bottom: 1px solid var(--border);
}

.nav-inner {
  max-width: 1150px;
  margin: auto;
  padding: 14px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 23px;
  font-weight: 800;
  color: var(--accent);
}

.nav-links {
  display: flex;
  gap: 22px;
  flex-wrap: wrap;
}

.nav-links a {
  font-size: 13px;
  color: var(--muted);
  transition: 0.3s;
}

.nav-links a:hover {
  color: var(--accent);
}

/* HERO */

.hero {
  display: grid;
  grid-template-columns: 1.5fr 1fr;
  gap: 45px;
  align-items: center;
  padding-top: 65px;
}

.intro {
  color: var(--accent);
  font-size: 14px;
  font-weight: 600;
}

.hero h1 {
  font-size: clamp(32px, 5vw, 53px);
  line-height: 1.25;
  margin: 12px 0;
}

.gradient {
  background: linear-gradient(90deg, #38bdf8, #a855f7);
  color: transparent;
  background-clip: text;
}

.hero h3 {
  color: var(--muted);
  font-size: 19px;
  font-weight: 400;
  margin-bottom: 15px;
}

.hero p {
  font-size: 14px;
  color: var(--muted);
  max-width: 650px;
}

.tags {
  display: flex;
  flex-wrap: wrap;
  gap: 9px;
  margin: 22px 0;
}

.tag {
  padding: 6px 12px;
  border: 1px solid var(--border);
  border-radius: 30px;
  font-size: 11px;
  color: var(--accent);
  background: #111827;
}

.actions {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  margin: 22px 0;
}

.btn {
  display: inline-block;
  padding: 10px 20px;
  border-radius: 30px;
  font-size: 13px;
  font-weight: 600;
  transition: 0.3s;
}

.btn-primary {
  color: #07111f;
  background: linear-gradient(120deg, #38bdf8, #818cf8);
}

.btn-outline {
  border: 1px solid var(--accent);
  color: var(--accent);
}

.btn:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px #38bdf844;
}

.hero-card {
  background: linear-gradient(145deg, #16263c, #101525);
  border: 1px solid var(--border);
  border-radius: 25px;
  padding: 30px;
  text-align: center;
  box-shadow: 0 20px 50px #0008;
}

.avatar {
  width: 115px;
  height: 115px;
  margin: 0 auto 18px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  font-size: 38px;
  font-weight: 700;
  color: #07111f;
  background: linear-gradient(135deg, #38bdf8, #a855f7);
  border: 4px solid #263449;
}

.hero-card h2 {
  font-size: 21px;
}

.hero-card p {
  font-size: 12px;
  color: var(--muted);
  margin: 5px 0 18px;
}

.metrics {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 12px;
}

.metric {
  background: #0b1020;
  border: 1px solid var(--border);
  border-radius: 13px;
  padding: 14px;
}

.metric h3 {
  color: var(--accent);
  font-size: 22px;
}

.metric span {
  font-size: 11px;
  color: var(--muted);
}

/* GENERAL SECTIONS */

section {
  margin-top: 75px;
  scroll-margin-top: 85px;
}

.section-heading {
  margin-bottom: 25px;
}

.section-heading h2 {
  font-size: 26px;
  margin-bottom: 5px;
}

.section-heading h2 span {
  color: var(--accent);
}

.section-heading p {
  font-size: 12px;
  color: var(--muted);
}

.grid-two {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
}

.card {
  background: var(--card);
  border: 1px solid var(--border);
  border-radius: var(--radius);
  padding: 22px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-4px);
  border-color: var(--accent);
  box-shadow: 0 12px 30px #0005;
}

.card h3 {
  font-size: 15px;
  margin-bottom: 5px;
}

.meta {
  color: var(--accent);
  font-size: 11px;
  margin-bottom: 10px;
}

.card p {
  font-size: 12px;
  color: var(--muted);
}

.card ul {
  padding-left: 18px;
  margin-top: 8px;
}

.card li {
  font-size: 12px;
  color: var(--muted);
  margin-bottom: 5px;
}

.badge {
  display: inline-block;
  padding: 4px 10px;
  border: 1px solid #38bdf855;
  color: var(--accent);
  border-radius: 30px;
  font-size: 10px;
  margin-top: 12px;
}

/* INTERNSHIPS */

.internship-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 18px;
}

/* SKILLS */

.skills-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

.skill-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
  margin-top: 12px;
}

.skill-tags span {
  background: #0b1020;
  border: 1px solid var(--border);
  padding: 5px 10px;
  border-radius: 30px;
  font-size: 11px;
  color: #cbd5e1;
}

/* PROJECTS */

.projects-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}

.project-number {
  color: var(--accent);
  font-size: 25px;
  font-weight: 700;
  margin-bottom: 8px;
}

.project-link {
  display: inline-block;
  color: var(--accent);
  font-size: 12px;
  margin-top: 15px;
}

.project-link:hover {
  color: #c084fc;
}

/* CERTIFICATIONS */

.cert-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 15px;
}

/* CONTACT */

.contact-box {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 20px;
}

.contact-item {
  margin: 14px 0;
  color: var(--muted);
  font-size: 13px;
  overflow-wrap: anywhere;
}

.contact-item strong {
  color: var(--accent);
}

.socials {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
  margin-top: 20px;
}

.socials a {
  padding: 8px 14px;
  border: 1px solid var(--border);
  border-radius: 25px;
  color: var(--accent);
  font-size: 12px;
}

.socials a:hover {
  background: #38bdf822;
}

/* FOOTER */

footer {
  margin-top: 70px;
  padding: 25px 10px;
  text-align: center;
  border-top: 1px solid var(--border);
  color: var(--muted);
  font-size: 12px;
}

/* RESPONSIVE */

@media(max-width: 850px) {
  .hero {
    grid-template-columns: 1fr;
  }

  .hero-card {
    max-width: 450px;
    width: 100%;
    margin: auto;
  }

  .skills-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media(max-width: 650px) {
  .nav-inner {
    flex-direction: column;
    gap: 12px;
  }

  .nav-links {
    justify-content: center;
    gap: 12px;
  }

  .grid-two,
  .internship-grid,
  .projects-grid,
  .cert-grid,
  .contact-box,
  .skills-grid {
    grid-template-columns: 1fr;
  }

  .hero {
    padding-top: 35px;
  }

  section {
    margin-top: 55px;
  }
}
</style>
</head>

<body>

<!-- NAVIGATION -->

<nav class="navbar">
  <div class="nav-inner">
    <a href="#home" class="logo">SL.</a>

    <div class="nav-links">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#education">Education</a>
      <a href="#internships">Internships</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#certifications">Certifications</a>
      <a href="#contact">Contact</a>
    </div>
  </div>
</nav>

<main class="container">

<!-- HERO SECTION -->

<section class="hero" id="home">

  <div>
    <div class="intro">WELCOME TO MY PORTFOLIO</div>

    <h1>
      Hi, I'm <span class="gradient">Swapnil Lonkar</span>
    </h1>

    <h3>Electronics & Telecommunication Engineer</h3>

    <p>
      Motivated Electronics and Telecommunication Engineering student
      with knowledge of Embedded Systems, STM32, C programming,
      and Edge AI. Interested in hardware development, firmware
      programming, circuit design and real-time embedded applications.
    </p>

    <div class="tags">
      <span class="tag">B.Tech 2023–2027</span>
      <span class="tag">Embedded Systems</span>
      <span class="tag">STM32</span>
      <span class="tag">Embedded C</span>
      <span class="tag">Hardware Development</span>
      <span class="tag">Edge AI</span>
    </div>

    <div class="actions">
      <a href="#projects" class="btn btn-primary">Explore Projects →</a>

      <a href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
         target="_blank" class="btn btn-outline">
        LinkedIn Profile
      </a>
    </div>

    <p>
      📧 swapnillonkar0606@gmail.com
      <br>
      📍 Ahilyanagar, Maharashtra, India
    </p>
  </div>

  <div class="hero-card">
    <div class="avatar">SL</div>

    <h2>Swapnil Lahu Lonkar</h2>
    <p>B.Tech – Electronics & Telecommunication</p>

    <div class="metrics">
      <div class="metric">
        <h3>7.31</h3>
        <span>CGPA / 10</span>
      </div>

      <div class="metric">
        <h3>03</h3>
        <span>Internships</span>
      </div>

      <div class="metric">
        <h3>05</h3>
        <span>Projects</span>
      </div>

      <div class="metric">
        <h3>2027</h3>
        <span>Graduation</span>
      </div>
    </div>
  </div>

</section>

<!-- ABOUT -->

<section id="about">

  <div class="section-heading">
    <h2>About <span>Me</span></h2>
    <p>Introduction and professional interests</p>
  </div>

  <div class="card">
    <h3>Electronics | Embedded Systems | Hardware</h3>

    <p>
      I am Swapnil Lahu Lonkar, pursuing B.Tech in Electronics
      and Telecommunication Engineering at MIT Academy of Engineering,
      Pune.

      I have developed technical knowledge in C Programming,
      C++, Python, Embedded C, PCB Basics, Sensors and Interfacing.

      I am interested in developing hardware-oriented solutions,
      embedded applications, firmware development and intelligent
      electronic systems.

      My academic projects and internship experiences have helped
      me improve my technical knowledge, teamwork, problem-solving
      and professional communication skills.
    </p>

    <span class="badge">Aspiring Embedded Systems Engineer</span>
  </div>

</section>

<!-- EDUCATION -->

<section id="education">

  <div class="section-heading">
    <h2>My <span>Education</span></h2>
    <p>Academic qualifications</p>
  </div>

  <div class="grid-two">

    <div class="card">
      <h3>MIT Academy of Engineering, Pune</h3>
      <div class="meta">2023 – 2027 | B.Tech</div>
      <p>Electronics and Telecommunication Engineering</p>
      <p><strong>CGPA: 7.31 / 10</strong></p>
      <span class="badge">Currently Pursuing</span>
    </div>

    <div class="card">
      <h3>Sahyadri International Junior College</h3>
      <div class="meta">2023 | 12th Standard</div>
      <p>MSBSHSE</p>
      <p><strong>Percentage: 71.67%</strong></p>
    </div>

    <div class="card">
      <h3>Residential High School</h3>
      <div class="meta">2021 | 10th Standard</div>
      <p>MSBSHSE</p>
      <p><strong>Percentage: 86.40%</strong></p>
    </div>

  </div>

</section>

<!-- INTERNSHIPS -->

<section id="internships">

  <div class="section-heading">
    <h2>Internships & <span>Experience</span></h2>
    <p>Virtual internship programs and technical experience</p>
  </div>

  <div class="internship-grid">

    <div class="card">
      <h3>Cisco Networking Academy</h3>
      <div class="meta">01 June 2025 – 30 August 2025</div>
      <p><strong>Cisco AICTE Virtual Internship Program 2025</strong></p>
      <p>
        Gained knowledge of computer networking, networking
        fundamentals, network security and LAN/WAN technologies.
      </p>
      <div class="skill-tags">
        <span>Computer Networking</span>
        <span>Network Security</span>
        <span>LAN & WAN</span>
      </div>
      <span class="badge">Networking</span>
    </div>

    <div class="card">
      <h3>Edunet Foundation</h3>
      <div class="meta">15 July 2025 – 07 August 2025</div>
      <p><strong>SkillsBuild & IBM Cloud Platform in Emerging Technologies (AI & Cloud)</strong></p>
      <p>
        Developed knowledge of data analytics, cloud computing,
        IBM Cloud and artificial intelligence.
      </p>
      <div class="skill-tags">
        <span>Data Analytics</span>
        <span>IBM Cloud</span>
        <span>Artificial Intelligence</span>
      </div>
      <span class="badge">AI & Cloud</span>
    </div>

    <div class="card">
      <h3>Eduskills</h3>
      <div class="meta">01 July 2024 – 30 September 2024</div>
      <p><strong>Android Developer</strong></p>
      <p>
        Developed knowledge of Android development,
        mobile application development and UI/UX design.
      </p>
      <div class="skill-tags">
        <span>Android Development</span>
        <span>Mobile Applications</span>
        <span>UI/UX Design</span>
      </div>
      <span class="badge">Android Development</span>
    </div>

  </div>

</section>

<!-- SKILLS -->

<section id="skills">

  <div class="section-heading">
    <h2>Technical <span>Skills</span></h2>
    <p>My technical knowledge and expertise</p>
  </div>

  <div class="skills-grid">

    <div class="card">
      <h3>Programming Languages</h3>
      <div class="skill-tags">
        <span>C Programming</span>
        <span>C++ Programming</span>
        <span>Python</span>
        <span>Embedded C</span>
      </div>
    </div>

    <div class="card">
      <h3>Embedded Systems</h3>
      <div class="skill-tags">
        <span>STM32</span>
        <span>Microcontrollers</span>
        <span>Sensor Interfacing</span>
        <span>Real-Time Systems</span>
      </div>
    </div>

    <div class="card">
      <h3>Electronics & Hardware</h3>
      <div class="skill-tags">
        <span>PCB Basics</span>
        <span>Basic Electronics</span>
        <span>Circuit Design</span>
        <span>Sensor Integration</span>
      </div>
    </div>

    <div class="card">
      <h3>Communication Systems</h3>
      <div class="skill-tags">
        <span>Digital Communication</span>
        <span>Wireless Communication</span>
        <span>Satellite Communication</span>
        <span>Networking</span>
      </div>
    </div>

    <div class="card">
      <h3>Software & Tools</h3>
      <div class="skill-tags">
        <span>MATLAB</span>
        <span>Simulink</span>
        <span>Arduino</span>
        <span>IBM Cloud</span>
      </div>
    </div>

    <div class="card">
      <h3>Professional Skills</h3>
      <div class="skill-tags">
        <span>Problem Solving</span>
        <span>Teamwork</span>
        <span>Communication</span>
        <span>Adaptability</span>
      </div>
    </div>

  </div>

</section>

<!-- PROJECTS -->

<section id="projects">

  <div class="section-heading">
    <h2>Academic <span>Projects</span></h2>
    <p>Engineering projects and practical implementations</p>
  </div>

  <div class="projects-grid">

    <div class="card">
      <div class="project-number">01</div>
      <h3>Digital Wireless Communication Link over Satellite Using Simulink</h3>
      <div class="meta">01 March 2025 – 30 April 2025</div>
      <p>
        Developed a simulation-based digital wireless communication
        link over the GSAT-31 satellite using MATLAB and Simulink.
        The project focuses on satellite communication and
        communication system performance evaluation.
      </p>
      <p><strong>Mentor:</strong> Prof. Vipin Yadav</p>
      <p><strong>Team Size:</strong> 4</p>
      <div class="skill-tags">
        <span>MATLAB</span>
        <span>Simulink</span>
        <span>Digital Communication</span>
        <span>GSAT-31</span>
      </div>
      <a class="project-link"
         href="https://drive.google.com/file/d/1jTvDosoLyYf_YAJYFBIQHs1KAvqEODDz/view?usp=drivesdk"
         target="_blank">View Project →</a>
    </div>

    <div class="card">
      <div class="project-number">02</div>
      <h3>Automatic Wiper for Automobiles Using Rain Sensor and Arduino</h3>
      <div class="meta">15 February 2025 – 01 April 2025</div>
      <p>
        Worked on an automatic automobile wiper system using
        a rain sensor and Arduino. The project focuses on
        sensor integration, microcontroller programming and
        real-time system design.
      </p>
      <p><strong>Mentor:</strong> Prof. Nutan Bansode</p>
      <p><strong>Team Size:</strong> 4</p>
      <div class="skill-tags">
        <span>Arduino</span>
        <span>Rain Sensor</span>
        <span>Microcontroller</span>
        <span>Signal Processing</span>
      </div>
      <a class="project-link"
         href="https://drive.google.com/drive/folders/1ZFIdEfJZ6wqCUmMwtMJo1w4aWWWvq-w5"
         target="_blank">View Project →</a>
    </div>

    <div class="card">
      <div class="project-number">03</div>
      <h3>Smart Traffic Management System</h3>
      <div class="meta">30 August 2024 – 25 December 2024</div>
      <p>
        Worked on a smart traffic management project
        focusing on IoT systems, traffic management,
        microcontroller programming and real-time data processing.
      </p>
      <p><strong>Mentor:</strong> Prof. Nutan Bansode</p>
      <p><strong>Team Size:</strong> 4</p>
      <div class="skill-tags">
        <span>IoT Systems</span>
        <span>Smart Traffic</span>
        <span>Microcontrollers</span>
        <span>Real-Time Processing</span>
      </div>
      <a class="project-link"
         href="https://drive.google.com/drive/folders/1Fej62i8V13O6EB6N0vvMSRivDZDA1XJ4"
         target="_blank">View Project →</a>
    </div>

    <div class="card">
      <div class="project-number">04</div>
      <h3>Automatic Plant Watering System</h3>
      <div class="meta">10 January 2024 – 21 May 2024</div>
      <p>
        Worked on an automatic plant watering system
        focusing on Arduino programming, microcontroller
        programming, automation systems and circuit design.
      </p>
      <p><strong>Mentor:</strong> Dr. Mahesh Gouder</p>
      <p><strong>Team Size:</strong> 3</p>
      <div class="skill-tags">
        <span>Arduino</span>
        <span>Automation</span>
        <span>Microcontrollers</span>
        <span>Circuit Design</span>
      </div>
      <a class="project-link"
         href="https://drive.google.com/drive/folders/1d2wSnKWCJ7j3pSnfPgo4NNGKGXvYk50k"
         target="_blank">View Project →</a>
    </div>

    <div class="card">
      <div class="project-number">05</div>
      <h3>Hardware and Electronics Practical Work</h3>
      <div class="meta">Technical Workshop Experience</div>
      <p>
        Participated in electronics workshops involving
        basic electronics, circuit prototyping,
        microcontroller basics and sensor interfacing
        at MIT Academy of Engineering, Pune.
      </p>
      <div class="skill-tags">
        <span>Basic Electronics</span>
        <span>Circuit Prototyping</span>
        <span>Sensor Interfacing</span>
      </div>
      <span class="badge">Workshop Experience</span>
    </div>

  </div>

</section>

<!-- CERTIFICATIONS -->

<section id="certifications">

  <div class="section-heading">
    <h2>Certifications & <span>Training</span></h2>
    <p>Additional learning and professional development</p>
  </div>

  <div class="cert-grid">

    <div class="card">
      <h3>AI Fluency for Nonprofits</h3>
      <div class="meta">Provider: ANTHROP/C (as listed in resume)</div>
    </div>

    <div class="card">
      <h3>AI Fluency: Framework & Foundations</h3>
      <div class="meta">Provider: ANTHROP/C (as listed in resume)</div>
    </div>

    <div class="card">
      <h3>AI Fluency for Students</h3>
      <div class="meta">Provider: ANTHROP/C (as listed in resume)</div>
    </div>

    <div class="card">
      <h3>Claude 101</h3>
      <div class="meta">Provider: ANTHROP/C (as listed in resume)</div>
    </div>

  </div>

  <div class="section-heading" style="margin-top:30px;">
    <h2>Seminars & <span>Workshops</span></h2>
  </div>

  <div class="grid-two">

    <div class="card">
      <h3>Electronic Workshop</h3>
      <div class="meta">28 August 2023 – 30 November 2023</div>
      <p>MIT Academy of Engineering, Pune</p>
      <p>Basic Electronics, Circuit Prototyping, Microcontroller Basics and Sensor Interfacing.</p>
    </div>

    <div class="card">
      <h3>CRPC Corporation</h3>
      <div class="meta">20 September 2023 – 20 October 2023</div>
      <p>MIT Academy of Engineering, Pune</p>
      <p>Career Planning, Resume Building, Interview Preparation and Professional Communication.</p>
    </div>

  </div>

</section>

<!-- INTERESTS -->

<section id="interests">

  <div class="section-heading">
    <h2>Personal <span>Interests</span></h2>
  </div>

  <div class="card">
    <div class="skill-tags">
      <span>Exploring New Technologies</span>
      <span>Reading</span>
      <span>Listening to Music</span>
      <span>Playing Sports</span>
      <span>Travelling</span>
    </div>
  </div>

</section>

<!-- CONTACT -->

<section id="contact">

  <div class="section-heading">
    <h2>Let's <span>Connect</span></h2>
    <p>Interested in engineering opportunities and collaboration</p>
  </div>

  <div class="contact-box">

    <div class="card">
      <h3>Contact Information</h3>

      <div class="contact-item">
        <strong>Email:</strong><br>
        <a href="mailto:swapnillonkar0606@gmail.com">
          swapnillonkar0606@gmail.com
        </a>
      </div>

      <div class="contact-item">
        <strong>College Email:</strong><br>
        <a href="mailto:202301070187@mitaoe.ac.in">
          202301070187@mitaoe.ac.in
        </a>
      </div>

      <div class="contact-item">
        <strong>Phone:</strong><br>
        <a href="tel:+918483040612">+91 84830 40612</a>
      </div>

      <div class="contact-item">
        <strong>Location:</strong><br>
        Ahilyanagar, Maharashtra, India
      </div>
    </div>

    <div class="card">
      <h3>Professional Profiles</h3>

      <p>
        I am interested in opportunities in hardware,
        embedded systems, electronics and firmware development.
        Feel free to connect with me.
      </p>

      <div class="socials">
        <a href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
           target="_blank">LinkedIn ↗</a>

        <a href="https://github.com/Swapnillonkar1"
           target="_blank">GitHub ↗</a>

        <a href="https://x.com/LonkarSwapnil1"
           target="_blank">Twitter ↗</a>
      </div>

      <div class="actions">
        <a class="btn btn-primary"
           href="mailto:swapnillonkar0606@gmail.com">
          Send Email
        </a>
      </div>
    </div>

  </div>

</section>

</main>

<footer>
  <p>© <span id="year"></span> Swapnil Lahu Lonkar</p>
  <p>Designed with passion for Electronics & Embedded Systems.</p>
</footer>

<script>
  document.getElementById("year").textContent =
    new Date().getFullYear();
</script>

</body>
</html>
