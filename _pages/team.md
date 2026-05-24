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
<!-- Typography Architecture Asset Injection -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=EB+Garamond:ital,wght@0,400;0,500;1,400&display=swap" rel="stylesheet">

<style>
/* ── SCALED NAMESPACED LAYOUT SYSTEM ── */
.team-page {
  max-width: 1100px;
  margin: 0 auto;
  padding: 3.5rem 2rem 6rem;
}

.team-page *, 
.team-page *::before, 
.team-page *::after { 
  box-sizing: border-box; 
}

/* ── INTERFACE COMPONENT TOKENS ── */
.team-page {
  --navy:     #0d1f3c;
  --navy-2:   #1b3a6b;
  --navy-3:   #2d5da1;
  --gold:     #91742a; /* Upgraded for dark AAA WCAG color contrast compliance */
  --gold-2:   #d4ad5a;
  --gold-3:   #f5e6c0;
  --ink:      #1a1a2e;
  --ink-2:    #4a4a6a;
  --ink-3:    #8888aa;
  --surface:  #f7f6f3;
  --white:    #ffffff;
  --border:   #e2dfd8;
  --r:        10px;
}

/* ── GLOBAL CORE SECTIONS ── */
.team-page section { 
  margin-bottom: 4.5rem; 
}

.team-page .sec-header {
  display: flex;
  align-items: baseline;
  gap: 1rem;
  margin-bottom: 2rem;
}

.team-page .sec-label {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.16em;
  text-transform: uppercase;
  color: var(--gold);
  font-weight: 500;
  flex-shrink: 0;
}

.team-page .sec-line {
  flex: 1;
  height: 1px;
  background: var(--border);
}

