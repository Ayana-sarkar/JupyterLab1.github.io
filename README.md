
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
        <h1>Special Functions</h1>
        </div>
    </section>

    <section id="curriculum" class="curriculum">
            <div class="card">
                <h2>1.Bessel functions</h2>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <p>Line 1: scipy.special.jv(v, z): This is the SciPy implementation for the Bessel function of the first kind of real order v and complex/real argument z, typically denoted mathematically as Jv(x).as bessel: This renames the function to bessel within the script to make the subsequent code more readable.<br> 
                Line 2: creates a NumPy array of 500 equally spaced points ranging from x = 0 to x = 15.<br> 
                Line3: range(0, 6): We are about to draw 6 curves, so this loops through the integer values 0, 1, 2, 3, 4, 5. These represent the orders (v) of the Bessel functions.<br> 
                Line 4: bessel(v, xbsl): In each iteration, SciPy vectorizes the operation. It evaluates the Bessel function of order v for all 500 points stored in xbsl simultaneously, returning an array of 500 corresponding y-values. <br> 
                Every time this loop runs, (plt.plot ) - overlays a new curveJ0(x) through J5(x) onto the same figure in a distinct color. <br>
                Line5-6: : plt.xlim: Clamps the horizontal viewing window tightly between x = 0 and x = 15.<br> 
                plt.ylim: Sets the vertical bounds from -0.5 to 1.1. This is ideal for these lower-order Bessel functions because J0(x)=1and they all damp out and oscillate well within these boundaries.<br> 
                Line 7: loc = 0: Tells Matplotlib to choose the "best" location for the legend box automatically, placing it where it minimizes overlap with the plotted data lines.<br>
                <img src="htt.png.png" alt="Data Visualization" class="box-image"></p>
            </div>
            <div class="card">
                <h2>2.Legendre Functions</h2>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <p>3rd-order Legendre polynomial, mathematically written as:<br> 
                P3(x) = ½ *(5x3 - 3x) = 2.5x3 - 1.5x <br> 
                In The First Output , The Array [ 2.5, 0. , -1.5, 0. ]: This array contains the coefficients of the polynomial, ordered from the highest power to the lowest power (x3, x2, x1, x0). <br> 
                In The Second Output, the top 3 represents the exponent (x3). The 3 is sitting directly over the first x, meaning 2.5 x3.<br> 
                The second x has nothing above it, which implies a default power of 1(meaning -1.5x1).<br> 
                Let’s plot all six Legendre polynomials for x ∈ (−1, 1). Polynomials within that range are orthogonal with weight w = 1 <br>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                Line 1: Why [-1, 1]? Legendre polynomials are natively orthogonal over the domain [-1, 1]. This is the standard mathematical interval used to study and plot them.<br>
                Line3: y0s(x) : Passing the array x into it evaluates the polynomial at all 200 points simultaneously, returning a new array of 200 numeric y-values. The script repeats this process efficiently on single lines using semicolons (e.g., y1s=Lp(1); y1=y1s(x)) all the way up to y6.<br> 
                pp:  Matplotlib accepts an arbitrary number of (x, y) pairs in a single call. This command plots 7 distinct lines sequentially: (x, y0), then (x, y1), up to (x, y6). </p>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
            </div>
            <div class="card">
                <h2>3. Airy Functions</h2>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <p>Line 2: Evaluates the Airy functions over your entire x domain in a single operation.<br> 
                The scipy.special.airy() function takes the input array x and simultaneously calculates and returns four separate output arrays of the exact same length (201 points each):<br> 
                ai: The Airy function of the first kind, Ai(x).<br> 
                aip: The derivative of the first kind,Ai'(x).<br> 
                bi: The Airy function of the second kind, Bi(x).<br> 
                bip: The derivative of the second kind, Bi’(x).<br> 
                Line 7: loc='upper left' explicitly forces the box into the top-left corner of the window. This is ideal because the Airy functions damp out/stay low on the left side of this plot, leaving that space open.<br>
                Matplotlib commands often return text or handle objects. Assigning the output to a throwaway variable name (like _t or just _) prevents Jupyter Notebook from printing a raw text line description of the legend object.</p>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
            </div>
            <div class="card">
                <h2>4.</h2>
                <img src="htt.png.png" alt="Data Visualization" class="box-image">
                <p>o</p>
            </div>
    </section>

</body>
