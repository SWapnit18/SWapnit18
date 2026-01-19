<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swapnit Patel - GitHub Profile Preview</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', Helvetica, Arial, sans-serif;
            background: #0d1117;
            color: #c9d1d9;
            padding: 20px;
        }

        .github-container {
            max-width: 1200px;
            margin: 0 auto;
            background: #0d1117;
            padding: 30px;
        }

        .header {
            text-align: center;
            margin-bottom: 30px;
        }

        .typing-text {
            font-size: 28px;
            font-weight: 600;
            background: linear-gradient(90deg, #00d9ff, #7b68ee, #00d9ff);
            background-size: 200% auto;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 20px;
            animation: gradient 3s linear infinite;
        }

        @keyframes gradient {
            0% { background-position: 0% center; }
            100% { background-position: 200% center; }
        }

        .divider {
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, transparent, #00d9ff, #7b68ee, #00d9ff, transparent);
            margin: 30px 0;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 0.5; }
            50% { opacity: 1; }
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .badge {
            background: #21262d;
            color: #58a6ff;
            padding: 5px 10px;
            border-radius: 6px;
            font-size: 12px;
            font-weight: 600;
            border: 1px solid #30363d;
        }

        h1 {
            font-size: 2em;
            margin: 20px 0;
            color: #c9d1d9;
        }

        h2 {
            font-size: 1.5em;
            margin: 30px 0 15px 0;
            padding-bottom: 8px;
            border-bottom: 1px solid #21262d;
            color: #c9d1d9;
        }

        .about-code {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            margin: 20px 0;
            font-family: 'Courier New', monospace;
            font-size: 14px;
            overflow-x: auto;
        }

        .code-line {
            margin: 5px 0;
        }

        .key {
            color: #ff7b72;
        }

        .value {
            color: #a5d6ff;
        }

        .string {
            color: #7ee787;
        }

        .tech-section {
            margin: 30px 0;
        }

        .tech-category {
            margin: 20px 0;
        }

        .tech-category h3 {
            font-size: 1.2em;
            margin-bottom: 12px;
            color: #58a6ff;
        }

        .tech-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin: 10px 0;
        }

        .tech-badge {
            display: inline-flex;
            align-items: center;
            padding: 6px 12px;
            border-radius: 6px;
            font-size: 13px;
            font-weight: 600;
            transition: transform 0.2s;
        }

        .tech-badge:hover {
            transform: scale(1.05);
        }

        .java { background: #ED8B00; color: white; }
        .javascript { background: #F7DF1E; color: #323330; }
        .python { background: #3670A0; color: white; }
        .html { background: #E34F26; color: white; }
        .css { background: #1572B6; color: white; }
        .react { background: #20232a; color: #61DAFB; }
        .node { background: #6DA55F; color: white; }
        .mongodb { background: #4ea94b; color: white; }
        .mysql { background: #00000f; color: white; border: 1px solid #4479A1; }
        .git { background: #F05033; color: white; }

        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .stat-card {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            text-align: center;
        }

        .stat-card img {
            max-width: 100%;
            height: auto;
            border-radius: 6px;
        }

        .contribution-graph {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 20px;
            margin: 20px 0;
            text-align: center;
        }

        .trophy-section {
            text-align: center;
            margin: 30px 0;
        }

        .trophy-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin: 20px 0;
        }

        .trophy {
            font-size: 48px;
            animation: bounce 2s infinite;
        }

        .focus-table {
            width: 100%;
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            margin: 20px 0;
            overflow: hidden;
        }

        .focus-table table {
            width: 100%;
            border-collapse: collapse;
        }

        .focus-table th {
            background: #21262d;
            padding: 15px;
            border-bottom: 2px solid #30363d;
            color: #58a6ff;
            font-size: 1.1em;
        }

        .focus-table td {
            padding: 15px;
            border-bottom: 1px solid #30363d;
            vertical-align: top;
        }

        .focus-table tr:last-child td {
            border-bottom: none;
        }

        .hobbies-section {
            margin: 30px 0;
        }

        .hobby-card {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 25px;
            margin: 20px 0;
            text-align: center;
        }

        .hobby-card h3 {
            color: #58a6ff;
            margin-bottom: 10px;
            font-size: 1.4em;
        }

        .hobby-card p {
            color: #8b949e;
            font-style: italic;
            margin: 10px 0;
        }

        .hobby-emoji {
            font-size: 80px;
            margin: 20px 0;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin: 30px 0;
        }

        .social-badge {
            display: inline-flex;
            align-items: center;
            padding: 8px 16px;
            border-radius: 6px;
            text-decoration: none;
            font-weight: 600;
            transition: transform 0.2s;
            gap: 5px;
        }

        .social-badge:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }

        .linkedin { background: #0077B5; color: white; }
        .instagram { background: linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%); color: white; }
        .github { background: #121011; color: white; }
        .twitter { background: #1DA1F2; color: white; }
        .portfolio { background: #FF7139; color: white; }
        .email { background: #D14836; color: white; }
        .chess { background: #769656; color: white; }

        .quote-section {
            text-align: center;
            margin: 40px 0;
            padding: 30px;
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
        }

        .quote {
            font-size: 16px;
            font-style: italic;
            color: #8b949e;
            margin: 15px 0;
        }

        .snake-container {
            text-align: center;
            margin: 30px 0;
            padding: 20px;
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
        }

        .snake-animation {
            font-size: 100px;
            animation: wiggle 2s infinite;
        }

        @keyframes wiggle {
            0%, 100% { transform: rotate(-3deg); }
            50% { transform: rotate(3deg); }
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .tagline {
            font-size: 1.4em;
            font-weight: 600;
            color: #58a6ff;
            text-align: center;
            margin: 30px 0;
        }

        @media (max-width: 768px) {
            .typing-text {
                font-size: 18px;
            }
            
            .stats-container {
                grid-template-columns: 1fr;
            }

            .focus-table {
                font-size: 14px;
            }
        }
    </style>
</head>
<body>
    <div class="github-container">
        <div class="header">
            <h1>Hi there, I'm Swapnit Patel 👋</h1>
            <div class="typing-text">B.Tech Computer Science Student | Web Developer | Full Stack Enthusiast | Chess Player ♟️ | Cricket Enthusiast 🏏 | Always Learning New Things!</div>
            <div class="badges">
                <span class="badge">👁️ Profile views: 1,234</span>
                <span class="badge">👥 Followers: 567</span>
            </div>
        </div>

        <div class="divider"></div>

        <h2>🚀 About Me</h2>
        <div class="about-code">
            <div class="code-line"><span class="key">const</span> swapnit = {</div>
            <div class="code-line">    <span class="key">pronouns:</span> <span class="string">"He"</span> | <span class="string">"Him"</span>,</div>
            <div class="code-line">    <span class="key">education:</span> <span class="string">"B.Tech in Computer Science Engineering"</span>,</div>
            <div class="code-line">    <span class="key">currentFocus:</span> <span class="string">"Web Development & Problem Solving"</span>,</div>
            <div class="code-line">    <span class="key">interests:</span> [<span class="string">"Full Stack Development"</span>, <span class="string">"Open Source"</span>, <span class="string">"DSA"</span>],</div>
            <div class="code-line">    <span class="key">hobbies:</span> [<span class="string">"Chess ♟️"</span>, <span class="string">"Cricket 🏏"</span>, <span class="string">"Coding 💻"</span>],</div>
            <div class="code-line">    <span class="key">askMeAbout:</span> [<span class="string">"Web Dev"</span>, <span class="string">"Tech"</span>, <span class="string">"Java"</span>, <span class="string">"JavaScript"</span>, <span class="string">"Chess Strategies"</span>],</div>
            <div class="code-line">    <span class="key">funFact:</span> <span class="string">"I debug with console.log() and I'm not ashamed! 😄"</span>,</div>
            <div class="code-line">    <span class="key">chessSkill:</span> <span class="string">"Strategic thinker on and off the board ♟️"</span>,</div>
            <div class="code-line">    <span class="key">cricketLove:</span> <span class="string">"Code in the day, cricket in the evening! 🏏"</span></div>
            <div class="code-line">};</div>
        </div>

        <div class="divider"></div>

        <h2>💻 Tech Stack</h2>
        <div class="tech-section">
            <div class="tech-category">
                <h3>Languages</h3>
                <div class="tech-badges">
                    <span class="tech-badge java">☕ Java</span>
                    <span class="tech-badge javascript">⚡ JavaScript</span>
                    <span class="tech-badge python">🐍 Python</span>
                    <span class="tech-badge html">🌐 HTML5</span>
                    <span class="tech-badge css">🎨 CSS3</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>Frontend Development</h3>
                <div class="tech-badges">
                    <span class="tech-badge react">⚛️ React</span>
                    <span class="tech-badge" style="background: #8511FA; color: white;">🅱️ Bootstrap</span>
                    <span class="tech-badge" style="background: #38B2AC; color: white;">💨 TailwindCSS</span>
                    <span class="tech-badge" style="background: #0769AD; color: white;">📜 jQuery</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>Backend Development</h3>
                <div class="tech-badges">
                    <span class="tech-badge node">🟢 Node.js</span>
                    <span class="tech-badge" style="background: #404d59; color: #61DAFB;">⚡ Express.js</span>
                    <span class="tech-badge" style="background: #6DB33F; color: white;">🍃 Spring Boot</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>Database</h3>
                <div class="tech-badges">
                    <span class="tech-badge mongodb">🍃 MongoDB</span>
                    <span class="tech-badge mysql">🐬 MySQL</span>
                    <span class="tech-badge" style="background: #316192; color: white;">🐘 PostgreSQL</span>
                </div>
            </div>

            <div class="tech-category">
                <h3>Tools & Technologies</h3>
                <div class="tech-badges">
                    <span class="tech-badge git">📚 Git</span>
                    <span class="tech-badge github">🐙 GitHub</span>
                    <span class="tech-badge" style="background: #0078d7; color: white;">💻 VS Code</span>
                    <span class="tech-badge" style="background: #FF6C37; color: white;">📮 Postman</span>
                    <span class="tech-badge" style="background: #F24E1E; color: white;">🎨 Figma</span>
                </div>
            </div>
        </div>

        <div class="divider"></div>

        <h2>📊 GitHub Stats</h2>
        <div class="stats-container">
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api?username=swapnitpatel&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub Stats">
            </div>
            <div class="stat-card">
                <img src="https://github-readme-streak-stats.herokuapp.com/?user=swapnitpatel&theme=tokyonight&hide_border=true" alt="GitHub Streak">
            </div>
        </div>
        <div class="stats-container">
            <div class="stat-card">
                <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=swapnitpatel&theme=tokyonight&hide_border=true&layout=compact" alt="Top Languages">
            </div>
        </div>

        <h2>📈 Contribution Graph</h2>
        <div class="contribution-graph">
            <img src="https://github-readme-activity-graph.vercel.app/graph?username=swapnitpatel&theme=tokyo-night&hide_border=true&area=true" alt="Contribution Graph" style="max-width: 100%;">
        </div>

        <div class="divider"></div>

        <h2>🏆 GitHub Trophies</h2>
        <div class="trophy-section">
            <div class="trophy-container">
                <span class="trophy">🏆</span>
                <span class="trophy">⭐</span>
                <span class="trophy">🎯</span>
                <span class="trophy">💎</span>
                <span class="trophy">🔥</span>
            </div>
        </div>

        <div class="divider"></div>

        <h2>🎯 Current Focus</h2>
        <div class="focus-table">
            <table>
                <thead>
                    <tr>
                        <th>💼 Professional</th>
                        <th>🎮 Personal</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>🔭 Working on <strong>Full Stack Web Development Projects</strong></td>
                        <td>♟️ Improving my <strong>Chess Game</strong></td>
                    </tr>
                    <tr>
                        <td>🌱 Learning <strong>Advanced Java & Spring Boot</strong></td>
                        <td>🏏 Playing <strong>Cricket</strong> on weekends</td>
                    </tr>
                    <tr>
                        <td>👯 Looking to collaborate on <strong>Open Source Projects</strong></td>
                        <td>📚 Reading <strong>Tech Articles & Blogs</strong></td>
                    </tr>
                    <tr>
                        <td>💬 Ask me about <strong>Web Development, Java, DSA</strong></td>
                        <td>⚡ <strong>Coffee + Code = Magic ☕💻</strong></td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="divider"></div>

        <h2>🎮 Hobbies & Interests</h2>
        <div class="hobbies-section">
            <div class="hobby-card">
                <h3>♟️ Chess Enthusiast</h3>
                <p><em>Strategic thinking is not just for code!</em></p>
                <div class="hobby-emoji">♟️</div>
                <p style="color: #58a6ff; font-weight: 600;">"In chess, as in coding, every move counts!"</p>
            </div>

            <div class="hobby-card">
                <h3>🏏 Cricket Lover</h3>
                <p><em>Team player on the field and in development!</em></p>
                <div class="hobby-emoji">🏏</div>
                <p style="color: #58a6ff; font-weight: 600;">"Code like you're batting - with patience and precision!"</p>
            </div>
        </div>

        <div class="divider"></div>

        <h2>🌐 Connect with Me</h2>
        <div class="social-links">
            <a href="https://linkedin.com/in/swapnitpatel" class="social-badge linkedin">💼 LinkedIn</a>
            <a href="https://www.instagram.com/swapnitpatel1/" class="social-badge instagram">📷 Instagram</a>
            <a href="https://github.com/swapnitpatel" class="social-badge github">🐙 GitHub</a>
            <a href="https://twitter.com/swapnitpatel" class="social-badge twitter">🐦 Twitter</a>
            <a href="https://swapnitpatel.dev" class="social-badge portfolio">🌐 Portfolio</a>
            <a href="mailto:swapnit@example.com" class="social-badge email">📧 Email</a>
            <a href="https://chess.com/member/swapnitpatel" class="social-badge chess">♟️ Chess.com</a>
        </div>

        <div class="divider"></div>

        <h2>💭 Random Dev Quote</h2>
        <div class="quote-section">
            <p class="quote">"First, solve the problem. Then, write the code." – John Johnson</p>
            <p class="quote">"Chess is the gymnasium of the mind." – Blaise Pascal</p>
            <p class="quote">"Cricket is a team game. If you want fame for yourself, go play an individual game." – Gautam Gambhir</p>
        </div>

        <div class="divider"></div>

        <h2>🐍 Contribution Snake</h2>
        <div class="snake-container">
            <div class="snake-animation">🐍</div>
            <p style="color: #8b949e; margin-top: 10px;">Watch the snake eat your contributions!</p>
        </div>

        <div class="divider"></div>

        <div class="tagline">💻 "Code. Chess. Cricket. Repeat." 💻</div>
    </div>
</body>
</html>