/* ── PLATFORM FOUNDING CARDS ── */
.team-page .fd-card {
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
.team-page .fd-card:hover { 
  box-shadow: 0 8px 32px rgba(13,31,60,0.1); 
}

.team-page .fd-photo-wrap {
  width: 90px; 
  height: 90px;
  border-radius: 8px;
  overflow: hidden;
  flex-shrink: 0;
  background: var(--gold-3);
  display: flex; 
  align-items: center; 
  justify-content: center;
}

.team-page .fd-photo-wrap img {
  width: 100%; 
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}
.team-page .fd-card:hover .fd-photo-wrap img { 
  transform: scale(1.07); 
}

.team-page .fd-name {
  font-family: 'EB Garamond', serif;
  font-size: 1.3rem;
  font-weight: 500;
  color: var(--navy);
  margin: 0 0 0.3rem 0;
}

.team-page .fd-role {
  font-size: 0.8rem;
  color: var(--ink-2);
  line-height: 1.5;
  margin-bottom: 0.5rem;
}

.team-page .fd-tenure {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  margin-top: 0.6rem;
  font-size: 0.75rem;
  letter-spacing: 0.06em;
  color: var(--gold);
  font-weight: 500;
  text-transform: uppercase;
}
.team-page .fd-tenure::before {
  content: '';
  display: inline-block;
  width: 14px; 
  height: 1px;
  background: var(--gold);
}

/* ── ACCESSIBLE FLEX TABS MENU ── */
.team-page .tabs {
  display: flex;
  flex-wrap: wrap; 
  gap: 4px;
  margin-bottom: 2rem;
  border-bottom: 1px solid var(--border);
  padding-bottom: 0;
}

.team-page .tab {
  padding: 0.55rem 1.2rem 0.65rem;
  font-family: 'DM Sans', sans-serif;
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
.team-page .tab:hover { 
  color: var(--navy); 
}
.team-page .tab.active {
  color: var(--navy);
  font-weight: 500;
  border-bottom: 2px solid var(--navy);
}

/* ── CORE MEMBERS RESPONSIVE GRID ── */
.team-page .member-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
  gap: 16px;
}

.team-page .member-card {
  background: var(--white);
  border: 1px solid var(--border);
  border-radius: var(--r);
  padding: 1.4rem;
  transition: box-shadow 0.2s, transform 0.2s;
  position: relative;
}
.team-page .member-card:hover {
  box-shadow: 0 6px 24px rgba(13,31,60,0.08);
  transform: translateY(-2px);
}
.team-page .member-card.hidden { 
  display: none !important; 
}

.team-page .card-photo {
  width: 58px; 
  height: 58px;
  border-radius: 7px;
  overflow: hidden;
  background: var(--gold-3);
  display: flex; 
  align-items: center; 
  justify-content: center;
  margin-bottom: 1rem;
  transition: border-radius 0.2s;
}
.team-page .member-card:hover .card-photo { 
  border-radius: 12px; 
}

.team-page .card-photo img {
  width: 100%; 
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}
.team-page .member-card:hover .card-photo img { 
  transform: scale(1.08); 
}

/* Isolated Non-Destructive Initial Elements */
.team-page .fallback-initials {
  display: none;
  font-family: 'EB Garamond', serif;
  font-size: 1.15rem;
  color: var(--navy-2);
  font-weight: 500;
}
.team-page .fd-photo-wrap .fallback-initials {
  font-size: 1.5rem;
}

.team-page .card-name {
  font-family: 'EB Garamond', serif;
  font-size: 1.05rem;
  font-weight: 500;
  color: var(--navy);
  line-height: 1.3;
  margin: 0 0 0.5rem 0;
}
.team-page .card-name a { 
  color: inherit; 
  text-decoration: none; 
}
.team-page .card-name a:hover { 
  color: var(--navy-3); 
}
.team-page .card-name.alumni { 
  color: var(--navy-3); 
}

.team-page .card-divider {
  height: 1px;
  background: var(--border);
  margin: 0.85rem 0;
}

.team-page .card-role {
  font-size: 0.8rem;
  color: var(--ink-2);
  line-height: 1.5;
  margin-bottom: 0.25rem;
}

.team-page .card-years {
  font-size: 0.75rem;
  color: var(--ink-3);
  margin-top: 0.25rem;
  letter-spacing: 0.03em;
}

.team-page .card-now {
  font-size: 0.75rem;
  color: var(--navy-3);
  margin-top: 0.45rem;
  font-style: italic;
}

/* Open Pipeline Structuring */
.team-page .member-card.open {
  border-style: dashed;
  border-color: var(--gold-2);
  background: #fdf9f0;
}
.team-page .member-card.open .card-photo {
  background: var(--gold-3);
  color: var(--gold);
}
.team-page .member-card.open .card-photo-plus {
  font-size: 1.5rem;
  font-weight: 300;
  font-family: 'DM Sans', sans-serif;
}
.team-page .member-card.open .card-name { 
  color: var(--gold); 
}
.team-page .open-badge {
  position: absolute;
  top: 1rem; 
  right: 1rem;
  font-size: 0.75rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--gold);
  background: var(--gold-3);
  padding: 2px 8px;
  border-radius: 20px;
  font-weight: 500;
}

/* ── COLLABORATORS GRID INTERACTION ── */
.team-page .collab-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr)); 
  gap: 12px;
}
.team-page .collab-card {
  background: var(--white);
  border: 1px solid var(--border);
  border-left: 3px solid var(--navy-3);
  border-radius: 0 var(--r) var(--r) 0;
  padding: 0.9rem 1.1rem;
  transition: border-left-color 0.2s;
}
.team-page .collab-card:hover { 
  border-left-color: var(--gold); 
}

.team-page .collab-name {
  font-family: 'EB Garamond', serif;
  font-size: 1rem;
  font-weight: 500;
  color: var(--navy);
  margin: 0;
}
.team-page .collab-inst {
  font-size: 0.75rem;
  color: var(--ink-3);
  margin-top: 0.25rem;
  line-height: 1.5;
}

/* ── KEYBOARD FOCUS OUTLINES FOR ACCESSIBILITY ── */
.team-page .tab:focus-visible,
.team-page .card-name a:focus-visible,
.team-page .collab-card:focus-visible {
  outline: 2px solid var(--gold);
  outline-offset: 4px;
  border-radius: 4px;
}

/* ── RESPONSIVE COMPACT LAYOUTS ── */
@media (max-width: 640px) {
  .team-page { padding: 2.5rem 1.25rem 4rem; }
  .team-page .fd-card { flex-direction: column; align-items: flex-start; gap: 1.25rem; padding: 1.5rem; }
}

