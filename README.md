<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Launching Soon | Modern Coming Soon Page</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #1a2a6c, #b21f1f, #fdbb2d);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
            color: white;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            overflow-x: hidden;
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
            padding: 40px 20px;
            background: rgba(0, 0, 0, 0.6);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.5);
            animation: fadeIn 1s ease-out;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .logo {
            font-size: 3.5rem;
            margin-bottom: 20px;
            color: #fdbb2d;
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
        }
        
        .tagline {
            font-size: 1.5rem;
            margin-bottom: 30px;
            color: #f8f8f8;
        }
        
        .description {
            font-size: 1.2rem;
            line-height: 1.6;
            margin-bottom: 40px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .countdown {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }
        
        .countdown-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            min-width: 100px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .countdown-number {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 5px;
        }
        
        .countdown-label {
            font-size: 1rem;
            text-transform: uppercase;
            letter-spacing: 1px;
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
            background: rgba(255, 255, 255, 0.9);
            transition: all 0.3s ease;
        }
        
        .form-input:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(253, 187, 45, 0.8);
            transform: scale(1.02);
        }
        
        .submit-btn {
            padding: 15px 20px;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: bold;
            background: #fdbb2d;
            color: #1a2a6c;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .submit-btn:hover {
            background: #ffcc44;
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
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 1.5rem;
            transition: all 0.3s ease;
            text-decoration: none;
        }
        
        .social-icon:hover {
            background: #fdbb2d;
            color: #1a2a6c;
            transform: translateY(-5px);
        }
        
        .footer {
            margin-top: 30px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .footer-links {
            margin-bottom: 10px;
        }
        
        .footer a {
            color: #fdbb2d;
            text-decoration: none;
            transition: color 0.3s ease;
        }
        
        .footer a:hover {
            color: #ffcc44;
            text-decoration: underline;
        }
        
        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 15px 25px;
            background: #4CAF50;
            color: white;
            border-radius: 5px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transform: translateX(150%);
            transition: transform 0.5s ease;
            z-index: 1000;
        }
        
        .notification.show {
            transform: translateX(0);
        }
        
        /* Responsive design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
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
            <i class="fas fa-rocket"></i>
        </div>
        
        <h1>Something Amazing Is Coming</h1>
        
        <p class="tagline">We're working hard to bring you an incredible experience.</p>
        
        <p class="description">Join our mailing list to be the first to know when we launch. We promise to only send you important updates and never spam your inbox.</p>
        
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
                <i class="fab fa-instagram"></i>
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
                <a href="#">Privacy Policy</a> | <a href="#">Terms of Service</a> | <a href="#">Contact Us</a>
            </div>
            <div>
                &copy; 2023 Your Company. Credits: <a href="http://html5up.net">HTML5 UP</a>
            </div>
        </footer>
    </div>
    
    <div class="notification" id="notification">
        Thank you for subscribing! We'll notify you when we launch.
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
