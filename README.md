<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>My Simple Portfolio</title>
  <style>
    :root{
      --bg:#f7f9fb;
      --card:#ffffff;
      --muted:#6b7280;
      --accent:#0ea5a4;
      --glass: rgba(255,255,255,0.6);
      font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,var(--bg),#eef6f5);color:#0f1724}
    header{
      display:flex;align-items:center;gap:20px;padding:28px;max-width:1100px;margin:28px auto;border-radius:16px;background:linear-gradient(90deg, rgba(255,255,255,0.85), rgba(250,250,250,0.75));box-shadow:0 6px 18px rgba(2,6,23,0.06);
    }
    .hero-img{width:120px;height:120px;flex:0 0 120px;border-radius:12px;object-fit:cover;border:2px solid rgba(15,23,36,0.06)}
    .hero-title{display:flex;flex-direction:column}
    h1{font-size:1.6rem;margin:0}
    p.lead{margin:6px 0 0;color:var(--muted)}

    nav{max-width:1100px;margin:0 auto;display:flex;justify-content:flex-end;padding:0 28px}
    nav a{margin-left:12px;text-decoration:none;color:var(--accent);font-weight:600}

    main{max-width:1100px;margin:20px auto;padding:12px}
    .grid{display:grid;grid-template-columns:1fr 340px;gap:20px}
    @media (max-width:880px){.grid{grid-template-columns:1fr} .hero-img{display:none}}

    .card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.04)}
    h2{margin:0 0 12px}
    ul.skills{list-style:none;padding:0;margin:0;display:flex;flex-wrap:wrap;gap:8px}
    ul.skills li{background:var(--glass);padding:8px 10px;border-radius:999px;font-weight:600;color:#064e4b}

    .contact a{display:inline-block;margin-right:10px;text-decoration:none;padding:8px 12px;border-radius:8px;background:linear-gradient(180deg,var(--accent),#02877f);color:#fff}
    .contact a.secondary{background:transparent;color:var(--accent);border:1px solid rgba(14,165,164,0.15)}

    footer{text-align:center;color:var(--muted);padding:20px;margin-top:18px}

    /* small helpers */
    .muted{color:var(--muted)}
    .small{font-size:0.9rem}

  </style>
</head>
<body>
  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
  </nav>

  <header>
    <!-- Using the uploaded image from the conversation as hero image -->
    <img class="hero-img" src="/mnt/data/a30abbe0-521f-45a4-9104-b19154185893.png" alt="Screenshot"/>
    <div class="hero-title">
      <h1>Hi — I'm Kian Jedric B. Catubag</h1>
      <p class="lead">I'm a 1st year college student who is starting my journey in web development. I like creating simple and clean websites that are easy to use.</p>
      <p class="small muted">Name: Kian Jedric B. Catubag • Year: 1st Year College • Age: 18 • Location: Philippines</p>
    </div>
  </header>

  <main>
    <div class="grid">
      <section class="card" id="about">
        <h2>About Me</h2>
        <p class="muted small">Write a short introduction: who you are, what you study, and a sentence about what you enjoy or hope to achieve. Keep it personal and professional.</p>
        <p style="margin-top:12px">Example: I'm a third-year Computer Science student focused on front-end development. I enjoy turning designs into responsive websites and learning new web technologies.</p>

        <h3 style="margin-top:16px">What I can do</h3>
        <ul>
          <li>Build responsive websites using HTML &amp; CSS</li>
          <li>Simple interactive pages with JavaScript</li>
          <li>Deploy projects via GitHub Pages</li>
        </ul>
      </section>

      <aside class="card">
        <h2 id="skills">Skills</h2>
        <p class="muted small">Short description of skills you're aiming to hone.</p>
        <ul class="skills" style="margin-top:12px">
          <li>HTML</li>
          <li>CSS</li>
          <li>Responsive Design</li>
          <li>Git / GitHub</li>
          <li>Basic JavaScript</li>
        </ul>

        <h3 style="margin-top:16px">Contact or Links</h3>
        <p class="small muted">Share a way for people to reach you or view your work.</p>
        <div class="contact" id="contact" style="margin-top:8px">
          <a href="mailto:youremail@example.com">Email me</a>
          <a class="secondary" href="#">LinkedIn</a>
        </div>

        <p class="small muted" style="margin-top:12px">Tip: Replace placeholders with your real links (GitHub repo, LinkedIn, or a message inviting connections).</p>
      </aside>

      <section class="card" style="grid-column:1/-1;margin-top:8px">
        <h2>Notes</h2>
        <p class="muted small">This single-file site is ready to be uploaded to GitHub Pages. Customize the text, replace the hero image, and update links before publishing.</p>
        <ol>
          <li>Save this file as <code>index.html</code>.</li>
          <li>Put it in the root of a GitHub repo named <code>&lt;your-username&gt;.github.io</code> or push to the main branch and enable GitHub Pages in repo settings.</li>
        </ol>
        <p class="small muted">If you'd like, I can adapt the design, add more sections (projects, resume download), or convert this to separate CSS/JS files.</p>
      </section>

    </div>

    <footer class="card">
      <p class="small muted">Made with ❤️ — edit this template to make it yours.</p>
    </footer>
  </main>

</body>
</html>