/* ── HW ACCELERATED STABLE TRANSITIONS ── */
@keyframes teamFadeUp {
  from { opacity: 0; transform: translateY(12px); }
  to   { opacity: 1; transform: translateY(0); }
}
.team-page .member-card, 
.team-page .collab-card, 
.team-page .fd-card {
  animation: teamFadeUp 0.35s cubic-bezier(0.16, 1, 0.3, 1) both;
}

@media (prefers-reduced-motion: reduce) {
  .team-page *,
  .team-page .member-card, 
  .team-page .collab-card, 
  .team-page .fd-card {
    animation: none !important;
    transition: none !important;
  }
}
</style>

<div class="team-page">

  <!-- FOUNDING DIRECTOR -->
  <section aria-labelledby="dir-heading">
    <div class="sec-header">
      <span class="sec-label" id="dir-heading">Founding Director</span>
      <div class="sec-line"></div>
    </div>

    <div class="fd-card">
      <div class="fd-photo-wrap">
        <img src="{{ '/assets/headshots/kk.JPG' | relative_url }}" 
             loading="lazy" 
             decoding="async" 
             alt="Krishnakumar Padinharath" 
             class="team-headshot">
        <span class="fallback-initials" aria-hidden="true">KP</span>
      </div>
      <div class="fd-info">
        <h2 class="fd-name"> Prof (Dr) Krishnakumar Padinharath</h3>
        <p class="fd-role">Founding Director, Centre for Interdisciplinary Brain Sciences<br>IMHANS, Kozhikode</p>
        <p class="fd-tenure">2022 – 2025</p>
      </div>
    </div>
  </section>

  <!-- TEAM MEMBERS -->
  <section aria-labelledby="team-heading">
    <div class="sec-header">
      <span class="sec-label" id="team-heading">Research Team</span>
      <div class="sec-line"></div>
    </div>

    <div class="tabs" role="tablist" aria-label="Filter Team Members">
      <button type="button" class="tab active" role="tab" aria-selected="true" aria-controls="team-grid" id="filter-current">Current Members</button>
      <button type="button" class="tab" role="tab" aria-selected="false" aria-controls="team-grid" id="filter-alumni">Alumni</button>
      <a class="tab" href="https://cibs-imhans.github.io/alum/" target="_blank" rel="noopener noreferrer" role="link">Interns ↗</a>
    </div>

    <div class="member-grid" id="team-grid">

      <!-- Current Members -->
      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/shabeesh.jpeg' | relative_url }}" loading="lazy" decoding="async" alt="Shabeesh Balan" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">SB</span>
        </div>
        <h3 class="card-name"><a href="https://linktr.ee/shabeeshbalan" target="_blank" rel="noopener noreferrer">Shabeesh Balan</a></h3>
        <div class="card-divider"></div>
        <p class="card-role">Principal Investigator</p>
        <p class="card-years">Scientist D (DHR-NRI Faculty Fellow), CIBS-IMHANS</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/rajith.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Rajith Ravindren" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">RR</span>
        </div>
        <h3 class="card-name"><a href="https://scholar.google.com/citations?hl=en&user=4J0rrcEAAAAJ" target="_blank" rel="noopener noreferrer">Rajith Ravindren</a></h3>
        <div class="card-divider"></div>
        <p class="card-role">Principal Investigator</p>
        <p class="card-years">Assistant Professor, Department of Psychiatry, IMHANS</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/aisha.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Aisha Shaju" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">AS</span>
        </div>
        <h3 class="card-name">Aisha Shaju</h3>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (ANRF)</p>
        <p class="card-years">Molecular Psychiatry</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/jasmine.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Jasmine John" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">JJ</span>
        </div>
        <h3 class="card-name">Jasmine John</h3>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (ANRF)</p>
        <p class="card-years">Molecular Psychiatry</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/ranjitha.jpeg' | relative_url }}" loading="lazy" decoding="async" alt="Ranjitha M" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">RM</span>
        </div>
        <h3 class="card-name">Ranjitha M</h3>
        <div class="card-divider"></div>
        <p class="card-role">Research Technician</p>
        <p class="card-years">Cytogenetics</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/najiya.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Fathimath Najiya" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">FN</span>
        </div>
        <h3 class="card-name">Fathimath Najiya</h3>
        <div class="card-divider"></div>
        <p class="card-role">Technical Assistant</p>
        <p class="card-years">Electrophysiology</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/MIdhun.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Midhun Sidharthan" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">MS</span>
        </div>
        <h3 class="card-name">Midhun S</h3>
        <div class="card-divider"></div>
        <p class="card-role">Visiting Researcher</p>
        <p class="card-years">Assistant Professor, Department of Psychiatry, Government Medical College Kozhikode</p>
      </div>

      <div class="member-card" data-type="current">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/nishanth.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Nishanth JH" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">NJ</span>
        </div>
        <h3 class="card-name">Nishanth JH</h3>
        <div class="card-divider"></div>
        <p class="card-role">Visiting Researcher</p>
        <p class="card-years">Assistant Professor, Department of Psychiatry, Government Medical College Kozhikode</p>
      </div>

      <!-- Open Hiring States -->
      <div class="member-card open" data-type="current">
        <div class="open-badge">Hiring</div>
        <div class="card-photo"><span class="card-photo-plus">+</span></div>
        <h3 class="card-name">Open Position</h3>
        <div class="card-divider"></div>
        <p class="card-role">Research Fellow (DHR Project)</p>
      </div>

      <div class="member-card open" data-type="current">
        <div class="open-badge">Hiring</div>
        <div class="card-photo"><span class="card-photo-plus">+</span></div>
        <h3 class="card-name">Open Position</h3>
        <div class="card-divider"></div>
        <p class="card-role">Project Fellow (SERB-SURE Project)</p>
      </div>

      <!-- Alumni Section Elements -->
      <div class="member-card hidden" data-type="alumni" aria-hidden="true">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/anu.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Anusree A Kumar" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">AK</span>
        </div>
        <h3 class="card-name alumni">Anusree A Kumar</h3>
        <div class="card-divider"></div>
        <p class="card-role">Project Fellow (KSCSTE)</p>
        <p class="card-years">2023 – 2026</p>
        <p class="card-now">→ PhD, Tohoku University, Japan</p>
      </div>

      <div class="member-card hidden" data-type="alumni" aria-hidden="true">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/shilpa.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Shilpa O" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">SO</span>
        </div>
        <h3 class="card-name alumni">Shilpa O</h3>
        <div class="card-divider"></div>
        <p class="card-role">Visiting Researcher (Post-Doctoral)</p>
        <p class="card-years">2023 – 2025</p>
        <p class="card-now">→ Assistant Professor, Nitte University</p>
      </div>

      <div class="member-card hidden" data-type="alumni" aria-hidden="true">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/varun.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Varun T K" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">VT</span>
        </div>
        <h3 class="card-name alumni">Varun T K</h3>
        <div class="card-divider"></div>
        <p class="card-role">Project Fellow (SERB-SURE)</p>
        <p class="card-years">2024 – 2025</p>
        <p class="card-now">→ Data Scientist, Yenepoya University</p>
      </div>

      <div class="member-card hidden" data-type="alumni" aria-hidden="true">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/shibila.jpeg' | relative_url }}" loading="lazy" decoding="async" alt="Shibila A M" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">SA</span>
        </div>
        <h3 class="card-name alumni">Shibila A M</h3>
        <div class="card-divider"></div>
        <p class="card-role">Technical Assistant (Electrophysiology)</p>
        <p class="card-years">2019 – 2025</p>
        <p class="card-now">→ Electrophysiologist, Dubai</p>
      </div>

      <div class="member-card hidden" data-type="alumni" aria-hidden="true">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/niketha.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Niketha Manoj" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">NM</span>
        </div>
        <h3 class="card-name alumni">Niketha Manoj</h3>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (ANRF)</p>
        <p class="card-years">2023 – 2024</p>
        <p class="card-now">→ PhD, NIT Calicut</p>
      </div>

      <div class="member-card hidden" data-type="alumni" aria-hidden="true">
        <div class="card-photo">
          <img src="{{ '/assets/headshots/mubashira.jpg' | relative_url }}" loading="lazy" decoding="async" alt="Mubashira V" class="team-headshot">
          <span class="fallback-initials" aria-hidden="true">MV</span>
        </div>
        <h3 class="card-name alumni">Mubashira V</h3>
        <div class="card-divider"></div>
        <p class="card-role">Junior Research Fellow (DHR)</p>
        <p class="card-years">2022 – 2024</p>
        <p class="card-now">→ UAE</p>
      </div>

    </div>
  </section>

  <!-- COLLABORATORS -->
  <section aria-labelledby="collab-heading">
    <div class="sec-header">
      <span class="sec-label" id="collab-heading">Collaborators</span>
      <div class="sec-line"></div>
    </div>

    <div class="collab-grid">
      <div class="collab-card">
        <h3 class="collab-name">Dr Dileep Vijayan</h3>
        <p class="collab-inst">Laboratory for Computational and Structural Biology, Jubilee Mission Medical College Hospital &amp; Research Institute, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Neetha Balaram</h3>
        <p class="collab-inst">Department of Neurology, Government Medical College Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Divya MS</h3>
        <p class="collab-inst">Department of Pathology, Sree Chitra Tirunal Institute for Medical Sciences and Technology, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Sreejith PS</h3>
        <p class="collab-inst">Multidisciplinary Research Unit (MRU), Government Medical College, Thiruvananthapuram, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Lijiya A</h3>
        <p class="collab-inst">Department of Computer Science and Engineering, NIT Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Arun Kumar Gangadharan</h3>
        <p class="collab-inst">Department of Molecular Biology, Kannur University, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Sanish Sathyan</h3>
        <p class="collab-inst">Department of Molecular Biology, Kannur University, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Joe Cherri Ross</h3>
        <p class="collab-inst">Department of Computer Science and Engineering, NIT Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Varsha Vidyadharan</h3>
        <p class="collab-inst">Department of Psychiatry, Government Medical College Calicut, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Dhanasooraj Dhanjayan</h3>
        <p class="collab-inst">Multidisciplinary Research Unit, Government Medical College, Kozhikode, Kerala</p>
      </div>
      <div class="collab-card">
        <h3 class="collab-name">Dr Geetha Govindraj</h3>
        <p class="collab-inst">Director Professor of Pediatrics, Government Medical College, Kozhikode; Professor, School of Family Health Studies, Kerala University of Health Sciences, Kerala, India</p>
      </div>
    </div>
  </section>

