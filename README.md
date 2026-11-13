<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>My Personal Portfolio | Computer Science</title>

<style>
:root {
    --bg: #f4f4f9;
    --text: #334155;
    --muted: #64748b;
    --card: #ffffff;
    --border: #e2e8f0;
    --brand: #172554;
    --accent: #3b82f6;
    --heading: #172554;
    --shadow: 0 4px 14px rgba(23,37,84,0.08);
}

* { box-sizing: border-box; }

html { scroll-behavior: smooth; }

body {
    font-family: "Segoe UI", Arial, sans-serif;
    margin: 0;
    background: var(--bg);
    color: var(--text);
    line-height: 1.7;
    text-align: center;
}

nav {
    position: sticky;
    top: 0;
    z-index: 10;
    background: var(--brand);
    padding: 14px;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 22px;
}

nav a {
    color: white;
    text-decoration: none;
}

nav a:hover { color: #93c5fd; }

header {
    background: linear-gradient(135deg,#172554,#1e3a8a);
    color: white;
    padding: 90px 20px 100px;
}

.badge {
    display: inline-block;
    background: rgba(255,255,255,0.12);
    border: 1px solid rgba(255,255,255,0.25);
    padding: 6px 16px;
    border-radius: 999px;
    margin-bottom: 22px;
}

header h1 {
    font-size: clamp(2.2rem,6vw,3.6rem);
    margin: 0 0 16px;
}

header p {
    max-width: 650px;
    margin: auto auto 30px;
    color: #dbeafe;
    font-size: 1.1rem;
}

.btn {
    display: inline-block;
    padding: 12px 28px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 600;
    margin: 6px;
}

.btn-primary {
    background: var(--accent);
    color: white;
}

.btn-outline {
    border: 2px solid white;
    color: white;
}

section { padding: 70px 20px; }

.wrap {
    max-width: 1000px;
    margin: auto;
}

h2 {
    color: var(--heading);
    font-size: 2rem;
}

h2::after {
    content: "";
    display: block;
    width: 56px;
    height: 4px;
    background: var(--accent);
    margin: 12px auto;
    border-radius: 4px;
}

.lead {
    max-width: 650px;
    margin: 18px auto;
    color: var(--muted);
}

.overview-text {
    max-width: 750px;
    margin: 25px auto;
}

.stats {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(180px,1fr));
    gap: 20px;
    margin-top: 40px;
}

.stat, .project {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 14px;
    padding: 25px;
    box-shadow: var(--shadow);
}

.stat strong {
    display: block;
    font-size: 2rem;
    color: var(--heading);
}

.stat span { color: var(--muted); }

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(260px,1fr));
    gap: 24px;
    margin-top: 40px;
}

.icon {
    font-size: 2rem;
    margin-bottom: 12px;
}

.project h3 { color: var(--heading); }

.project p { color: var(--muted); }

footer {
    background: var(--brand);
    color: white;
    padding: 30px;
}

@media(max-width:600px) {
    header { padding: 60px 20px; }
    section { padding: 50px 18px; }
}
</style>
</head>

<body>

<nav>
    <a href="#top">Home</a>
    <a href="#overview">Overview</a>
    <a href="#features">Features</a>
    <a href="#structure">Structure</a>
    <a href="#future">Future</a>
</nav>

<!-- TITLE -->
<header id="top">
    <span class="badge">Computer Science Student | Portfolio 2026</span>

    <h1>My Personal Portfolio</h1>

    <p>
        Welcome to my personal portfolio! I am a Computer Science student
        passionate about technology, programming and problem-solving.
        This platform showcases my skills, projects and continuous
        learning journey in the world of computing.
    </p>

    <a class="btn btn-primary" href="#features">Explore My Skills</a>
    <a class="btn btn-outline" href="#overview">About My Portfolio</a>
</header>

