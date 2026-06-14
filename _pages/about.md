---
layout: about
title: about
permalink: /
social: false
selected_papers: false

announcements:
  enabled: false

latest_posts:
  enabled: false
---

<div id="alex-home">

<div id="topbar" class="topbar">
  <div class="topbar-inner">
    <nav class="navlinks">
      <a href="#bio">Bio</a>
      <a href="#vitae">Vitæ</a>
      <button type="button" class="theme-toggle" title="Change theme" aria-label="Change color theme">
        <i class="fa-half-sun-moon toggle-system"></i>
        <i class="fa-solid fa-moon toggle-dark"></i>
        <i class="fa-solid fa-sun toggle-light"></i>
      </button>
    </nav>
  </div>
</div>

<header id="top" class="hero">
  <img class="hero-photo" src="/assets/img/profile_pic.jpeg" alt="Alex Evans">
  <div class="hero-body">
    <h1 class="hero-name">Alex Evans</h1>
    <p class="hero-tagline">DPhil candidate in Materials, University of Oxford</p>
    <div class="hero-socials">
      <a href="mailto:alexander.evans@reuben.ox.ac.uk" aria-label="Email"><i class="fa-solid fa-envelope"></i></a>
      <a href="https://github.com/alexxevans" target="_blank" rel="noopener" aria-label="GitHub"><i class="fa-brands fa-github"></i></a>
      <a href="https://www.linkedin.com/in/alex-evans-84b1881a5/" target="_blank" rel="noopener" aria-label="LinkedIn"><i class="fa-brands fa-linkedin"></i></a>
    </div>
  </div>
</header>

<section id="bio" class="home-section">
  <h2>Bio</h2>
  <p>I'm a DPhil candidate in Materials at the <strong>University of Oxford</strong>, where my research explores projection and energy-guided sampling for the <em>de novo</em> design of virus-like particles.</p>
  <p>My work sits at the intersection of <strong>generative AI and the physical sciences</strong> — applying diffusion models, normalising flows, and Bayesian inference to problems in physics, metrology, and structural design. Previously I completed an <strong>MRes in Machine Learning in the Physical Sciences</strong> (Distinction) at <strong>Imperial College London</strong>, modelling the quantum apparatus used in dark-matter and gravitational-wave research, and worked as a <strong>Scientist at the National Physical Laboratory (NPL)</strong>, where I built generative models to calibrate a European Space Agency satellite for the TRUTHS climate mission.</p>
  <p>I was a <strong>STEM for Britain 2025 finalist</strong>, presenting my research at the UK Parliament.</p>
</section>

<section id="vitae" class="home-section">
  <h2>Vitæ</h2>
  <p class="cv-download"><a href="/assets/pdf/Alex_Evans_CV.pdf" target="_blank" rel="noopener"><i class="fa-solid fa-download"></i> Download full CV (PDF)</a></p>
  <div class="timeline">
    <div class="timeline-item">
      <div class="timeline-content">
        <div class="timeline-date">2025 — Present</div>
        <div class="timeline-title">University of Oxford</div>
        <div class="timeline-detail">DPhil in Materials · De Novo Protein Design</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-content">
        <div class="timeline-date">2024 — 2025</div>
        <div class="timeline-title">National Physical Laboratory</div>
        <div class="timeline-detail">Scientist · Data Science Division</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-content">
        <div class="timeline-date">2023 — 2024</div>
        <div class="timeline-title">Imperial College London</div>
        <div class="timeline-detail">MRes Machine Learning &amp; Big Data in the Physical Sciences · Distinction</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-content">
        <div class="timeline-date">2021 — 2024</div>
        <div class="timeline-title">National Physical Laboratory</div>
        <div class="timeline-detail">Data Analyst</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-content">
        <div class="timeline-date">2018 — 2019</div>
        <div class="timeline-title">University of Melbourne</div>
        <div class="timeline-detail">BEng Mechanical Engineering · Exchange Year</div>
      </div>
    </div>
    <div class="timeline-item">
      <div class="timeline-content">
        <div class="timeline-date">2016 — 2020</div>
        <div class="timeline-title">University of Birmingham</div>
        <div class="timeline-detail">BEng Mechanical Engineering · Upper 2:1</div>
      </div>
    </div>
  </div>
</section>

</div>

<script>
  (function () {
    var bar = document.getElementById("topbar");
    if (!bar) return;
    var docEl = document.documentElement;

    function setScrollbarWidth() {
      var sbw = window.innerWidth - docEl.clientWidth;
      docEl.style.setProperty("--scrollbar-width", sbw + "px");
    }

    function onScroll() {
      var max = docEl.scrollHeight - docEl.clientHeight;
      var pct = max > 0 ? (docEl.scrollTop / max) * 100 : 0;
      bar.style.setProperty("--scroll-progress", pct + "%");
    }

    setScrollbarWidth();
    onScroll();
    window.addEventListener("scroll", onScroll, { passive: true });
    window.addEventListener("resize", function () {
      setScrollbarWidth();
      onScroll();
    });

    // Wire both theme toggles (hero + top bar) to al-folio's theme cycle (theme.js).
    if (typeof toggleThemeSetting === "function") {
      document.querySelectorAll("#alex-home .theme-toggle").forEach(function (btn) {
        btn.addEventListener("click", toggleThemeSetting);
      });
    }
  })();
</script>
