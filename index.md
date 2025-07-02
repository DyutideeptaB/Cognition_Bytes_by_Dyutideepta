---
layout: home
title: ""
---

<style>
/* ✅ Fix layout for the site title and nav */
.header-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding: 0 1rem;
  gap: 0.5rem;
  margin-bottom: 1.5rem;
}

.site-title {
  font-size: 1.8rem;
  margin: 0;
}

.site-title a {
  text-decoration: none;
  color: inherit;
}

/* ✅ Navigation bar */
nav.site-nav {
  display: flex;
  flex-wrap: wrap;
  gap: 1.2rem;
}

nav.site-nav .page-link {
  text-decoration: none;
  color: #444;
  font-weight: 500;
  font-size: 1rem;
}

/* ✅ Responsive layout for mobile */
@media (max-width: 600px) {
  .header-wrapper {
    align-items: flex-start;
  }

  .site-title {
    font-size: 1.3rem;
  }

  nav.site-nav {
    flex-wrap: wrap;
    gap: 0.8rem;
  }

  nav.site-nav .page-link {
    font-size: 0.95rem;
  }
}

/* ✅ Preserve layout of your custom responsive-nav */
.responsive-nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  max-width: 800px;
  margin: 10px auto;
  font-size: 0.95em;
  gap: 8px;
}

.responsive-nav a {
  margin: 6px 10px;
  text-decoration: none;
  color: inherit;
  display: flex;
  align-items: center;
}

.responsive-nav img {
  margin-right: 6px;
}

@media (max-width: 600px) {
  .responsive-nav {
    flex-direction: column;
    align-items: flex-start;
    padding: 0 10px;
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
