<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abhishek Tiwari - Dark Theme with Neon Accents</title>
    <style>
        body {
            font-family: 'Courier New', monospace;
            line-height: 1.6;
            color: #00ff00;
            background-color: #000000;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2 {
            color: #ff00ff;
            text-shadow: 0 0 5px #ff00ff;
        }
        .center {
            text-align: center;
        }
        .gif-container {
            display: flex;
            justify-content: center;
            margin: 20px 0;
        }
        .section {
            border: 1px solid #00ff00;
            border-radius: 5px;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 0 10px #00ff00;
        }
        .skills {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
        }
        .skill-icon {
            width: 40px;
            height: 40px;
            filter: drop-shadow(0 0 2px #00ffff);
        }
        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
        }
        .stats img {
            margin: 10px;
            max-width: 100%;
            border: 1px solid #00ffff;
            border-radius: 5px;
        }
        .connect {
            display: flex;
            justify-content: center;
            gap: 10px;
        }
        .connect img {
            transition: transform 0.3s ease;
        }
        .connect img:hover {
            transform: scale(1.1);
        }
        a {
            color: #00ffff;
            text-decoration: none;
        }
        a:hover {
            text-shadow: 0 0 5px #00ffff;
        }
    </style>
</head>
<body>
    <h1 class="center">👋 Hello World! I'm Abhishek Tiwari</h1>
    <p class="center"><em>Learning skills with consistency and exploring the world of tech!</em></p>
    <div class="gif-container">
        <img src="https://media1.giphy.com/media/TPl5N4Ci49ZQY/giphy.gif?cid=ecf05e47za80g6ltso1o7f71jkoak398c5qnbpb3ckqos3vf&ep=v1_gifs_search&rid=giphy.gif&ct=g" width="400" alt="Coding GIF">
    </div>
    <div class="section">
        <h2>🌱 About Me</h2>
        <ul>
            <li>💡 Currently learning <strong>Data Structures and Algorithms</strong> in C++ and <strong>Full Stack Development</strong>.</li>
            <li>💬 Ask me about <strong>Data Structures</strong>, <strong>Web Development</strong>, or <strong>React</strong>.</li>
            <li>📫 Reach me at: <a href="mailto:akt343243@gmail.com">akt343243@gmail.com</a></li>
            <li>🎨 Check out my work: <a href="https://abhishek3432.github.io/MyPortfolio/" target="_blank">Portfolio</a></li>
            <li>📄 <a href="https://www.linkedin.com/in/abhishek3432/" target="_blank">LinkedIn Profile</a></li>
        </ul>
    </div>
    <div class="section">
        <h2>📚 Education</h2>
        <ul>
            <li><strong>B.Tech in Computer Science Engineering</strong><br>
                KCC Institute of Technology and Management, Greater Noida, UP, India (2025)</li>
            <li><strong>12th Grade</strong><br>
                Shree Tyagi Modern Public School, Hodal, Haryana, India</li>
        </ul>
    </div>
    <div class="section">
        <h2>🔧 Languages & Tools</h2>
        <div class="skills">
            <img src="https://skillicons.dev/icons?i=git,github,bootstrap,c,cpp,codepen,css,discord,express,html,java,js,linux,mongodb,mysql,nodejs,react,vscode" alt="Skills">
        </div>
    </div>
    <div class="section">
        <h2>📈 GitHub Stats</h2>
        <div class="stats">
            <img src="https://github-readme-stats.vercel.app/api?username=abhishek3432&show_icons=true&theme=radical" alt="GitHub Stats" width="45%">
            <img src="https://github-readme-streak-stats.herokuapp.com/?user=abhishek3432&theme=radical" alt="GitHub Streak" width="45%">
            <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=abhishek3432&layout=compact&theme=radical" alt="Top Languages" width="45%">
        </div>
    </div>
    <div class="section">
        <h2>🌐 Connect with Me</h2>
        <div class="connect">
            <a href="https://github.com/abhishek3432" target="_blank">
                <img src="https://img.shields.io/badge/GitHub-171515?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
            </a>
            <a href="https://www.linkedin.com/in/abhishek3432/" target="_blank">
                <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
            </a>
        </div>
    </div>
    <div class="section center">
        <h2>📊 GitHub Profile Views</h2>
        <img src="https://profile-counter.glitch.me/abhishek3432/count.svg" alt="Profile Views">
    </div>
    <div class="center">
        <img src="https://github.com/dibyendu415/dibyendu415/blob/master/marquee.svg" width="100%" alt="Thank you for visiting!">
    </div>
    <script>
        document.addEventListener('DOMContentLoaded', (event) => {
            const sections = document.querySelectorAll('.section');
            sections.forEach((section, index) => {
                section.style.opacity = '0';
                section.style.transform = 'translateX(-20px)';
                section.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                setTimeout(() => {
                    section.style.opacity = '1';
                    section.style.transform = 'translateX(0)';
                }, 200 * index);
            });
        });
    </script>
</body>
</html>
