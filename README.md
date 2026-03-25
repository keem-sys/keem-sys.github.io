<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Ebenezer Kouakou — CV</title>
  <link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Mono:wght@300;400;500&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet"/>
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --bg: #0c0f0a;
      --surface: #141710;
      --border: #2a2e24;
      --accent: #b8f55a;
      --accent-dim: #8ab83e;
      --text: #e8ead4;
      --muted: #7a7d6a;
      --tag-bg: #1c2014;
    }

    html { scroll-behavior: smooth; }

    body {
      background: var(--bg);
      color: var(--text);
      font-family: 'DM Sans', sans-serif;
      font-weight: 300;
      line-height: 1.7;
      min-height: 100vh;
      padding: 0;
      overflow-x: hidden;
    }

    /* Grain overlay */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
      pointer-events: none;
      z-index: 100;
      opacity: 0.4;
    }

    .container {
      max-width: 860px;
      margin: 0 auto;
      padding: 60px 32px 100px;
    }

    /* Header */
    header {
      border-bottom: 1px solid var(--border);
      padding-bottom: 48px;
      margin-bottom: 56px;
      animation: fadeUp 0.6s ease both;
    }

    .header-top {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 24px;
      flex-wrap: wrap;
    }

    .name-block h1 {
      font-family: 'DM Serif Display', serif;
      font-size: clamp(2.4rem, 6vw, 4rem);
      font-weight: 400;
      line-height: 1.1;
      letter-spacing: -0.02em;
      color: var(--text);
    }

    .name-block h1 span {
      color: var(--accent);
    }

    .name-block .title {
      font-family: 'DM Mono', monospace;
      font-size: 0.78rem;
      color: var(--muted);
      letter-spacing: 0.12em;
      text-transform: uppercase;
      margin-top: 8px;
    }

    .contact-block {
      display: flex;
      flex-direction: column;
      gap: 6px;
      align-items: flex-end;
      padding-top: 6px;
    }

    .contact-block a {
      font-family: 'DM Mono', monospace;
      font-size: 0.75rem;
      color: var(--muted);
      text-decoration: none;
      transition: color 0.2s;
      letter-spacing: 0.02em;
    }

    .contact-block a:hover { color: var(--accent); }

    .contact-block span {
      font-family: 'DM Mono', monospace;
      font-size: 0.75rem;
      color: var(--muted);
    }

    .profile-text {
      margin-top: 32px;
      font-size: 1.05rem;
      color: #b8baa6;
      max-width: 640px;
      line-height: 1.8;
    }

    /* Sections */
    section {
      margin-bottom: 52px;
      animation: fadeUp 0.6s ease both;
    }

    section:nth-child(2) { animation-delay: 0.1s; }
    section:nth-child(3) { animation-delay: 0.2s; }
    section:nth-child(4) { animation-delay: 0.3s; }
    section:nth-child(5) { animation-delay: 0.4s; }

    .section-label {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--accent);
      margin-bottom: 24px;
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .section-label::after {
      content: '';
      flex: 1;
      height: 1px;
      background: var(--border);
    }

    /* Education */
    .edu-item {
      display: grid;
      grid-template-columns: 1fr auto;
      gap: 8px 24px;
      padding: 20px 0;
      border-bottom: 1px solid var(--border);
    }

    .edu-item:last-child { border-bottom: none; }

    .edu-degree {
      font-size: 0.95rem;
      font-weight: 500;
      color: var(--text);
      line-height: 1.4;
    }

    .edu-school {
      font-size: 0.85rem;
      color: var(--muted);
      margin-top: 2px;
    }

    .edu-badge {
      background: var(--tag-bg);
      border: 1px solid var(--border);
      color: var(--accent-dim);
      font-family: 'DM Mono', monospace;
      font-size: 0.65rem;
      padding: 3px 8px;
      border-radius: 2px;
      letter-spacing: 0.08em;
      white-space: nowrap;
      height: fit-content;
      margin-top: 4px;
    }

    .edu-date {
      font-family: 'DM Mono', monospace;
      font-size: 0.72rem;
      color: var(--muted);
      text-align: right;
      grid-column: 2;
      grid-row: 1;
    }

    /* Projects */
    .project-item {
      padding: 24px;
      border: 1px solid var(--border);
      border-radius: 4px;
      margin-bottom: 16px;
      background: var(--surface);
      transition: border-color 0.2s, transform 0.2s;
      position: relative;
      overflow: hidden;
    }

    .project-item::before {
      content: '';
      position: absolute;
      left: 0; top: 0; bottom: 0;
      width: 2px;
      background: var(--accent);
      transform: scaleY(0);
      transition: transform 0.2s;
      transform-origin: bottom;
    }

    .project-item:hover {
      border-color: #3a3e30;
      transform: translateX(4px);
    }

    .project-item:hover::before { transform: scaleY(1); }

    .project-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 16px;
      margin-bottom: 10px;
      flex-wrap: wrap;
    }

    .project-name {
      font-family: 'DM Serif Display', serif;
      font-size: 1.1rem;
      color: var(--text);
      font-weight: 400;
    }

    .project-link {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      color: var(--accent-dim);
      text-decoration: none;
      border: 1px solid var(--border);
      padding: 3px 10px;
      border-radius: 2px;
      transition: all 0.2s;
      white-space: nowrap;
    }

    .project-link:hover {
      border-color: var(--accent);
      color: var(--accent);
    }

    .project-desc {
      font-size: 0.88rem;
      color: #9a9c88;
      line-height: 1.7;
    }

    .project-desc li {
      margin-left: 16px;
      margin-bottom: 4px;
    }

    /* Skills */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }

    .skill-group h4 {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--muted);
      margin-bottom: 12px;
    }

    .skill-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
    }

    .tag {
      background: var(--tag-bg);
      border: 1px solid var(--border);
      color: #b0b29e;
      font-family: 'DM Mono', monospace;
      font-size: 0.72rem;
      padding: 4px 10px;
      border-radius: 2px;
      letter-spacing: 0.04em;
      transition: border-color 0.2s, color 0.2s;
    }

    .tag:hover {
      border-color: var(--accent-dim);
      color: var(--accent);
    }

    /* References */
    .ref-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
      gap: 16px;
    }

    .ref-card {
      padding: 20px;
      border: 1px solid var(--border);
      border-radius: 4px;
      background: var(--surface);
    }

    .ref-name {
      font-weight: 500;
      font-size: 0.95rem;
      color: var(--text);
      margin-bottom: 4px;
    }

    .ref-role {
      font-size: 0.8rem;
      color: var(--muted);
      margin-bottom: 10px;
      line-height: 1.4;
    }

    .ref-contact {
      font-family: 'DM Mono', monospace;
      font-size: 0.72rem;
      color: var(--accent-dim);
      text-decoration: none;
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--border);
      padding-top: 24px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 12px;
    }

    footer span {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      color: var(--muted);
    }

    footer a {
      font-family: 'DM Mono', monospace;
      font-size: 0.7rem;
      color: var(--accent-dim);
      text-decoration: none;
    }

    footer a:hover { color: var(--accent); }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(20px); }
      to   { opacity: 1; transform: translateY(0); }
    }

    @media (max-width: 600px) {
      .container { padding: 40px 20px 80px; }
      .header-top { flex-direction: column; }
      .contact-block { align-items: flex-start; }
      .edu-item { grid-template-columns: 1fr; }
      .edu-date { text-align: left; grid-column: 1; grid-row: auto; }
    }
  </style>
