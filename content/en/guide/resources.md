---
title: Resources
weight: 1
prev: /guide/
next: N
---

<style>
  .custom-tooltip-box {
    position: fixed; 
    
    /* Solid dark background */
    background: #1a1a1a; 
    color: #f7f7f7;
    
    padding: 1.2rem 1.4rem;
    border-radius: 12px; 
    width: max-content;
    max-width: 280px;
    
    /* Standard dark drop-shadow */
    box-shadow: 0 8px 25px rgba(0, 0, 0, 0.5);
    
    /* The new golden border */
    border: 1px solid #FFD700; 
    
    z-index: 9999;
    
    /* Bouncy drop-in animation */
    opacity: 0;
    visibility: hidden;
    transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    transform: translateY(-10px);
    pointer-events: none;
  }
  
  .custom-tooltip-box.show {
    opacity: 1;
    visibility: visible;
    transform: translateY(0);
    pointer-events: auto;
  }

  /* THE POINTER ARROW */
  .custom-tooltip-box::before {
    content: "";
    position: absolute;
    top: -7px; 
    right: 15px; 
    width: 14px;
    height: 14px;
    background: #1a1a1a; 
    
    /* Matched the golden border for the arrow */
    border-top: 1px solid #FFD700;
    border-left: 1px solid #FFD700;
    
    transform: rotate(45deg);
    border-top-left-radius: 3px;
    z-index: 0;
  }
</style>

<div id="topbar-tooltip" class="custom-tooltip-box">
  <button id="close-tooltip-btn" style="position: absolute; top: 10px; right: 12px; background: none; border: none; cursor: pointer; font-size: 20px; line-height: 1; color: inherit; opacity: 0.6; transition: opacity 0.2s;">&times;</button>
  
  <p style="margin: 0 0 6px 0; padding-right: 15px; font-size: 1rem; font-weight: 600; line-height: 1.4;">
    Pre-registrations for the AO Guide Astrophysics Challenge 2026 are open!
  </p>
  
  <p style="margin: 0; font-size: 0.85rem; color: #d4c5ff; font-weight: 500;">
    Register now!
  </p>
</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const tooltip = document.getElementById('topbar-tooltip');
    
    // NOTE: Replace "/your-real-page/" with your actual URL
    const iconLink = document.querySelector('a[href*="https://aoac.aoguide.app"]');
    const closeBtn = document.getElementById('close-tooltip-btn');

    // Function to calculate position and show the tooltip
    function positionAndShowTooltip() {
      if (!iconLink || !tooltip) return;
      
      const rect = iconLink.getBoundingClientRect();
      
      // Position it just below the icon
      tooltip.style.top = (rect.bottom + 15) + 'px';
      
      // Align it relative to the right side of the screen
      tooltip.style.right = (window.innerWidth - rect.right - 10) + 'px';
      
      // Trigger the CSS animation
      tooltip.classList.add('show');
    }

    // 1. Show automatically on load (after 200ms delay)
    setTimeout(positionAndShowTooltip, 200);

    // 2. Hide tooltip when the close button is clicked (Verified logic)
    if (closeBtn && tooltip) {
      closeBtn.addEventListener('click', (event) => {
        event.preventDefault(); // Extra safety to prevent link behavior
        tooltip.classList.remove('show');
      });
    }

    // 3. Keep it attached to the icon if the user resizes their browser window
    window.addEventListener('resize', () => {
      if (tooltip && tooltip.classList.contains('show')) {
        positionAndShowTooltip();
      }
    });
  });
</script>

Most of the textbooks used in writing the guide have been mentioned in the About page. Here are some additional resources that you may find useful:

## General

