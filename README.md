<!DOCTYPE html>
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
