<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hillary Agbele | Coming Soon</title>
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
            max-width: 800px;
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
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            color: #8892b0;
        }
        
        .countdown {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }
        
        .countdown-item {
            background: rgba(100, 255, 218, 0.1);
            padding: 20px;
            border-radius: 10px;
            min-width: 100px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            border: 1px solid rgba(100, 255, 218, 0.2);
        }
        
        .countdown-number {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 5px;
            color: #64ffda;
        }
        
        .countdown-label {
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: #ccd6f6;
        }
        
        .signup-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 500px;
            margin: 0 auto 40px;
        }
        
        .form-input {
            padding: 15px 20px;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            background: rgba(136, 146, 176, 0.2);
            color: #e6f1ff;
            transition: all 0.3s ease;
        }
        
        .form-input::placeholder {
            color: #a8b2d1;
        }
        
        .form-input:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(100, 255, 218, 0.5);
            transform: scale(1.02);
            background: rgba(136, 146, 176, 0.3);
        }
        
        .submit-btn {
            padding: 15px 20px;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: bold;
            background: #64ffda;
            color: #0a192f;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .submit-btn:hover {
            background: #88ffdf;
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
        }
        
        .submit-btn:active {
            transform: translateY(0);
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
        
        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 15px 25px;
            background: #64ffda;
            color: #0a192f;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transform: translateX(150%);
            transition: transform 0.5s ease;
            z-index: 1000;
            font-weight: bold;
        }
        
        .notification.show {
            transform: translateX(0);
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
            
            .countdown {
                gap: 10px;
            }
            
            .countdown-item {
                min-width: 80px;
                padding: 15px;
            }
            
            .countdown-number {
                font-size: 2rem;
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
            
            .countdown-item {
                min-width: 70px;
                padding: 10px;
            }
            
            .countdown-number {
                font-size: 1.5rem;
            }
            
            .countdown-label {
                font-size: 0.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="logo">
            <i class="fas fa-code"></i>
        </div>
        
        <h1>Coming Soon<span class="name-highlight">Hillary Agbele</span></h1>
        
        <p class="tagline">Creating digital experiences that make an impact</p>
        
        <p class="description">I'm working on something amazing! Join my mailing list to be the first to know when I launch. Get updates on my latest projects and insights.</p>
        
        <div class="countdown">
            <div class="countdown-item">
                <div class="countdown-number" id="days">00</div>
                <div class="countdown-label">Days</div>
            </div>
            <div class="countdown-item">
                <div class="countdown-number" id="hours">00</div>
                <div class="countdown-label">Hours</div>
            </div>
            <div class="countdown-item">
                <div class="countdown-number" id="minutes">00</div>
                <div class="countdown-label">Minutes</div>
            </div>
            <div class="countdown-item">
                <div class="countdown-number" id="seconds">00</div>
                <div class="countdown-label">Seconds</div>
            </div>
        </div>
        
        <form class="signup-form" id="signup-form">
            <input type="email" class="form-input" id="email" placeholder="Your Email Address" required>
            <button type="submit" class="submit-btn">Notify Me on Launch</button>
        </form>
        
        <div class="social-icons">
            <a href="#" class="social-icon">
                <i class="fab fa-twitter"></i>
            </a>
            <a href="#" class="social-icon">
                <i class="fab fa-linkedin-in"></i>
            </a>
            <a href="#" class="social-icon">
                <i class="fab fa-github"></i>
            </a>
            <a href="#" class="social-icon">
                <i class="fas fa-envelope"></i>
            </a>
        </div>
        
        <footer class="footer">
            <div class="footer-links">
                <a href="#">Privacy Policy</a> | <a href="#">Terms of Service</a> | <a href="#">Contact</a>
            </div>
            <div>
                &copy; 2023 Hillary Agbele. All rights reserved.
            </div>
        </footer>
    </div>
    
    <div class="notification" id="notification">
        Thank you for subscribing! I'll notify you when I launch.
    </div>
    
    <script>
        // Set launch date (2 months from now)
        const launchDate = new Date();
        launchDate.setMonth(launchDate.getMonth() + 2);
        
        // Countdown timer
        function updateCountdown() {
            const now = new Date();
            const diff = launchDate - now;
            
            const days = Math.floor(diff / (1000 * 60 * 60 * 24));
            const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((diff % (1000 * 60)) / 1000);
            
            document.getElementById('days').textContent = days.toString().padStart(2, '0');
            document.getElementById('hours').textContent = hours.toString().padStart(2, '0');
            document.getElementById('minutes').textContent = minutes.toString().padStart(2, '0');
            document.getElementById('seconds').textContent = seconds.toString().padStart(2, '0');
        }
        
        // Initial call
        updateCountdown();
        
        // Update every second
        setInterval(updateCountdown, 1000);
        
        // Form submission
        document.getElementById('signup-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const email = document.getElementById('email').value;
            
            // Simple validation
            if (!validateEmail(email)) {
                alert('Please enter a valid email address.');
                return;
            }
            
            // Show notification
            const notification = document.getElementById('notification');
            notification.classList.add('show');
            
            // Hide notification after 3 seconds
            setTimeout(() => {
                notification.classList.remove('show');
            }, 3000);
            
            // Reset form
            this.reset();
            
            // In a real application, you would send the email to your server here
            console.log('Email submitted:', email);
        });
        
        // Email validation
        function validateEmail(email) {
            const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            return re.test(email);
        }
    </script>
</body>
</html>
