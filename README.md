<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Prantik — Dev Portfolio</title>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <script src="https://kit.fontawesome.com/a2d9b6f0b2.js" crossorigin="anonymous"></script>
  <style>
    :root{
      --bg:#0f1115; --card:#0f1720; --muted:#98a0aa; --accent:#22c55e;
      --glass: rgba(255,255,255,0.03);
      font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    html,body{height:100%; margin:0; background:
      radial-gradient(1200px 600px at 10% 10%, rgba(34,197,94,0.04), transparent 6%),
      linear-gradient(180deg,#05060a 0%, #0b0d10 100%); color:#e6eef6;}
    .wrap{max-width:1100px;margin:48px auto;padding:28px; display:grid; gap:28px;
      grid-template-columns: 320px 1fr;}
    .left{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent); padding:26px; border-radius:18px; box-shadow: 0 6px 24px rgba(2,6,23,0.6);}
    .avatar{width:220px;height:220px;border-radius:50%; overflow:hidden; border:6px solid rgba(255,255,255,0.02); margin:0 auto; display:block; box-shadow: 0 8px 30px rgba(0,0,0,0.6);}
    .name{font-weight:800;font-size:22px;margin-top:14px;text-align:center;}
    .role{color:var(--muted);text-align:center;margin-top:6px}
    .bio{margin-top:14px;color:var(--muted); font-size:14px; text-align:center; line-height:1.45}
    .btns{display:flex; gap:10px; justify-content:center; margin-top:18px;}
    .btn{background:transparent;border:1px solid rgba(255,255,255,0.06); padding:8px 12px;border-radius:10px; color:var(--muted); text-decoration:none; font-weight:600;}
    .btn.primary{background: linear-gradient(90deg,var(--accent), #10b981); color:#042017; border:none; box-shadow: 0 8px 24px rgba(34,197,94,0.08);}
    .stat-grid{display:flex; justify-content:space-between; margin-top:20px; gap:8px}
    .stat{background:var(--glass); padding:12px;border-radius:10px; text-align:center; flex:1}
    .stat strong{display:block;font-size:18px}
    .right{display:flex; flex-direction:column; gap:18px;}
    .card{background: linear-gradient(180deg, rgba(255,255,255,0.01), transparent); padding:20px; border-radius:14px; box-shadow: 0 6px 20px rgba(2,6,23,0.5)}
    .hero{display:flex; justify-content:space-between; align-items:center; gap:12px}
    .hero .intro{max-width:70%}
    .hero h1{margin:0;font-size:22px}
    .hero p{margin:6px 0;color:var(--muted)}
    .repos{display:grid; grid-template-columns:repeat(auto-fit, minmax(220px,1fr)); gap:12px; margin-top:12px}
    .repo{border-radius:10px;padding:12px;background:rgba(255,255,255,0.02); border:1px solid rgba(255,255,255,0.02)}
    .repo h4{margin:0 0 8px 0}
    .skills{display:flex; gap:8px; flex-wrap:wrap}
    .chip{padding:8px 10px;border-radius:999px;background:rgba(255,255,255,0.02); color:var(--muted); font-weight:600; font-size:13px}
    .projects-carousel{display:flex; gap:12px; overflow:auto; padding-bottom:6px}
    .project{min-width:320px; border-radius:12px; padding:16px; background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent); border:1px solid rgba(255,255,255,0.02)}
    footer{color:var(--muted); text-align:center; margin-top:8px; font-size:13px}
    /* small screens */
    @media(max-width:880px){
      .wrap{grid-template-columns:1fr;padding:18px}
      .avatar{width:160px;height:160px}
      .hero .intro{max-width:100%}
    }
  </style>
</head>
<body>
  <main class="wrap">
    <aside class="left card">
      <img class="avatar" src="/mnt/data/61037391-763d-45de-8f31-28dc28a39b56.png" alt="avatar">
      <div class="name">Prantik De</div>
      <div class="role">Undergrad CSE • Full-Stack Developer</div>
      <p class="bio">I build clean, scalable web apps with React • Node • MongoDB. I love open-source, automation and clean UI.</p>

      <div class="btns">
        <a class="btn primary" href="https://github.com/CS-Prantik" target="_blank"><i class="fa-solid fa-code-branch"></i>&nbsp;GitHub</a>
        <a class="btn" href="mailto:you@example.com"><i class="fa-solid fa-envelope"></i>&nbsp;Contact</a>
      </div>

      <div class="stat-grid" style="margin-top:18px">
        <div class="stat"><strong>22</strong><small style="color:var(--muted)">Contribs</small></div>
        <div class="stat"><strong>6</strong><small style="color:var(--muted)">Repos</small></div>
        <div class="stat"><strong>2</strong><small style="color:var(--muted)">Followers</small></div>
      </div>

      <div style="margin-top:18px">
        <h4 style="margin:6px 0 10px 0">Skills</h4>
        <div class="skills">
          <span class="chip">React</span>
          <span class="chip">Node.js</span>
          <span class="chip">MongoDB</span>
          <span class="chip">EJS</span>
          <span class="chip">Python</span>
        </div>
      </div>
    </aside>

    <section class="right">
      <div class="card hero">
        <div class="intro">
          <h1>Featured projects & work</h1>
          <p>Pin the repos you want shown here (or keep this as a dynamic grid). Below are quick links to your latest and most-popular work.</p>
          <div style="margin-top:12px" class="skills">
            <a class="chip" href="#">CRUD-Using-NodeJS-Express-MongoDB</a>
            <a class="chip" href="#">Prantik_Portfolio</a>
            <a class="chip" href="#">Payment_Integration-App</a>
          </div>
        </div>
        <div style="min-width:210px; text-align:right">
          <div style="font-weight:700">Open-source</div>
          <div style="color:var(--muted); margin-top:8px">Contributions • Projects • Demos</div>
        </div>
      </div>

      <div class="card">
        <h3 style="margin:0 0 10px 0">Pinned repositories</h3>
        <div class="repos">
          <div class="repo">
            <h4>CRUD-USING-NODEJS-EXPRESS-MONGODB</h4>
            <div style="color:var(--muted); font-size:13px">EJS • Express • MongoDB — small CRUD app demo</div>
          </div>
          <div class="repo">
            <h4>Prantik_Portfolio</h4>
            <div style="color:var(--muted); font-size:13px">Static portfolio (this site)</div>
          </div>
          <div class="repo">
            <h4>Payment_Integration-App</h4>
            <div style="color:var(--muted); font-size:13px">Payment integration example</div>
          </div>
        </div>
      </div>

      <div class="card">
        <h3 style="margin:0 0 10px 0">Projects carousel</h3>
        <div class="projects-carousel" id="projects">
          <article class="project">
            <h4>WhatsApp Clone</h4>
            <p style="color:var(--muted)">Realtime chat with socket.io, JWT auth and MongoDB.</p>
            <div style="margin-top:12px"><small style="color:var(--muted)">React • Node • Socket.io</small></div>
          </article>
          <article class="project">
            <h4>FakeTech News Website</h4>
            <p style="color:var(--muted)">News aggregator demo with server-side rendering (EJS).</p>
            <div style="margin-top:12px"><small style="color:var(--muted)">EJS • Express</small></div>
          </article>
          <article class="project">
            <h4>B_Tech Final Year Project</h4>
            <p style="color:var(--muted)">Protein interaction using ML (project summary).</p>
            <div style="margin-top:12px"><small style="color:var(--muted)">Python • ML</small></div>
          </article>
        </div>
      </div>

      <div class="card" style="display:flex; justify-content:space-between; align-items:center;">
        <div>
          <h3 style="margin:0">Contact & Links</h3>
          <p style="color:var(--muted); margin:6px 0 0 0">LinkedIn • LeetCode • Portfolio</p>
        </div>
        <div style="display:flex; gap:10px">
          <a class="btn" href="https://linkedin.com/in/prantik-de-963a17215" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
          <a class="btn" href="https://leetcode.com/u/mrprantikde622/" target="_blank"><i class="fa-solid fa-terminal-code"></i></a>
          <a class="btn" href="https://github.com/CS-Prantik" target="_blank"><i class="fa-brands fa-github"></i></a>
        </div>
      </div>

      <footer>Built with ❤️ • Customize this on your GitHub Pages or profile README.</footer>
    </section>
  </main>

  <script>
    // small enhancement: lazy-scroll projects carousel with arrow keys
    const carousel = document.getElementById('projects');
    document.addEventListener('keydown', e => {
      if(e.key === 'ArrowRight') carousel.scrollBy({left:320, behavior:'smooth'});
      if(e.key === 'ArrowLeft') carousel.scrollBy({left:-320, behavior:'smooth'});
    });
  </script>
  <!-- README.md for GitHub profile -->
<h1 align="left">Hi 👋, I'm Prantik De</h1>
<p align="left">Undergrad CSE • Full-stack dev • Open-source enthusiast</p>

- 🔭 I’m currently working on: **CRUD-Using-NodeJS-Express-MongoDB**
- 🌱 I’m learning: **Machine Learning** and advanced React patterns
- 👯 I’m looking to collaborate on: full-stack projects & open-source tooling
- 💬 Ask me about: JavaScript, Node.js, EJS, MongoDB

### Featured Projects
- **CRUD-USING-NODEJS-EXPRESS-MONGODB** — small full-stack demo.
- **Prantik_Portfolio** — personal site + GitHub Pages.
- **Payment_Integration-App** — payments demo.

### Connect
[![LinkedIn][linkedin-shield]][linkedin-url] [![LeetCode][leetcode-shield]][leetcode-url] [![GitHub][github-shield]][github-url]

[linkedin-shield]: https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white
[leetcode-shield]: https://img.shields.io/badge/LeetCode-FE7A16?style=for-the-badge&logo=leetcode&logoColor=white
[github-shield]: https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white

[linkedin-url]: https://www.linkedin.com/in/prantik-de-963a17215
[leetcode-url]: https://leetcode.com/u/mrprantikde622/
[github-url]: https://github.com/CS-Prantik

</body>
</html>
