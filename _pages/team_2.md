---
title: Team
permalink: /team/
layout: splash
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: "https://images.unsplash.com/photo-1494059980473-813e73ee784b?auto=format&fit=crop&w=1769&q=80"
  caption: "[Hans-Peter Gauster](https://unsplash.com/@sloppyperfectionist) on [Unsplash](https://unsplash.com)"
---

{% raw %}

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
.team-wrap * { box-sizing: border-box; }
.team-wrap {
  font-family: 'Inter', sans-serif;
  max-width: 1100px;
  margin: 0 auto;
  padding: 2rem 2rem 5rem;
  --ink:#111827; --ink-2:#4b5563; --ink-3:#9ca3af;
  --white:#fff; --accent:#1e3a6e; --accent-mid:#2563eb;
  --border:#e5e7eb; --radius:14px;
}
.sec-title {
  font-size:1.1rem;font-weight:600;
  border-bottom:1px solid var(--border);
  padding-bottom:0.6rem;margin-bottom:1.25rem;
}
section { margin-bottom:3rem; }
.member-grid {
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(220px,1fr));
  gap:14px;
}
.member-card {
  border:1px solid var(--border);
  border-radius:var(--radius);
  padding:1.1rem;
  background:#fff;
}
.member-card.tm-hidden { display:none; }
.member-card.open {
  background:#f0fdf4;
  border-color:#bbf7d0;
  cursor:pointer;
}
</style>

<div class="team-wrap">

<section>
<p class="sec-title">🏛️ Founding Director</p>
<div class="member-card">
<p><strong>Krishnakumar Padinharath</strong><br>Founding Director (2022–2025)</p>
</div>
</section>

<section>
<p class="sec-title">Team Members</p>

<div>
<button onclick="teamFilter('current',this)">Current</button>
<button onclick="teamFilter('alumni',this)">Alumni</button>
</div>

<div class="member-grid">

<div class="member-card" data-type="current">Shabeesh Balan</div>
<div class="member-card" data-type="current">Rajith Ravindren</div>

<div class="member-card open" data-type="current" onclick="window.location='/join/'">
Open Position
</div>

<div class="member-card tm-hidden" data-type="alumni">
Varun Thachan Kundil
</div>

</div>
</section>

</div>

<script>
function teamFilter(type, btn) {
  document.querySelectorAll('.member-card').forEach(card => {
    card.classList.toggle('tm-hidden', card.dataset.type !== type);
  });
}
</script>

{% endraw %}
