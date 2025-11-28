<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Swapnil Lonkar | Portfolio</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <meta
    name="description"
    content="Portfolio of Swapnil Lahu Lonkar – B.Tech Electronics & Telecommunication Engineering student with experience in AI/ML, Embedded Systems, Networking, and Cloud."
  />
  <!-- Google Fonts -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link
    href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
    rel="stylesheet"
  />
  <!-- Font Awesome Icons -->
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css"
    integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA=="
    crossorigin="anonymous"
    referrerpolicy="no-referrer"
  />

  <style>
    :root {
      --bg: #050816;
      --bg-alt: #0b1020;
      --card: #111827;
      --accent: #38bdf8;
      --accent-soft: rgba(56, 189, 248, 0.15);
      --text: #e5e7eb;
      --muted: #9ca3af;
      --border: #1f2937;
      --radius-lg: 18px;
      --radius-xl: 24px;
      --shadow-soft: 0 18px 45px rgba(15, 23, 42, 0.6);
      --transition: 0.25s ease;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: "Poppins", system-ui, -apple-system, BlinkMacSystemFont,
        "Segoe UI", sans-serif;
      background: radial-gradient(circle at top, #1f2937 0, #020617 45%, #000 100%);
      color: var(--text);
      line-height: 1.6;
      scroll-behavior: smooth;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    img {
      max-width: 100%;
      display: block;
    }

    .page {
      max-width: 1120px;
      margin: 0 auto;
      padding: 24px 16px 48px;
    }

    /* Navbar */
    .navbar {
      position: sticky;
      top: 0;
      z-index: 30;
      backdrop-filter: blur(16px);
      background: linear-gradient(
        to bottom,
        rgba(15, 23, 42, 0.95),
        rgba(15, 23, 42, 0.7),
        transparent
      );
    }

    .navbar-inner {
      max-width: 1120px;
      margin: 0 auto;
      padding: 10px 16px 8px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .brand-logo {
      width: 36px;
      height: 36px;
      border-radius: 999px;
      background: radial-gradient(circle at 30% 0, #38bdf8, #4f46e5);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-weight: 700;
      font-size: 18px;
      color: #0b1120;
      box-shadow: 0 10px 25px rgba(56, 189, 248, 0.5);
    }

    .brand-text {
      display: flex;
      flex-direction: column;
    }

    .brand-text span:first-child {
      font-weight: 600;
      font-size: 15px;
    }

    .brand-text span:last-child {
      font-size: 12px;
      color: var(--muted);
    }

    .nav-links {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      font-size: 13px;
    }

    .nav-links a {
      padding: 6px 11px;
      border-radius: 999px;
      border: 1px solid transparent;
      color: var(--muted);
      transition: var(--transition);
    }

    .nav-links a:hover {
      border-color: var(--accent-soft);
      background: rgba(15, 23, 42, 0.9);
      color: var(--text);
    }

    /* Hero */
    .hero {
      display: grid;
      grid-template-columns: minmax(0, 3fr) minmax(0, 2.4fr);
      gap: 32px;
      margin-top: 32px;
      align-items: center;
    }

    @media (max-width: 860px) {
      .hero {
        grid-template-columns: 1fr;
      }
      .hero-visual {
        order: -1;
      }
      .navbar-inner {
        flex-direction: column;
        align-items: flex-start;
      }
    }

    .hero-heading {
      font-size: clamp(28px, 4vw, 36px);
      font-weight: 700;
      margin-bottom: 8px;
    }

    .hero-gradient {
      background: linear-gradient(90deg, #38bdf8, #a855f7, #f59e0b);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }

    .hero-subtitle {
      font-size: 15px;
      color: var(--muted);
      margin-bottom: 18px;
    }

    .hero-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 20px;
    }

    .tag {
      font-size: 12px;
      padding: 5px 10px;
      border-radius: 999px;
      border: 1px solid var(--border);
      background: rgba(15, 23, 42, 0.9);
      color: var(--muted);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-bottom: 16px;
    }

    .btn {
      border-radius: 999px;
      padding: 9px 16px;
      font-size: 13px;
      border: 1px solid transparent;
      cursor: pointer;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      transition: var(--transition);
    }

    .btn-primary {
      background: linear-gradient(135deg, #38bdf8, #6366f1);
      color: #0b1120;
      font-weight: 600;
      box-shadow: 0 12px 30px rgba(56, 189, 248, 0.55);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 16px 40px rgba(56, 189, 248, 0.7);
    }

    .btn-ghost {
      background: rgba(15, 23, 42, 0.9);
      color: var(--muted);
      border-color: var(--border);
    }

    .btn-ghost:hover {
      border-color: var(--accent-soft);
      color: var(--text);
    }

    .hero-contact {
      font-size: 13px;
      color: var(--muted);
    }

    .hero-contact a {
      color: var(--accent);
    }

    .hero-visual {
      border-radius: var(--radius-xl);
      background: radial-gradient(circle at top left, #22d3ee25, #1e293b);
      padding: 18px 18px 22px;
      box-shadow: var(--shadow-soft);
      border: 1px solid var(--border);
      position: relative;
      overflow: hidden;
    }

    .hero-visual::after {
      content: "";
      position: absolute;
      inset: 0;
      background-image: radial-gradient(circle at 10% 0, #22d3ee11 0, transparent 55%),
        radial-gradient(circle at 90% 90%, #a855f711 0, transparent 55%);
      opacity: 0.8;
      pointer-events: none;
    }

    .hero-card-inner {
      position: relative;
      z-index: 1;
    }

    .hero-name {
      font-size: 18px;
      font-weight: 600;
      margin-bottom: 2px;
    }

    .hero-role {
      font-size: 13px;
      color: var(--muted);
      margin-bottom: 10px;
    }

    .hero-pill-row {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-bottom: 14px;
    }

    .pill {
      font-size: 11px;
      padding: 4px 8px;
      border-radius: 999px;
      border: 1px solid rgba(148, 163, 184, 0.4);
      color: #e5e7eb;
      background: rgba(15, 23, 42, 0.8);
    }

    .metrics {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 8px;
      margin-bottom: 16px;
    }

    .metric-card {
      border-radius: 14px;
      border: 1px solid var(--border);
      background: rgba(15, 23, 42, 0.9);
      padding: 8px 10px;
    }

    .metric-label {
      font-size: 11px;
      color: var(--muted);
    }

    .metric-value {
      font-size: 14px;
      font-weight: 600;
    }

    .stack-chips {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
      margin-bottom: 10px;
    }

    .stack-chip {
      border-radius: 999px;
      padding: 3px 7px;
      font-size: 11px;
      border: 1px solid rgba(148, 163, 184, 0.5);
      color: #e5e7eb;
    }

    .hero-footer-text {
      font-size: 11px;
      color: var(--muted);
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 8px;
      margin-top: 8px;
    }

    .hero-socials {
      display: flex;
      gap: 8px;
      font-size: 15px;
    }

    .hero-socials a {
      width: 26px;
      height: 26px;
      border-radius: 999px;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      background: rgba(15, 23, 42, 0.9);
      border: 1px solid var(--border);
      color: var(--muted);
      transition: var(--transition);
    }

    .hero-socials a:hover {
      color: var(--accent);
      border-color: var(--accent-soft);
      transform: translateY(-1px);
    }

    /* Sections */
    section {
      margin-top: 40px;
    }

    .section-header {
      display: flex;
      align-items: baseline;
      justify-content: space-between;
      gap: 12px;
      margin-bottom: 18px;
    }

    .section-title {
      font-size: 20px;
      font-weight: 600;
    }

    .section-subtitle {
      font-size: 12px;
      color: var(--muted);
    }

    /* Education & Experience */
    .grid-two {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 18px;
    }

    @media (max-width: 720px) {
      .grid-two {
        grid-template-columns: 1fr;
      }
    }

    .card {
      background: var(--card);
      border-radius: var(--radius-lg);
      padding: 14px 14px 16px;
      border: 1px solid var(--border);
      box-shadow: 0 10px 28px rgba(15, 23, 42, 0.75);
    }

    .card-header {
      display: flex;
      align-items: flex-start;
      justify-content: space-between;
      gap: 10px;
      margin-bottom: 6px;
    }

    .card-title {
      font-size: 14px;
      font-weight: 600;
    }

    .card-meta {
      font-size: 11px;
      color: var(--muted);
    }

    .badge {
      font-size: 10px;
      padding: 3px 8px;
      border-radius: 999px;
      border: 1px solid var(--accent-soft);
      background: rgba(15, 23, 42, 0.9);
      color: var(--accent);
      white-space: nowrap;
    }

    .card-body {
      font-size: 12px;
      color: var(--muted);
      margin-top: 4px;
    }

    .card-footer {
      margin-top: 8px;
      font-size: 11px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 8px;
      color: var(--muted);
    }

    .card-footer a {
      color: var(--accent);
      font-size: 11px;
    }

    .list-compact {
      list-style: none;
      padding-left: 0;
      margin-top: 6px;
    }

    .list-compact li {
      font-size: 12px;
      color: var(--muted);
      margin-bottom: 3px;
    }

    .pill-sm {
      display: inline-flex;
      align-items: center;
      gap: 4px;
      border-radius: 999px;
      padding: 3px 8px;
      font-size: 11px;
      border: 1px solid var(--border);
      background: rgba(15, 23, 42, 0.9);
      margin-top: 4px;
    }

    /* Skills */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 14px;
    }

    @media (max-width: 860px) {
      .skills-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }

    @media (max-width: 600px) {
      .skills-grid {
        grid-template-columns: 1fr;
      }
    }

    .skill-category-title {
      font-size: 13px;
      font-weight: 600;
      margin-bottom: 6px;
    }

    .skill-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 6px;
    }

    .skill-tag {
      font-size: 11px;
      padding: 4px 9px;
      border-radius: 999px;
      border: 1px solid var(--border);
      background: rgba(15, 23, 42, 0.9);
      color: var(--muted);
    }

    /* Projects */
    .projects-grid {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 18px;
    }

    @media (max-width: 880px) {
      .projects-grid {
        grid-template-columns: 1fr;
      }
    }

    .project-title {
      font-size: 14px;
      font-weight: 600;
      margin-bottom: 2px;
    }

    .project-meta {
      font-size: 11px;
      color: var(--muted);
      margin-bottom: 6px;
    }

    .project-body {
      font-size: 12px;
      color: var(--muted);
    }

    .project-footer {
      margin-top: 8px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      font-size: 11px;
      color: var(--muted);
    }

    .project-footer a {
      color: var(--accent);
    }

    /* Contact */
    .contact-content {
      display: grid;
      grid-template-columns: minmax(0, 2.3fr) minmax(0, 2fr);
      gap: 18px;
    }

    @media (max-width: 820px) {
      .contact-content {
        grid-template-columns: 1fr;
      }
    }

    .contact-list {
      list-style: none;
      padding-left: 0;
      font-size: 13px;
      color: var(--muted);
    }

    .contact-list li {
      margin-bottom: 6px;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .contact-list i {
      width: 18px;
      text-align: center;
      font-size: 13px;
      color: var(--accent);
    }

    .small-note {
      font-size: 11px;
      color: var(--muted);
      margin-top: 8px;
    }

    footer {
      margin-top: 40px;
      padding-top: 20px;
      border-top: 1px solid var(--border);
      font-size: 11px;
      color: var(--muted);
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 8px;
    }
  </style>
</head>
<body>
  <header class="navbar">
    <div class="navbar-inner">
      <a href="#top" class="brand">
        <div class="brand-logo">SL</div>
        <div class="brand-text">
          <span>Swapnil Lonkar</span>
          <span>Electronics & Telecommunication</span>
        </div>
      </a>
      <nav class="nav-links">
        <a href="#about">About</a>
        <a href="#education">Education</a>
        <a href="#internships">Internships</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <main class="page" id="top">
    <!-- Hero -->
    <section class="hero" id="about">
      <div>
        <h1 class="hero-heading">
          Building with <span class="hero-gradient">Electronics, AI & Code.</span>
        </h1>
        <p class="hero-subtitle">
          I’m <strong>Swapnil Lahu Lonkar</strong>, a B.Tech Electronics & Telecommunication student at
          <strong>MIT Academy of Engineering</strong>.  
          I enjoy working on <strong>AI/ML, embedded systems, networking, and cloud projects</strong> that solve real-world problems.
        </p>

        <div class="hero-tags">
          <span class="tag">B.Tech (2023 – 2027)</span>
          <span class="tag">AI / ML</span>
          <span class="tag">Embedded Systems</span>
          <span class="tag">Networking & Cybersecurity</span>
          <span class="tag">IBM Cloud</span>
        </div>

        <div class="hero-actions">
          <a href="#projects" class="btn btn-primary">
            <i class="fa-solid fa-code"></i>
            View My Projects
          </a>
          <a
            href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
            target="_blank"
            rel="noreferrer"
            class="btn btn-ghost"
          >
            <i class="fa-brands fa-linkedin"></i>
            Connect on LinkedIn
          </a>
        </div>

        <p class="hero-contact">
          📧 <a href="mailto:202301070187@mitaoe.ac.in">202301070187@mitaoe.ac.in</a>  
          📍 Ahilyanagar, Maharashtra, India
        </p>
      </div>

      <aside class="hero-visual">
        <div class="hero-card-inner">
          <div class="hero-name">Swapnil Lahu Lonkar</div>
          <div class="hero-role">B.Tech – Electronics & Telecommunication</div>
          <div class="hero-pill-row">
            <span class="pill">MIT Academy of Engineering</span>
            <span class="pill">Class of 2027</span>
          </div>

          <div class="metrics">
            <div class="metric-card">
              <div class="metric-label">CGPA</div>
              <div class="metric-value">6.98 / 10</div>
            </div>
            <div class="metric-card">
              <div class="metric-label">Internships</div>
              <div class="metric-value">6+</div>
            </div>
            <div class="metric-card">
              <div class="metric-label">Projects</div>
              <div class="metric-value">15+</div>
            </div>
          </div>

          <div class="stack-chips">
            <span class="stack-chip">Python</span>
            <span class="stack-chip">TensorFlow</span>
            <span class="stack-chip">Scikit-Learn</span>
            <span class="stack-chip">STM32 & Arduino</span>
            <span class="stack-chip">Cisco Packet Tracer</span>
            <span class="stack-chip">IBM Cloud</span>
          </div>

          <div class="hero-footer-text">
            <span>Open to internships & project collaborations.</span>
            <div class="hero-socials">
              <a
                href="mailto:202301070187@mitaoe.ac.in"
                title="Email"
              >
                <i class="fa-regular fa-envelope"></i>
              </a>
              <a
                href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
                target="_blank"
                rel="noreferrer"
                title="LinkedIn"
              >
                <i class="fa-brands fa-linkedin-in"></i>
              </a>
            </div>
          </div>
        </div>
      </aside>
    </section>

    <!-- Education & Internships -->
    <section id="education">
      <div class="section-header">
        <h2 class="section-title">Education</h2>
        <p class="section-subtitle">My academic journey so far.</p>
      </div>

      <div class="grid-two">
        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">
                MIT Academy of Engineering, Pune
              </div>
              <div class="card-meta">
                B.Tech – Electronics & Telecommunication • 2023 – 2027
              </div>
            </div>
            <span class="badge">Current</span>
          </div>
          <div class="card-body">
            CGPA: <strong>6.98 / 10</strong>  
            Focus areas: Communication systems, embedded systems, AI/ML & networking.
          </div>
        </article>

        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">Sahyadri International Jr. College</div>
              <div class="card-meta">
                12th – MSBSHSE • 2023
              </div>
            </div>
          </div>
          <div class="card-body">
            Percentage: <strong>71.67%</strong>
          </div>

          <div class="card-header" style="margin-top: 10px;">
            <div>
              <div class="card-title">Residential High School</div>
              <div class="card-meta">
                10th – MSBSHSE • 2021
              </div>
            </div>
          </div>
          <div class="card-body">
            Percentage: <strong>86.40%</strong>
          </div>
        </article>
      </div>
    </section>

    <section id="internships">
      <div class="section-header">
        <h2 class="section-title">Internships & Programs</h2>
        <p class="section-subtitle">
          Hands-on experience through virtual and on-campus programs.
        </p>
      </div>

      <div class="grid-two">
        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">Eduskills AICTE</div>
              <div class="card-meta">
                AI/ML Virtual Internship • Jul 2025 – Sep 2025
              </div>
            </div>
            <span class="badge">AI / ML</span>
          </div>
          <div class="card-body">
            Worked on data preprocessing, feature engineering, supervised and
            unsupervised learning, and fundamentals of neural networks and deep learning using Python.
          </div>
        </article>

        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">Cisco Networking Academy</div>
              <div class="card-meta">
                AICTE Virtual Internship Program 2025 • Jun 2025 – Aug 2025
              </div>
            </div>
            <span class="badge">Networking</span>
          </div>
          <div class="card-body">
            Gained experience in networking fundamentals, IP addressing, routing & switching,
            basic security and troubleshooting via virtual labs and Packet Tracer.
          </div>
        </article>

        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">SmartBridge</div>
              <div class="card-meta">
                AI & ML Experiential Program • Jul 2025 – Aug 2025
              </div>
            </div>
          </div>
          <div class="card-body">
            Built ML models in Python using TensorFlow and Scikit-Learn; applied
            concepts like model training, evaluation, and optimization to practical problems.
          </div>
        </article>

        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">Edunet Foundation</div>
              <div class="card-meta">
                IBM SkillsBuild – AI & Cloud • Jul 2025 – Aug 2025
              </div>
            </div>
            <span class="badge">Cloud</span>
          </div>
          <div class="card-body">
            Worked with IBM Cloud, designed chatbots using Watsonx Assistant,
            explored Agentic AI and AutoAI experiments, and completed project-based learning modules.
          </div>
        </article>

        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">Eduskills</div>
              <div class="card-meta">
                Android Developer • Jul 2024 – Sep 2024
              </div>
            </div>
            <span class="badge">Android</span>
          </div>
          <div class="card-body">
            Developed Android applications and strengthened fundamentals in mobile app development.
          </div>
        </article>

        <article class="card">
          <div class="card-header">
            <div>
              <div class="card-title">CISCO</div>
              <div class="card-meta">
                Virtual Internship (Cybersecurity) • May 2024 – Jul 2024
              </div>
            </div>
            <span class="badge">Cybersecurity</span>
          </div>
          <div class="card-body">
            Learned cybersecurity concepts, industry tools, and best practices for protecting networks and systems from emerging threats.
          </div>
        </article>
      </div>
    </section>

    <!-- Skills -->
    <section id="skills">
      <div class="section-header">
        <h2 class="section-title">Skills</h2>
        <p class="section-subtitle">
          Tools, technologies and areas I enjoy working with.
        </p>
      </div>

      <div class="skills-grid">
        <div class="card">
          <div class="skill-category-title">Programming & ML</div>
          <div class="skill-tags">
            <span class="skill-tag">Python</span>
            <span class="skill-tag">TensorFlow</span>
            <span class="skill-tag">Scikit-Learn</span>
            <span class="skill-tag">Pandas / NumPy</span>
            <span class="skill-tag">Supervised & Unsupervised ML</span>
            <span class="skill-tag">Model Evaluation</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">Embedded & Electronics</div>
          <div class="skill-tags">
            <span class="skill-tag">STM32 Nucleo</span>
            <span class="skill-tag">Arduino</span>
            <span class="skill-tag">ADC & Timers</span>
            <span class="skill-tag">7-Segment Displays</span>
            <span class="skill-tag">Digital Communication</span>
            <span class="skill-tag">RC Filters</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">Networking & Security</div>
          <div class="skill-tags">
            <span class="skill-tag">Cisco Packet Tracer</span>
            <span class="skill-tag">IP Addressing</span>
            <span class="skill-tag">Routing & Switching</span>
            <span class="skill-tag">Basic Network Security</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">Cloud & Platforms</div>
          <div class="skill-tags">
            <span class="skill-tag">IBM Cloud</span>
            <span class="skill-tag">Watsonx Assistant</span>
            <span class="skill-tag">AutoAI</span>
            <span class="skill-tag">Git & GitHub</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">Tools & Software</div>
          <div class="skill-tags">
            <span class="skill-tag">MATLAB & Simulink</span>
            <span class="skill-tag">OpenCV (Basics)</span>
            <span class="skill-tag">Android Studio</span>
            <span class="skill-tag">MS Office</span>
          </div>
        </div>

        <div class="card">
          <div class="skill-category-title">Soft Skills</div>
          <div class="skill-tags">
            <span class="skill-tag">Problem Solving</span>
            <span class="skill-tag">Teamwork</span>
            <span class="skill-tag">Communication</span>
            <span class="skill-tag">Time Management</span>
            <span class="skill-tag">Adaptability</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Projects -->
    <section id="projects">
      <div class="section-header">
        <h2 class="section-title">Selected Projects</h2>
        <p class="section-subtitle">
          A few academic and hobby projects I’ve worked on.
        </p>
      </div>

      <div class="projects-grid">
        <article class="card">
          <div class="project-title">
            Digital Wireless Communication Link over Satellite
          </div>
          <div class="project-meta">
            Simulink • QPSK • Rician Channel • Team Size: 4
          </div>
          <div class="project-body">
            Simulated a digital wireless link over GSAT-31 with ACELP & Huffman
            source coding, Hamming (31,26) channel coding, QPSK modulation and
            Rician fading channel between ground stations (Pune – Kolhapur).
          </div>
          <div class="project-footer">
            <a href="https://drive.google.com/file/d/1jTvDosoLyYf_YAJYFBIQHs1KAvqEODDz/view?usp=drivesdk" target="_blank" rel="noreferrer">
              View project docs →
            </a>
            <span class="pill-sm">
              <i class="fa-solid fa-signal"></i>
              Communication Systems
            </span>
          </div>
        </article>

        <article class="card">
          <div class="project-title">
            Traffic Management System using OpenCV
          </div>
          <div class="project-meta">
            OpenCV • Image Processing • Team Size: 4
          </div>
          <div class="project-body">
            Built a smart traffic system with real-time vehicle detection, traffic
            density estimation, number plate recognition and rule violation detection
            to dynamically control signals and improve traffic flow.
          </div>
          <div class="project-footer">
            <a href="https://drive.google.com/drive/folders/1ROzzsUgLu7AKTiY9bB5iZmFm3wN7l-uH" target="_blank" rel="noreferrer">
              View repository / files →
            </a>
            <span class="pill-sm">
              <i class="fa-solid fa-car-side"></i>
              Smart City
            </span>
          </div>
        </article>

        <article class="card">
          <div class="project-title">ARM Based Embedded System</div>
          <div class="project-meta">
            STM32 • Embedded C • Solo Project
          </div>
          <div class="project-body">
            Interfaced ADC & 7-segment display with STM32 to map 0–3V analog inputs
            to discrete display values (0–3) using timers and precise delay generation.
          </div>
          <div class="project-footer">
            <a href="https://drive.google.com/drive/folders/1R5WFZS6xA5QODdhc30HRtjpnzRYf8Scd" target="_blank" rel="noreferrer">
              View documentation →
            </a>
            <span class="pill-sm">
              <i class="fa-solid fa-microchip"></i>
              Embedded
            </span>
          </div>
        </article>

        <article class="card">
          <div class="project-title">Automatic Plant Watering System</div>
          <div class="project-meta">
            Arduino • IoT Basics • Team Size: 3
          </div>
          <div class="project-body">
            Developed a smart irrigation system using soil moisture sensor and
            water pump control that automatically waters plants when soil is dry,
            reducing water wastage and manual effort.
          </div>
          <div class="project-footer">
            <a href="https://drive.google.com/drive/folders/1d2wSnKWCJ7j3pSnfPgo4NNGKGXvYk50k" target="_blank" rel="noreferrer">
              View project →
            </a>
            <span class="pill-sm">
              <i class="fa-solid fa-seedling"></i>
              IoT Concept
            </span>
          </div>
        </article>

        <article class="card">
          <div class="project-title">Monopole Patch Antenna for Head Imaging</div>
          <div class="project-meta">
            Antenna Design • Team Size: 4
          </div>
          <div class="project-body">
            Worked on a circular slotted patch with defected ground monopole
            antenna to improve bandwidth, gain and radiation performance for
            microwave-based head imaging applications.
          </div>
          <div class="project-footer">
            <a href="https://docs.google.com/presentation/d/1v6I2f2nfFChBYedDO7e4Z0qKBrf12m6a/edit?usp=drivesdk" target="_blank" rel="noreferrer">
              View slides →
            </a>
            <span class="pill-sm">
              <i class="fa-solid fa-wave-square"></i>
              RF / Antenna
            </span>
          </div>
        </article>

        <article class="card">
          <div class="project-title">Smart Traffic & Lighting System</div>
          <div class="project-meta">
            IoT • Smart City • Team Size: 4
          </div>
          <div class="project-body">
            Designed an intelligent traffic light and solar street-light system
            that adapts to lane density and movement detection, reducing energy
            waste and congestion.
          </div>
          <div class="project-footer">
            <a href="https://drive.google.com/drive/folders/1Fej62i8V13O6EB6N0vvMSRivDZDA1XJ4" target="_blank" rel="noreferrer">
              View project →
            </a>
            <span class="pill-sm">
              <i class="fa-solid fa-city"></i>
              Smart Infrastructure
            </span>
          </div>
        </article>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact">
      <div class="section-header">
        <h2 class="section-title">Contact</h2>
        <p class="section-subtitle">Let’s connect or collaborate.</p>
      </div>

      <div class="contact-content">
        <div class="card">
          <p style="font-size: 13px; color: var(--muted); margin-bottom: 10px;">
            I’m open to opportunities in <strong>AI/ML, embedded systems, networking,
            and cloud-based projects</strong>.  
            If you’d like to discuss an internship, project, or collaboration, feel free to reach out.
          </p>

          <ul class="contact-list">
            <li>
              <i class="fa-regular fa-envelope"></i>
              <span>
                <a href="mailto:202301070187@mitaoe.ac.in">202301070187@mitaoe.ac.in</a>
              </span>
            </li>
            <li>
              <i class="fa-regular fa-envelope"></i>
              <span>
                <a href="mailto:swapnillonkar0606@gmail.com">swapnillonkar0606@gmail.com</a>
              </span>
            </li>
            <li>
              <i class="fa-solid fa-phone"></i>
              <span>+91 84830 40612</span>
            </li>
            <li>
              <i class="fa-brands fa-linkedin"></i>
              <span>
                <a
                  href="https://www.linkedin.com/in/swapnil-lonkar-5304a6283"
                  target="_blank"
                  rel="noreferrer"
                >
                  linkedin.com/in/swapnil-lonkar-5304a6283
                </a>
              </span>
            </li>
            <li>
              <i class="fa-solid fa-location-dot"></i>
              <span>Georai, Tal. Newasa, Dist. Ahilyanagar, Maharashtra – 414604</span>
            </li>
          </ul>

          <p class="small-note">
            Languages: English, Marathi, Hindi · Date of Birth: 06 Apr 2005
          </p>
        </div>

        <div class="card">
          <div class="skill-category-title" style="margin-bottom: 8px;">
            Quick Message Template
          </div>
          <p style="font-size: 12px; color: var(--muted); margin-bottom: 8px;">
            You can copy-paste this while emailing me:
          </p>
          <pre
            style="
              background: #020617;
              border-radius: 12px;
              padding: 10px;
              font-size: 11px;
              color: #e5e7eb;
              overflow-x: auto;
              border: 1px solid var(--border);
            "
          >Subject: Opportunity for Collaboration / Internship

    <footer>
      <span>© <span id="year"></span> Swapnil Lahu Lonkar</span>
      <span>Built with HTML & CSS · Hosted on GitHub Pages</span>
    </footer>
  </main>

  <script>
    // Set current year in footer
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
