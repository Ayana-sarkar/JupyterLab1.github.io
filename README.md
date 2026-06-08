#JupyterLab1.github.io
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mastering JupyterLab</title>
    <style>
        /* Modern Reset & Variables */
        * {
            margin: 0;
            padding: 0;
            box-box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        :root {
            --bg-color: #0f172a;
            --card-bg: #1e293b;
            --accent-orange: #f97316;
            --accent-blue: #38bdf8;
            --text-main: #f8fafc;
            --text-muted: #94a3b8;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
        }

        /* Navbar */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.5rem 10%;
            padding-bottom: 0px; 
            margin-bottom: 0px;
            background-color: rgba(15, 23, 42, 0.8);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            padding-bottom: 0px; 
            margin-bottom: 0px;
            color: var(--text-main);
        }
        .logo span {
            color: var(--accent-orange);
        }
        .nav-links a {
            color: var(--text-muted);
            text-decoration: none;
            margin-left: 2rem;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: var(--accent-blue);
        }

        /* Hero Section */
        .hero {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 5rem 10%;
            min-height: 80vh;
        }
       .hero-content, [class*="hero"] {
          width: 100% !important;
           max-width: 950px !important; 
           margin: 0 auto !important;  
           padding: 40px 20px !important;
          text-align: left !important;  
        }

    .hero-content h1 {
         font-size: 3.5rem;
         line-height: 1.2;
         margin-bottom: 1.5rem;
        }

     .hero-content h1 span {
         color: var(--accent-orange);
       }
       .h1 {
       margin-top: 10px;
    }


     .hero-content p {
          font-size: 1.2rem;
         color: var(--text-muted);
         margin-bottom: 2rem;
         max-width: 800px; 
       }
       .btn {
        display: inline-block;
        background: linear-gradient(135deg, var(--accent-orange), #ea580c);
        color: white;
        padding: 0.8rem 2rem;
        border-radius: 5px;
        text-decoration: none;
        font-weight: bold;
        transition: transform 0.3s, box-shadow 0.3s;
    }
    .btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 4px 20px rgba(249, 115, 22, 0.4);
    }
       
        /* Interactive Code Box Demo */
        .hero-visual {
            max-width: 45%;
            width: 100%;
        }
        .code-box {
            background-color: var(--card-bg);
            border-radius: 8px;
            padding: 1.5rem;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            border: 1px solid #334155;
        }
        .code-header {
            display: flex;
            gap: 0.5rem;
            margin-bottom: 1rem;
        }
        
        .code-input {
            color: var(--accent-blue);
            font-family: 'Courier New', Courier, monospace;
            margin-bottom: 1rem;
        }
        .code-output {
            background-color: #0f172a;
            padding: 1rem;
            border-radius: 4px;
            border-left: 4px solid var(--accent-orange);
            font-family: monospace;
        }

        /* Curriculum Section */
        .curriculum {
            padding: 5rem 10%;
            background-color: #0b111e;
        }
        .curriculum h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
        }
        .grid,.row, [class*="card-container"], [class*="wrapper"]{
            display:flex !important;
            flex-direction: column !important;
            align-items: center !important;
            width: 100% !important; 
        }
        .card,[class*="box"], [class*="item"]{
            background-color: var(--card-bg);
            width: 100% !important;
            max-width: 800px !important;
            margin-bottom: 24px !important; 
            padding: 24px !important;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .card h3 {
            color: var(--accent-blue);
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--text-muted);
            border-top: 1px solid #1e293b;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero {
                flex-direction: column;
                text-align: center;
                padding-top: 2rem;
            }
            .hero-content {
                max-width: 100%;
                margin-bottom: 3rem;
            }
            .hero-visual {
                max-width: 100%;
            }
            .nav-links {
                display: none; /* Keep it simple for mobile */
            }
    </style>
</head>
<body>

    <nav>
        <div class="logo">🚀 Learn<span>Jupyter</span></div>
        <div class="nav-links">
        </div>
    </nav>

    <section class="hero">
        <div class="hero-content">
            <a href="https://ayana-sarkar.github.io/Home2.github.io/" class="btn">Basic</a>
         <a href="https://ayana-sarkar.github.io/JupyterLab4.github.io/" class="btn">Plotting with List</a>
        <a href="https://ayana-sarkar.github.io/JupyterLab5.github.io/" class="btn">Plotting with Arrays</a>
        <a href="https://ayana-sarkar.github.io/JupyterLab2.github.io/" class="btn">Interpolation</a>
        <h1>Let's Practice more!</h1>
        </div>
    </section>

    <section id="curriculum" class="curriculum">
            <div class="card">
                <h2>1. Interface & Setup</h2>
                <p>Install Anaconda, launch JupyterLab, and master the left sidebar, file browser, and tabbed layouts.</p>
            </div>
            <div class="card">
                <h2>2. Cells & Markdown</h2>
                <p>Grlding certification (like LEED etc) systems to ensure adherence to 
                sustainable building standards and performance criteria</p>
            </div>
            <div class="card">
                <h2>3. Keyboard Shortcuts</h2>
                <p>Speed up your workflow drastically using Command and Edit modes, cell execution shortcuts, and deletions.</p>
            </div>
            <div class="card">
                <h2>4. Data & Visuals</h2>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <p>Import CSVs, run Pandas operations, and render beautiful Matplotlib/Seaborn plots directly inside your notebook.</p>
            </div>
    </section>

</body>
