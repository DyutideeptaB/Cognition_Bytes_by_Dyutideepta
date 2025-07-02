---
layout: home
title: ""
---

<style>
/* ✅ Default layout: fine on desktop, no changes */
.site-header .wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
}

.responsive-nav img {
  width: 20px !important;
  height: 20px !important;
  margin-right: 6px;
  flex-shrink: 0;
}
  

/* ✅ Fix mobile layout */
@media (max-width: 600px) {
  .site-header .wrapper {
    flex-direction: column;
    align-items: center;
  }

  .site-title {
    text-align: center;
    font-size: 1.4rem;
    margin-bottom: 0.5rem;
  }

  .site-nav {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 0.6rem;
    padding: 0 0 0.5rem 0;
  }

  .site-nav .page-link {
    font-size: 0.95rem;
    text-decoration: none;
  }
}
</style>


## Hi, I'm Dyutideepta! Here is my journey in a nutshell.

🌌 **Data Physicist** working at the intersection of AI, imaging, and innovation.  
🚀 From lunar rille detection and fluid mechanics to health-tech UX and encrypted QR systems.

<div class="responsive-nav">
  <a href="https://www.linkedin.com/in/dyutideepta-banerjee" target="_blank">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/linkedin.svg" alt="LinkedIn">
    LinkedIn
  </a>

  <a href="https://github.com/DyutideeptaB" target="_blank">
    <img src="https://cdn.jsdelivr.net/npm/simple-icons@v9/icons/github.svg" alt="GitHub">
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
