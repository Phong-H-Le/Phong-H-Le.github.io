---
layout: default
title: Home
---

<link rel="stylesheet" href="/assets/css/home.css">

<div class="hero-section">
  <div class="hero-content">
    <h2 class="section-title">About Me</h2>
    <p>
      Hey! 👋 I'm <strong>Phong Le</strong>. I'm a first generation college student at Duke University. Son of immigrant parents & raised in Myrtle Beach, SC.
    </p>
    <p>
      I enjoy breaking down complex systems into clear, simple blocks. Hobbies include reading classics & theology, going to the gym, and cooking. 
    </p>
  </div>
  <div class="hero-image-container">
    <img src="/assets/images/background_headshot.png" alt="Phong Le" class="hero-image">
  </div>
</div>

<div class="focus-section">
  <h1 class="education-heading">Duke University: Biomedical Engineering & Computer Science</h1>
  <h2>Current Focus & Future Goals</h2>
  <p>
    I'm actively seeking full-time opportunities and internships in medical device development, imaging technology, and applied machine learning. Experience includes applied ML/hardware projects and research in data analysis, policy, & computational modeling. 
  </p>
  <p>
    I'm actively seeking full-time opportunities and internships in medical device development, imaging technology, and applied machine learning. Experience includes applied ML/hardware projects and research in data analysis, policy, & computational modeling. 
  </p>
  <p>
    Looking ahead, I'm passionate about building technologies that can impact <strong>healthcare</strong>, <strong>defense</strong>, and <strong>public systems</strong>. I love leveraging new research to make end-to-end projects.
  </p>
</div>

<div class="resources-section">
  <h2>Resources</h2>
  <div class="resources-grid">
    <a href="/projects/" class="resource-card">
      <img src="/assets/images/resources/projects.jpg" alt="Projects preview" class="resource-card-image">
      <div class="resource-card-content">
        <h3>Projects</h3>
        <p>View my portfolio</p>
      </div>
    </a>
    <a href="https://www.linkedin.com/in/phong-h-le/" target="_blank" class="resource-card">
      <img src="/assets/images/resources/linkedin.jpg" alt="LinkedIn profile preview" class="resource-card-image">
      <div class="resource-card-content">
        <h3>LinkedIn</h3>
        <p>Connect with me</p>
      </div>
    </a>
    <a href="/assets/Resume.pdf" download class="resource-card">
      <img src="/assets/images/resources/resume.png" alt="Resume preview" class="resource-card-image">
      <div class="resource-card-content">
        <h3>Resume</h3>
        <p>Download PDF</p>
      </div>
    </a>
    <a href="https://medium.com/@ryoku_wave" target="_blank" class="resource-card">
      <img src="/assets/images/resources/blog.jpg" alt="Blog preview" class="resource-card-image">
      <div class="resource-card-content">
        <h3>Blog</h3>
        <p>Read my articles</p>
      </div>
    </a>
    <a href="mailto:phl6@duke.edu" class="resource-card">
      <img src="/assets/images/resources/contact.jpg" alt="Contact preview" class="resource-card-image">
      <div class="resource-card-content">
        <h3>Contact</h3>
        <p>phl6@duke.edu</p>
      </div>
    </a>
    <a href="https://www.goodreads.com/user/show/185259908-letsunami" class="resource-card">
      <img src="/assets/images/resources/goodreads.png" alt="Goodreads profile preview" class="resource-card-image">
      <div class="resource-card-content">
        <h3>GoodReads</h3>
        <p>Read my book reviews</p>
      </div>
    </a>
  </div>
</div>

<section class="gallery-section">
  <h2 class="section-title">Gallery</h2>

  <!-- Add or remove <figure class="slide"> blocks — the script is dynamic -->
  <div class="gallery" id="js-gallery" aria-roledescription="carousel" aria-label="Image gallery">
    <figure class="slide">
      <img src="/assets/images/gallery/gal1.jpg" alt="Caption for image 1" loading="lazy">
      <figcaption class="caption">14 y.o. me</figcaption>
    </figure>

    <figure class="slide">
      <img src="/assets/images/gallery/gal2.jpg" alt="Caption for image 2" loading="lazy">
      <figcaption class="caption">City Skyline of Phoenix, AZ</figcaption>
    </figure>

    <figure class="slide">
      <img src="/assets/images/gallery/gal3.jpg" alt="Caption for image 3" loading="lazy">
      <figcaption class="caption">Selfie w/ President of Intervarsity</figcaption>
    </figure>

    <figure class="slide">
      <img src="/assets/images/gallery/gal4.jpg" alt="Caption for image 4" loading="lazy">
      <figcaption class="caption">Selfie w/ Influencer @aarondrizzy_</figcaption>
    </figure>

    <figure class="slide">
      <img src="/assets/images/gallery/gal5.jpg" alt="Caption for image 5" loading="lazy">
      <figcaption class="caption">CIEMAS @ Duke University</figcaption>
    </figure>

    <figure class="slide">
      <img src="/assets/images/gallery/gal6.jpg" alt="Caption for image 6" loading="lazy">
      <figcaption class="caption">Selfie w/ YouTuber Josh Starmer (StatQuest)</figcaption>
    </figure>

    <figure class="slide">
      <img src="/assets/images/gallery/gal7.jpg" alt="Caption for image 7" loading="lazy">
      <figcaption class="caption">Snowman in a Snowday</figcaption>
    </figure>
  </div>

  <!-- dots will be injected here by JS -->
  <div class="gallery-dots" id="js-dots" aria-hidden="false"></div>
