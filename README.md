<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Shreyas Rao | Electronics & AI Engineer</title>

  <meta name="description"
        content="Shreyas Rao — Electronics and Communication Engineering student passionate about Embedded Systems, IoT, AI, Edge AI and Full-Stack Development.">

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap"
        rel="stylesheet">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Inter", sans-serif;
      background: #0b0f14;
      color: #e6edf3;
      line-height: 1.6;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(1150px, 92%);
      margin: auto;
    }

    /* NAVBAR */

    nav {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(11, 15, 20, 0.85);
      backdrop-filter: blur(15px);
      border-bottom: 1px solid #21262d;
    }

    .nav-container {
      height: 70px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 22px;
      font-weight: 800;
    }

    .logo span {
      color: #58a6ff;
    }

    .nav-links {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    .nav-links a {
      color: #8b949e;
      font-size: 14px;
      transition: 0.3s;
    }

    .nav-links a:hover {
      color: #58a6ff;
    }

    /* HERO */

    .hero {
      min-height: 90vh;
      display: flex;
      align-items: center;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: "";
      position: absolute;
      width: 500px;
      height: 500px;
      background: #1f6feb;
      opacity: 0.08;
      filter: blur(120px);
      border-radius: 50%;
      top: 10%;
      left: 50%;
      transform: translateX(-50%);
    }

    .hero-content {
      position: relative;
      width: 100%;
    }

    .profile-img {
      width: 145px;
      height: 145px;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid #30363d;
      margin-bottom: 25px;
    }

    .hero h1 {
      font-size: clamp(40px, 7vw, 72px);
      font-weight: 800;
      letter-spacing: -3px;
    }

    .hero h1 span {
      color: #58a6ff;
    }

    .hero h2 {
      margin-top: 12px;
      font-size: clamp(18px, 3vw, 25px);
      color: #8b949e;
      font-weight: 500;
    }

    .hero p {
      max-width: 720px;
      margin: 22px auto;
      color: #8b949e;
      font-size: 16px;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 12px;
      flex-wrap: wrap;
      margin-top: 25px;
    }

    .btn {
      padding: 12px 22px;
      border-radius: 8px;
      border: 1px solid #30363d;
      font-weight: 600;
      font-size: 14px;
      transition: 0.3s;
    }

    .btn-primary {
      background: #238636;
      border-color: #238636;
    }

    .btn:hover {
      transform: translateY(-2px);
      border-color: #58a6ff;
    }

    /* SECTIONS */

    section {
      padding: 90px 0;
    }

    .section-title {
      font-size: 32px;
      margin-bottom: 12px;
    }

    .section-subtitle {
      color: #8b949e;
      margin-bottom: 40px;
    }

    /* ABOUT */

    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 40px;
    }

    .about-card {
      background: #11161d;
      border: 1px solid #21262d;
      border-radius: 14px;
      padding: 28px;
    }

    .about-card h3 {
      margin-bottom: 15px;
    }

    .about-card p {
      color: #8b949e;
    }

    /* SKILLS */

    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
      gap: 18px;
    }

    .skill-card {
      background: #11161d;
      border: 1px solid #21262d;
      border-radius: 12px;
      padding: 22px;
      transition: 0.3s;
    }

    .skill-card:hover {
      transform: translateY(-5px);
      border-color: #58a6ff;
    }

    .skill-card h3 {
      margin-bottom: 15px;
    }

    .badges {
      display: flex;
      flex-wrap: wrap;
      gap: 7px;
    }

    .badges img {
      height: 25px;
    }

    /* PROJECTS */

    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .project-card {
      background: #11161d;
      border: 1px solid #21262d;
      border-radius: 14px;
      padding: 25px;
      display: flex;
      flex-direction: column;
      transition: 0.3s;
    }

    .project-card:hover {
      transform: translateY(-6px);
      border-color: #58a6ff;
    }

    .project-card h3 {
      margin-bottom: 12px;
    }

    .project-card p {
      color: #8b949e;
      font-size: 14px;
      margin-bottom: 20px;
    }

    .project-tech {
      margin-top: auto;
      color: #58a6ff;
      font-size: 13px;
    }

    .project-link {
      display: inline-block;
      margin-top: 15px;
      color: #58a6ff;
      font-weight: 600;
    }

    /* STATS */

    .stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
    }

    .stats img {
      width: 100%;
      border-radius: 10px;
      background: #11161d;
    }

    /* CONTACT */

    .contact {
      text-align: center;
    }

    .socials {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 12px;
      margin-top: 25px;
    }

    .social {
      padding: 12px 18px;
      border: 1px solid #30363d;
      border-radius: 8px;
      color: #c9d1d9;
      transition: 0.3s;
    }

    .social:hover {
      border-color: #58a6ff;
      color: #58a6ff;
    }

    /* QUOTE */

    .quote {
      text-align: center;
      border-top: 1px solid #21262d;
      border-bottom: 1px solid #21262d;
      padding: 60px 20px;
    }

    .quote blockquote {
      font-size: 22px;
      font-weight: 600;
      max-width: 700px;
      margin: auto;
    }

    .quote p {
      margin-top: 15px;
      color: #8b949e;
    }

    /* FOOTER */

    footer {
      padding: 35px 0;
      text-align: center;
      color: #6e7681;
      font-size: 13px;
    }

    /* MOBILE */

    @media (max-width: 768px) {

      .nav-links {
        display: none;
      }

      .about {
        grid-template-columns: 1fr;
      }

      .hero {
        min-height: 80vh;
      }

      section {
        padding: 65px 0;
      }

      .hero h1 {
        letter-spacing: -2px;
      }
    }
  </style>
