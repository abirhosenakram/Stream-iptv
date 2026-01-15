<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>STREAM IPTV by abirhosenakram</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-bg: #0f0c29;
            --gradient: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
            --accent-color: #4a90e2;
            --warning-bg: #fff5f5;
            --text-main: #333;
            --text-light: #fff;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: #f8fafc;
            margin: 0;
            padding: 20px;
            color: var(--text-main);
            line-height: 1.6;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        .header {
            text-align: center;
            background: var(--gradient);
            padding: 60px 20px;
            border-radius: 20px;
            color: var(--text-light);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .logo-box {
            width: 120px;
            height: 120px;
            background-color: #007bff;
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 20px;
            margin-bottom: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
            border: 3px solid rgba(255,255,255,0.2);
        }

        .play-button {
            width: 0;
            height: 0;
            border-top: 25px solid transparent;
            border-bottom: 25px solid transparent;
            border-left: 40px solid black;
            margin-left: 8px;
        }

        .header h1 {
            margin: 10px 0;
            font-size: 2.8em;
            letter-spacing: -1px;
        }

        .header p {
            font-size: 1.1em;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto 25px;
        }

        .badge-group {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
        }

        .warning-box {
            background: var(--warning-bg);
            border-left: 5px solid #e53e3e;
            padding: 20px;
            margin: 30px 0;
            border-radius: 12px;
            color: #c53030;
        }

        .warning-box h3 { margin-top: 0; display: flex; align-items: center; gap: 10px; }

        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: -30px;
            padding: 0 20px;
        }

        .feature-card {
            background: #fff;
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
            border: 1px solid #edf2f7;
        }

        .feature-card:hover { transform: translateY(-5px); }

        .feature-card i { font-size: 40px; color: var(--accent-color); margin-bottom: 15px; }

        .section {
            background: #fff;
            margin-top: 30px;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        .section h2 {
            border-bottom: 2px solid #edf2f7;
            padding-bottom: 10px;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            list-style: none;
            padding: 0;
            margin-bottom: 25px;
        }

        .tech-item {
            background: #f1f5f9;
            padding: 8px 15px;
            border-radius: 8px;
            font-size: 0.9em;
            font-weight: 600;
        }

        .footer {
            text-align: center;
            margin-top: 60px;
            padding: 40px;
            background: #fff;
            border-radius: 20px;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
        }

        @media (max-width: 600px) {
            .header h1 { font-size: 2em; }
            .features { margin-top: 20px; }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header">
        <div class="logo-box">
            <div class="play-button"></div>
        </div>
        <h1>STREAM IPTV</h1>
        <p>Elevating Your Live Streaming Experience with seamless performance and high-quality content.</p>
        
        <div class="badge-group">
            <a href="https://abirhosenakram.github.io/Stream-iptv/" target="_blank">
                <img src="https://img.shields.io/badge/Launch_Web_App-0078D4?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Web App">
            </a>
            <a href="https://github.com/abirhosenakram/Stream-iptv/releases">
                <img src="https://img.shields.io/badge/Download_APK-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android">
            </a>
        </div>
    </div>

    <div class="features">
        <div class="feature-card">
            <i class="fas fa-bolt"></i>
            <h3>Ultra Fast</h3>
            <p>Optimized buffers for seamless and instant channel switching.</p>
        </div>
        <div class="feature-card">
            <i class="fas fa-mobile-alt"></i>
            <h3>Fully Responsive</h3>
            <p>Flawless viewing experience on Desktop, Tablets & Mobile devices.</p>
        </div>
        <div class="feature-card">
            <i class="fas fa-code-branch"></i>
            <h3>GPL Licensed</h3>
            <p>Open source project. All types of improvements are highly welcome.</p>
        </div>
    </div>

    <div class="section">
        <h2><i class="fas fa-layer-group"></i> Technical Architecture</h2>
        <ul class="tech-stack">
            <li class="tech-item">HTML5</li>
            <li class="tech-item">CSS3</li>
            <li class="tech-item">Vanilla JavaScript ES6+</li>
            <li class="tech-item">HLS Protocol</li>
            <li class="tech-item">GitHub Pages</li>
        </ul>

        <hr style="border: 0; border-top: 1px solid #eee; margin: 30px 0;">

<h2><i class="fas fa-balance-scale"></i> License & Disclaimer</h2>
<p>
    <strong>Content Ownership:</strong> The developer does not host any of the channels or streams available in this application. All content is aggregated from publicly available <a href="https://raw.githubusercontent.com/FunctionError/PiratesTv/main/combined_playlist.m3u" target="_blank">playlists</a> on the internet.
</p>
        <p>
            <strong>Connectivity:</strong> Due to geo-blocking restrictions, some channels may not be accessible in all regions. We recommend using a <strong>VPN</strong> for an unrestricted experience.
        </p>
        <p>
            <strong>Open Source:</strong> This project is distributed under the <strong>GPL License</strong>. We believe in community-driven growth; therefore, all kinds of improvements, bug fixes, and feature suggestions are more than welcome.
        </p>
    </div>

    <div class="footer">
        <h2>Developed By Abir Hosen Akram</h2>
        <div class="social-links">
            <a href="https://www.linkedin.com/in/abir-hosen-93b409368" target="_blank">
                <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
            </a>
        </div>
        <p style="margin-top: 20px; font-size: 0.8em; color: #777;">&copy; 2026 Stream IPTV. Licensed under <b>GPL</b>.</p>
    </div>
</div>

</body>
</html>
