---
layout: home
title: ""
---

<style>
/* ===== FIX OVERLAP BETWEEN HEADER + MAIN PAGE CONTENT ===== */

/* Make sure header is static */
header.site-header {
  position: static;
  z-index: 0;
}

/* Add vertical space between header and page content */
main.page-content {
  padding-top: 3.5rem;
}

/* Nav bar stays horizontal always */
nav.responsive-theme-nav {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 1.2rem;
  margin-top: 0.5rem;
}

/* Link style */
nav.responsive-theme-nav .page-link {
  text-decoration: none;
  color: #444;
  font-weight: 500;
}

/* Title style on mobile */
@media (max-width: 600px) {
  .site-title {
    text-align: center;
    font-size: 1.2rem;
    margin-bottom: 0.2rem;
  }

  nav.responsive-theme-nav {
    flex-direction: row;
    gap: 0.8rem;
    padding-top: 0.5rem;
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