</section>

<!-- Inline script (minimal, unobtrusive) -->
<script>
(function () {
  const gallery = document.getElementById('js-gallery');
  if (!gallery) return;

  const slides = Array.from(gallery.querySelectorAll('.slide'));
  const dotsContainer = document.getElementById('js-dots');
  if (!slides.length) return;

  let active = Math.floor(slides.length / 2); // start centered (middle)
  const spacing = Math.max(140, Math.round(window.innerWidth / 7)); // responsive gap
  const maxVisibleDistance = 3; // how many neighbors to reasonably show

  // make slides focusable and set ARIA roles
  slides.forEach((s, i) => {
    s.setAttribute('role', 'group');
    s.setAttribute('aria-roledescription', 'slide');
    s.setAttribute('aria-label', (i+1) + ' of ' + slides.length);
    s.tabIndex = 0;
  });

  // create dots
  function buildDots() {
    dotsContainer.innerHTML = '';
    dotsContainer.setAttribute('role', 'tablist');
    slides.forEach((_, i) => {
      const btn = document.createElement('button');
      btn.className = 'dot';
      btn.type = 'button';
      btn.setAttribute('aria-label', 'Show image ' + (i+1));
      btn.addEventListener('click', () => { goTo(i); });
      dotsContainer.appendChild(btn);
    });
  }

  // apply transforms based on active index
  function layout() {
    slides.forEach((slide, i) => {
      const d = i - active;
      const abs = Math.abs(d);

      // calculate translate based on distance and screen-size scaling
      const offset = d * spacing;
      let scale = 1 - 0.12 * Math.min(abs, maxVisibleDistance);
      let opacity = 1 - 0.2 * Math.min(abs, maxVisibleDistance);
      let z = 100 - abs;

      // very far slides get a little smaller/less opaque but still visible
      if (abs >= maxVisibleDistance) {
        scale = 0.62;
        opacity = 0.4;
        z = 10;
      }

      // compute final transform (centered point is translate(-50%,-50%), we move from center)
      slide.style.transform = `translate(calc(-50% + ${offset}px), -50%) scale(${scale})`;
      slide.style.zIndex = z;
      slide.style.opacity = opacity;
      // show caption on active
      const caption = slide.querySelector('.caption');
      if (caption) caption.style.opacity = (abs === 0 ? '1' : '0');
    });

    // update dots active class
    const dots = Array.from(dotsContainer.children);
    dots.forEach((d, i) => d.classList.toggle('active', i === active));
  }

  function goTo(i) {
    active = Math.max(0, Math.min(slides.length - 1, i));
    layout();
    // move focus to current slide for better keyboard/a11y
    const s = slides[active];
    if (s && typeof s.focus === 'function') s.focus();
  }

  // next/prev helpers
  function next() { goTo(active + 1 === slides.length ? slides.length - 1 : active + 1); }
  function prev() { goTo(active - 1 < 0 ? 0 : active - 1); }

  // click on slide sets it active
  slides.forEach((s, i) => s.addEventListener('click', () => goTo(i)));

  // keyboard navigation
  document.addEventListener('keydown', (ev) => {
    if (ev.key === 'ArrowRight') { next(); ev.preventDefault(); }
    if (ev.key === 'ArrowLeft')  { prev(); ev.preventDefault(); }
  });

  // recompute spacing on resize
  let resizeTimer;
  window.addEventListener('resize', () => {
    clearTimeout(resizeTimer);
    resizeTimer = setTimeout(() => {
      // recalc spacing
      // prefer at least 110px, responsive to viewport
      const newSpacing = Math.max(110, Math.round(window.innerWidth / 7));
      // mutate closure var by reassigning spacing? it's const — so instead we re-layout using computed offset per active.
      // To keep it simple, just reload page layout by forcing layout with new spacing stored on element dataset
      gallery.dataset.spacing = newSpacing;
      layout();
    }, 120);
  });

  // initial positioning: set container relative center baseline
  // We'll absolutely position slides via CSS; the script just sets transforms.
  // Add CSS necessary classes to slides (done by the page CSS).
  // Build dots and layout
  buildDots();

  // ensure slides are absolutely centered by applying an initial transform origin
  slides.forEach(s => {
    s.style.position = 'absolute';
    s.style.top = '50%';
    s.style.left = '50%';
    s.style.transform = 'translate(-50%, -50%) scale(0.78)';
  });

  // small accessibility: clicking dot moves active slide and announces change
  dotsContainer.addEventListener('click', () => {
    // layout will handle focus/visibility
  });

  // finally layout
  layout();

  // expose small API for dev console if needed
  window._gallery = { goTo, next, prev, slidesCount: slides.length };
})();
</script>