</head>

<body>

  <!-- NAVIGATION -->

  <nav>
    <div class="container nav-container">

      <a href="#" class="logo">
        SR<span>.</span>
      </a>

      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#stats">GitHub</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>

    </div>
  </nav>


  <!-- HERO -->

  <header class="hero">

    <div class="container hero-content">

      <!-- Replace with your own photo -->
      <img
        src="https://avatars.githubusercontent.com/u/YOUR_GITHUB_ID"
        alt="Shreyas Rao"
        class="profile-img"
      >

      <h1>
        Hi, I'm <span>Shreyas Rao</span> 👋
      </h1>

      <h2>
        Electronics & Communication Engineering Student
      </h2>

      <p>
        I build intelligent systems at the intersection of
        <strong>Embedded Systems, IoT, AI, Edge AI and Software Development.</strong>
        I enjoy turning hardware ideas into practical, connected products.
      </p>

      <div class="buttons">

        <a
          href="https://github.com/YOUR_USERNAME"
          target="_blank"
          class="btn btn-primary"
        >
          View GitHub
        </a>

        <a
          href="https://www.linkedin.com/in/YOUR_LINKEDIN"
          target="_blank"
          class="btn"
        >
          LinkedIn
        </a>

        <a
          href="#projects"
          class="btn"
        >
          Explore Projects
        </a>

      </div>

    </div>

  </header>


  <!-- ABOUT -->

  <section id="about">

    <div class="container">

      <h2 class="section-title">👨‍💻 About Me</h2>

      <p class="section-subtitle">
        A quick introduction
      </p>

      <div class="about">

        <div class="about-card">

          <h3>🚀 Who I Am</h3>

          <p>
            I'm an Electronics and Communication Engineering student passionate
            about developing intelligent hardware and software systems.
            My interests include embedded systems, IoT, AI/ML, Edge AI,
            firmware development and full-stack applications.
          </p>

          <br>

          <p>
            I enjoy working on projects that combine sensors, microcontrollers,
            communication protocols, cloud platforms and intelligent algorithms.
          </p>

        </div>


        <div class="about-card">

          <h3>🎯 Current Focus</h3>

          <p>
            Currently improving my skills in:
          </p>

          <br>

          <ul>
            <li>⚡ Embedded Systems & Firmware</li>
            <li>🤖 Artificial Intelligence & Machine Learning</li>
            <li>🌐 IoT & Wireless Sensor Networks</li>
            <li>🧠 Edge AI</li>
            <li>💻 Full-Stack Development</li>
            <li>🧩 Data Structures & Algorithms</li>
          </ul>

        </div>

      </div>

    </div>

  </section>


  <!-- SKILLS -->

  <section id="skills">

    <div class="container">

      <h2 class="section-title">🛠️ Skills & Technologies</h2>

      <p class="section-subtitle">
        Technologies I work with and continuously explore.
      </p>


      <div class="skills-grid">

        <!-- Programming -->

        <div class="skill-card">

          <h3>💻 Programming</h3>

          <div class="badges">

            <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white">

            <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black">

            <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white">

            <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">

          </div>

        </div>


        <!-- Embedded -->

        <div class="skill-card">

          <h3>⚡ Embedded Systems</h3>

          <div class="badges">

            <img src="https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white">

            <img src="https://img.shields.io/badge/STM32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white">

            <img src="https://img.shields.io/badge/FreeRTOS-003B57?style=for-the-badge">

            <img src="https://img.shields.io/badge/UART%20%7C%20SPI%20%7C%20I2C-555555?style=for-the-badge">

          </div>

        </div>


        <!-- AI -->

        <div class="skill-card">

          <h3>🤖 AI / ML</h3>

          <div class="badges">

            <img src="https://img.shields.io/badge/Machine%20Learning-F7931E?style=for-the-badge">

            <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white">

            <img src="https://img.shields.io/badge/AI-412991?style=for-the-badge">

            <img src="https://img.shields.io/badge/GenAI-8E44AD?style=for-the-badge">

          </div>

        </div>


        <!-- IoT -->

        <div class="skill-card">

          <h3>🌐 IoT & Connectivity</h3>

          <div class="badges">

            <img src="https://img.shields.io/badge/IoT-0082FC?style=for-the-badge">

            <img src="https://img.shields.io/badge/LoRa-0D8ABC?style=for-the-badge">

            <img src="https://img.shields.io/badge/Blynk-23C48E?style=for-the-badge">

            <img src="https://img.shields.io/badge/Google%20Apps%20Script-4285F4?style=for-the-badge&logo=google&logoColor=white">

          </div>

        </div>


        <!-- Web -->

        <div class="skill-card">

          <h3>🌎 Web Development</h3>

          <div class="badges">

            <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">

            <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white">

            <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">

            <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white">

          </div>

        </div>


        <!-- Tools -->

        <div class="skill-card">

          <h3>🔧 Tools</h3>

          <div class="badges">

            <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white">

            <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github">

            <img src="https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white">

            <img src="https://img.shields.io/badge/LTspice-B31B1B?style=for-the-badge">

          </div>

        </div>

      </div>

    </div>

  </section>


  <!-- PROJECTS -->

  <section id="projects">

    <div class="container">

      <h2 class="section-title">🚀 Featured Projects</h2>

      <p class="section-subtitle">
        Selected projects demonstrating my engineering and development skills.
      </p>


      <div class="projects">


        <!-- PROJECT 1 -->

        <div class="project-card">

          <h3>🌱 Smart Agriculture WSN</h3>

          <p>
            AI-assisted wireless sensor network designed for smart agriculture.
            Uses ESP32 sensor nodes, LoRa communication and intelligent
            irrigation prediction with animal-threat detection.
          </p>

          <div class="project-tech">
            ESP32 • LoRa • AI/ML • IoT • Sensors
          </div>

          <a
            href="https://github.com/YOUR_USERNAME/smart-agriculture"
            target="_blank"
            class="project-link"
          >
            View Project →
          </a>

        </div>


        <!-- PROJECT 2 -->

        <div class="project-card">

          <h3>💧 IoT Automated Irrigation</h3>

          <p>
            ESP32-based automated irrigation and energy monitoring system
            featuring soil monitoring, pump control, sequential solenoid
            valves and cloud-based data logging.
          </p>

          <div class="project-tech">
            ESP32 • Blynk • Google Apps Script • IoT
          </div>

          <a
            href="https://github.com/YOUR_USERNAME/iot-irrigation"
            target="_blank"
            class="project-link"
          >
            View Project →
          </a>

        </div>


        <!-- PROJECT 3 -->

        <div class="project-card">

          <h3>🎮 RetroArcade</h3>

          <p>
            Browser-based arcade platform built with HTML5 Canvas and
            Supabase, featuring interactive games and leaderboard functionality.
          </p>

          <div class="project-tech">
            HTML5 • CSS • JavaScript • Supabase
          </div>

          <a
            href="https://github.com/YOUR_USERNAME/retroarcade"
            target="_blank"
            class="project-link"
          >
            View Project →
          </a>

        </div>


        <!-- PROJECT 4 -->

        <div class="project-card">

          <h3>🚁 STM32 Drone Flight Controller</h3>

          <p>
            Embedded drone flight-control system using STM32, MPU6050,
            PID control and FreeRTOS-based task scheduling for sensor
            acquisition, communication and motor control.
          </p>

          <div class="project-tech">
            STM32 • FreeRTOS • MPU6050 • PID • Embedded C
          </div>

          <a
            href="https://github.com/YOUR_USERNAME/stm32-drone"
            target="_blank"
            class="project-link"
          >
            View Project →
          </a>

        </div>


      </div>

    </div>

  </section>


  <!-- GITHUB STATS -->

  <section id="stats">

    <div class="container">

      <h2 class="section-title">📊 GitHub Statistics</h2>

      <p class="section-subtitle">
        My coding activity and open-source journey.
      </p>


      <div class="stats">

        <img
          src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=github_dark&hide_border=true"
          alt="GitHub Statistics"
        >

        <img
          src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=github_dark&hide_border=true"
          alt="Most Used Languages"
        >

      </div>

    </div>

  </section>


  <!-- CONTACT -->

  <section id="contact">

    <div class="container contact">

      <h2 class="section-title">📬 Let's Connect</h2>

      <p class="section-subtitle">
        Interested in technology, collaboration, internships or interesting projects?
        Feel free to connect with me.
      </p>


      <div class="socials">

        <a
          href="https://github.com/YOUR_USERNAME"
          target="_blank"
          class="social"
        >
          🐙 GitHub
        </a>

        <a
          href="https://www.linkedin.com/in/YOUR_LINKEDIN"
          target="_blank"
          class="social"
        >
          💼 LinkedIn
        </a>

        <a
          href="mailto:YOUR_EMAIL@example.com"
          class="social"
        >
          📧 Email
        </a>

        <a
          href="https://yourportfolio.com"
          target="_blank"
          class="social"
        >
          🌐 Portfolio
        </a>

      </div>

    </div>

  </section>


  <!-- QUOTE -->

  <div class="quote">

    <blockquote>
      "Build things that solve real problems. Keep learning. Keep improving."
    </blockquote>

    <p>
      — Shreyas Rao
    </p>

  </div>


  <!-- FOOTER -->

  <footer>

    <div class="container">

      © 2026 Shreyas Rao • Built with HTML & CSS • Always learning 🚀

    </div>

  </footer>


</body>
</html>
