# CodeAlpha_Portfoliosite
<!-- FILE NAME: index.html -->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Yuvaraj Portfolio</title>

  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:'Poppins',sans-serif;
      scroll-behavior:smooth;
    }

    body{
      background:#0f172a;
      color:white;
    }

    /* Navbar */

    nav{
      position:fixed;
      top:0;
      width:100%;
      padding:18px 8%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      background:rgba(15,23,42,0.95);
      backdrop-filter:blur(10px);
      z-index:1000;
    }

    nav h1{
      color:#38bdf8;
      font-size:28px;
    }

    nav ul{
      display:flex;
      list-style:none;
      gap:25px;
    }

    nav ul li a{
      color:white;
      text-decoration:none;
      transition:0.3s;
    }

    nav ul li a:hover{
      color:#38bdf8;
    }

    /* Hero Section */

    .hero{
      min-height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      flex-wrap:wrap;
      padding:120px 8% 60px;
      gap:50px;
    }

    .hero-image img{
      width:320px;
      height:320px;
      object-fit:cover;
      border-radius:50%;
      border:6px solid #38bdf8;
      box-shadow:0 0 30px rgba(56,189,248,0.5);
      animation:float 3s ease-in-out infinite;
    }

    @keyframes float{
      0%,100%{
        transform:translateY(0);
      }
      50%{
        transform:translateY(-10px);
      }
    }

    .hero-text{
      max-width:600px;
    }

    .hero-text h2{
      font-size:55px;
      margin-bottom:10px;
    }

    .hero-text h2 span{
      color:#38bdf8;
    }

    .hero-text h3{
      color:#94a3b8;
      margin-bottom:20px;
      font-weight:400;
    }

    .hero-text p{
      line-height:1.8;
      color:#cbd5e1;
    }

    .btn{
      display:inline-block;
      margin-top:25px;
      padding:12px 28px;
      background:#38bdf8;
      color:black;
      text-decoration:none;
      border-radius:30px;
      font-weight:600;
      transition:0.3s;
    }

    .btn:hover{
      background:white;
      transform:scale(1.05);
    }

    /* Sections */

    section{
      padding:90px 8%;
    }

    .title{
      text-align:center;
      font-size:40px;
      margin-bottom:50px;
      color:#38bdf8;
    }

    /* About */

    .about-box{
      background:#1e293b;
      padding:35px;
      border-radius:20px;
      line-height:1.9;
      transition:0.4s;
    }

    .about-box:hover{
      transform:translateY(-5px);
    }

    /* Skills */

    .skills{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
      gap:25px;
    }

    .skill-card{
      background:#1e293b;
      padding:30px;
      border-radius:20px;
      text-align:center;
      transition:0.4s;
    }

    .skill-card:hover{
      background:#38bdf8;
      color:black;
      transform:translateY(-10px);
    }

    /* Projects */

    .projects{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:25px;
    }

    .project-card{
      background:#1e293b;
      padding:25px;
      border-radius:20px;
      transition:0.4s;
    }

    .project-card:hover{
      transform:translateY(-10px);
      box-shadow:0 0 25px rgba(56,189,248,0.4);
    }

    .project-card h3{
      color:#38bdf8;
      margin-bottom:15px;
    }

    /* Resume */

    .resume{
      text-align:center;
    }

    .resume img{
      width:100%;
      max-width:800px;
      border-radius:20px;
      border:4px solid #38bdf8;
      box-shadow:0 0 25px rgba(56,189,248,0.3);
    }

    /* Contact */

    .contact{
      text-align:center;
      line-height:2;
      font-size:18px;
    }

    footer{
      text-align:center;
      padding:20px;
      background:#020617;
      color:#94a3b8;
    }

    /* Responsive */

    @media(max-width:768px){

      nav{
        flex-direction:column;
        gap:15px;
      }

      nav ul{
        flex-wrap:wrap;
        justify-content:center;
      }

      .hero{
        text-align:center;
      }

      .hero-text h2{
        font-size:38px;
      }

      .hero-image img{
        width:250px;
        height:250px;
      }

      .title{
        font-size:32px;
      }
    }

  </style>
</head>

<body>

  <!-- NAVBAR -->

  <nav>
    <h1>YUVARAJ</h1>

    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#resume">Resume</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->

  <section class="hero" id="home">

    <div class="hero-image">

      <!-- Replace your image name here -->
      <img src="yuvaraj.jpg" alt="Yuvaraj">

    </div>

    <div class="hero-text">

      <h2>Hello, I'm <span>Yuvaraj V</span></h2>

      <h3>Web Designer | BE CSE Student</h3>

      <p>
        Motivated and enthusiastic Computer Science student with strong interest in
        Web Design and Cybersecurity. Passionate about learning modern technologies
        and building creative responsive websites.
      </p>

      <a href="#projects" class="btn">View Projects</a>

    </div>

  </section>

  <!-- ABOUT -->

  <section id="about">

    <h2 class="title">About Me</h2>

    <div class="about-box">

      <p>
        I am currently pursuing BE Computer Science and Engineering.
        I enjoy creating modern websites and user-friendly interfaces.
        I am interested in Front-End Development, UI/UX Design,
        Cybersecurity and Problem Solving.
      </p>

    </div>

  </section>

  <!-- SKILLS -->

  <section id="skills">

    <h2 class="title">Skills</h2>

    <div class="skills">

      <div class="skill-card">
        <h3>HTML</h3>
      </div>

      <div class="skill-card">
        <h3>CSS</h3>
      </div>

      <div class="skill-card">
        <h3>JavaScript</h3>
      </div>

      <div class="skill-card">
        <h3>Web Design</h3>
      </div>

      <div class="skill-card">
        <h3>UI/UX Design</h3>
      </div>

      <div class="skill-card">
        <h3>GitHub</h3>
      </div>

    </div>

  </section>

  <!-- PROJECTS -->

  <section id="projects">

    <h2 class="title">Projects</h2>

    <div class="projects">

      <div class="project-card">
        <h3>Cyber Protect AI</h3>

        <p>
          AI-based cybersecurity system for detecting malicious and phishing websites.
        </p>
      </div>

      <div class="project-card">
        <h3>Image Gallery</h3>

        <p>
          Responsive image gallery with hover effects and smooth animations.
        </p>
      </div>

      <div class="project-card">
        <h3>Music Player</h3>

        <p>
          Stylish Tamil music player with playlist and audio controls.
        </p>
      </div>

    </div>

  </section>

  <!-- RESUME -->

  <section id="resume">

    <h2 class="title">My Resume</h2>

    <div class="resume">

      <!-- Replace your resume image name -->
      <img src="resume.jpg" alt="Resume">

      <br>

      <!-- Optional Resume PDF -->
      <a href="resume.pdf" class="btn" download>
        Download Resume
      </a>

    </div>

  </section>

  <!-- CONTACT -->

  <section id="contact">

    <h2 class="title">Contact Me</h2>

    <div class="contact">

      <p>📞 +91 8438201053</p>

      <p>📧 yuvaraj72227@gmail.com</p>

      <p>🌐 yuvaraj.wordpress.com</p>

      <p>📍 Chennai, Tamil Nadu, India</p>

    </div>

  </section>

  <!-- FOOTER -->

  <footer>
    © 2026 Yuvaraj V | Portfolio Website
  </footer>

</body>
</html>