- This [Drive](https://drive.google.com/drive/folders/1gZDmKb3n2vXHpVZMwFaUJ1ukUccCfYKD?usp=sharing) contains all the sources used, and more. Many national and international olympiad papers too are available here.
- A really awesome and comprehensive [resource for IOAA](https://drive.google.com/file/d/13bRXOBf5ri0Q-ipmvBewzgD4ETMWo_xW/view) by Lee Yiu Sing. Can be followed alongside the guide for a different perspective on topics.
- Sean Ken M. Galanza's [astronomy handouts](https://drive.google.com/drive/folders/1i7HR025iR4HO7PHhx7RmDCRa5aRi14hX?usp=sharing)
- Kevin Zhou's [Physics Olympiad Handouts](https://knzhou.github.io), mainly M6 and X3
- [USAAAO Guide](https://www.usaaao.guide/handouts) - Handouts for USAAAO and IOAA preparation
- Astronomy Olympiad Discord Server's [POTD Archive](https://rajit13.github.io/website_docs/Astro_POTD.pdf) by Fahim Rajit Hossain
- [Blogs](https://physolympacademy.com/blog/) by Armin Hodaei
- [Celestial Sphere](https://bunchofcellulose.github.io/celestialsphere/) - A webapp to play with spherical diagrams
- Astronomy Olympiad Discord Server ([AODS](https://discord.gg/cuVC54FksD)) - a community of astronomy enthusiasts and olympiad participants. Great place to ask questions, share resources, and connect with others who share your interest in astronomy.
- [BDOAA Preparation Material](https://drive.google.com/drive/folders/0BxnDs515DNddbWg1VTBRZktZODA?resourcekey=0-evWmK0fkUFSEv7l4icX5OQ)
- [CAAO Preparation Material](https://caao.ca/wp-content/uploads/2023/02/CAAO-tutorial.pdf)
- [Relevant Physics Olympiad Problems](https://sheikhabrar140.github.io/website_docs/problems_Pho.pdf) for IOAA, compiled by Sheikh Hasin Abrar Alvi and me. Contains problems from IPhO, national physics olympiads, and physics contests that are relevant for IOAA preparation.
- Kaiwen's orz [astronomy notes](https://apochrome.notion.site/Astronomy-c2080a4c5b464868a99f5cddec3e0bbb)
- A very comprehensive analysis of the [analemma](https://rajit13.github.io/website_docs/Analemma_Primer.pdf) by Fahim Rajit Hossain.
- A guide for [problem writing for Astronomy Olympiads](https://rajit13.github.io/website_docs/Astronomy_via_LaTeX.pdf) by Fahim Rajit Hossain.
- [aoXiv](https://aoxiv.aoguide.app/) - an archive of problems from various astronomy olympiads throughout the globe. Community-driven and open source, so feel free to add any problems you find to the archive!
- [phoXiv](https://phoxiv.org) - an archive of problems from various physics olympiads throughout the globe. Community-driven and open source, so feel free to add any problems you find to the archive!

## Practical

- [Practical Handouts for Olympiad](https://drive.google.com/drive/u/0/folders/1Nft4B755uvtxfaSGLp2ZsVuHQGZ9pEt-) by Ayush Tiwari. Covers all aspects of data analysis and most observation skills required for IOAA.
- [Star Maps 101 and Practices](https://github.com/Rajit13/Star-Maps-101-and-Practices) by Fahim Rajit Hossain
- [Learn the Sky](https://www.youtube.com/@learnthesky) - A YouTube channel with videos on finding constellations, planets and navigating the sky.
- [Sky Academy](https://play.google.com/store/apps/details?id=digital.dong.skyacademy&hl=en_IN) - An android app which you can use to learn constellations, stars and Messier objects.
- [Stellar Guesser](https://stellarguesser.github.io/) - a tool for learning the sky in a game-like manner.
- Stellarium [Mobile App](https://play.google.com/store/apps/details?id=com.noctuasoftware.stellarium_free&hl=en_IN) and [Desktop App](https://stellarium.org/) - a planetarium software that shows a realistic sky in 3D, just like what you see with the naked eye, binoculars or a telescope.
- [BAAO Observational Handouts](https://drive.google.com/drive/folders/141B0qiKer2hnpNKzf0yNuLKOqcTA2Cpf)
- [Skychart Tasks](https://anatolieursu.github.io/sky-chart-practice/) - a tool where you can import your skycharts and practice them online.

## Competitions and Olympiad Archives

- [AO Guide Astrophysics Challenge](https://aoac.aoguide.app/) - an online competition organized by us, with original problems designed to test your physics and astrophysics problem-solving skills.
- [Official IOAA Website](https://ioaastrophysics.org)
- [Astronomy Olympiad Archives](https://mega.nz/folder/3ZBWDbTL#U8-utZdSD-6URDjXS1t9Ag) by Stefan Ivanov
- [Astroarena](https://astroarena.github.io/astroarena/index.html) - Contains all pre 2020 IOAA papers
- [AstroSandbox](https://astrosandbox.com/eng) - A website founded by Ukrainian IOAA participants, gives lectures, organizes events, manages clubs, composes our own astronomy tasks, as well as collects existing problems from Olympiads and public sources.
- [USAAAO](https://usaaao.org/resources/past-exams/) Archives - First Round and NAC papers of USA's astronomy olympiad
- [SAO](https://drive.google.com/drive/folders/1fVdcMhwshartqgcSSFr2O37m2NEpnciU) Archives - Singapore Astronomy Olympiad past papers
- [INAO](https://olympiads.hbcse.tifr.res.in/how-to-prepare/past-papers/) Archives - Indian National Astronomy Olympiad past papers
- [OAAO](https://oaaoinfo.org) - the Online Astronomy and Astrophysics Olympiad

If you have any other resources that you think would be useful, feel free to share them in the resources channel on our Discord server.

## Country-specific Advice

{{< cards >}}
  {{< card link="https://bunchofcells.vercel.app/blog/indian-astronomy-olympiads" title="🇮🇳 India" subtitle="Akshat Srivastava, IOAA 2025" icon="trending-up" >}}
  {{< card link="/assets/advice/IND1.pdf" title="🇮🇳 India" subtitle="Akarsh Raj Sahay, IOAA 2023" icon="trending-up" >}}
  {{< card link="/assets/advice/NEP1.pdf" title="🇳🇵 Nepal" subtitle="Osish Niraula, IOAA 2024 & 2025" icon="support" >}}
  {{< card link="/assets/advice/ROU1.pdf" title="🇷🇴 Romania" subtitle="Teodor Bichir, IOAA 2024 & 2025" icon="document" >}}
  {{< card link="/assets/advice/SGP1.pdf" title="🇸🇬 Singapore" subtitle="Wang Jun Min, IOAA 2025" icon="flag" >}}
  {{< card link="/assets/advice/BGL1.pdf" title="🇧🇩 Bangladesh" subtitle="Sheikh Hasin Abrar Alvi, IOAA 2024" icon="academic-cap" >}}
{{< /cards >}}

If you have represented your country in IOAA and would like to contribute a similar advice document for future participants from your country, please reach out to us on our [Discord server](https://discord.gg/bV8bxvTmzU).

## References & Sources

AO Guide is built upon the foundational work of many excellent textbooks, research papers, and educational resources. These books were not written with IOAA in mind, but they're wonderful in general!

### Primary Textbooks

- [Astronomy: Principles and Practice](https://drive.google.com/file/d/1LBJJhPa87_UqNKCdONRnhYcKN_B12iz5/view?usp=sharing) by A. E. Roy and D. Clarke
- [Fundamental Astronomy](https://drive.google.com/file/d/1jAAtkF0YCrT3Fm9B4I2kxez393olF_iy/view?usp=sharing) by Hannu Karttunen et al.
- [Fundamentals of Astronomy](https://drive.google.com/file/d/15bDhuOIYbaz2CmQemkBOSsJuuQPXRJdL/view?usp=sharing) by Flavio Salvati
- [Introduction to Cosmology](https://drive.google.com/file/d/1EU9BMWuDMEkYaPJGurBBH4JUUrz4RIOD/view?usp=sharing) by Barbara Ryden
- [Foundations of Astrophysics](https://drive.google.com/file/d/16I3sen7AG04qKWSP_nJ0A7mziUKnMhfE/view?usp=sharing) by Barbara Ryden
- [An Introduction to Modern Astrophysics](https://drive.google.com/file/d/1V12rbls_OdmsxS4HSG2sudghqPZ54Wfz/view?usp=sharing) by Bradley W. Carroll and Dale A. Ostlie
- [A Problem book in Astronomy and Astrophysics](https://drive.google.com/file/d/1gFn2rYAE5QMrge7B0cz1x4K12mr2Ca1s/view?usp=sharing) by Aniket Sule

### Data Sources

- [International Astronomical Union (IAU)](https://www.iau.org) - Constants and definitions
- [Wikipedia](https://www.wikipedia.org) - For general reference and quick lookups (always cross-verify with primary sources)
- [CODATA](https://physics.nist.gov/cuu/pdf/wall_2022.pdf) - Fundamental physical constants

A [list of useful constants](/guide/resources/#constants-list) is provided at the end of the page.

### Problem Sources

- Previous IOAA Problems (2007-2025) - Official competition problems and solutions
- National Astronomy Olympiads - Problems from various countries' national competitions
- Physics Competitions - Adapted problems from IPhO, national physics olympiads, and physics contests
- Other Astronomy Competitions - Problems from regional astronomy contests and university-level competitions
- Original Problems - Custom problems designed specifically for IOAA preparation by us
- Research Literature - Adapted problems from peer-reviewed journals

## Constants List

<div style="margin-top: 2rem;"></div>

{{< pdf "/assets/constants.pdf" >}}
