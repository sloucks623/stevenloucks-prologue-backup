---
layout: default
title: Steven Loucks – Cybersecurity Portfolio
---

<style>
  body {
    background-color: #1d1f21;
    color: #ddd;
  }

  .hero {
    text-align: center;
    margin: 2rem auto;
  }

  .hero h1 {
    font-size: 2.5rem;
    color: #ffffff;
    margin-bottom: 0.25rem;
  }

  .hero p {
    font-size: 1.1rem;
    color: #bbb;
  }

  .section {
    margin: 2rem auto;
    max-width: 900px;
    padding: 1rem;
  }

  .card-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    justify-content: center;
  }

  .card {
    background: #2d2f33;
    padding: 1rem;
    border-radius: 10px;
    flex: 1 1 250px;
    text-align: center;
    border: 1px solid #444;
    box-shadow: 0 2px 6px rgba(0,0,0,0.2);
  }

  .card h3 {
    color: #fff;
    margin: 0.5rem 0;
  }

  .button {
    display: inline-block;
    margin-top: 0.5rem;
    padding: 0.5rem 1rem;
    background: #007acc;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: background 0.2s ease-in-out;
  }

  .button:hover {
    background: #005fa3;
  }

  footer {
    margin-top: 3rem;
    padding: 1rem;
    text-align: center;
    font-size: 0.9rem;
    color: #888;
  }

  .toggle-wrapper {
    text-align: center;
    margin-bottom: 2rem;
  }

  #comptia-cert-grid,
  #isc2-cert-grid {
    display: none;
    margin-top: 2rem;
    transition: all 0.3s ease-in-out;
  }

  #comptia-cert-grid.show,
  #isc2-cert-grid.show {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1.5rem;
  }
</style>

<div class="hero">
  <h1>Steven Loucks</h1>
  <p>Cybersecurity Student | Cloud Enthusiast | Lab Builder</p>
  <p style="text-align: center; font-size: 1.1rem; color: #ccc;">
    I’m a U.S. Navy veteran and Cybersecurity student at WGU, building hands-on labs and professional skills for a career in cyber defense and cloud security.
  </p>
</div>

<nav style="text-align: center; margin: 2rem 0;">
  <a href="#certs" style="margin-right: 1rem;">Certifications</a>
  <a href="#labs" style="margin-right: 1rem;">Labs</a>
  <a href="#contact">Contact</a>
</nav>

<div class="section" id="about">
  <h2>My Journey into Cybersecurity</h2>
  <p>
    After more than two decades operating tower cranes on high-risk job sites, managing Domino’s Pizza stores, and owning a luxury auto transport company, I began a strategic career transition into cybersecurity. I bring with me a mindset built on safety, accountability, and problem-solving under pressure—traits I now apply to digital defense and automation.
  </p>
  <p>
    I’m currently pursuing a Bachelor of Science in Cybersecurity and Information Assurance at Western Governors University (WGU), with a hands-on approach to building, testing, and documenting my own home labs.
  </p>
</div>

<div class="section" id="why-cyber">
  <h2>Why Cybersecurity Now?</h2>
  <p>
    Cybersecurity isn’t just a career shift for me—it’s a natural evolution. I’ve spent over 20 years solving high-stakes problems, leading teams, and securing physical systems. Now, I apply that same mindset to protecting digital ones.
  </p>
</div>

