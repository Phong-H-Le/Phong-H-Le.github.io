---
layout: default
title: Home
---


<link rel="stylesheet" href="/assets/css/home.css">

<!-- Minimal, high-specificity mobile override using an ID -->
<style>
  /* Only applies on narrow screens and uses an ID for higher specificity */
  @media (max-width: 720px) {
    /* Force a column layout so text is above the image */
    #hero {
      display: flex !important;
      flex-direction: column !important;
      align-items: stretch !important;
      gap: 0.75rem;
      padding: 0.75rem 1rem !important;
      width: 100% !important;
      box-sizing: border-box !important;
    }

    /* Ensure the text uses full width and wraps normally */
    #hero .hero-content {
      order: 1 !important;
      width: 100% !important;
      max-width: 100% !important;
      min-width: 0 !important;
      text-align: left !important;
      display: block !important;
      float: none !important;
    }

    #hero .hero-content p {
      white-space: normal !important;
      word-break: break-word !important;
      hyphens: auto !important;
      margin-bottom: 0.9rem !important;
      font-size: 1rem !important;
      line-height: 1.6 !important;
    }

    /* Put the image below the text and center it */
    #hero .hero-image-container {
      order: 2 !important;
      width: 100% !important;
      display: flex !important;
      justify-content: center !important;
      margin-top: 0.6rem !important;
      float: none !important;
    }

    #hero .hero-image {
      max-width: 260px !important;
      width: 70% !important;
      height: auto !important;
      display: block !important;
      margin: 0 auto !important;
      box-shadow: 0 8px 30px rgba(0,0,0,0.12) !important;
    }
  }
</style>

<div id="hero" class="hero-section">
  <div class="hero-content">
    <h2 class="section-title">About Me</h2>
    <p>
      Hey! 👋 I'm <strong>Phong Le</strong>. 
    </p>
    <p>
      I'm a first generation college student at Duke University. Son of immigrant parents and raised in Myrtle Beach, SC.
    </p>
    <p>
      Hobbies include reading classics & theology, going to the gym, and cooking. 
    </p>
  </div>
  <div class="hero-image-container">
    <img src="/assets/images/background_headshot.png" alt="Phong Le" class="hero-image">
  </div>
</div>

<div class="focus-section">
  <h1 class="education-heading">Duke University: Biomedical Engineering & Computer Science</h1>
  <h2>Focus & Future Goals</h2>
    <p>
    What consistently motivates me is understanding how complex systems behave and making them work end to end. Whether I’m working with data, sensors, or models, I enjoy the work to distill the messy & abstract to the tangible. Super frustrating in the process, but it is super satisfying in the end. Always willing to learn or lend a helping hand.
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
