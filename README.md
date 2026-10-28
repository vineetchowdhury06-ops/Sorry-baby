# Sorry-baby
html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For V ❤️ From S</title>
    <style>
        :root {
            --bg-color: #ffeef2;
            --card-color: #ffffff;
            --primary-pink: #ff8fa3;
            --dark-pink: #ff4d6d;
            --text-color: #5c3d46;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden;
            position: relative;
        }

        /* Floating Hearts Background */
        .heart-bg {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            z-index: 1;
            pointer-events: none;
        }

        .floating-heart {
            position: absolute;
            color: var(--primary-pink);
            opacity: 0.6;
            animation: floatUp 6s linear infinite;
            font-size: 20px;
        }

        @keyframes floatUp {
            0% { transform: translateY(105vh) scale(0.5); opacity: 0; }
            10% { opacity: 0.6; }
            90% { opacity: 0.6; }
            100% { transform: translateY(-10vh) scale(1.2); opacity: 0; }
        }

        /* Website Container */
        .container {
            width: 90%;
            max-width: 500px;
            background: var(--card-color);
            padding: 30px;
            border-radius: 30px;
            box-shadow: 0 10px 30px rgba(255, 143, 163, 0.2);
            text-align: center;
            z-index: 10;
            position: relative;
            border: 4px dashed var(--primary-pink);
            min-height: 450px;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        /* Pages */
        .page {
            display: none;
            animation: fadeIn 0.5s ease-in-out forwards;
        }

        .page.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Decorations */
        .deco-icon {
            font-size: 50px;
            margin-bottom: 15px;
            display: inline-block;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        h2 {
            color: var(--dark-pink);
            margin-bottom: 15px;
            font-size: 24px;
        }

        p {
            line-height: 1.6;
            font-size: 16px;
            margin-bottom: 15px;
        }

        .letter-content {
            background: #fff5f7;
            padding: 20px;
            border-radius: 20px;
            border-left: 5px solid var(--primary-pink);
            text-align: left;
            font-style: italic;
            max-height: 250px;
            overflow-y: auto;
        }

        /* Navigation Buttons */
        .nav-buttons {
            display: flex;
            justify-content: space-between;
            margin-top: 25px;
            gap: 10px;
        }

        button {
            padding: 12px 25px;
            border: none;
            border-radius: 20px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.2s;
            flex: 1;
        }

        .btn-next {
            background-color: var(--primary-pink);
            color: white;
        }

        .btn-next:hover {
            background-color: var(--dark-pink);
        }

        .btn-back {
            background-color: #e0e0e0;
            color: #666;
        }

        .btn-back:hover {
            background-color: #d0d0d0;
        }

        /* Final Interaction Buttons */
        .choice-buttons {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 20px;
        }

        .btn-choice {
            padding: 15px;
            border-radius: 25px;
            background: white;
            border: 2px solid var(--primary-pink);
            color: var(--dark-pink);
        }

        .btn-choice:hover {
            background: var(--bg-color);
        }

        #success-message {
            display: none;
            color: var(--dark-pink);
            font-weight: bold;
            margin-top: 20px;
            animation: bounce 0.5s ease infinite alternate;
        }

        @keyframes bounce {
            from { transform: translateY(0); }
            to { transform: translateY(-5px); }
        }
    </style>
</head>
<body>

    <div class="heart-bg" id="heartBg"></div>

    <div class="container">
        <!-- PAGE 1: Welcome -->
        <div class="page active" id="page1">
            <span class="deco-icon">🧸</span>
            <h2>For Someone Very Special</h2>
            <p>Hi V, I made this space just for you because my heart has a lot it wants to say. I am so sorry for everything lately.</p>
            <p>Please take a small moment to flip through these pages... ❤️</p>
        </div>

        <!-- PAGE 2: The Apology Letter -->
        <div class="page" id="page2">
            <span class="deco-icon">🌷</span>
            <h2>My Sincerest Apology</h2>
            <div class="letter-content">
                <p>Dear V,</p>
                <p>I want to deeply apologize for letting my anger get the better of me. Seeing you hurt because of my actions breaks my heart completely.</p>
                <p>You deserve only patience, kindness, and gentleness, and I failed to give you that. I am truly sorry for my behavior, and I promise to work harder on managing my emotions so I never make you feel this way again.</p>
                <p>Love always, S</p>
            </div>
        </div>

        <!-- PAGE 3: Heartfelt Message -->
        <div class="page" id="page3">
            <span class="deco-icon">💌</span>
            <h2>I Miss Your Smile</h2>
            <p>Nothing feels right when things are heavy between us. Your happiness means the world to me, and knowing I disrupted your peace hurts deeply.</p>
            <p>I value you, our bond, and every single memory we share way too much to let my mistakes get in the way. I want to make things right.</p>
        </div>

        <!-- PAGE 4: Forgiveness -->
        <div class="page" id="page4">
            <span class="deco-icon">💖</span>
            <h2>When You Are Ready...</h2>
            <p>I don't expect everything to be perfect right away, and I want you to take all the time you need. But when you are ready, do you think you could forgive me?</p>
            
            <div class="choice-buttons">
                <button class="btn-choice" onclick="forgive()">Yes, I forgive you 💖</button>
                <button class="btn-choice" onclick="takeTime()">I still need a little time 💕</button>
            </div>
            <div id="success-message"></div>
        </div>

        <!-- Navigation System -->
        <div class="nav-buttons" id="navGroup">
            <button class="btn-back" id="backBtn" onclick="changePage(-1)" style="visibility: hidden;">Back 🧸</button>
            <button class="btn-next" id="nextBtn" onclick="changePage(1)">Next 🧸</button>
        </div>
    </div>

    <script>
        let currentPage = 1;
        const totalPages = 4;

        function changePage(direction) {
            // Hide current page
            document.getElementById(`page${currentPage}`).classList.remove('active');
            
            // Update page number
            currentPage += direction;
            
            // Show new page
            document.getElementById(`page${currentPage}`).classList.add('active');

            // Handle navigation visibility
            document.getElementById('backBtn').style.visibility = currentPage === 1 ? 'hidden' : 'visible';
            
            if (currentPage === totalPages) {
                document.getElementById('navGroup').style.display = 'none';
            } else {
                document.getElementById('navGroup').style.display = 'flex';
            }
        }

        function forgive() {
            const msg = document.getElementById('success-message');
            msg.innerHTML = "Thank you so much, V! 😭❤️ You just made my entire world bright again. I promise to cherish you!";
            msg.style.display = 'block';
        }

        function takeTime() {
            const msg = document.getElementById('success-message');
            msg.innerHTML = "I completely understand. Take all the time you need, V. I'll be right here waiting gently. 💕";
            msg.style.display = 'block';
        }

        // Generate Background Floating Hearts
        const heartBg = document.getElementById('heartBg');
        const heartSymbols = ['❤️', '💖', '💗', '💕', '🌷'];
        
        function createHeart() {
            const heart = document.createElement('div');
            heart.classList.add('floating-heart');
            heart.innerText = heartSymbols[Math.floor(Math.random() * heartSymbols.length)];
            heart.style.left = Math.random() * 100 + 'vw';
            heart.style.animationDuration = (Math.random() * 3 + 4) + 's'; 
            heartBg.appendChild(heart);

            setTimeout(() => {
                heart.remove();
            }, 7000);
        }

        setInterval(createHeart, 400);
    </script>
</body>
</html>