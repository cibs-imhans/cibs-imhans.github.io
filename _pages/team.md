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
<style>
*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
:root {
  --navy:    #0d1f3c;
  --navy-2:  #1b3a6b;
  --navy-3:  #2d5da1;
  --gold:    #b8963e;
  --gold-2:  #d4ad5a;
  --gold-3:  #f5e6c0;
  --ink:     #1a1a2e;
  --ink-2:   #4a4a6a;
  --ink-3:   #8888aa;
  --surface: #f7f6f3;
  --white:   #ffffff;
  --border:  #e2dfd8;
  --r:       10px;
}
/* ── LAYOUT ── */
.page {
  max-width: 1100px;
  margin: 0 auto;
  padding: 3.5rem 2rem 6rem;
}
/* ── SECTION HEADERS ── */
.sec-header {
  display: flex;
  align-items: baseline;
  gap: 1rem;
  margin-bottom: 2rem;
}
.sec-label {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.68rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--gold);
  font-weight: 500;
  flex-shrink: 0;
}
.sec-line {
  flex: 1;
  height: 1px;
  background: var(--border);
}
.sec-title-text {
  font-family: 'EB Garamond', serif;
  font-size: 1.55rem;
  font-weight: 500;
  color: var(--navy);
  margin-bottom: 0.2rem;
}
section { margin-bottom: 4.5rem; }
/* ── FOUNDING DIRECTOR ── */
.fd-card {
  display: flex;
  align-items: center;
  gap: 2rem;
  background: var(--white);
  border: 1px solid var(--border);
  border-top: 3px solid var(--navy);
  border-radius: var(--r);
  padding: 2rem 2.5rem;
  max-width: 560px;
  transition: box-shadow 0.2s;
}
.fd-card:hover { box-shadow: 0 8px 32px rgba(13,31,60,0.1); }
.fd-photo-wrap {
  width: 90px; height: 90px;
  border-radius: 8px;
  overflow: hidden;
  flex-shrink: 0;
  background: var(--gold-3);
  display: flex; align-items: center; justify-content: center;
  font-family: 'EB Garamond', serif;
  font-size: 1.5rem;
  color: var(--navy-2);
}
.fd-photo-wrap img {
  width: 100%; height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}
.fd-card:hover .fd-photo-wrap img { transform: scale(1.07); }
.fd-info {}
.fd-name {
  font-family: 'EB Garamond', serif;
  font-size: 1.3rem;
  font-weight: 500;
  color: var(--navy);
  margin-bottom: 0.3rem;
}
.fd-role {
  font-size: 0.8rem;
  color: var(--ink-2);
  line-height: 1.5;
}
.fd-tenure {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  margin-top: 0.6rem;
  font-size: 0.72rem;
  letter-spacing: 0.06em;
  color: var(--gold);
  font-weight: 500;
  text-transform: uppercase;
}
.fd-tenure::before {
  content: '';
  display: inline-block;
  width: 14px; height: 1px;
  background: var(--gold);
}
/* ── TABS ── */
.tabs {
  display: flex;
  gap: 4px;
  margin-bottom: 2rem;
  border-bottom: 1px solid var(--border);
  padding-bottom: 0;
}
.tab {
  padding: 0.55rem 1.2rem 0.65rem;
  font-size: 0.82rem;
  font-weight: 400;
  letter-spacing: 0.02em;
  border: none;
  background: none;
  color: var(--ink-3);
  cursor: pointer;
  position: relative;
  transition: color 0.15s;
  text-decoration: none;
  display: inline-block;
  margin-bottom: -1px;
  border-bottom: 2px solid transparent;
}
.tab:hover { color: var(--navy); }
.tab.active {
  color: var(--navy);
  font-weight: 500;
  border-bottom: 2px solid var(--navy);
}
/* ── MEMBER GRID ── */
.member-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
  gap: 16px;
}
.member-card {
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: var(--r);
  padding: 1.4rem;
  transition: box-shadow 0.2s, transform 0.2s;
  position: relative;
}
.member-card:hover {
  box-shadow: 0 6px 24px rgba(13,31,60,0.08);
  transform: translateY(-2px);
}
.member-card.hidden { display: none; }
.card-photo {
  width: 58px; height: 58px;
  border-radius: 7px;
  overflow: hidden;
  background: var(--gold-3);
  display: flex; align-items: center; justify-content: center;
  font-family: 'EB Garamond', serif;
  font-size: 1.1rem;
  color: var(--navy-2);
  margin-bottom: 1rem;
  transition: border-radius 0.2s;
}
.member-card:hover .card-photo { border-radius: 12px; }
.card-photo img {
  width: 100%; height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}