</head>
<body>
<div class="container">

  <header>
    <div class="header-top">
      <div class="name-block">
        <h1>Ebenezer<br/><span>Kouakou</span></h1>
        <p class="title">Aspiring Software Developer &nbsp;·&nbsp; Cape Town, ZA</p>
      </div>
      <div class="contact-block">
        <a href="mailto:230480152@mycput.ac.za">230480152@mycput.ac.za</a>
        <a href="tel:+27607443984">+27 607 443 984</a>
        <a href="https://ebenezerkouakou.com" target="_blank">ebenezerkouakou.com</a>
        <a href="https://github.com/keem-sys" target="_blank">github.com/keem-sys</a>
        <a href="https://linkedin.com/in/ebenezer-kouakou" target="_blank">linkedin.com/in/ebenezer-kouakou</a>
      </div>
    </div>
    <p class="profile-text">
      Aspiring software developer with a strong foundation in Java, object-oriented programming, and database fundamentals. Experienced in academic and team-based projects, with consistent academic distinction. Seeking an internship to apply technical skills, gain industry exposure, and contribute to real-world software solutions.
    </p>
  </header>

  <section>
    <div class="section-label">Education</div>
    <div class="edu-item">
      <div>
        <div class="edu-degree">Diploma: ICT in Applications Development</div>
        <div class="edu-school">Cape Peninsula University of Technology</div>
      </div>
      <div class="edu-date">2024 – 2026</div>
    </div>
    <div class="edu-item">
      <div>
        <div class="edu-degree">Higher Certificate: ICT in Information Technology</div>
        <div class="edu-school">Cape Peninsula University of Technology</div>
      </div>
      <div style="text-align:right;">
        <div class="edu-date">2023</div>
        <div class="edu-badge">Summa Cum Laude</div>
      </div>
    </div>
    <div class="edu-item">
      <div>
        <div class="edu-degree">High School Matric</div>
        <div class="edu-school">College Catholique Mgr Kirman</div>
      </div>
      <div class="edu-date">2018 – 2022</div>
    </div>
  </section>

  <section>
    <div class="section-label">Projects</div>

    <div class="project-item">
      <div class="project-header">
        <div class="project-name">ZipStore — Full Stack E-commerce Platform</div>
        <a class="project-link" href="https://zipstore-shop.vercel.app/" target="_blank">↗ Live</a>
      </div>
      <ul class="project-desc">
        <li>Engineered an e-commerce website using Java Spring Boot REST API and a React frontend.</li>
        <li>Features include secure Stripe payment processing, stateless JWT authentication, and server-state caching with React Query.</li>
      </ul>
    </div>

    <div class="project-item">
      <div class="project-header">
        <div class="project-name">Student Accommodation Finder</div>
        <a class="project-link" href="https://github.com/keemsys/ResFinder/releases" target="_blank">↗ GitHub</a>
      </div>
      <ul class="project-desc">
        <li>Collaborated with classmates to build a Java Swing desktop app helping students search and find suitable accommodations.</li>
      </ul>
    </div>

    <div class="project-item">
      <div class="project-header">
        <div class="project-name">Client–Server Enrollment System</div>
        <a class="project-link" href="https://github.com/keemsys/student-enrolment-system" target="_blank">↗ GitHub</a>
      </div>
      <ul class="project-desc">
        <li>Developed a Java Swing client-server application for managing student enrollments.</li>
        <li>Students can register for courses while administrators manage course and student data through CRUD operations.</li>
      </ul>
    </div>

    <div class="project-item">
      <div class="project-header">
        <div class="project-name">OptiPrice — Price Comparison Website</div>
        <a class="project-link" href="https://github.com/keemsys/OptiPrice" target="_blank">↗ GitHub</a>
      </div>
      <ul class="project-desc">
        <li>Currently developing a website that compares product prices across Shoprite, Pick n Pay, and Checkers.</li>
      </ul>
    </div>
  </section>

  <section>
    <div class="section-label">Skills</div>
    <div class="skills-grid">
      <div class="skill-group">
        <h4>Languages</h4>
        <div class="skill-tags">
          <span class="tag">Java</span>
          <span class="tag">JavaScript</span>
          <span class="tag">Python</span>
          <span class="tag">HTML5</span>
          <span class="tag">CSS3</span>
        </div>
      </div>
      <div class="skill-group">
        <h4>Frameworks & Libraries</h4>
        <div class="skill-tags">
          <span class="tag">Spring Boot</span>
          <span class="tag">React</span>
          <span class="tag">Redux</span>
          <span class="tag">Tailwind</span>
          <span class="tag">Hibernate/JPA</span>
          <span class="tag">React Query</span>
        </div>
      </div>
      <div class="skill-group">
        <h4>Database & Backend</h4>
        <div class="skill-tags">
          <span class="tag">MySQL</span>
          <span class="tag">PostgreSQL</span>
          <span class="tag">REST APIs</span>
          <span class="tag">JWT Auth</span>
        </div>
      </div>
      <div class="skill-group">
        <h4>Tools & Testing</h4>
        <div class="skill-tags">
          <span class="tag">Git</span>
          <span class="tag">GitHub</span>
          <span class="tag">Maven</span>
          <span class="tag">JUnit</span>
          <span class="tag">Mockito</span>
          <span class="tag">Figma</span>
          <span class="tag">Docker</span>
        </div>
      </div>
    </div>
  </section>

  <section>
    <div class="section-label">References</div>
    <div class="ref-grid">
      <div class="ref-card">
        <div class="ref-name">Chris De-Tchambila</div>
        <div class="ref-role">Software Engineer, Capgemini</div>
        <a class="ref-contact" href="mailto:christ.tchambila@gmail.com">christ.tchambila@gmail.com</a>
      </div>
      <div class="ref-card">
        <div class="ref-name">H. Botha</div>
        <div class="ref-role">Lecturer in IT Service Management, Northlink College</div>
        <a class="ref-contact" href="tel:+27827294046">+27 82 729 4046</a>
      </div>
    </div>
  </section>
  
  <footer>
    <span>Ebenezer Kouakou &nbsp;·&nbsp; Cape Town, South Africa</span>
    <a href="https://github.com/keem-sys" target="_blank">github.com/keem-sys</a>
  </footer>

</div>
</body>
</html>
