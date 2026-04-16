---
title: Team
permalink: /team/
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "https://images.unsplash.com/photo-1494059980473-813e73ee784b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1769&q=80"
  caption: "[Hans-Peter Gauster](https://unsplash.com/@sloppyperfectionist) on [Unsplash](https://unsplash.com)"
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
  .team-wrap * { box-sizing: border-box; }
  .team-wrap {
    font-family: 'Inter', sans-serif;
    max-width: 1100px; margin: 0 auto; padding: 2rem 2rem 5rem;
    --ink: #111827; --ink-2: #4b5563; --ink-3: #9ca3af;
    --white: #fff; --accent: #1e3a6e; --accent-mid: #2563eb;
    --border: #e5e7eb; --radius: 14px;
  }
  .team-wrap .sec-title {
    display: flex; align-items: center; gap: 0.5rem;
    font-size: 1.1rem; font-weight: 600; color: var(--ink);
    border-bottom: 1px solid var(--border); padding-bottom: 0.6rem; margin-bottom: 1.25rem;
  }
  .team-wrap section { margin-bottom: 3rem; }

  /* Founding Director */
  .fd-card {
    display: inline-flex; align-items: center; gap: 1.25rem;
    background: var(--white); border: 1px solid var(--border);
    border-radius: var(--radius); padding: 1.1rem 1.5rem; margin-bottom: 2.5rem;
  }
  .fd-photo {
    width: 80px; height: 80px; border-radius: 10px; flex-shrink: 0;
    background: #dde3ec; overflow: hidden;
    display: flex; align-items: center; justify-content: center;
    font-size: 1.4rem; font-weight: 600; color: var(--accent);
  }
  .fd-photo img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.25s ease; }
  .fd-card:hover .fd-photo img { transform: scale(1.12); }
  .fd-name { font-size: 1.05rem; font-weight: 600; color: var(--ink); margin: 0; }
  .fd-role { font-size: 0.82rem; color: var(--ink-2); margin: 3px 0 0; }
  .fd-years { font-size: 0.78rem; color: var(--ink-3); margin: 2px 0 0; }

  /* Tabs */
  .team-tabs { display: flex; gap: 6px; margin-bottom: 1.75rem; flex-wrap: wrap; }
  .team-tab {
    padding: 6px 18px; border-radius: 8px; font-size: 0.85rem; font-weight: 500;
    border: 1px solid var(--border); background: var(--white); color: var(--ink-2);
    cursor: pointer; transition: all 0.15s ease; text-decoration: none; display: inline-block;
  }
  .team-tab:hover { border-color: #93c5fd; color: var(--accent-mid); }
  .team-tab.active { background: var(--accent); color: #fff !important; border-color: var(--accent); }

  /* Member grid */
  .member-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 14px; }
  .member-card {
    background: var(--white); border: 1px solid var(--border);
    border-radius: var(--radius); padding: 1.1rem 1.1rem 1rem;
    transition: box-shadow 0.18s ease, transform 0.18s ease;
  }
  .member-card:hover { box-shadow: 0 6px 20px rgba(0,0,0,0.07); transform: translateY(-2px); }
  .member-card.tm-hidden { display: none; }

  .card-top { display: flex; align-items: center; gap: 0.8rem; margin-bottom: 0.85rem; }
  .member-photo {
    width: 54px; height: 54px; border-radius: 8px; flex-shrink: 0;
    background: #dde3ec; overflow: hidden;
    display: flex; align-items: center; justify-content: center;
    font-weight: 600; font-size: 0.9rem; color: var(--accent);
  }
  .member-photo img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.25s ease; }
  .member-card:hover .member-photo img { transform: scale(1.12); }
  .member-name { font-size: 0.92rem; font-weight: 600; color: var(--ink); line-height: 1.3; margin: 0; }
  .member-name.alumni { color: var(--accent-mid); }
  .member-name a { color: inherit; text-decoration: none; }
  .member-name a:hover { text-decoration: underline; }

  .card-body { border-top: 1px solid var(--border); padding-top: 0.75rem; }
  .member-role  { font-size: 0.8rem; color: var(--ink-2); margin: 0; }
  .member-years { font-size: 0.78rem; color: var(--ink-3); margin: 2px 0 0; }
  .member-now   { font-size: 0.78rem; color: var(--accent-mid); font-style: italic; margin: 5px 0 0; }

  .member-card.open { background: #f0fdf4; border-color: #bbf7d0; }
  .member-card.open .member-photo { background: #dcfce7; color: #166534; }
  .member-card.open .member-role { color: #166534; }

  /* Collaborators */
  .collab-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); gap: 10px; }
  .collab-item { background: var(--white); border: 1px solid var(--border); border-radius: 10px; padding: 0.8rem 1rem; }
  .collab-name  { font-size: 0.85rem; font-weight: 600; color: var(--ink); margin: 0; }
  .collab-place { font-size: 0.75rem; color: var(--ink-3); margin: 2px 0 0; line-height: 1.4; }
</style>

<div class="team-wrap">

  <!-- Founding Director -->
  <section>
    <p class="sec-title">🏛️ Founding Director</p>
    <div class="fd-card">
      <div class="fd-photo">
        <img src="https://cibs-imhans.github.io/assets/headshots/kk.JPG"
             onerror="this.style.display='none'; this.parentNode.textContent='KP';"
             alt="Krishnakumar Padinharath">
      </div>
      <div>
        <p class="fd-name">Krishnakumar Padinharath</p>
        <p class="fd-role">Founding Director, CIBS · IMHANS</p>
        <p class="fd-years">2022 – 2025</p>
      </div>
    </div>
  </section>

  <!-- Team Members -->
  <section>
    <p class="sec-title"> Team Members</p>

    <div class="team-tabs">
      <button class="team-tab active" onclick="teamFilter('current', this)">Current</button>
      <button class="team-tab" onclick="teamFilter('alumni', this)">Alumni</button>
      <a class="team-tab" href="/alum/" target="_blank">Interns ↗</a>
    </div>

    <div class="member-grid">

      <!-- Current -->
      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/shabeesh.jpeg"
                 onerror="this.style.display='none'; this.parentNode.textContent='SB';" alt="Shabeesh Balan">
          </div>
          <p class="member-name"><a href="https://linktr.ee/shabeeshbalan">Shabeesh Balan</a></p>
        </div>
        <div class="card-body">
          <p class="member-role">Principal Investigator · Scientist</p>
          <p class="member-years">DHR Faculty Fellow · CIBS, IMHANS</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/rajith.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='RR';" alt="Rajith Ravindren">
          </div>
          <p class="member-name"><a href="https://scholar.google.com/citations?hl=en&user=4J0rrcEAAAAJ">Rajith Ravindren</a></p>
        </div>
        <div class="card-body">
          <p class="member-role">Principal Investigator</p>
          <p class="member-years">Research Investigator (Asst. Professor)</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/anu.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='AK';" alt="Anusree A Kumar">
          </div>
          <p class="member-name">Anusree A Kumar</p>
        </div>
        <div class="card-body">
          <p class="member-role">Project Fellow (KSCSTE)</p>
          <p class="member-years">2023–Present · Molecular Psychiatry</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/aisha.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='AS';" alt="Aisha Shaju">
          </div>
          <p class="member-name">Aisha Shaju</p>
        </div>
        <div class="card-body">
          <p class="member-role">Junior Research Fellow (SERB)</p>
          <p class="member-years">Molecular Psychiatry</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/jasmine.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='JJ';" alt="Jasmine John">
          </div>
          <p class="member-name">Jasmine John</p>
        </div>
        <div class="card-body">
          <p class="member-role">Junior Research Fellow (SERB)</p>
          <p class="member-years">Molecular Psychiatry</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/ranjitha.jpeg"
                 onerror="this.style.display='none'; this.parentNode.textContent='RM';" alt="Ranjitha M">
          </div>
          <p class="member-name">Ranjitha M</p>
        </div>
        <div class="card-body">
          <p class="member-role">Research Technician</p>
          <p class="member-years">Cytogenetics</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/najiya.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='FN';" alt="Fathimath Najiya">
          </div>
          <p class="member-name">Fathimath Najiya</p>
        </div>
        <div class="card-body">
          <p class="member-role">Technical Assistant</p>
          <p class="member-years">Electrophysiology</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/MIdhun.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='MS';" alt="Midhun Sidharthan">
          </div>
          <p class="member-name">Midhun Sidharthan</p>
        </div>
        <div class="card-body">
          <p class="member-role">Visiting Researcher</p>
        </div>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/nishanth.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='NJ';" alt="Nishanth JH">
          </div>
          <p class="member-name">Nishanth JH</p>
        </div>
        <div class="card-body">
          <p class="member-role">Visiting Researcher</p>
        </div>
      </div>

      <div class="member-card open" data-type="current">
        <div class="card-top">
          <div class="member-photo">+</div>
          <p class="member-name">Open Position</p>
        </div>
        <div class="card-body">
          <p class="member-role">Research Fellow (DHR project)</p>
        </div>
      </div>

      <div class="member-card open" data-type="current">
        <div class="card-top">
          <div class="member-photo">+</div>
          <p class="member-name">Open Position</p>
        </div>
        <div class="card-body">
          <p class="member-role">Project Fellow (SERB-SURE project)</p>
        </div>
      </div>

      <!-- Alumni -->
      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/varun.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='VK';" alt="Varun Thachan Kundil">
          </div>
          <p class="member-name alumni">Varun Thachan Kundil</p>
        </div>
        <div class="card-body">
          <p class="member-role">Project Fellow (SERB-SURE)</p>
          <p class="member-years">2024–2025</p>
          <p class="member-now">Data Scientist, Yenepoya University</p>
        </div>
      </div>

      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/anu.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='AK';" alt="Anusree A Kumar">
          </div>
          <p class="member-name alumni">Anusree A Kumar</p>
        </div>
        <div class="card-body">
          <p class="member-role">Project Fellow (KSCSTE)</p>
          <p class="member-years">2023–2026</p>
          <p class="member-now">PhD, Tohoku University, Japan</p>
        </div>
      </div>

      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/shilpa.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='SO';" alt="Shilpa O">
          </div>
          <p class="member-name alumni">Shilpa O</p>
        </div>
        <div class="card-body">
          <p class="member-role">Visiting Researcher (Post-Doc)</p>
          <p class="member-years">2023–2025</p>
          <p class="member-now">Assistant Professor, Nitte University</p>
        </div>
      </div>

      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/varun_tk.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='VT';" alt="Varun T K">
          </div>
          <p class="member-name alumni">Varun T K</p>
        </div>
        <div class="card-body">
          <p class="member-role">Project Fellow (SERB-SURE)</p>
          <p class="member-years">2024–2025</p>
          <p class="member-now">Data Scientist, Yenepoya University</p>
        </div>
      </div>

      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/shibila.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='SA';" alt="Shibila A M">
          </div>
          <p class="member-name alumni">Shibila A M</p>
        </div>
        <div class="card-body">
          <p class="member-role">Technical Assistant (Electrophysiology)</p>
          <p class="member-years">2019–2025</p>
          <p class="member-now">Electrophysiologist, Dubai</p>
        </div>
      </div>

      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/niketha.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='NM';" alt="Niketha Manoj">
          </div>
          <p class="member-name alumni">Niketha Manoj</p>
        </div>
        <div class="card-body">
          <p class="member-role">Junior Research Fellow (SERB)</p>
          <p class="member-years">2023–2024</p>
          <p class="member-now">PhD, NIT Calicut</p>
        </div>
      </div>

      <div class="member-card tm-hidden" data-type="alumni">
        <div class="card-top">
          <div class="member-photo">
            <img src="https://cibs-imhans.github.io/assets/headshots/mubashira.jpg"
                 onerror="this.style.display='none'; this.parentNode.textContent='MV';" alt="Mubashira V">
          </div>
          <p class="member-name alumni">Mubashira V</p>
        </div>
        <div class="card-body">
          <p class="member-role">Junior Research Fellow (DHR)</p>
          <p class="member-years">2022–2024</p>
          <p class="member-now">UAE</p>
        </div>
      </div>

    </div>
  </section>

  <!-- Collaborators -->
  <section>
    <p class="sec-title"> Collaborators</p>
    <div class="collab-grid">
      <div class="collab-item"><p class="collab-name">Dr Dileep Vijayan</p><p class="collab-place">Laboratory for Computational and Structural Biology, Jubilee Mission Medical College Hospital &amp; Research Institute, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Neetha Balaram</p><p class="collab-place">Department of Neurology, Government Medical College Calicut, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Divya MS</p><p class="collab-place">Department of Pathology, Sree Chitra Tirunal Institute for Medical Sciences and Technology, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Sreejith PS</p><p class="collab-place">Multidisciplinary Research Unit (MRU), Government Medical College, Thiruvananthapuram, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Lijiya A</p><p class="collab-place">Department of Computer Science and Engineering, NIT Calicut, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Arun Kumar Gangadharan</p><p class="collab-place">Department of Molecular Biology, Kannur University, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Sanish Sathyan</p><p class="collab-place">Department of Molecular Biology, Kannur University, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Joe Cherri Ross</p><p class="collab-place">Department of Computer Science and Engineering, NIT Calicut, Kerala</p></div>
      <div class="collab-item"><p class="collab-name">Dr Varsha Vidyadharan</p><p class="collab-place">Department of Psychiatry, Government Medical College Calicut, Kerala</p></div>
    </div>
  </section>

</div>

<script>
  function teamFilter(type, btn) {
    document.querySelectorAll('.team-tab').forEach(t => t.classList.remove('active'));
    btn.classList.add('active');
    document.querySelectorAll('.member-card').forEach(card => {
      card.classList.toggle('tm-hidden', card.dataset.type !== type);
    });
  }
</script>
