---
layout: home
title: ""
---

<!-- Responsive layout fixes for mobile and desktop -->
<style>
/* Desktop: preserve Minima layout */
.site-header .wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

/* 🛠️ Fix for mobile layout */
@media (max-width: 600px) {
  .site-header .wrapper {
    display: block; /* Stack title and nav naturally */
    text-align: center;
  }

  .site-title {
    font-size: 1.4rem;
    margin-bottom: 1.2rem;
  }

  .site-nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.7rem;
    margin-bottom: 1rem;
  }

  .site-nav .page-link {
    font-size: 0.95rem;
    text-decoration: none;
  }
}

/* 🔗 Custom link section (LinkedIn, GitHub, CV) */
.responsive-nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  max-width: 800px;
  margin: 20px auto;
  font-size: 0.95em;
  padding: 0 1rem;
}

.responsive-nav a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: inherit;
  min-width: 120px;
  justify-content: center;
  margin: 6px 0;
}

.responsive-nav img {
  width: 20px;
  height: 20px;
  margin-right: 6px;
  vertical-align: middle;
  flex-shrink: 0;
}

/* 📱 Mobile: stack links left-aligned with breathing space */
@media (max-width: 600px) {
  .responsive-nav {
    flex-direction: column;
    align-items: flex-start;
    gap: 12px;
    padding-left: 10px;
  }

  .responsive-nav a {
    justify-content: flex-start;
  }
}
</style>

## Hi, I'm Dyutideepta! Here is my journey in a nutshell.

🌌 **Data Physicist** working at the intersection of AI, imaging, and innovation.  
🚀 From lunar rille detection and fluid mechanics to health-tech UX and encrypted QR systems.

<div class="responsive-nav">

  <a href="https://www.linkedin.com/in/dyutideepta-banerjee" target="_blank">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" alt="LinkedIn" width="20" height="20">
    LinkedIn
  </a>

  <a href="https://github.com/DyutideeptaB" target="_blank">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" alt="GitHub" width="20" height="20">
    GitHub
  </a>

  <a href="https://dyutideeptab.github.io/Cognition_Bytes_by_Dyutideepta/assets/DyutideeptaBanerjee_CV.pdf" target="_blank">
    <span style="font-size: 18px;">📄</span>&nbsp;View My CV
  </a>

</div>

---

### 🌟 Selected Projects

- [🛰️ AI for Lunar Sinuous Rilles](./Project/planetary-feature-detection/)  
  Deep learning for planetary feature detection with GUI & spectral imaging

- [🔐 Encrypted QR generator with Decryption algorithm](./Project/qr_generator_algorithms/)  
  Industrial-grade Python toolkit for data tagging & visual security

More coming soon: medical imaging, motion tracking, vision pipelines.