<!-- OVERVIEW -->
<section id="overview">
<div class="wrap">

    <h2>Portfolio Overview</h2>

    <p class="lead">
        A digital platform presenting my academic journey,
        technical abilities and achievements in Computer Science.
    </p>

    <p class="overview-text">
        This personal portfolio has been developed to introduce
        my background as a Computer Science student and provide
        an overview of my interests, technical skills and
        programming projects. It serves as a central platform
        where my academic work and practical experiences can
        be presented in an organised manner.
    </p>

    <p class="overview-text">
        The portfolio is designed using HTML and CSS to provide
        a clean, attractive and user-friendly experience.
        It demonstrates my understanding of web development,
        website structure and responsive design while providing
        room to showcase new projects and skills as I continue
        developing my knowledge in technology.
    </p>

    <div class="stats">
        <div class="stat">
            <strong>01</strong>
            <span>Personal Portfolio</span>
        </div>

        <div class="stat">
            <strong>06</strong>
            <span>Core Features</span>
        </div>

        <div class="stat">
            <strong>03</strong>
            <span>Main Technologies</span>
        </div>

        <div class="stat">
            <strong>∞</strong>
            <span>Learning Opportunities</span>
        </div>
    </div>

</div>
</section>

<!-- FEATURES -->
<section id="features">
<div class="wrap">

    <h2>Portfolio Features</h2>

    <p class="lead">
        Key sections and functionalities that make this
        portfolio informative, organised and easy to use.
    </p>

    <div class="grid">

        <div class="project">
            <div class="icon">👩‍💻</div>
            <h3>About Me</h3>
            <p>
                Introduces my background, academic journey,
                interests and passion for Computer Science.
            </p>
        </div>

        <div class="project">
            <div class="icon">💻</div>
            <h3>Technical Skills</h3>
            <p>
                Highlights my programming knowledge,
                technical abilities and developing skills
                in computer applications.
            </p>
        </div>

        <div class="project">
            <div class="icon">📂</div>
            <h3>My Projects</h3>
            <p>
                Displays my academic assignments,
                practical programming exercises and
                personal development projects.
            </p>
        </div>

        <div class="project">
            <div class="icon">🎓</div>
            <h3>Education</h3>
            <p>
                Presents my academic background and
                learning progress as a Computer Science student.
            </p>
        </div>

        <div class="project">
            <div class="icon">📱</div>
            <h3>Responsive Design</h3>
            <p>
                Provides a flexible layout that adapts
                to mobile phones, tablets and desktop computers.
            </p>
        </div>

        <div class="project">
            <div class="icon">📧</div>
            <h3>Contact Information</h3>
            <p>
                Provides a section where visitors can
                find ways to connect and communicate with me.
            </p>
        </div>

    </div>
</div>
</section>

<!-- STRUCTURE -->
<section id="structure">
<div class="wrap">

    <h2>Portfolio Structure</h2>

    <p class="lead">
        Organisation of the website files and technologies.
    </p>

    <div class="project">
        <p><strong>index.html</strong> – Contains the website content and structure.</p>
        <p><strong>style.css</strong> – Controls the appearance, colours and layout.</p>
        <p><strong>script.js</strong> – Can be used to add interactive functionality.</p>
        <p><strong>assets/</strong> – Stores images and other website resources.</p>
    </div>

</div>
</section>

<!-- FUTURE -->
<section id="future">
<div class="wrap">

    <h2>Future Improvements</h2>

    <p class="lead">
        Planned developments to improve the portfolio.
    </p>

    <div class="grid">

        <div class="project">
            <h3>1. Project Expansion</h3>
            <p>
                Add more programming projects and practical
                work as my technical knowledge grows.
            </p>
        </div>

        <div class="project">
            <h3>2. Interactive Features</h3>
            <p>
                Introduce JavaScript to improve user
                interaction and website functionality.
            </p>
        </div>

        <div class="project">
            <h3>3. Improved Design</h3>
            <p>
                Continue improving the website's appearance,
                accessibility and responsiveness.
            </p>
        </div>

        <div class="project">
            <h3>4. Professional Development</h3>
            <p>
                Update my skills, achievements and experience
                as I progress in my Computer Science studies.
            </p>
        </div>

    </div>