<!-- FEATURED COMPTIA TOGGLE SECTION -->
<div class="section toggle-wrapper" id="comptia-featured">
  <h2>CompTIA Certifications (Core + Stackables)</h2>
  <p style="color: #ccc; font-size: 1.05rem;">A growing collection of industry-recognized credentials in hardware, networking, security, and support.</p>

  <img src="/assets/icons/comptia-neutral.png"
       alt="CompTIA"
       style="height: 120px; margin-top: 1rem; cursor: pointer;"
       onclick="toggleComptiaGrid()" />

  <div id="comptia-cert-grid">
    <a href="https://www.credly.com/badges/b131130a-1f81-4d02-891d-f7e772d02c3d/public_url" target="_blank">
      <img src="/assets/icons/comptia-a-plus.png" alt="CompTIA A+" style="height: 80px;" />
    </a>
    <a href="https://www.credly.com/badges/d8cd5829-4fda-407f-b1ac-f8cad9eacd8e/public_url" target="_blank">
      <img src="/assets/icons/comptia-network-plus.png" alt="CompTIA Network+" style="height: 80px;" />
    </a>
    <a href="https://www.credly.com/badges/bfd3f1d4-239e-4ee4-a5db-327cfd884f82/public_url" target="_blank">
      <img src="/assets/icons/comptia-security-plus.png" alt="CompTIA Security+" style="height: 80px;" />
    </a>
    <a href="https://www.credly.com/badges/b286fc02-58d9-41ad-8caa-0687e67fd53d/public_url" target="_blank">
      <img src="/assets/icons/comptia-cios.png" alt="CompTIA CIOS" style="height: 80px;" />
    </a>
    <a href="https://www.credly.com/badges/796b7e03-c9f8-41f0-a4f6-a30bd534a5a3/public_url" target="_blank">
      <img src="/assets/icons/comptia-csis.png" alt="CompTIA CSIS" style="height: 80px;" />
    </a>
  </div>
</div>

<!-- FEATURED ISC² TOGGLE SECTION -->
<div class="section toggle-wrapper" id="isc2-featured">
  <h2>ISC² Certifications</h2>
  <p style="color: #ccc; font-size: 1.05rem;">
    Entry-level and advanced credentials for cybersecurity professionals from ISC².
  </p>

  <img src="/assets/icons/isc2-neutral.png"
       alt="ISC² Certifications"
       style="height: 100px; margin-top: 1rem; cursor: pointer;"
       onclick="toggleIsc2Grid()" />

  <div id="isc2-cert-grid">
    <a href="https://www.credly.com/badges/1cfbbf3f-ec91-4c17-90e0-41089a41c8bb/public_url" target="_blank" title="Certified in Cybersecurity (CC)">
      <img src="/assets/icons/isc2-cc.png" alt="ISC² Certified in Cybersecurity (CC)" style="height: 80px; border-radius: 8px;" />
    </a>
  </div>
</div>

<!-- OTHER CERTIFICATIONS SECTION -->
<div class="section" id="certs">
  <h2>Other Certifications</h2>
  <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 1.5rem; margin-top: 1rem;">
    <a href="https://www.credly.com/badges/b0bf80d4-ce82-409f-9fbf-ce566e35f719/public_url" target="_blank">
      <img src="/assets/icons/linux-essentials.png" alt="Linux Essentials" style="height: 60px;" />
    </a>
  </div>
</div>

<!-- LABS SECTION -->
<div class="section" id="labs">
  <h2>Lab Projects</h2>
  <div class="card-grid">
    <div class="card">
      <h3>SOC Automation Project</h3>
      <p>Integrated Shuffle with Elastic Stack and Slack to streamline alert triage and SOC workflow automation.</p>
      <a class="button" href="/labs/soc-automation">View Lab</a>
    </div>
    <div class="card">
      <h3>Active Directory Lab 1.0</h3>
      <p>Set up a basic Windows AD environment with domain controller, user/group configuration, DNS, and DHCP.</p>
      <a class="button" href="/labs/ad-lab-1">View Lab</a>
    </div>
    <div class="card">
      <h3>Active Directory Lab 2.0</h3>
      <p>Expanded AD lab with organizational units, GPOs, PowerShell automation, and network segmentation.</p>
      <a class="button" href="/labs/ad-lab-2">View Lab</a>
    </div>
  </div>
</div>

<script>
  function toggleComptiaGrid() {
    const grid = document.getElementById("comptia-cert-grid");
    grid.classList.toggle("show");
  }

  function toggleIsc2Grid() {
    const grid = document.getElementById("isc2-cert-grid");
    grid.classList.toggle("show");
  }
</script>

<footer>
  &copy; 2025 Steven Loucks — Built with GitHub Pages & Midnight Theme
</footer>
