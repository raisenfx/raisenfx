<!-- RAISENFX README ✨ -->
<!DOCTYPE html>
<html>
<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
            color: #ffffff;
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        /* Animations */
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        
        @keyframes glow {
            0%, 100% { box-shadow: 0 0 20px rgba(255, 30, 30, 0.3); }
            50% { box-shadow: 0 0 30px rgba(255, 30, 30, 0.6); }
        }
        
        @keyframes textShine {
            0% { background-position: 0% 50%; }
            100% { background-position: 100% 50%; }
        }
        
        /* Header Section */
        .header {
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }
        
        .banner {
            width: 100%;
            border-radius: 20px;
            animation: glow 3s ease-in-out infinite;
            transition: transform 0.3s ease;
        }
        
        .banner:hover {
            transform: scale(1.02);
        }
        
        .spotify-player {
            margin-top: 1.5rem;
            padding: 1rem;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            display: inline-block;
        }
        
        /* Content Sections */
        .section {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 20px;
            padding: 2rem;
            margin-bottom: 2rem;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }
        
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
        }
        
        .section-title {
            font-family: 'Poppins', sans-serif;
            font-size: 1.5rem;
            margin-bottom: 1.5rem;
            background: linear-gradient(90deg, #ff6b6b, #ffa500, #ff6b6b);
            background-size: 200% auto;
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: textShine 3s linear infinite;
        }
        
        /* Profile Section */
        .profile-container {
            display: flex;
            align-items: center;
            gap: 2rem;
        }
        
        .profile-gif {
            width: 220px;
            border-radius: 15px;
            animation: float 4s ease-in-out infinite;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .profile-text {
            flex: 1;
            font-size: 1rem;
            color: #d1d5db;
        }
        
        .highlight {
            background: rgba(255, 107, 107, 0.2);
            padding: 0.2rem 0.5rem;
            border-radius: 6px;
            color: #ff6b6b;
            font-weight: 500;
        }
        
        /* Tech Stack */
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(80px, 1fr));
            gap: 1rem;
            margin-top: 1rem;
        }
        
        .tech-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 1rem;
            border-radius: 12px;
            text-align: center;
            transition: all 0.3s ease;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        
        .tech-item:hover {
            transform: scale(1.1);
            background: rgba(255, 107, 107, 0.2);
        }
        
        .tech-icon {
            font-size: 2rem;
            margin-bottom: 0.5rem;
        }
        
        /* Stats */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1rem;
            margin-top: 1rem;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            background: rgba(255, 107, 107, 0.1);
        }
        
        .stat-number {
            font-size: 2rem;
            font-weight: 700;
            color: #ff6b6b;
        }
        
        /* Footer */
        .footer {
            text-align: center;
            margin-top: 3rem;
            padding: 2rem;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .profile-container {
                flex-direction: column;
                text-align: center;
            }
            
            .profile-gif {
                width: 180px;
            }
            
            .tech-grid {
                grid-template-columns: repeat(4, 1fr);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="header">
            <img src="https://raw.githubusercontent.com/raisenfx/raisenfx/main/assets/banner.png" 
                 alt="Raisen Banner" class="banner">
            
            <div class="spotify-player">
                🎧 
                <a href="https://open.spotify.com/intl-tr/track/7ytrEtJNzhMEhoBp5Thmvr?si=f417dc728e744ef0"
                   target="_blank"
                   style="color:#1DB954; font-weight:bold; text-decoration:none;">
                   <span style="font-family:'Inter',sans-serif; letter-spacing:1px;">𝔑 Now Playing</span>
                </a>
            </div>
        </div>

        <!-- Who Am I Section -->
        <div class="section">
            <h2 class="section-title">👨‍💻 Who Am I?</h2>
            <div class="profile-container">
                <img src="https://media.tenor.com/Gh3LKX9HMFkAAAAj/hollow-knight-knight.gif" 
                     alt="Hollow Knight" class="profile-gif">
                <div class="profile-text">
                    <p>I'm a student of <span class="highlight">Computer Engineering at the İzmir University of Economics</span>.</p>
                    <p>My journey in technology started with a passion for creating immersive experiences. I began writing small scripts in <span class="highlight">FiveM</span>, which eventually sparked a deeper interest in programming and development.</p>
                    <p>Over time, I developed a strong eye for both functionality and design — striving to build digital experiences that are not only efficient but also visually engaging.</p>
                    <p>While I explore the full-stack ecosystem, my true passion lies in <span class="highlight">Front-End Development</span>, where I combine logic with visual creativity. I believe great code should be both elegant and maintainable.</p>
                </div>
            </div>
        </div>

        <!-- About Me Section -->
        <div class="section">
            <div class="profile-container">
                <div class="profile-text">
                    <h3 class="section-title">🎯 A Little More About Me</h3>
                    <ul style="list-style: none; padding: 0;">
                        <li style="margin-bottom: 0.8rem; padding-left: 1.5rem; position: relative;">
                            <span style="position: absolute; left: 0; color: #ff6b6b;">▶</span>
                            I grow stronger through complex challenges
                        </li>
                        <li style="margin-bottom: 0.8rem; padding-left: 1.5rem; position: relative;">
                            <span style="position: absolute; left: 0; color: #ff6b6b;">▶</span>
                            Learning advanced React & performance tuning
                        </li>
                        <li style="margin-bottom: 0.8rem; padding-left: 1.5rem; position: relative;">
                            <span style="position: absolute; left: 0; color: #ff6b6b;">▶</span>
                            I love mentoring new devs & sharing knowledge
                        </li>
                        <li style="margin-bottom: 0.8rem; padding-left: 1.5rem; position: relative;">
                            <span style="position: absolute; left: 0; color: #ff6b6b;">▶</span>
                            Fast, lightweight & maintainable code is the goal
                        </li>
                        <li style="margin-bottom: 0.8rem; padding-left: 1.5rem; position: relative;">
                            <span style="position: absolute; left: 0; color: #ff6b6b;">▶</span>
                            Design philosophy: "Less is more, with impact"
                        </li>
                    </ul>
                </div>
                <img src="https://i.pinimg.com/originals/10/27/f8/1027f80aeabcbb74a2e698be71829e9e.gif" 
                     alt="Samurai" class="profile-gif">
            </div>
        </div>

        <!-- Tech Stack -->
        <div class="section">
            <h3 class="section-title">🛠️ My Tech Stack</h3>
            <div class="tech-grid">
                <div class="tech-item">
                    <div class="tech-icon">🌐</div>
                    <span>HTML5</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">🎨</div>
                    <span>CSS3</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">⚡</div>
                    <span>JavaScript</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">☕</div>
                    <span>Java</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">🔗</div>
                    <span>Node.js</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">🐍</div>
                    <span>Python</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">🎮</div>
                    <span>Lua</span>
                </div>
                <div class="tech-item">
                    <div class="tech-icon">⚛️</div>
                    <span>React</span>
                </div>
            </div>
        </div>

        <!-- Stats -->
        <div class="section">
            <h3 class="section-title">📊 GitHub Stats</h3>
            <div class="stats-container">
                <div class="stat-card">
                    <div class="stat-number">15+</div>
                    <div>Projects</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">2K+</div>
                    <div>Code Commits</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">500+</div>
                    <div>Contributions</div>
                </div>
                <div class="stat-card">
                    <div class="stat-number">24/7</div>
                    <div>Learning Mode</div>
                </div>
            </div>
        </div>

        <!-- Footer -->
        <div class="footer">
            <div style="font-size: 2rem; margin-bottom: 1rem;">⚡</div>
            <h3 style="margin-bottom: 1rem; font-family: 'Poppins', sans-serif;">Ready for the Next Challenge</h3>
            <p style="color: #9ca3af; margin-bottom: 1.5rem;">
                Let's build something amazing together. Innovation through code, perfection through design.
            </p>
            <div style="display: flex; justify-content: center; gap: 1rem; margin-bottom: 1.5rem;">
                <a href="https://github.com/raisenfx" target="_blank" style="color: #fff; text-decoration: none; padding: 0.5rem 1rem; background: rgba(255, 255, 255, 0.1); border-radius: 8px; transition: all 0.3s ease;">
                    GitHub
                </a>
                <a href="https://discord.com/users/ichbinraisen" target="_blank" style="color: #fff; text-decoration: none; padding: 0.5rem 1rem; background: rgba(255, 255, 255, 0.1); border-radius: 8px; transition: all 0.3s ease;">
                    Discord
                </a>
            </div>
            <p style="color: #6b7280; font-size: 0.9rem;">
                Crafted with precision 🥷🏿 — <strong>RaisenFX</strong> • 2024
            </p>
        </div>
    </div>

    <script>
        // Add some interactive effects
        document.addEventListener('DOMContentLoaded', function() {
            // Add hover effects to all interactive elements
            const interactiveElements = document.querySelectorAll('.tech-item, .stat-card, .section');
            
            interactiveElements.forEach(element => {
                element.addEventListener('mouseenter', function() {
                    this.style.transform = 'translateY(-5px)';
                });
                
                element.addEventListener('mouseleave', function() {
                    this.style.transform = 'translateY(0)';
                });
            });
            
            // Animate stats counting (simplified)
            const statNumbers = document.querySelectorAll('.stat-number');
            statNumbers.forEach(stat => {
                const target = parseInt(stat.textContent);
                let current = 0;
                const increment = target / 50;
                const timer = setInterval(() => {
                    current += increment;
                    if (current >= target) {
                        current = target;
                        clearInterval(timer);
                    }
                    stat.textContent = Math.floor(current) + (stat.textContent.includes('+') ? '+' : '');
                }, 30);
            });
        });
    </script>
</body>
</html>
