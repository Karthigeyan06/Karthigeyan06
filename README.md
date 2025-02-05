
  
  <!DOCTYPE html>
  <html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Karthigeyan G. Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/animate.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/gsap@3.9.1/dist/gsap.min.js"></script>
    <style>
        /* Custom Tailwind CSS */
        body {
            font-family: 'Poppins', sans-serif;
        }
        .bg-gradient-custom {
            background: linear-gradient(to bottom right, #000000, #434343);
        }
        .bg-gradient-button {
            background: linear-gradient(to right, #00b5cc, #8b5cf6);
        }
        .btn-hover:hover {
            background: #ec4899;
            transform: scale(1.05);
        }
        .scale-on-hover:hover {
            transform: scale(1.05);
        }
        .animate__animated {
            animation-duration: 1s;
        }

        /* Hero Section - Text Visibility Fix */
        .hero-name {
            background: linear-gradient(to right, #00b5cc, #8b5cf6);
            -webkit-background-clip: text;
            color: transparent;
            font-size: 4rem;
            font-weight: 800;
            text-align: center;
            animation: pulse 1.5s infinite;
        }

        /* Project Box Styles */
        .project-box {
            background: linear-gradient(to bottom, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.9));
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .project-box:hover {
            border: 3px solid #00b5cc;
            box-shadow: 0 0 15px 5px #00b5cc;
            transform: scale(1.05);
        }

        .project-box .project-image-container {
            overflow: hidden;
        }

        .project-box img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
            transition: transform 0.3s ease;
        }

        .project-box:hover img {
            transform: scale(1.1);
        }

        .project-content {
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            padding: 10px;
            color: white;
            transition: transform 0.3s ease;
            display: flex;
            flex-direction: column; /* Stack elements vertically */
        }

        .project-content::before { /* Gradient overlay below text */
            content: "";
            position: absolute;
            top: 0;  /* Start from the top of the content */
            left: 0;
            width: 100%;
            height: 100%; /* Cover the entire content area */
            background: linear-gradient(to bottom, transparent, rgba(0, 0, 0, 0.5)); /* Transparent to solid */
            z-index: -1; /* Place behind the text */
        }

        .project-content:hover {
            transform: translateY(-10px);
        }

        .project-content h3 {
            margin-bottom: 5px;
        }

        .project-content a {
            background-color: #00b5cc;
            padding: 5px 10px;
            border-radius: 5px;
            text-decoration: none;
            color: white;
            display: inline-block;
        }
    </style>
  </head>
  <body class="bg-gradient-custom text-white">
    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 right-0 bg-black bg-opacity-80 shadow-lg z-50 py-4 px-8 flex justify-between items-center border-b border-gray-700">
      <h1 class="text-2xl font-bold text-cyan-400">Karthigeyan G.</h1>
      <ul class="flex space-x-6 text-lg">
        <li><a href="#about" class="hover:text-cyan-400 transition">About</a></li>
        <li><a href="#projects" class="hover:text-cyan-400 transition">Projects</a></li>
        <li><a href="#experience" class="hover:text-cyan-400 transition">Experience</a></li>
        <li><a href="#skills" class="hover:text-cyan-400 transition">Skills</a></li>
        <li><a href="#contact" class="hover:text-cyan-400 transition">Contact</a></li>
      </ul>
    </nav>
  
    <!-- Hero Section -->
    <section class="h-screen flex flex-col items-center justify-center text-center px-4 mt-16">
      <h1 class="hero-name animate__animated animate__pulse">Hello, I'm Karthigeyan</h1>
      <p class="text-lg md:text-xl text-gray-400 max-w-2xl animate__animated animate__fadeIn animate__delay-500ms">Embedded Systems & IoT Enthusiast | Electronics & Communication Engineer</p>
      <div class="mt-8 flex space-x-8 animate__animated animate__fadeIn animate__delay-1000ms">
        <a href="mailto:karthigeyanganesan06@gmail.com" class="text-gray-400 hover:text-cyan-400 transition"><img src="https://img.icons8.com/ios-filled/50/000000/mail.png" alt="Mail" class="w-9 h-9" /></a>
        <a href="https://www.linkedin.com/in/karthigeyan-ganesan-203066257/" target="_blank" class="text-gray-400 hover:text-cyan-400 transition"><img src="https://img.icons8.com/ios-filled/50/000000/linkedin.png" alt="Linkedin" class="w-9 h-9" /></a>
        <a href="https://github.com/Karthigeyan06" target="_blank" class="text-gray-400 hover:text-cyan-400 transition"><img src="https://img.icons8.com/ios-filled/50/000000/github.png" alt="Github" class="w-9 h-9" /></a>
      </div>
    </section>
  
     <!-- Projects Section -->
     <section id="projects" class="py-20 bg-gradient-custom px-8">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-10 max-w-6xl mx-auto">
            <div class="project-box scale-on-hover rounded-2xl shadow-lg overflow-hidden transition duration-300">
                <div class="project-image-container"> <img src="C:\Users\karth\Downloads\20241118_082657.jpg" alt="Project 1" /> </div>
                <div class="project-content">  <h3>Project 1</h3>
                    <p>Description of project 1</p>
                    <a href="https://github.com/Karthigeyan06" target="_blank">View Project</a>
                </div>
            </div>

            <div class="project-box scale-on-hover rounded-2xl shadow-lg overflow-hidden transition duration-300">
                <div class="project-image-container"> <img src="https://via.placeholder.com/300x200?text=Project+2" alt="Project 2" /> </div>
                <div class="project-content">  <h3>Project 2</h3>
                    <p>Description of project 2</p>
                    <a href="https://github.com/Karthigeyan06" target="_blank">View Project</a>
                </div>
            </div>

            <div class="project-box scale-on-hover rounded-2xl shadow-lg overflow-hidden transition duration-300">
                <div class="project-image-container"> <img src="https://via.placeholder.com/300x200?text=Project+3" alt="Project 3" /> </div>
                 <div class="project-content">  <h3>Project 3</h3>
                    <p>Description of project 3</p>
                    <a href="https://github.com/Karthigeyan06" target="_blank">View Project</a>
                </div>
            </div>

        </div>

    </section>
  
  
    <!-- About Section -->
    <section id="about" class="py-20 bg-gradient-custom px-8">
      <h2 class="text-4xl font-bold text-center mb-6 text-cyan-400 animate__animated animate__fadeInUp">About Me</h2>
      <p class="text-center text-lg text-gray-400 max-w-3xl mx-auto animate__animated animate__fadeInUp animate__delay-500ms">
        I'm an Electronics & Communication Engineer with a passion for Embedded Systems and IoT. Over the years, I've worked on projects involving microcontrollers, automation systems, and smart devices.
      </p>
    </section>
  
    
    <!-- Experience Section -->
    <section id="experience" class="py-20 bg-gradient-custom px-8">
      <h2 class="text-4xl font-bold text-center mb-6 text-cyan-400 animate__animated animate__fadeInUp">Experience</h2>
      <div class="max-w-4xl mx-auto space-y-8">
        <div class="p-6 bg-gray-800 shadow-md rounded-2xl">
          <h3 class="text-2xl font-semibold text-cyan-400">Delphi-TVS Technologies Limited</h3>
          <p class="text-gray-400">Engineering Intern | Dec 2024 – Jan 2025</p>
          <p class="mt-2 text-gray-400">Worked on machine troubleshooting, PLC programming, and CNC maintenance. Developed a QR code-based web app to track machine data.</p>
        </div>
        <div class="p-6 bg-gray-800 shadow-md rounded-2xl">
          <h3 class="text-2xl font-semibold text-cyan-400">Rook Ecom Pvt Ltd</h3>
          <p class="text-gray-400">Techie Intern | Jan 2023 – Apr 2023</p>
          <p class="mt-2 text-gray-400">Enhanced WordPress websites and optimized user experience.</p>
        </div>
      </div>
    </section>
  
    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-gradient-custom px-8">
      <h2 class="text-4xl font-bold text-center mb-12 text-cyan-400 animate__animated animate__fadeInUp">Skills & Tools</h2>
      <div class="max-w-6xl mx-auto space-y-12 text-center">
        <div>
          <h3 class="text-2xl font-semibold text-cyan-400 mb-4">Programming Languages</h3>
          <div class="flex flex-wrap justify-center gap-6">
           
            <div class="scale-on-hover p-4 bg-gray-800 rounded-xl shadow-md cursor-pointer">
              <img src="https://via.placeholder.com/50x50?text=C++" alt="C++" class="mx-auto mb-2" />
              <p class="text-center text-gray-400 font-medium">C++</p>
            </div>
  
            <div class="scale-on-hover p-4 bg-gray-800 rounded-xl shadow-md cursor-pointer">
              <img src="C:\Users\karth\Downloads\Python-logo-notext.svg.png" alt="Python" class="mx-auto mb-2 w-16 h-16 object-contain" />
              <p class="text-center text-gray-400 font-medium">Python</p>
            </div>
            <!-- More Skills -->
          </div>
        </div>
      </div>
    </section>
  
    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gradient-custom px-8">
      <h2 class="text-4xl font-bold text-center mb-6 text-cyan-400 animate__animated animate__fadeInUp">Get In Touch</h2>
      <div class="text-center mb-6">
        <p class="text-lg text-gray-400 mb-6">Feel free to reach out to me for collaboration or any inquiries.</p>
        <a href="mailto:karthigeyanganesan06@gmail.com" class="btn-hover text-black bg-cyan-400 px-8 py-3 rounded-full shadow-lg">Email Me</a>
      </div>
    </section>
  
  
    <footer class="bg-black bg-opacity-80 py-4 text-center text-gray-400">
      <p>&copy; 2025 Karthigeyan G. All Rights Reserved.</p>
    </footer>
  
    <script>
      // Animation using GSAP
      gsap.from("section", { opacity: 0, duration: 1, y: 50, stagger: 0.3 });
    </script>
  </body>
  </html>
  
  
