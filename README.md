<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abhishek's Terminal</title>
    <style>
        body {
            margin: 0;
            font-family: monospace;
            background-color: #111827;
            color: #4ade80;
            min-height: 100vh;
            padding: 2rem;
        }
        .container {
            max-width: 64rem;
            margin: 0 auto;
        }
        .terminal-header {
            background-color: #1f2937;
            border-radius: 0.5rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            padding: 1rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
        }
        .terminal-title {
            font-size: 1.25rem;
            font-weight: bold;
            margin-left: 0.5rem;
        }
        .terminal-body {
            background-color: #1f2937;
            border-radius: 0.5rem;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            padding: 1rem;
            height: 600px;
            overflow: auto;
        }
        .terminal-input {
            display: flex;
            align-items: center;
            margin-top: 1rem;
        }
        .terminal-input input {
            background-color: transparent;
            border: none;
            outline: none;
            color: #4ade80;
            width: 100%;
            font-family: monospace;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="terminal-header">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
                <polyline points="4 17 10 11 4 5"></polyline>
                <line x1="12" y1="19" x2="20" y2="19"></line>
            </svg>
            <span class="terminal-title">Abhishek's Terminal</span>
        </div>
        <div class="terminal-body">
            <pre id="terminal-text"></pre>
            <div class="terminal-input">
                <span>$</span>
                <input type="text" placeholder="Type 'help' for more information...">
            </div>
        </div>
    </div>

    <script>
        const fullText = `
> Abhishek Tiwari
> Learning skills with consistency

> Skills:
  Git, GitHub, Bootstrap, C, C++, CSS, HTML, Java, JavaScript, Linux, MongoDB, MySQL, Node.js, React, VS Code

> Currently learning:
  - DSA in C++
  - Full Stack Development

> Contact:
  - GitHub: https://github.com/abhishek3432
  - LinkedIn: https://www.linkedin.com/in/abhishek3432/
  - Email: akt343243@gmail.com

> Portfolio: https://abhishek3432.github.io/MyPortfolio/

> Type 'help' for more information.
`;

        let i = 0;
        const terminalText = document.getElementById('terminal-text');
        const timer = setInterval(() => {
            terminalText.textContent = fullText.slice(0, i);
            i++;
            if (i > fullText.length) clearInterval(timer);
        }, 20);
    </script>
</body>
</html>