</div>
</section>

<footer>
    <p>© 2026 My Personal Portfolio | Computer Science Student</p>
    <p>Learning Today, Building Tomorrow.</p>
</footer>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>My Project</title>
<style>
    :root {
        --bg: #f4f4f9;
        --text: #334155;
        --muted: #64748b;
        --card: #ffffff;
        --border: #e2e8f0;
        --brand: #172554;
        --accent: #3b82f6;
        --heading: #172554;
        --code-bg: #eef0f7;
        --shadow: 0 4px 14px rgba(23, 37, 84, 0.08);
    }
    @media (prefers-color-scheme: dark) {
        :root:not([data-theme="light"]) {
            --bg: #0f172a;
            --text: #cbd5e1;
            --muted: #94a3b8;
            --card: #1e293b;
            --border: #334155;
            --heading: #bfdbfe;
            --code-bg: #0b1220;
            --shadow: 0 4px 14px rgba(0, 0, 0, 0.35);
        }
    }
    :root[data-theme="dark"] {
        --bg: #0f172a;
        --text: #cbd5e1;
        --muted: #94a3b8;
        --card: #1e293b;
        --border: #334155;
        --heading: #bfdbfe;
        --code-bg: #0b1220;
        --shadow: 0 4px 14px rgba(0, 0, 0, 0.35);
    }

    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }

    body {
        font-family: "Segoe UI", Arial, sans-serif;
        margin: 0;
        background: var(--bg);
        color: var(--text);
        line-height: 1.7;
        text-align: center;
    }

    /* ---------- NAV ---------- */
    nav {
        position: sticky;
        top: 0;
        z-index: 10;
        background: var(--brand);
        padding: 12px 20px;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 6px 22px;
    }
    nav a {
        color: #dbeafe;
        text-decoration: none;
        font-size: 0.95rem;
        padding: 4px 2px;
        border-bottom: 2px solid transparent;
        transition: border-color 0.2s, color 0.2s;
    }
    nav a:hover { color: #fff; border-color: var(--accent); }

    /* ---------- TITLE / HERO ---------- */
    header {
        background: linear-gradient(135deg, #172554 0%, #1e3a8a 100%);
        color: #fff;
        padding: 90px 20px 100px;
    }
    .badge {
        display: inline-block;
        background: rgba(255, 255, 255, 0.12);
        border: 1px solid rgba(255, 255, 255, 0.25);
        padding: 6px 16px;
        border-radius: 999px;
        font-size: 0.85rem;
        letter-spacing: 0.04em;
        margin-bottom: 22px;
    }
    header h1 {
        font-size: clamp(2.2rem, 6vw, 3.6rem);
        margin: 0 0 16px;
        line-height: 1.15;
    }
    header p {
        max-width: 620px;
        margin: 0 auto 32px;
        font-size: 1.1rem;
        color: #dbeafe;
    }
    .btn {
        display: inline-block;
        padding: 12px 28px;
        border-radius: 8px;
        text-decoration: none;
        font-weight: 600;
        margin: 6px;<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>My Project</title>
<style>
    :root {
        --bg: #f4f4f9;
        --text: #333;
        --card: #ffffff;
        --brand: #172554;
        --heading: #172554;
        --code-bg: #eef0f7;
        box-sizing: border-box;
        padding-top: env(safe-area-inset-top, 0px);
        padding-bottom: env(safe-area-inset-bottom, 0px);
    }
    @media (prefers-color-scheme: dark) {
        :root:not([data-theme="light"]) {
            --bg: #0f172a;
            --text: #e2e8f0;
            --card: #1e293b;
            --heading: #bfdbfe;
            --code-bg: #0f172a;
        }
    }
    :root[data-theme="dark"] {
        --bg: #0f172a;
        --text: #e2e8f0;
        --card: #1e293b;
        --heading: #bfdbfe;
        --code-bg: #0f172a;
    }
    html { scroll-padding-top: env(safe-area-inset-top, 0px); }
    * { box-sizing: border-box; }

    body {
        font-family: Arial, sans-serif;
        margin: 0;
        background: var(--bg);
        color: var(--text);
        text-align: center;
        line-height: 1.6;
    }

    header {
        background: var(--brand);
        color: white;
        padding: 40px 20px;
    }
    header p { margin: 8px 0 0; opacity: 0.85; }

    section {
        padding: 30px 20px;
    }

    h2 {
        color: var(--heading);
    }

    .project {
        background: var(--card);
        padding: 20px;
        margin: 15px auto;
        max-width: 500px;
        border-radius: 10px;
    }
    .project h3 { margin-top: 0; color: var(--heading); }
    .project p { margin: 0; }

    .overview { max-width: 600px; margin: 0 auto; }

    .code-wrap {
        max-width: 500px;
        margin: 15px auto;
        overflow-x: auto;
        text-align: left;
        background: var(--code-bg);
        border-radius: 10px;
    }
    pre { margin: 0; padding: 20px; font-size: 14px; }

    footer {
        background: var(--brand);
        color: white;
        padding: 15px;
        padding-bottom: calc(15px + env(safe-area-inset-bottom, 0px));
    }
</style>
</head>
<body>

<header>
    <h1>Project Title</h1>
    <p>A short one-line tagline describing what your project does</p>
</header>

<section id="overview">
    <h2>Overview</h2>
    <p class="overview">
        Describe your project here: what problem it solves, who it is for, and
        the technologies you used to build it. Keep it to two or three sentences
        so a visitor understands the goal at a glance.
    </p>
</section>

<section id="features">
    <h2>Features</h2>
    <div class="project">
        <h3>Feature One</h3>
        <p>A brief description of what this feature does for the user.</p>
    </div>
    <div class="project">
        <h3>Feature Two</h3>
        <p>A brief description of what this feature does for the user.</p>
    </div>
    <div class="project">
        <h3>Feature Three</h3>
        <p>A brief description of what this feature does for the user.</p>
    </div>
</section>

<section id="structure">
    <h2>Structure</h2>
    <div class="code-wrap">
<pre>project/
├── index.html      # page content
├── style.css       # styling
├── script.js       # behaviour
└── assets/         # images and icons</pre>
    </div>
    <div class="project">
        <p>Explain how the parts fit together, for example: the front end calls the back end, which reads from the database.</p>
    </div>
</section>

<section id="future">
    <h2>Future Improvements</h2>
    <div class="project">
        <h3>Planned Enhancements</h3>
        <p>Add user accounts, improve performance, and support more devices.</p>
    </div>
    <div class="project">
        <h3>Ideas I’d Like to Try</h3>
        <p>Add search, a dark mode toggle, and automated tests.</p>
    </div>
</section>

<footer>
    <p>© 2026 Your Name. All rights reserved.</p>
</footer>

</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: #f4f4f9;
            color: #333;
            text-align: center;
        }

        header {
            background: #172554;
            color: white;
            padding: 40px 20px;
        }

        section {
            padding: 30px 20px;
        }

        h2 {
            color: #172554;
        }

        .project {
            background: white;
            padding: 20px;
            margin: 15px auto;
            max-width: 500px;
            border-radius: 10px;
        }

        footer {
            background: #172554;
            color: white;
            padding: 15px;
        }
    </style>
</head>

<body>

<header>
    <h1>Welcome to My Portfolio</h1>
    <p>Computer Science Student | Aspiring Developer</p>
</header>

<section>
    <h2>About Me</h2>
    <p>Hello! I am a Computer Science student passionate about
    programming, technology and web development.</p>
</section>

<section>
    <h2>My Skills</h2>
    <p>HTML | CSS | C++ | Python | Java</p>
</section>

<section>
    <h2>My Projects</h2>

    <div class="project">
        <h3>My First Portfolio</h3>
        <p>A personal website showcasing my skills and projects.</p>
    </div>
</section>

<footer>
    <p>My Portfolio | 2026</p>
</footer>

</body>
</html>
