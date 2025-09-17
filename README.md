<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hillary Agbele | About Me</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0a192f, #112240, #233554);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: #e6f1ff;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow-x: hidden;
            padding: 20px;
        }
        
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .container {
            max-width: 1000px;
            width: 90%;
            text-align: center;
            padding: 50px 30px;
            background: rgba(13, 25, 48, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
            animation: fadeIn 1s ease-out;
            border: 1px solid rgba(100, 255, 218, 0.2);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .logo {
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: #64ffda;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        h1 {
            font-size: 3rem;
            margin-bottom: 15px;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            color: #ccd6f6;
        }
        
        .name-highlight {
            color: #64ffda;
            font-weight: bold;
            display: block;
            font-size: 3.5rem;
            margin-top: 10px;
        }
        
        .tagline {
            font-size: 1.5rem;
            margin-bottom: 30px;
            color: #a8b2d1;
        }
        
        .description {
            font-size: 1.2rem;
            line-height: 1.6;
            margin-bottom: 40px;
            max-width: 800px;
            margin-left: auto;
            margin-right: auto;
            color: #8892b0;
            text-align: left;
        }
        
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
            text-align: left;
        }
        
        .info-card {
            background: rgba(100, 255, 218, 0.1);
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            border: 1px solid rgba(100, 255, 218, 0.2);
        }
        
        .info-card h3 {
            color: #64ffda;
            margin-bottom: 15px;
            font-size: 1.5rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .info-card p {
            color: #a8b2d1;
            line-height: 1.6;
        }
        
        .skills {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }
        
        .skill {
            background: rgba(100, 255, 218, 0.2);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #64ffda;
        }
        
        .courses {
            list-style-type: none;
        }
        
        .courses li {
            padding: 8px 0;
            border-bottom: 1px solid rgba(100, 255, 218, 0.1);
            color: #a8b2d1;
        }
        
        .courses li:last-child {
            border-bottom: none;
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .social-icon {
            display: inline-flex;
            justify-content: center;
            align-items: center;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: rgba(136, 146, 176, 0.1);
            color: #64ffda;
            font-size: 1.5rem;
            transition: all 0.3s ease;
            text-decoration: none;
            border: 1px solid rgba(100, 255, 218, 0.2);
        }
        
        .social-icon:hover {
            background: #64ffda;
            color: #0a192f;
            transform: translateY(-5px);
        }
        
        .footer {
            margin-top: 30px;
            color: rgba(136, 146, 176, 0.7);
        }
        
        .footer-links {
            margin-bottom: 10px;
        }
        
        .footer a {
            color: #64ffda;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer a:hover {
            color: #88ffdf;
            text-decoration: underline;
        }
        
        /* Responsive design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            .name-highlight {
                font-size: 2.8rem;
            }
            
            .tagline {
                font-size: 1.2rem;
            }
            
            .info-grid {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 480px) {
            .container {
                padding: 30px 15px;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .name-highlight {
                font-size: 2.2rem;
            }
            
            .tagline {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="logo">
            <i class="fas fa-laptop-code"></i>
        </div>
        
        <h1>About <span class="name-highlight">Hillary Agbele</span></h1>
        
        <p class="tagline">Computer Science Major | Class of 2026</p>
        
        <div class="info-grid">
            <div class="info-card">
                <h3><i class="fas fa-graduation-cap"></i> Education</h3>
                <p>I'm currently pursuing a Bachelor's degree in Computer Science, expecting to graduate in 2026. This website is part of a project for one of my classes where I'm learning web development and design principles.</p>
            </div>
            
            <div class="info-card">
                <h3><i class="fas fa-map-marker-alt"></i> Background</h3>
                <p>I'm originally from West Africa, which has given me a unique perspective on technology's role in solving real-world problems. I'm passionate about using technology to create positive change in communities.</p>
            </div>
            
            <div class="info-card">
                <h3><i class="fas fa-code"></i> Skills</h3>
                <p>As a computer science student, I'm developing skills in various programming languages and technologies:</p>
                <div class="skills">
                    <span class="skill">Java</span>
                    <span class="skill">Python</span>
                    <span class="skill">HTML/CSS</span>
                    <span class="skill">JavaScript</span>
                    <span class="skill">SQL</span>
                    <span class="skill">Git</span>
                </div>
            </div>
            
            <div class="info-card">
                <h3><i class="fas fa-book"></i> Relevant Courses</h3>
                <ul class="courses">
                    <li>Data Structures and Algorithms</li>
                    <li>Web Development</li>
                    <li>Database Systems</li>
                    <li>Software Engineering</li>
                    <li>Computer Networks</li>
                </ul>
            </div>
        </div>
        
        <div class="social-icons">
            <a href="#" class="social-icon">
                <i class="fab fa-linkedin-in"></i>
            </a>
            <a href="#" class="social-icon">
                <i class="fab fa-github"></i>
            </a>
            <a href="#" class="social-icon">
                <i class="fab fa-twitter"></i>
            </a>
            <a href="#" class="social-icon">
                <i class="fas fa-envelope"></i>
            </a>
        </div>
        
        <footer class="footer">
            <div class="footer-links">
                <a href="#">Resume</a> | <a href="#">Projects</a> | <a href="#">Contact</a>
            </div>
            <div>
                &copy; 2023 Hillary Agbele. This is a class project.
            </div>
        </footer>
    </div>
</body>
</html>