.member-card:hover .card-photo img { transform: scale(1.08); }
.card-name {
  font-family: 'EB Garamond', serif;
  font-size: 1.05rem;
  font-weight: 500;
  color: var(--navy);
  line-height: 1.3;
  margin-bottom: 0.5rem;
}
.card-name a { color: inherit; text-decoration: none; }
.card-name a:hover { color: var(--navy-3); }
.card-name.alumni { color: var(--navy-3); }
.card-divider {
  height: 1px;
  background: var(--border);
  margin: 0.85rem 0;
}
.card-role {
  font-size: 0.77rem;
  color: var(--ink-2);
  line-height: 1.5;
}
.card-years {
  font-size: 0.72rem;
  color: var(--ink-3);
  margin-top: 0.25rem;
  letter-spacing: 0.03em;
}
.card-now {
  font-size: 0.74rem;
  color: var(--navy-3);
  margin-top: 0.45rem;
  font-style: italic;
}
/* Open position card */
.member-card.open {
  border-style: dashed;
  border-color: var(--gold-2);
  background: #fdf9f0;
}
.member-card.open .card-photo {
  background: var(--gold-3);
  color: var(--gold);
  font-size: 1.5rem;
  font-weight: 300;
}
.member-card.open .card-name { color: var(--gold); }
.member-card.open .card-role { color: var(--ink-2); }
.open-badge {
  position: absolute;
  top: 1rem; right: 1rem;
  font-size: 0.62rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--gold);
  background: var(--gold-3);
  padding: 2px 8px;
  border-radius: 20px;
  font-weight: 500;
}
/* ── COLLABORATORS ── */
.collab-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(310px, 1fr));
  gap: 10px;
}
.collab-card {
  background: var(--white);
  border: 1px solid var(--border);
  border-left: 3px solid var(--navy-3);
  border-radius: 0 var(--r) var(--r) 0;
  padding: 0.9rem 1.1rem;
  transition: border-left-color 0.2s;
}
.collab-card:hover { border-left-color: var(--gold); }
.collab-name {
  font-family: 'EB Garamond', serif;
  font-size: 1rem;
  font-weight: 500;
  color: var(--navy);
}
.collab-inst {
  font-size: 0.74rem;
  color: var(--ink-3);
  margin-top: 0.25rem;
  line-height: 1.5;
}
/* ── RESPONSIVE ── */
@media (max-width: 640px) {
  .page { padding: 2.5rem 1.25rem 4rem; }
  .fd-card { flex-direction: column; align-items: flex-start; gap: 1.25rem; padding: 1.5rem; }
}
/* ── ANIMATIONS ── */
@keyframes fadeUp {
  from { opacity: 0; transform: translateY(16px); }
  to   { opacity: 1; transform: translateY(0); }
}
.member-card, .collab-card, .fd-card {
  animation: fadeUp 0.4s ease both;
}
.member-card:nth-child(1)  { animation-delay: 0.05s; }
.member-card:nth-child(2)  { animation-delay: 0.10s; }
.member-card:nth-child(3)  { animation-delay: 0.15s; }
.member-card:nth-child(4)  { animation-delay: 0.20s; }
.member-card:nth-child(5)  { animation-delay: 0.25s; }
.member-card:nth-child(6)  { animation-delay: 0.30s; }
.member-card:nth-child(7)  { animation-delay: 0.35s; }
.member-card:nth-child(8)  { animation-delay: 0.40s; }
.member-card:nth-child(9)  { animation-delay: 0.45s; }
.member-card:nth-child(10) { animation-delay: 0.50s; }
</style>
 
