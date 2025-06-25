<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yeasin Miazi - GitHub Banner</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Fira Code', monospace;
            background-color: #0a0a0a;
            overflow: hidden;
        }
        
        .banner {
            width: 100%;
            height: 300px;
            background-color: #111111;
            position: relative;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
            display: flex;
        }
        
        .content-wrapper {
            width: 60%;
            padding: 30px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            position: relative;
            z-index: 3;
        }
        
        .image-wrapper {
            width: 40%;
            height: 100%;
            position: relative;
            z-index: 2;
            display: flex;
            align-items: center;
            justify-content: center;
            overflow: hidden;
        }
        
        .profile-image {
            width: 100%;
            height: 80%;
            object-fit: cover;
            object-position: center;
            transition: all 0.5s ease;
            position: absolute;
            bottom: 0;
        }
        
        .profile-image:hover {
            transform: scale(1.03);
        }
        
        .image-placeholder {
            width: 80%;
            height: 80%;
            background: linear-gradient(135deg, #0f2027, #203a43, #2c5364);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: rgba(255,255,255,0.3);
            font-size: 0.9rem;
            text-align: center;
            border: 2px dashed rgba(0, 255, 200, 0.3);
        }
        
        .code-background {
            position: absolute;
            width: 100%;
            height: 100%;
            opacity: 0.08;
            background-image: 
                repeating-linear-gradient(0deg, 
                    rgba(0, 255, 150, 0.1) 0px, 
                    transparent 2px, 
                    transparent 15px),
                repeating-linear-gradient(90deg, 
                    rgba(0, 200, 255, 0.1) 0px, 
                    transparent 2px, 
                    transparent 15px);
        }
        
        .name {
            position: relative;
            z-index: 2;
            color: #ffffff;
            font-size: 2.5rem;
            font-weight: 700;
            text-shadow: 0 0 10px rgba(0, 255, 200, 0.3);
        }
        
        .title {
            position: relative;
            z-index: 2;
            color: #84ffff;
            font-size: 1.5rem;
            margin-top: 1rem;
        }
        
        .contact {
            position: relative;
            z-index: 2;
            margin-top: 1.5rem;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            color: #b0bec5;
            margin-bottom: 0.7rem;
            transition: all 0.3s ease;
        }
        
        .contact-item:hover {
            color: #ffffff;
            text-shadow: 0 0 8px rgba(100, 255, 218, 0.5);
        }
        
        .contact-icon {
            margin-right: 10px;
            font-size: 1.2rem;
        }
        
        .code-element {
            position: absolute;
            color: rgba(0, 255, 200, 0.7);
            font-size: 0.8rem;
            opacity: 0.4;
            animation: float 8s infinite ease-in-out;
            z-index: 2;
        }
        
        @keyframes float {
            0%, 100% {
                transform: translateY(0) translateX(0);
            }
            50% {
                transform: translateY(-20px) translateX(10px);
            }
        }
        
        @keyframes pulse {
            0%, 100% {
                opacity: 0.2;
            }
            50% {
                opacity: 0.5;
            }
        }
        
        .decoration {
            position: absolute;
            width: 300px;
            height: 300px;
            background: radial-gradient(circle, rgba(0, 212, 255, 0.2) 0%, rgba(9, 9, 121, 0) 70%);
            border-radius: 50%;
            filter: blur(20px);
            animation: pulse 5s infinite ease-in-out;
            z-index: 1;
        }
        
        .decoration:nth-child(2) {
            right: -100px;
            top: -100px;
            background: radial-gradient(circle, rgba(255, 0, 212, 0.2) 0%, rgba(9, 9, 121, 0) 70%);
        }
        
        .decoration:nth-child(3) {
            right: 150px;
            bottom: -150px;
            width: 200px;
            height: 200px;
            background: radial-gradient(circle, rgba(255, 230, 0, 0.2) 0%, rgba(9, 9, 121, 0) 70%);
        }
        
        .binary-rain {
            position: absolute;
            opacity: 0.2;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 100px;
            overflow: hidden;
            z-index: 1;
        }
        
        .binary-column {
            display: inline-block;
            margin-right: 40px;
            animation: binaryFall linear infinite;
            animation-duration: calc(5s + (var(--speed) * 5s));
        }
        
        @keyframes binaryFall {
            0% {
                transform: translateY(-100%);
            }
            100% {
                transform: translateY(100vh);
            }
        }
    </style>
</head>
<body>
    <div class="banner">
        <div class="code-background"></div>
        <div class="decoration"></div>
        <div class="decoration"></div>
        <div class="decoration"></div>
        
        <div class="content-wrapper">
            <h1 class="name">Yeasin Miazi</h1>
            <h2 class="title">Front End Developer</h2>
            
            <div class="contact">
                <div class="contact-item">
                    <i class="fas fa-phone-alt contact-icon"></i>
                    <span>01608072719</span>
                </div>
                <div class="contact-item">
                    <i class="fas fa-envelope contact-icon"></i>
                    <span>yeasinmiazi1997@gmail.com</span>
                </div>
            </div>
        </div>
        
        <div class="image-wrapper">
            <!-- Replace the src with your actual image URL -->
            <img src="https://i.ibb.co/pvrMxN2Z/yeasin.png" alt="Profile Image" class="profile-image" id="profileImage" onerror="showPlaceholder()">
            <div class="image-placeholder" id="imagePlaceholder" style="display: none;">
                <div>
                    <i class="fas fa-user-astronaut" style="font-size: 2rem; margin-bottom: 10px;"></i><br>
                    Your Image Here<br>
                    (Replace with your profile image URL)
                </div>
            </div>
        </div>
        
        <div class="binary-rain" id="binaryRain"></div>
        
        <!-- Animated code elements -->
        <div class="code-element" style="top: 20%; left: 45%;">function createBanner() {</div>
        <div class="code-element" style="top: 30%; left: 35%;">return developerProfile;</div>
        <div class="code-element" style="top: 45%; left: 40%;">}</div>
        <div class="code-element" style="top: 55%; left: 30%;">const banner = createBanner();</div>
    </div>

    <script>
        // Create binary rain effect
        const binaryRain = document.getElementById('binaryRain');
        const binaryChars = ['0', '1', '0', '1', '0', '1', '0', '1', '0', '1', '0', '1', '0', '1'];
        
        // Create multiple columns of binary rain
        for (let i = 0; i < 20; i++) {
            const column = document.createElement('div');
            column.classList.add('binary-column');
            
            // Random speed for each column
            const speed = Math.random();
            column.style.setProperty('--speed', speed);
            column.style.left = `${i * 50}px`;
            
            // Create random binary characters
            for (let j = 0; j < 15; j++) {
                const char = document.createElement('div');
                char.textContent = binaryChars[Math.floor(Math.random() * binaryChars.length)];
                char.style.opacity = Math.random() * 0.5 + 0.1;
                char.style.marginBottom = '20px';
                char.style.color = `rgb(0, ${Math.floor(Math.random() * 255)}, ${Math.floor(Math.random() * 100 + 155)})`;
                column.appendChild(char);
            }
            
            binaryRain.appendChild(column);
        }

        // Show placeholder if image fails to load
        function showPlaceholder() {
            document.getElementById('profileImage').style.display = 'none';
            document.getElementById('imagePlaceholder').style.display = 'flex';
        }

        // Add some interactive elements
        document.querySelectorAll('.contact-item').forEach(item => {
            item.addEventListener('mouseover', function() {
                const icon = this.querySelector('.contact-icon');
                icon.style.transform = 'translateX(-5px)';
                icon.style.transition = 'all 0.3s ease';
            });
            
            item.addEventListener('mouseout', function() {
                const icon = this.querySelector('.contact-icon');
                icon.style.transform = 'translateX(0)';
            });
        });
    </script>
</body>
</html>
## Hi there 👋

<!--
**miazi2003/miazi2003** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
