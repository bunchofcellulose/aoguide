---
title: Guide
next: /guide/resources
comments: false
sidebar:
  open: true
cascade:
  type: docs
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

Welcome to the AO Guide! To navigate the guide, use the sidebar on the left. You can also search for topics using the search bar at the top right. A table containing all useful constants is provided on the rightmost tab of the top bar.

## Prerequisites

The guide assumes that the reader has a basic understanding of high school level mathematics and physics. Familiarity with calculus and basic mechanics is required. We have tried to keep the guide mathematically rigorous, however, we have made sure all necessary concepts are explained in detail.

## How to start your journey

If you're just beginning, the following order is recommended:

1. **Positional Astronomy**: Start with the basics of celestial coordinates, timekeeping, and the motion of celestial objects.
2. **Photometry**: Learn about the tools and techniques used to measure the brightness of celestial objects.
3. **Celestial Mechanics**: Understand the laws governing the motion of celestial bodies.
4. **Stellar Astrophysics**: Explore the physics of stars, including their structure and evolution.
5. **Galactic and Extragalactic Astrophysics**: Study the large-scale structure of the universe, including galaxies and clusters, along with cosmology.

For those of you who are already familiar with the basics, feel free to jump to any chapter that interests you.

The index page of each unit lists several resources to read from in the Recommended Reading section. If you find something confusing or hard to understand in the guide (let us know!), we highly recommend checking out the resources listed there. They are a great way to get a different perspective on the topic and can help clarify any doubts you may have.

The guide goes over pretty much all of the theoretical concepts needed for astronomy olympiads. However, theory is not the only thing asked in olympiads. The IOAA has three exams: a theory exam, a data analysis exam, and an observation exam (usually split into several exams). The guide primarily focuses on the theory part, but it is important to know that the other two parts are equally important, carrying 25% of the total points each (50% theory, 25% data analysis and 25% observation). The resources page contains links to past papers and other useful resources.

- **Data Analysis** requires you to read and draw graphs, speedrun your calculator, and interpret data. You will be given a set of data, and you will have to answer questions based on that data. The data can be in the form of tables, graphs, or images. Be prepared to do a lot of calculations, and draw a lot of graphs. A good understanding of statistics is also required.
- **Observational Skills** can too be broken down into three parts: Telescope handling, Naked eye observation and sky maps. For each of these, be prepared to remember all 88 constellations, all the Messier objects, all the bright stars (with their names, and maybe RA/Dec and magnitudes of a few too), and a good amount of star hopping skills.

  - **Telescope handling** requires you to know how to set up and use a telescope. You will be given a telescope, and you will have to set it up and use it to point at and observe celestial objects. You will also be required to know how to align the telescope, and how to use the different parts of the telescope.
  - **Naked eye observation** requires you to know how to identify celestial objects using just your eyes. You will typically be given a list of celestial objects, and you will have to identify them in the night sky. A good amount of familiarity with the night sky is required.
  - **Sky maps** require you to know how to read and interpret sky maps. You will be given a sky map, and you will have to answer questions based on that sky map. This could be to identify constellations, mark deep sky objects, find missing stars, etc. Be prepared to practice a lot of star maps.

## How the Guide is structured

The guide is structured in a way that allows you to start from the basics and gradually build up your knowledge. It has been divided into 5 units, each unit having several chapters, with each chapter covering a specific topic in detail. The chapters are further divided into sections for easier navigation.

To make the guide more interactive, we have included several diagrams and illustrations to help you visualize the concepts being discussed. Additionally, we have included links to external resources for further reading. Eye-catching callout boxes are used to highlight important points, tips, and additional information. Here are the different types of callout boxes used in the guide:

<br/>

{{< callout type="remark" >}}
This is a remark callout box. It is used to convey additional information or clarify a point made in the main text.
{{< /callout >}}

{{< callout type="image" >}}
This is an image callout box. It is used to display images or diagrams that are relevant to the topic being discussed.
{{< /callout >}}

{{< callout type="trivia" >}}
This is a trivia callout box. It contains interesting facts or historical context related to the topic.
{{< /callout >}}

{{< callout type="math" >}}
This is a math callout box. It shows complex mathematical derivations required to arrive at an equation.
{{< /callout >}}

{{< callout type="table" >}}
This is a table callout box. It is used to present data or information in a tabular format.
{{< /callout >}}

{{< callout type="why" >}}
This is a why callout box. It goes into explanation of a non-trivial concept or fact mentioned in the main text.
{{< /callout >}}

{{< callout type="DIY" >}}
This is a DIY callout box. It contains exercises or problems for the reader to solve, encouraging active engagement with the material.
{{< /callout >}}

<br/>

Many chapters contain in-text problems, as well as problems at the end of the chapter (It takes a lot of time and effort to make problems, so please be patient! We will add problems for every chapter). These problems are designed to test your understanding of the concepts covered in the chapter (They can be hard, so don't be discouraged if you find them challenging!).

{{< tabs >}}
    {{< tab name="P1" >}}
    What to do if I get stuck on a problem?
    {{< /tab >}}

    {{< tab name="Solution" >}}
    Ask for ideas on our discord server!
    {{< /tab >}}
{{< /tabs >}}

## Contributing to the Guide

The guide is a living document, and is constantly being updated and improved. If you have any suggestions or feedback, please feel free to reach out to us on our [Discord server](https://discord.gg/bV8bxvTmzU). We highly welcome any explanations, derivations, or diagrams that you think would improve the guide. If you find any errors or typos, please let us know so we can fix them. Constructive criticism is always appreciated!

The [github repository](https://github.com/bunchofcellulose/aoguide) for the guide is public, and you can create issues or pull requests if you want to contribute directly.

You can use the comment section at the bottom of the page to discuss the content, post extra resources, and report typos. For longer discussions, please join our Discord server.