</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const tabButtons = document.querySelectorAll('.tabs button[role="tab"]');
    const memberCards = document.querySelectorAll('.member-grid .member-card');

    // ── CENTRALIZED DOM FILTER SYSTEM ──
    function filterMembers(targetType) {
      memberCards.forEach(card => {
        if (card.dataset.type === targetType) {
          card.classList.remove('hidden');
          card.removeAttribute('aria-hidden');
        } else {
          card.classList.add('hidden');
          card.setAttribute('aria-hidden', 'true');
        }
      });
    }

    tabButtons.forEach(button => {
      button.addEventListener('click', function() {
        tabButtons.forEach(btn => {
          btn.classList.remove('active');
          btn.setAttribute('aria-selected', 'false');
        });

        this.classList.add('active');
        this.setAttribute('aria-selected', 'true');

        const filterTarget = this.id === 'filter-current' ? 'current' : 'alumni';
        filterMembers(filterTarget);
      });
    });

    // ── NON-DESTRUCTIVE FALLBACK INITIAL EVENT SYSTEM ──
    const images = document.querySelectorAll('.team-page img.team-headshot');
    images.forEach(img => {
      img.addEventListener('error', function() {
        this.style.display = 'none';
        const fallbackSpan = this.parentNode.querySelector('.fallback-initials');
        if (fallbackSpan) {
          fallbackSpan.style.display = 'flex';
        }
      });
      
      // Dynamic programmatic check for background cached scenarios
      if (img.complete && img.naturalWidth === 0) {
        img.dispatchEvent(new Event('error'));
      }
    });
  });
</script>
