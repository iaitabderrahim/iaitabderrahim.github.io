# iaitabderrahim.github.io
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Imène Ait Abderrahim | Researcher in Operations Research & AI</title>

    <meta name="description"
          content="Academic webpage of Imène Ait Abderrahim, researcher in Operations Research, Combinatorial Optimization, Metaheuristics, Automatic Algorithm Configuration, and Machine Learning.">

    <link rel="stylesheet"
          href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: "Segoe UI", Arial, sans-serif;
            line-height: 1.7;
            color: #263238;
            background: #f7f9fb;
        }

        a {
            color: #1769aa;
            text-decoration: none;
        }

        a:hover {
            color: #0d47a1;
        }

        /* ---------- Navigation ---------- */

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255,255,255,0.96);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid #e5e9ed;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1150px;
            margin: auto;
            padding: 14px 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.25rem;
            font-weight: 700;
            color: #263238;
        }

        .nav-links {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .nav-links a {
            color: #455a64;
            font-size: 0.95rem;
            font-weight: 500;
        }

        .nav-links a:hover {
            color: #1769aa;
        }

        /* ---------- Hero ---------- */

        .hero {
            min-height: 92vh;
            display: flex;
            align-items: center;
            padding: 120px 25px 70px;
            background:
                linear-gradient(135deg, #eef5fa 0%, #ffffff 55%, #f3f7fa 100%);
        }

        .hero-container {
            max-width: 1100px;
            width: 100%;
            margin: auto;
            display: grid;
            grid-template-columns: 1fr 300px;
            gap: 70px;
            align-items: center;
        }

        .hero h1 {
            font-size: 3.3rem;
            line-height: 1.15;
            margin-bottom: 18px;
            color: #172b3a;
        }

        .hero h2 {
            font-size: 1.35rem;
            font-weight: 500;
            color: #1769aa;
            margin-bottom: 25px;
        }

        .hero p {
            font-size: 1.08rem;
            max-width: 720px;
            color: #546e7a;
            margin-bottom: 28px;
        }

        .profile-image {
            width: 260px;
            height: 260px;
            object-fit: cover;
            border-radius: 50%;
            border: 7px solid white;
            box-shadow: 0 10px 35px rgba(0,0,0,0.12);
            display: block;
            margin: auto;
        }

        .buttons {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
        }

        .button {
            display: inline-block;
            padding: 11px 20px;
            border-radius: 6px;
            font-weight: 600;
            transition: 0.2s;
        }

        .button-primary {
            background: #1769aa;
            color: white;
        }

        .button-primary:hover {
            background: #0d47a1;
            color: white;
        }

        .button-secondary {
            border: 1px solid #b0bec5;
            color: #455a64;
            background: white;
        }

        .button-secondary:hover {
            border-color: #1769aa;
            color: #1769aa;
        }

        /* ---------- Sections ---------- */

        section {
            padding: 85px 25px;
        }

        .section-container {
            max-width: 1050px;
            margin: auto;
        }

        .section-title {
            font-size: 2rem;
            color: #172b3a;
            margin-bottom: 12px;
        }

        .section-subtitle {
            color: #78909c;
            margin-bottom: 40px;
        }

        /* ---------- About ---------- */

        .about-grid {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 45px;
        }

        .about-text p {
            margin-bottom: 18px;
        }

        .info-card {
            background: white;
            padding: 25px;
            border-radius: 10px;
            border: 1px solid #e5e9ed;
        }

        .info-card h3 {
            margin-bottom: 15px;
            color: #1769aa;
        }

        .info-card ul {
            list-style: none;
        }

        .info-card li {
            margin-bottom: 10px;
        }

        /* ---------- Research ---------- */

        .research-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 22px;
        }

        .research-card {
            background: white;
            padding: 28px;
            border-radius: 10px;
            border: 1px solid #e5e9ed;
            transition: 0.25s;
        }

        .research-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.07);
        }

        .research-card i {
            font-size: 1.8rem;
            color: #1769aa;
            margin-bottom: 15px;
        }

        .research-card h3 {
            margin-bottom: 10px;
            color: #263238;
        }

        .research-card p {
            color: #607d8b;
            font-size: 0.95rem;
        }

        /* ---------- Projects ---------- */

        .project {
            background: white;
            border-left: 4px solid #1769aa;
            padding: 25px 30px;
            margin-bottom: 20px;
            border-radius: 0 8px 8px 0;
            border-top: 1px solid #e5e9ed;
            border-right: 1px solid #e5e9ed;
            border-bottom: 1px solid #e5e9ed;
        }

        .project h3 {
            color: #263238;
            margin-bottom: 8px;
        }

        .project p {
            color: #607d8b;
        }

        .tags {
            margin-top: 14px;
        }

        .tag {
            display: inline-block;
            background: #eef5fa;
            color: #1769aa;
            padding: 4px 10px;
            border-radius: 20px;
            font-size: 0.78rem;
            margin: 3px 4px 3px 0;
        }

        /* ---------- Publications ---------- */

        .publication {
            background: white;
            padding: 24px 28px;
            margin-bottom: 16px;
            border-radius: 8px;
            border: 1px solid #e5e9ed;
        }

        .publication h3 {
            font-size: 1.05rem;
            color: #263238;
            margin-bottom: 7px;
        }

        .publication .authors {
            color: #607d8b;
            font-size: 0.94rem;
        }

        .publication .venue {
            color: #1769aa;
            font-size: 0.92rem;
            margin-top: 5px;
        }

        /* ---------- Experience ---------- */

        .timeline {
            border-left: 3px solid #d8e2e8;
            padding-left: 30px;
        }

        .timeline-item {
            position: relative;
            margin-bottom: 35px;
        }

        .timeline-item::before {
            content: "";
            position: absolute;
            width: 12px;
            height: 12px;
            background: #1769aa;
            border-radius: 50%;
            left: -38px;
            top: 8px;
        }

        .timeline-item h3 {
            color: #263238;
        }

        .timeline-item .date {
            color: #1769aa;
            font-size: 0.9rem;
            font-weight: 600;
        }

        /* ---------- Contact ---------- */

        .contact {
            background: #172b3a;
            color: white;
        }

        .contact .section-title {
            color: white;
        }

        .contact .section-subtitle {
            color: #b0bec5;
        }

        .contact-links {
            display: flex;
            flex-wrap: wrap;
            gap: 18px;
        }

        .contact-link {
            display: flex;
            align-items: center;
            gap: 9px;
            color: white;
            border: 1px solid #546e7a;
            padding: 11px 17px;
            border-radius: 6px;
        }

        .contact-link:hover {
            background: #263f50;
            color: white;
        }

        /* ---------- Footer ---------- */

        footer {
            background: #10212c;
            color: #90a4ae;
            text-align: center;
            padding: 25px;
            font-size: 0.88rem;
        }

        /* ---------- Responsive ---------- */

        @media (max-width: 800px) {

            .nav-links {
                display: none;
            }

            .hero-container {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .buttons {
                justify-content: center;
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .research-grid {
                grid-template-columns: 1fr;
            }

            .hero {
                padding-top: 110px;
            }
        }
    </style>
</head>

<body>

<!-- ================= NAVIGATION ================= -->

<nav>
    <div class="nav-container">

        <div class="logo">
            I. Ait Abderrahim
        </div>

        <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#research">Research</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#publications">Publications</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>

    </div>
</nav>


<!-- ================= HERO ================= -->

<header class="hero">

    <div class="hero-container">

        <div>

            <h1>Imène Ait Abderrahim</h1>

            <h2>
                Researcher in Operations Research, Optimization & Artificial Intelligence
            </h2>

            <p>
                I work at the intersection of <strong>Operations Research</strong>,
                <strong>Combinatorial Optimization</strong>,
                <strong>Metaheuristics</strong>,
                <strong>Automatic Algorithm Configuration</strong>,
                and <strong>Machine Learning</strong>.
            </p>

            <p>
                My research focuses on developing adaptive and data-driven
                optimization algorithms that can dynamically adjust their
                search behaviour according to problem characteristics and
                the state of the optimization process.
            </p>

            <div class="buttons">

                <a class="button button-primary"
                   href="#research">
                    <i class="fas fa-flask"></i>
                    Research
                </a>

                <a class="button button-secondary"
                   href="#publications">
                    <i class="fas fa-book"></i>
                    Publications
                </a>

                <a class="button button-secondary"
                   href="cv.pdf">
                    <i class="fas fa-file-pdf"></i>
                    CV
                </a>

            </div>

        </div>


        <div>

            <!-- Replace profile.jpg with your photograph -->
            <img src="profile.jpg"
                 alt="Imène Ait Abderrahim"
                 class="profile-image">

        </div>

    </div>

</header>


<!-- ================= ABOUT ================= -->

<section id="about">

    <div class="section-container">

        <h2 class="section-title">About Me</h2>

        <p class="section-subtitle">
            Research, optimization and intelligent algorithm design
        </p>

        <div class="about-grid">

            <div class="about-text">

                <p>
                    I am a researcher in Computer Science and Operations Research
                    working on computational methods for difficult combinatorial
                    optimization problems.
                </p>

                <p>
                    My research combines mathematical optimization,
                    metaheuristics, machine learning and automated algorithm
                    configuration. A particular focus of my work is the design
                    of <strong>adaptive optimization algorithms</strong> whose
                    parameters and search strategies can evolve during the
                    optimization process.
                </p>

                <p>
                    I am particularly interested in understanding the relationship
                    between <strong>problem characteristics</strong>,
                    <strong>algorithm behaviour</strong>, and
                    <strong>optimization performance</strong>.
                </p>

                <p>
                    This perspective motivates my work on feature-driven
                    algorithm configuration, hyper-configuration and dynamic
                    parameter control for metaheuristics.
                </p>

            </div>


            <div class="info-card">

                <h3>Research Profile</h3>

                <ul>
                    <li>
                        <strong>Field:</strong><br>
                        Computer Science & Operations Research
                    </li>

                    <li>
                        <strong>Focus:</strong><br>
                        Combinatorial Optimization
                    </li>

                    <li>
                        <strong>Methods:</strong><br>
                        Metaheuristics & Machine Learning
                    </li>

                    <li>
                        <strong>Specialization:</strong><br>
                        Automatic Algorithm Configuration
                    </li>
                </ul>

            </div>

        </div>

    </div>

</section>


<!-- ================= RESEARCH ================= -->

<section id="research">

    <div class="section-container">

        <h2 class="section-title">Research Interests</h2>

        <p class="section-subtitle">
            Main research directions
        </p>


        <div class="research-grid">

            <div class="research-card">

                <i class="fas fa-project-diagram"></i>

                <h3>Combinatorial Optimization</h3>

                <p>
                    Exact and heuristic approaches for complex
                    NP-hard optimization problems.
                </p>

            </div>


            <div class="research-card">

                <i class="fas fa-robot"></i>

                <h3>Metaheuristics</h3>

                <p>
                    Iterated Local Search, Tabu Search, PSO,
                    ALNS, Genetic Algorithms and hybrid methods.
                </p>

            </div>


            <div class="research-card">

                <i class="fas fa-sliders-h"></i>

                <h3>Algorithm Configuration</h3>

                <p>
                    Automatic and data-driven configuration of
                    optimization algorithms.
                </p>

            </div>


            <div class="research-card">

                <i class="fas fa-brain"></i>

                <h3>Machine Learning</h3>

                <p>
                    Learning-based approaches for predicting,
                    controlling and adapting algorithm behaviour.
                </p>

            </div>


            <div class="research-card">

                <i class="fas fa-chart-line"></i>

                <h3>Algorithm Behaviour</h3>

                <p>
                    Analysis of search dynamics, landscapes,
                    features and exploration-exploitation behaviour.
                </p>

            </div>


            <div class="research-card">

                <i class="fas fa-ship"></i>

                <h3>Maritime Optimization</h3>

                <p>
                    Berth allocation and related scheduling problems
                    in maritime transportation and logistics.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- ================= PROJECTS ================= -->

<section id="projects">

    <div class="section-container">

        <h2 class="section-title">Research Projects</h2>

        <p class="section-subtitle">
            Selected research directions and ongoing work
        </p>


        <div class="project">

            <h3>
                Feature-Driven Adaptive Algorithm Configuration
            </h3>

            <p>
                Development of hybrid approaches combining offline automatic
                algorithm configuration with online machine-learning-based
                dynamic parameter adjustment. The objective is to allow
                optimization algorithms to adapt their behaviour during a run
                according to problem characteristics and search dynamics.
            </p>

            <div class="tags">
                <span class="tag">ADAC</span>
                <span class="tag">AAC</span>
                <span class="tag">Machine Learning</span>
                <span class="tag">Metaheuristics</span>
                <span class="tag">Dynamic Parameters</span>
            </div>

        </div>


        <div class="project">

            <h3>
                Hyper-Configurable ALNS for Multi-Port Berth Allocation
            </h3>

            <p>
                Adaptive Large Neighborhood Search for multi-port continuous
                berth allocation, with parameter values dynamically controlled
                through problem and search-state features.
            </p>

            <div class="tags">
                <span class="tag">ALNS</span>
                <span class="tag">Berth Allocation</span>
                <span class="tag">Logistics</span>
                <span class="tag">Hyper-Configuration</span>
            </div>

        </div>


        <div class="project">

            <h3>
                Quadratic 3-Dimensional Assignment Problem
            </h3>

            <p>
                Hybrid metaheuristic approaches for the Q3AP, including
                Iterated Local Search, Tabu Search and Particle Swarm
                Optimization, together with automatic algorithm configuration.
            </p>

            <div class="tags">
                <span class="tag">Q3AP</span>
                <span class="tag">ILS</span>
                <span class="tag">Tabu Search</span>
                <span class="tag">PSO</span>
                <span class="tag">Automatic Configuration</span>
            </div>

        </div>


        <div class="project">

            <h3>
                Algorithm Behaviour & Landscape Analysis
            </h3>

            <p>
                Investigation of algorithm trajectories, time-series features,
                exploration-exploitation dynamics and the relationship between
                optimization behaviour and problem characteristics.
            </p>

            <div class="tags">
                <span class="tag">Time Series</span>
                <span class="tag">Landscape Analysis</span>
                <span class="tag">Features</span>
                <span class="tag">Explainability</span>
            </div>

        </div>

    </div>

</section>


<!-- ================= PUBLICATIONS ================= -->

<section id="publications">

    <div class="section-container">

        <h2 class="section-title">Selected Publications</h2>

        <p class="section-subtitle">
            Selected scientific contributions
        </p>


        <!-- Replace these entries with your final publications -->

        <div class="publication">

            <h3>
                Hyper-configurable reactive adaptive large neighborhood
                search for multi-port berth allocation
            </h3>

            <div class="authors">
                I. Ait Abderrahim et al.
            </div>

            <div class="venue">
                Scientific publication — details and DOI to be added
            </div>

        </div>


        <div class="publication">

            <h3>
                Hybrid metaheuristic approaches for the
                Quadratic 3-Dimensional Assignment Problem
            </h3>

            <div class="authors">
                I. Ait Abderrahim et al.
            </div>

            <div class="venue">
                Scientific publication — details and DOI to be added
            </div>

        </div>


        <div class="publication">

            <h3>
                Automatic configuration and adaptive search
                for combinatorial optimization
            </h3>

            <div class="authors">
                I. Ait Abderrahim et al.
            </div>

            <div class="venue">
                Scientific publication — details and DOI to be added
            </div>

        </div>


        <p style="margin-top:30px;">
            <a href="#">
                <strong>→ View complete publication list</strong>
            </a>
        </p>

    </div>

</section>


<!-- ================= EXPERIENCE ================= -->

<section id="experience">

    <div class="section-container">

        <h2 class="section-title">Academic Experience</h2>

        <p class="section-subtitle">
            Academic and research activities
        </p>


        <div class="timeline">

            <div class="timeline-item">

                <div class="date">
                    2025 – Present
                </div>

                <h3>
                    Postdoctoral Researcher
                </h3>

                <p>
                    Sorbonne University, France
                </p>

                <p>
                    Research on optimization, automatic algorithm configuration,
                    adaptive metaheuristics and machine learning.
                </p>

            </div>


            <div class="timeline-item">

                <div class="date">
                    Previous Research Experience
                </div>

                <h3>
                    International Research Collaborations
                </h3>

                <p>
                    Research collaborations and stays involving automatic
                    algorithm configuration, combinatorial optimization,
                    algorithm features and data-driven optimization.
                </p>

            </div>


            <div class="timeline-item">

                <div class="date">
                    PhD
                </div>

                <h3>
                    PhD in Computer Science
                </h3>

                <p>
                    University of Oran 1 Ahmed Ben Bella, Algeria
                </p>

                <p>
                    Research on metaheuristic optimization for the
                    Quadratic 3-Dimensional Assignment Problem.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- ================= CONTACT ================= -->

<section id="contact" class="contact">

    <div class="section-container">

        <h2 class="section-title">
            Contact & Academic Profiles
        </h2>

        <p class="section-subtitle">
            Feel free to connect for research collaborations,
            academic opportunities and scientific discussions.
        </p>


        <div class="contact-links">

            <!-- Replace "#" with your actual profile URLs -->

            <a class="contact-link" href="mailto:YOUR_EMAIL@example.com">
                <i class="fas fa-envelope"></i>
                Email
            </a>

            <a class="contact-link"
               href="https://github.com/iaitabderrahim"
               target="_blank">
                <i class="fab fa-github"></i>
                GitHub
            </a>

            <a class="contact-link"
               href="#"
               target="_blank">
                <i class="fas fa-graduation-cap"></i>
                Google Scholar
            </a>

            <a class="contact-link"
               href="#"
               target="_blank">
                <i class="fab fa-orcid"></i>
                ORCID
            </a>

            <a class="contact-link"
               href="#"
               target="_blank">
                <i class="fab fa-linkedin"></i>
                LinkedIn
            </a>

        </div>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <p>
        © 2026 Imène Ait Abderrahim.
        Academic personal website.
    </p>

</footer>


</body>
</html>
```
