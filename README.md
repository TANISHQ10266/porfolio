# porfolio
ABOUT MYSELF
<!--
Personal Portfolio — single-file HTML template
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Tanishq Naik — Portfolio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <meta name="description" content="Personal portfolio of Tanishq Naik — Student Developer and Designer." />
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#5eead4; --muted:#94a3b8; --glass: rgba(255,255,255,0.04);
      --radius:16px; font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;background:linear-gradient(180deg,#071028 0%,var(--bg) 100%);color:#e6eef6}
    .container{max-width:980px;margin:36px auto;padding:28px}
    header{display:flex;align-items:center;gap:18px}
    .avatar{width:112px;height:112px;border-radius:18px;background:linear-gradient(135deg,var(--accent),#60a5fa);display:flex;align-items:center;justify-content:center;font-weight:800;color:#082;flex-shrink:0;overflow:hidden}
    .avatar img{width:100%;height:100%;object-fit:cover}
    h1{margin:0;font-size:28px}
    p.lead{margin:6px 0 0;color:var(--muted)}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.015));padding:20px;border-radius:var(--radius);box-shadow: 0 6px 30px rgba(2,6,23,0.6);}

    nav{display:flex;gap:10px;margin-left:auto}
    nav a{padding:8px 12px;border-radius:10px;text-decoration:none;color:var(--muted);font-weight:600}
    nav a.cta{background:var(--glass);color:var(--accent)}

    .grid{display:grid;grid-template-columns:1fr 320px;gap:20px;margin-top:22px}
    @media (max-width:880px){.grid{grid-template-columns:1fr}nav{display:none}}

    section{margin-bottom:18px}
    h2{font-size:18px;margin:0 0 10px}
    .about p{line-height:1.6;color:#d9e9f7}

    .skills{display:flex;flex-wrap:wrap;gap:10px}
    .skill{background:var(--glass);padding:8px 10px;border-radius:999px;font-weight:600;color:var(--muted)}

    .projects{display:flex;flex-direction:column;gap:12px}
    .proj{display:flex;gap:12px;align-items:center;padding:12px;border-radius:12px;background:linear-gradient(90deg, rgba(255,255,255,0.01), rgba(255,255,255,0.01))}
    .proj img{width:84px;height:64px;border-radius:8px;object-fit:cover}
    .proj .meta{flex:1}
    .proj .meta h3{margin:0;font-size:16px}
    .proj .meta p{margin:6px 0 0;color:var(--muted);font-size:13px}
    .btn{display:inline-block;padding:8px 12px;border-radius:10px;text-decoration:none;font-weight:700}
    .btn-primary{background:linear-gradient(90deg,var(--accent),#60a5fa);color:#042;}

    aside .contact-card{display:flex;flex-direction:column;gap:8px}
    .contact-row{display:flex;gap:10px;align-items:center}
    .contact-row svg{width:18px;height:18px;opacity:0.9}

    footer{margin-top:26px;text-align:center;color:var(--muted);font-size:13px}

    /* small utility */
    .muted{color:var(--muted)}
    .pill{background:rgba(255,255,255,0.03);padding:6px 8px;border-radius:999px}
  </style>
</head>
<body>
  <div class="container">
    <header class="card">
      <div class="avatar" aria-hidden="true">
        <span style="font-size:34px;color:rgba(255,255,255,0.95);">TN</span>
      </div>
      <div>
        <h1>Tanishq Naik <span class="muted">— Student • Developer • Designer</span></h1>
        <p class="lead">A passionate student who loves technology, design, and building innovative projects. Always exploring new ideas and improving skills.</p>
        <nav>
          <a href="#about">About</a>
          <a href="#projects">Projects</a>
          <a href="#contact" class="cta">Contact</a>
        </nav>
      </div>
    </header>

    <div class="grid">
      <main>
        <section id="about" class="card about">
          <h2>About me</h2>
          <p>Hello — I'm <strong>Tanishq Naik</strong>, a Class 10 student at <em>KVS Vastrapur</em>. I’m a budding developer and designer with a keen interest in technology, gadgets, and AI-based projects like <strong>AgriPal</strong>. I enjoy creating things that blend creativity and functionality.</p>

          <h3 style="margin-top:14px">Skills</h3>
          <div class="skills">
            <div class="skill">Python</div>
            <div class="skill">HTML & CSS</div>
            <div class="skill">Arduino</div>
            <div class="skill">AI / ML</div>
            <div class="skill">Public Speaking</div>
          </div>
        </section>

        <section id="projects" class="card projects">
          <h2>Selected Projects</h2>

          <article class="proj">
            <img src="https://via.placeholder.com/320x200.png?text=AgriPal" alt="AgriPal screenshot">
            <div class="meta">
              <h3>AgriPal — AI Chatbot for Farmers</h3>
              <p class="muted">An AI-powered chatbot prototype created using Dialogflow and MIT App Inventor to help farmers with instant information. Developed with a user-friendly interface for rural use.</p>
            </div>
            <div>
              <a class="btn btn-primary" href="#">View</a>
            </div>
          </article>

          <article class="proj">
            <img src="https://via.placeholder.com/320x200.png?text=Project+2" alt="Project 2 screenshot">
            <div class="meta">
              <h3>Project Name</h3>
              <p class="muted">A one-line summary of another personal project or experiment showcasing creativity and coding skills.</p>
            </div>
            <div>
              <a class="btn" href="#">View</a>
            </div>
          </article>

        </section>

        <section id="work" class="card">
          <h2>Experience & Education</h2>
          <p class="muted">School: Kendriya Vidyalaya Vastrapur — Class 10. Participant in INSPIRE Awards and other science & tech competitions. Always eager to learn and explore real-world applications of tech.</p>
        </section>

      </main>

      <aside>
        <section class="card contact-card" id="contact">
          <h2>Contact</h2>
          <div class="contact-row"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><path d="M21 8v6a2 2 0 0 1-2 2H5l-4 3V7a2 2 0 0 1 2-2h4"/></svg><div><strong>Email</strong><div class="muted">youremail@example.com</div></div></div>
          <div class="contact-row"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor"><path d="M3 5h18M3 12h18M3 19h18"/></svg><div><strong>Phone / UPI</strong><div class="muted">+91-XXXXXXXXXX / UPI@id</div></div></div>

          <div style="margin-top:10px"><a class="btn btn-primary" href="mailto:youremail@example.com">Email me</a></div>

          <h3 style="margin-top:14px">Social</h3>
          <div style="display:flex;gap:8px;flex-wrap:wrap">
            <a class="pill" href="#">GitHub</a>
            <a class="pill" href="#">LinkedIn</a>
            <a class="pill" href="#">Fiverr</a>
          </div>
        </section>

        <section class="card" style="margin-top:12px">
          <h2>Quick facts</h2>
          <p class="muted" style="margin:0">Location: Ahmedabad, India</p>
          <p class="muted" style="margin:6px 0 0">Availability: Open for small freelance projects • School student</p>
        </section>
      </aside>
    </div>

    <footer>
      <div class="muted">Made with ❤️ • Tanishq Naik — © <span id="year"></span></div>
    </footer>
  </div>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', e=>{
        e.preventDefault();
        const t = document.querySelector(a.getAttribute('href'));
        if(t) t.scrollIntoView({behavior:'smooth', block:'start'});
      })
    });
  </script>
</body>
</html>
