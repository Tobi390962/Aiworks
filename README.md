<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Learning Platform</title>
    <link rel="stylesheet" href="styles.css">
    <script src="script.js" defer></script>
    <style>
        @keyframes slideDown {
            from { opacity: 0; transform: translateY(-50px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: scale(0.8); }
            to { opacity: 1; transform: scale(1); }
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        @keyframes glow {
            0% { box-shadow: 0 0 10px rgba(0, 198, 255, 0.5); }
            50% { box-shadow: 0 0 20px rgba(0, 198, 255, 1); }
            100% { box-shadow: 0 0 10px rgba(0, 198, 255, 0.5); }
        }

        @keyframes staggeredFadeIn {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(120deg, #1c1c1c, #003366);
            color: white;
            text-align: center;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
        }
        header {
            padding: 20px;
            background: rgba(0, 0, 0, 0.8);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.5);
            font-size: 1.5rem;
            animation: slideDown 1s ease-in-out;
        }
        .hero {
            padding: 80px 20px;
            animation: fadeIn 1.5s ease-in-out;
        }
        button {
            padding: 12px 24px;
            font-size: 18px;
            background: linear-gradient(to right, #00c6ff, #0072ff);
            border: none;
            color: white;
            cursor: pointer;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s;
            border-radius: 25px;
            animation: glow 2s infinite alternate;
        }
        button:hover {
            transform: scale(1.1);
            box-shadow: 0 0 15px rgba(0, 198, 255, 0.6);
        }
        .features {
            display: flex;
            justify-content: center;
            padding: 50px;
            flex-wrap: wrap;
            gap: 20px;
        }
        .feature {
            background: rgba(255, 255, 255, 0.1);
            padding: 30px;
            border-radius: 15px;
            transition: transform 0.3s, box-shadow 0.3s;
            cursor: pointer;
            width: 280px;
            text-align: center;
            margin: 10px;
            animation: staggeredFadeIn 1s ease-in-out both;
        }
        .feature:hover {
            transform: scale(1.1);
            box-shadow: 0px 0px 20px rgba(255, 255, 255, 0.3);
        }
        .about-us {
            text-align: center;
            padding: 50px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            margin: 20px;
            cursor: pointer;
            transition: transform 0.3s ease-in-out, box-shadow 0.3s;
        }
        .about-us:hover {
            transform: scale(1.05);
            box-shadow: 0 0 15px rgba(255, 255, 255, 0.3);
        }
        .team-members {
            display: none;
            margin-top: 20px;
        }
        .team-members a {
            display: block;
            color: #00c6ff;
            text-decoration: none;
            font-size: 1.2rem;
            margin: 10px 0;
        }
        .team-members a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <header>
        <h1>🚀 AI Powered Personalized Learning 🚀</h1>
    </header>
    
    <section class="hero">
        <h2>🌟 Learn Smarter with AI 🌟</h2>
        <p>Get a personalized learning experience powered by artificial intelligence.</p>
        <button onclick="window.open('https://www.unesco.org/en/education', '_blank')">Get Started</button>
    </section>
    
    <section class="features">
        <div class="feature" onclick="window.open('https://www.khanacademy.org/', '_blank')">
            <h3>🤖 Adaptive Learning</h3>
            <p>AI tailors the lessons based on your progress.</p>
        </div>
    </section>
    
    <section class="about-us" onclick="toggleTeam()">
        <h2>📢 About Us</h2>
        <p>Meet the team behind this platform!</p>
        <div class="team-members" id="team">
            <a href="resume1.pdf" target="_blank">👤 noel</a>
            <a href="resume2.pdf" target="_blank">👤 nino 2</a>
            <a href="resume3.pdf" target="_blank">👤 Member 3</a>
        </div>
    </section>
    
    <footer>
        <p>&copy; 2025 AI Learning Platform | Designed with ❤️ for the Future</p>
    </footer>
    
    <script>
        function toggleTeam() {
            var team = document.getElementById('team');
            team.style.display = team.style.display === 'block' ? 'none' : 'block';
        }
    </script>
</body>
</html>

