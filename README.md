<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Omkar's Website</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* General Styling */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: #f4f4f4;
            color: #333;
            transition: background 0.4s, color 0.4s;
        }

        /* Dark Mode */
        body.dark-mode {
            background: #1a1a1a;
            color: #fff;
        }

        /* Header */
        header {
            background: #007bff;
            color: white;
            text-align: center;
            padding: 15px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            width: 100%;
        }

        header h1 {
            font-size: 24px;
        }

        /* Dark Mode Button */
        #dark-mode-toggle {
            background: white;
            border: none;
            padding: 8px 12px;
            font-size: 14px;
            cursor: pointer;
            border-radius: 5px;
            transition: 0.3s;
        }

        #dark-mode-toggle:hover {
            background: #ddd;
        }

        /* Navigation */
        nav {
            background: #0056b3;
            padding: 12px;
            width: 100%;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        nav ul li {
            margin: 5px 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 16px;
            padding: 8px 12px;
            border-radius: 5px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            background: yellow;
            color: black;
        }

        /* Sections */
        section {
            padding: 50px;
            text-align: center;
            transition: 0.3s;
        }

        section:hover {
            transform: scale(1.02);
        }

        /* Fixing Dark Mode for News and Q&A */
        .news-container, .qna-container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            width: 90%;
            max-width: 600px;
            margin: auto;
            text-align: left;
        }

        body.dark-mode .news-container, body.dark-mode .qna-container {
            background: #333;
            color: white;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 15px;
            margin-top: 20px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Omkar's Website</h1>
        <button id="dark-mode-toggle">🌙 Dark Mode</button>
    </header>

    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#coding">Coding</a></li>
            <li><a href="#microcontroller">Microcontrollers</a></li>
            <li><a href="#news">News</a></li>
            <li><a href="#qna">QnA</a></li>
            <li><a href="mailto:omkarbhutkar2010@gmail.com">📧 Contact Omkar</a></li>
        </ul>
    </nav>

    <section id="home">
        <h2>Welcome to Omkar's Website</h2>
        <p>Start your journey with easy-to-understand tutorials.</p>
    </section>

    <section id="coding">
        <h2>Coding</h2>
        <p>Learn different programming languages and create real-world projects.</p>
    </section>

    <section id="microcontroller">
        <h2>Microcontrollers</h2>
        <p>Build amazing projects with Arduino, ESP8266, and more.</p>
    </section>

    <!-- Funny Tech News Section -->
    <section id="news">
        <h2>Latest Funny Tech News 😂</h2>
        <div class="news-container">
            <p><strong>🤖 AI Gone Wild:</strong> A new AI chatbot refused to answer questions until it got coffee! ☕ Scientists are now working on an "AI Wake-Up Mode."</p>
            <p><strong>📱 iPhone 16 Leaks:</strong> Apple is removing **all buttons, charging ports, and even the screen!** They say it's "Minimalism 3000." How will it work? Nobody knows! 😂</p>
            <p><strong>🕹️ Gamer’s Nightmare:</strong> A man accidentally deleted **his 500-hour save file** while trying to "speed up loading time." His Wi-Fi router is now missing. 😭</p>
            <p><strong>💰 Elon Musk's New Invention:</strong> A device that **charges people for talking too much.** Twitter users are panicking. 🤣</p>
        </div>
    </section>

    <!-- Fun QnA Section -->
    <section id="qna">
        <h2>Fun Coding QnA 🧠</h2>
        <div class="qna-container">
            <p><strong>Q1:</strong> Why do programmers hate nature?</p>
            <p><strong>A:</strong> Because it has too many bugs! 🐛😂</p>

            <p><strong>Q2:</strong> Why did the programmer quit his job?</p>
            <p><strong>A:</strong> Because he didn't get arrays! 😆</p>

            <p><strong>Q3:</strong> Why was the JavaScript developer sad?</p>
            <p><strong>A:</strong> Because he didn’t ‘null’ his feelings! 😢</p>

            <p><strong>Q4:</strong> How do you comfort a JavaScript bug?</p>
            <p><strong>A:</strong> You ‘console’ it. 😂</p>
        </div>
    </section>

    <footer>
        <p>© 2025 Omkar's Website | Designed by Omkar</p>
    </footer>

    <script>
        // Dark Mode Toggle
        const darkModeToggle = document.getElementById('dark-mode-toggle');
        const body = document.body;

        darkModeToggle.addEventListener('click', () => {
            body.classList.toggle('dark-mode');
            darkModeToggle.textContent = body.classList.contains('dark-mode') ? '☀️ Light Mode' : '🌙 Dark Mode';
        });
    </script>

</body>
</html>