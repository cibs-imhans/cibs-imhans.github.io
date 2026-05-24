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
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=EB+Garamond:wght@400;500;600&display=swap" rel="stylesheet">

<style>
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

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

.team-page {
  max-width: 1100px;
  margin: 0 auto;
  padding: 3.5rem 2rem 6rem;
}

.team-page section {
  margin-bottom: 4.5rem;
}

/* ─────────────────────────────
   SECTION HEADERS
───────────────────────────── */
.sec-header {
  display: flex;
  align-items: baseline;
  gap: 1rem;
  margin-bottom: 2rem;
}

.sec-label {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.75rem;
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

/* ─────────────────────────────
   FOUNDING DIRECTOR
───────────────────────────── */
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
  transition: box-shadow 0.2s ease;
}

.fd-card:hover {
  box-shadow: 0 8px 32px rgba(13,31,60,0.1);
}

.fd-photo-wrap {
  width: 90px;
  height: 90px;
  border-radius: 8px;
  overflow: hidden;
  flex-shrink: 0;
  background: var(--gold-3);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'EB Garamond', serif;
  font-size: 1.5rem;
  color: var(--navy-2);
}

.fd-photo-wrap img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}

.fd-card:hover .fd-photo-wrap img {
  transform: scale(1.07);
}

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
  width: 14px;
  height: 1px;
  background: var(--gold);
}

/* ─────────────────────────────
   TABS
───────────────────────────── */
.tabs {
  display: flex;
  flex-wrap: wrap;
  gap: 4px;
  margin-bottom: 2rem;
  border-bottom: 1px solid var(--border);
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
  transition: color 0.15s ease;
  text-decoration: none;
  display: inline-block;
  margin-bottom: -1px;
  border-bottom: 2px solid transparent;
}

.tab:hover {
  color: var(--navy);
}

.tab.active {
  color: var(--navy);
  font-weight: 500;
  border-bottom: 2px solid var(--navy);
}

.tab:focus-visible,
.card-name a:focus-visible {
  outline: 2px solid var(--gold);
  outline-offset: 2px;
}

/* ─────────────────────────────
   MEMBER GRID
───────────────────────────── */
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
  transition:
    box-shadow 0.2s ease,
    transform 0.2s ease;
  position: relative;
  animation: fadeUp 0.4s ease both;
}

.member-card:hover {
  box-shadow: 0 6px 24px rgba(13,31,60,0.08);
  transform: translateY(-2px);
}

.member-card.hidden {
  display: none;
}

.card-photo {
  width: 58px;
  height: 58px;
  border-radius: 7px;
  overflow: hidden;
  background: var(--gold-3);
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'EB Garamond', serif;
  font-size: 1.1rem;
  color: var(--navy-2);
  margin-bottom: 1rem;
  transition: border-radius 0.2s ease;
}

.member-card:hover .card-photo {
  border-radius: 12px;
}

.card-photo img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease;
}

.member-card:hover .card-photo img {
  transform: scale(1.08);
}

.card-name {
  font-family: 'EB Garamond', serif;
  font-size: 1.05rem;
  font-weight: 500;
  color: var(--navy);
  line-height: 1.3;
  margin-bottom: 0.5rem;
}

.card-name a {
  color: inherit;
  text-decoration: none;
}

.card-name a:hover {
  color: var(--navy-3);
}

.card-name.alumni {
  color: var(--navy-3);
}

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
  font-size: 0.74rem;
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

/* ─────────────────────────────
   OPEN POSITION CARD
───────────────────────────── */
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

.member-card.open .card-name {
  color: var(--gold);
}

.open-badge {
  position: absolute;
  top: 1rem;
  right: 1rem;
  font-size: 0.62rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--gold);
  background: var(--gold-3);
  padding: 2px 8px;
  border-radius: 20px;
  font-weight: 500;
}

/* ─────────────────────────────
   COLLABORATORS
───────────────────────────── */
.collab-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
  gap: 10px;
}

.collab-card {
  background: var(--white);
  border: 1px solid var(--border);
  border-left: 3px solid var(--navy-3);
  border-radius: 0 var(--r) var(--r) 0;
  padding: 0.9rem 1.1rem;
  transition: border-left-color 0.2s ease;
}

.collab-card:hover {
  border-left-color: var(--gold);
}

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

/* ─────────────────────────────
   RESPONSIVE
───────────────────────────── */
@media (max-width: 640px) {
  .team-page {
    padding: 2.5rem 1.25rem 4rem;
  }

  .fd-card {
    flex-direction: column;
    align-items: flex-start;
    gap: 1.25rem;
    padding: 1.5rem;
  }
}

/* ─────────────────────────────
   REDUCED MOTION
───────────────────────────── */
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation: none !important;
    transition: none !important;
    scroll-behavior: auto !important;
  }
}

/* ─────────────────────────────
   ANIMATION
───────────────────────────── */
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(16px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

<div class="team-page">

  <!-- FOUNDING DIRECTOR -->
  <section>

    <div class="sec-header">
      <span class="sec-label">Founding Director</span>
      <div class="sec-line"></div>
    </div>

    <div class="fd-card">

      <div class="fd-photo-wrap">
        <img
          src="{{ '/assets/headshots/kk.JPG' | relative_url }}"
          loading="lazy"
          decoding="async"
          alt="Krishnakumar Padinharath"
          onerror="this.remove(); this.parentNode.innerHTML='KP';">
      </div>

      <div class="fd-info">
        <h2 class="fd-name">Krishnakumar Padinharath</h2>

        <p class="fd-role">
          Founding Director, Centre for Interdisciplinary Brain Sciences<br>
          IMHANS, Kozhikode
        </p>

        <p class="fd-tenure">2022 – 2025</p>
      </div>

    </div>

  </section>

</div>

<script>
document.addEventListener('DOMContentLoaded', () => {

  const tabs = document.querySelectorAll('.tab-btn');
  const cards = document.querySelectorAll('.member-card');

  function filterMembers(type, activeBtn) {

    tabs.forEach(tab => {
      tab.classList.remove('active');
      tab.setAttribute('aria-selected', 'false');
    });

    activeBtn.classList.add('active');
    activeBtn.setAttribute('aria-selected', 'true');

    cards.forEach(card => {

      const show = card.dataset.type === type;

      card.classList.toggle('hidden', !show);
      card.setAttribute('aria-hidden', !show);

    });
  }

  tabs.forEach(tab => {

    tab.addEventListener('click', () => {
      filterMembers(tab.dataset.filter, tab);
    });

  });

});
</script>