<div class="page">
 
 
  <!-- FOUNDING DIRECTOR -->
  <section>
    <div class="sec-header">
      <span class="sec-label">Founding Director</span>
      <div class="sec-line"></div>
    </div>
    <div class="fd-card">
      <div class="fd-photo-wrap">
        <img src="https://cibs-imhans.github.io/assets/headshots/kk.JPG"
             onerror="this.style.display='none'; this.parentNode.textContent='KP';"
             alt="Krishnakumar Padinharath">
      </div>
      <div class="fd-info">
        <p class="fd-name">Krishnakumar Padinharath</p>
        <p class="fd-role">Founding Director, Centre for Interdisciplinary Brain Sciences<br>IMHANS, Kozhikode</p>
        <p class="fd-tenure">2022 – 2025</p>
      </div>
    </div>
  </section>
  <!-- TEAM MEMBERS -->
  <section>
    <div class="sec-header">
      <span class="sec-label">Research Team</span>
      <div class="sec-line"></div>
    </div>
    <div class="tabs">
      <button class="tab active" onclick="filter('current', this)">Current Members</button>
      <button class="tab" onclick="filter('alumni', this)">Alumni</button>
      <a class="tab" href="https://cibs-imhans.github.io/alum/" target="_blank">Interns ↗</a>
    </div>
 
    <div class="member-grid">
 
      <!-- Current -->
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/shabeesh.jpeg"
               onerror="this.style.display='none'; this.parentNode.textContent='SB';" alt="Shabeesh Balan">
        </div>
        <p class="card-name"><a href="https://linktr.ee/shabeeshbalan">Shabeesh Balan</a></p>
        <div class="card-divider"></div>
        <p class="card-role">Principal Investigator</p>
        <p class="card-years">Scientist D (DHR-NRI Faculty Fellow)</p>
        <p class="card-years">CIBS-IMHANS</p>
      </div>
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/rajith.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='RR';" alt="Rajith Ravindren">
        </div>
        <p class="card-name"><a href="https://scholar.google.com/citations?hl=en&user=4J0rrcEAAAAJ">Rajith Ravindren</a></p>
        <div class="card-divider"></div>
        <p class="card-role">Principal Investigator</p>
        <p class="card-years">Assistant Professor, Department of Psychiatry, IMHANS</p>
      </div>
 
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/aisha.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='AS';" alt="Aisha Shaju">
        </div>
        <p class="card-name">Aisha Shaju</p>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (ANRF)</p>
        <p class="card-years">Molecular Psychiatry</p>
      </div>
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/jasmine.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='JJ';" alt="Jasmine John">
        </div>
        <p class="card-name">Jasmine John</p>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (ANRF)</p>
        <p class="card-years">Molecular Psychiatry</p>
      </div>
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/ranjitha.jpeg"
               onerror="this.style.display='none'; this.parentNode.textContent='RM';" alt="Ranjitha M">
        </div>
        <p class="card-name">Ranjitha M</p>
        <div class="card-divider"></div>
        <p class="card-role">Research Technician</p>
        <p class="card-years">Cytogenetics</p>
      </div>
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/najiya.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='FN';" alt="Fathimath Najiya">
        </div>
        <p class="card-name">Fathimath Najiya</p>
        <div class="card-divider"></div>
        <p class="card-role">Technical Assistant</p>
        <p class="card-years">Electrophysiology</p>
      </div>
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/MIdhun.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='MS';" alt="Midhun Sidharthan">
        </div>
        <p class="card-name">Midhun Sidharthan</p>
        <div class="card-divider"></div>
        <p class="card-role">Visiting Researcher</p>
        <p class="card-years">Assistant Professor, Department of Psychiatry, Government Medical College Kozhikode</p>
      </div>
 
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/nishanth.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='NJ';" alt="Nishanth JH">
        </div>
        <p class="card-name">Nishanth JH</p>
        <div class="card-divider"></div>
        <p class="card-role">Visiting Researcher</p>
        <p class="card-years">Assistant Professor, Department of Psychiatry, Government Medical College Kozhikode</p>
      </div>
 
      <div class="member-card open" data-type="current">
        <div class="open-badge">Hiring</div>
        <div class="card-photo">+</div>
        <p class="card-name">Open Position</p>
        <div class="card-divider"></div>
        <p class="card-role">Research Fellow (DHR Project)</p>
      </div>
 
      <div class="member-card open" data-type="current">
        <div class="open-badge">Hiring</div>
        <div class="card-photo">+</div>
        <p class="card-name">Open Position</p>
        <div class="card-divider"></div>
        <p class="card-role">Project Fellow (SERB-SURE Project)</p>
      </div>
 
      <!-- Alumni -->
 
      <div class="member-card hidden" data-type="alumni">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/anu.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='AK';" alt="Anusree A Kumar">
        </div>
        <p class="card-name alumni">Anusree A Kumar</p>
        <div class="card-divider"></div>
        <p class="card-role">Project Fellow (KSCSTE)</p>
        <p class="card-years">2023 – 2026</p>
        <p class="card-now">→ PhD, Tohoku University, Japan</p>
      </div>
 
      <div class="member-card hidden" data-type="alumni">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/shilpa.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='SO';" alt="Shilpa O">
        </div>
        <p class="card-name alumni">Shilpa O</p>
        <div class="card-divider"></div>
        <p class="card-role">Visiting Researcher (Post-Doctoral Researcher)</p>
        <p class="card-years">2023 – 2025</p>
        <p class="card-now">→ Assistant Professor, Nitte University</p>
      </div>
 
      <div class="member-card hidden" data-type="alumni">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/varun_tk.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='VT';" alt="Varun T K">
        </div>
        <p class="card-name alumni">Varun T K</p>
        <div class="card-divider"></div>
        <p class="card-role">Project Fellow (SERB-SURE)</p>
        <p class="card-years">2024 – 2025</p>
        <p class="card-now">→ Data Scientist, Yenepoya University</p>
      </div>
 
      <div class="member-card hidden" data-type="alumni">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/shibila.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='SA';" alt="Shibila A M">
        </div>
        <p class="card-name alumni">Shibila A M</p>
        <div class="card-divider"></div>
        <p class="card-role">Technical Assistant (Electrophysiology)</p>
        <p class="card-years">2019 – 2025</p>
        <p class="card-now">→ Electrophysiologist, Dubai</p>
      </div>
 
      <div class="member-card hidden" data-type="alumni">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/niketha.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='NM';" alt="Niketha Manoj">
        </div>
        <p class="card-name alumni">Niketha Manoj</p>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (ANRF)</p>
        <p class="card-years">2023 – 2024</p>
        <p class="card-now">→ PhD, NIT Calicut</p>
      </div>
 
      <div class="member-card hidden" data-type="alumni">
        <div class="card-photo">
          <img src="https://cibs-imhans.github.io/assets/headshots/mubashira.jpg"
               onerror="this.style.display='none'; this.parentNode.textContent='MV';" alt="Mubashira V">
        </div>
        <p class="card-name alumni">Mubashira V</p>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (DHR)</p>
        <p class="card-years">2022 – 2024</p>
        <p class="card-now">→ UAE</p>
      </div>
 
    </div>
  </section>
  <!-- COLLABORATORS -->
  <section>
    <div class="sec-header">
      <span class="sec-label">Collaborators</span>
      <div class="sec-line"></div>
    </div>
    <div class="collab-grid">
      <div class="collab-card">
        <p class="collab-name">Dr Dileep Vijayan</p>
        <p class="collab-inst">Laboratory for Computational and Structural Biology, Jubilee Mission Medical College Hospital &amp; Research Institute, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Neetha Balaram</p>
        <p class="collab-inst">Department of Neurology, Government Medical College Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Divya MS</p>
        <p class="collab-inst">Department of Pathology, Sree Chitra Tirunal Institute for Medical Sciences and Technology, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Sreejith PS</p>
        <p class="collab-inst">Multidisciplinary Research Unit (MRU), Government Medical College, Thiruvananthapuram, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Lijiya A</p>
        <p class="collab-inst">Department of Computer Science and Engineering, NIT Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Arun Kumar Gangadharan</p>
        <p class="collab-inst">Department of Molecular Biology, Kannur University, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Sanish Sathyan</p>
        <p class="collab-inst">Department of Molecular Biology, Kannur University, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Joe Cherri Ross</p>
        <p class="collab-inst">Department of Computer Science and Engineering, NIT Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Varsha Vidyadharan</p>
        <p class="collab-inst">Department of Psychiatry, Government Medical College Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Dhanasooraj Dhanjayan</p>
        <p class="collab-inst">Multidisciplinary Research Unit, Government Medical College, Kozhikode, Kerala</p>
      </div>
      <div class="collab-card">
        <p class="collab-name">Dr Geetha Govindraj</p>
        <p class="collab-inst">Director Professor of Pediatrics, Government Medical College, Kozhikode; Professor, School of Family Health Studies, Kerala University of Health Sciences, Kerala, India</p>
      </div>
    </div>
  </section>
</div>
<script>
  function filter(type, btn) {
    document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
    btn.classList.add('active');
    document.querySelectorAll('.member-card').forEach(card => {
      card.classList.toggle('hidden', card.dataset.type !== type);
    });
  }
</script>
























<!--- {% include lab_member_gallery.html%} -->
<!--- {% include lab_alum_gallery.html%} -->

