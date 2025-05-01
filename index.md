-----
layout: default
title: Home
---

<style>
  .rotate-icon {
    animation: slow-spin 8s linear infinite;
    display: inline-block;
  }

  @keyframes slow-spin {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
  }
</style>

<header>
  <h1>Steven Loucks</h1>
  ...
  <p>Cybersecurity Student | Cloud Enthusiast | Lab Builder</p>
  <nav>
    <a href="#certs">Certifications</a>
    <a href="#labs">Labs</a>
    <a href="#blog">Blog</a>
  </nav>
</header>

<section id="certs">
  <h2>Certifications</h2>
  <details>
    <summary>CompTIA Security+</summary>
    <p>Core security concepts, risk management, threat analysis, cryptography, and incident response. Verified and current.</p>
  </details>
  <details>
    <summary>ISC² Certified in Cybersecurity</summary>
    <p>Entry-level cert focusing on cybersecurity principles, network security, and access controls.</p>
  </details>
  <details>
    <summary>LPIC-1 Linux Essentials</summary>
    <p>Linux command line basics, file permissions, package management, and basic system admin knowledge.</p>
  </details>
</section>

<section id="labs">
  <h2>Lab Work</h2>

  <details>
    <summary>
      <img src="/assets/icons/windows.png" alt="AD Icon" style="height: 24px; vertical-align: middle; margin-right: 8px;" />
      Active Directory Lab (VirtualBox + Shuffle + Slack)
    </summary>
    <p>Built a functional AD environment using VirtualBox. Integrated Shuffle for automation and Slack for alerting.</p>
    <span style="display: inline-block; background: #222; padding: 0.2rem 0.5rem; border-radius: 4px; margin-right: 0.5rem;">VirtualBox</span>
    <span style="display: inline-block; background: #222; padding: 0.2rem 0.5rem; border-radius: 4px;">Automation</span><br />
    <a href="https://github.com/sloucks623/ad-lab" class="button" target="_blank">View Repository</a>
  </details>

  <details>
    <summary>
      <img src="/assets/icons/kali.png" alt="Kali Icon" style="height: 24px; vertical-align: middle; margin-right: 8px;" />
      Kali Linux Recon Lab
    </summary>
    <p>Used Kali tools like Nmap and Dirb to scan a target. Documented findings with MITRE ATT&CK mapping.</p>
    <span style="display: inline-block; background: #222; padding: 0.2rem 0.5rem; border-radius: 4px; margin-right: 0.5rem;">Kali</span>
    <span style="display: inline-block; background: #222; padding: 0.2rem 0.5rem; border-radius: 4px;">Recon</span><br />
    <a href="https://github.com/sloucks623/kali-recon-lab" class="button" target="_blank">View Repository</a>
  </details>
</section>

<section id="blog">
  <h2>Latest Blog Entries</h2>
  <p>Coming soon — articles on certifications, labs, and learning journeys will appear here.</p>
</section>

<footer>
  &copy; 2025 Steven Loucks — Built with GitHub Pages
</footer>
