---
title: About
type: about
toc: false
comments: false
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

<div class="about-section">
<div class="section-content">

<div class="section-title">About AO Guide</div>

Hey, thanks for dropping by! We're grateful to have you here. Let's talk a bit about why we built AO Guide.

When we were preparing for astronomy olympiads, we found ourselves (and others) jumping between massive textbooks (that had way more info than we needed), scattered handouts from random websites, and outdated materials that didn't really capture what IOAA was all about. It was honestly pretty overwhelming. It's understandable, they weren't really designed with IOAA in mind, but we wanted to fix this.

Therefore, we built AO Guide. It's not a textbook or another handout, the main goal of AO Guide is to be *complete* and *concise*. That doesn't mean it's just short, dry text without any motivation, we have actively tried to do the exact opposite; but that it contains a lot more of what is needed for the olympiads.

<div class="subsection-title">What We're Really Trying to Do</div>

We wanted to create something that we wish we had when we started our olympiad journey:

1. **Everything you actually need** for IOAA – no more, no less. We've been through this, so we know what matters.
2. **Built the way we learn** – step by step, with plenty of examples and explanations that actually make sense.
3. **Modern and accessible** – because studying shouldn't feel like punishment, and everyone deserves good resources.
4. **Visual and engaging** – diagrams, and other interactive elements that help visualise concepts.
5. **Real problem-solving practice** – not just theory, but the kind of problems you'll actually face in competitions.

<div class="subsection-title">Why This Exists</div>

Astronomy and astrophysics are incredible subjects that we really do love. But preparing for olympiads caused us a lot of frustrations, and not for a lack of trying. Most textbooks were either too advanced, or woefully incomplete for IOAA.

It was because of this frustration that we decided to write AO Guide. We don't really benefit much from it, it's free for you to use and modify after all! But honestly, just allowing for a far smoother way to learn for the next person who wanted to get into astronomy is quite rewarding in itself :)

Olympiads aren't about memorizing formulas (though you do really need some of them). It's about really understanding how things work, being able to think through problems step by step, and having the confidence to tackle something you've never seen before. That's what we're trying to help you build, we have a plethora of problems with solutions for you to go through!

<div class="feature-grid">
  <div class="feature-item">
    <h4>Targeted Content</h4>
    <p>Every section is specifically designed for IOAA preparation, ensuring relevance and efficiency.</p>
  </div>
  <div class="feature-item">
    <h4>Living Document</h4>
    <p>Continuously updated with new problems, explanations, and improvements based on user feedback.</p>
  </div>
  <div class="feature-item">
    <h4>Global Community</h4>
    <p>Built by and for the international astronomy Olympiad community.</p>
  </div>
</div>

</div>
</div>

<div class="about-section">
<div class="section-content">

<div class="section-title">The People Behind This</div>

<div class="author-card">
  <img src="/assets/images/start/akshat.png" class="author-avatar">
  <div class="author-info">
    <h4>Akshat Srivastava</h4>
    <p><strong>Creator & Author</strong></p>
    <p>Hi! I'm a high school student from India and a Gold medalist from IOAA 2025. I love physics, astronomy and math, along with few other subjects (including but not limited to cs, linguistics, chemistry and engineering). I like mathematical rigor in solving problems, and I believe I have been successfully able to reflect this in the guide. You can reach out to me on my <a href="https://discord.gg/bV8bxvTmzU" target="_blank">Discord server</a>, or dm me at @bunchofcells (I like cucumbers).</p>
    <div class="author-links">
      <a href="https://bunchofcells.vercel.app/" target="_blank">Website</a>
    </div>
  </div>
</div>

<div class="author-card">
  <img src="/assets/images/start/lilian.png" alt="Lilian" class="author-avatar">
  <div class="author-info">
    <h4>Lilian</h4>
    <p><strong>Editor</strong></p>
    <p>I'm a high school student from India passionate about mathematics, physics, cs, literature, and philosophy (yes it's a bit of a weird combo). I was a PROMYS 2025 Alumni, and was the leader of Physics Olympiad Co-operation for BL4S, which was shortlisted. I help make sure our explanations are correct, and most importantly clear! You can contact me on discord at @jardindelys, but do send a cat pic if you decide to :D</p>
  </div>
</div>

A special thanks to <strong>Madhav Gupta</strong><a href="https://github.com/Madhav2609/" target="_blank"> (@Madhav2609)</a> for helping with mobile compatibility, CSS improvements, and hosting the website.

<div class="subsection-title">Want to Help Out?</div>

This project is way bigger than just the two of us, and we'd love your help! Whether you're a fellow student who's found a mistake, an educator with suggestions, or just someone who loves astronomy:

1. **Spot an error?** Please let us know! We're human and definitely make mistakes.
2. **Have a great problem or explanation?** We'd love to include it (with credit, of course).
3. **Ideas for improvements?** We're always looking for ways to make this better.
4. **Want to spread the word?** Tell your friends, teachers, or anyone who might find this useful!

Check out the [GitHub repository](https://github.com/bunchofcellulose/aoguide) to get involved. Every contribution helps make this better for everyone.

</div>
</div>

<div class="about-section">
<div class="section-content">

<div class="section-title">Thanks to Everyone Who Made This Possible!</div>

There were a lot of people and institutions that helped create this. Its not possible to credit all of them, and we're sorry if we missed you, we do really appreciate your contribution. Huge thanks to:

### Educational Institutions
1. **Homi Bhabha Centre for Science Education (HBCSE)** – For creating such an amazing olympiad culture in India and giving us opportunities we never thought we'd have
2. **IOAA** – For organizing the international olympiad and making astronomy education a global priority
3. **National Olympiad Committees worldwide** – For maintaining high standards and sharing resources with the community

### The Tech That Powers This
1. **Hugo** – For making our website fast and beautiful
2. **Hextra Theme** – For the gorgeous design foundation that makes everything look professional
3. **KaTeX** – For making our math equations look crisp and readable
4. **GitHub** – For making collaboration so easy
5. **Vercel** – For reliable, fast, and hassle-free website hosting
6. **Name.com** – For domain registration and DNS management

### Our Amazing Community
1. **IOAA alumni and participants** – For sharing problems, giving feedback, and helping us improve constantly
2. **Astronomy teachers and mentors** – For reviewing our content and making sure we're not leading anyone astray
3. **Open source contributors** – For helping with code, bug fixes, and feature improvements
4. **Early users and beta testers** – For putting up with our mistakes and helping us make this actually useful

</div>
</div>

<div class="about-section">
<div class="section-content">

<div class="section-title">License & Usage</div>

<div class="license-box">
<h4>📄 How You Can Use This</h4>
<p>AO Guide is released under the <strong>Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)</strong>.</p>
</div>

Here's what this means in plain English:

<div class="subsection-title">You're totally free to:</div>

1. **Share it** – Copy, download, and share with anyone who might find it useful
2. **Modify it** – Adapt, remix, or build upon our content for your own non-commercial use

<div class="subsection-title">Just remember to:</div>

1. **Give us credit** – Let people know where the original came from and mention if you've made changes
2. **Keep it non-commercial** – Don't sell this or use it to make money
3. **Share your improvements** – If you make something cool based on our work, share it under the same license

<div class="subsection-title">What Counts as Commercial Use?</div>

Basically, if you're making money from it, that's commercial use:

1. Selling the content or anything based on it
2. Using it in paid courses or tutoring services
3. Including it in commercial apps or software
4. Any other profit-making activities

<div class="subsection-title">For Students and Educators</div>

This guide is completely free for educational use! Use it for studying, teaching, school projects, or olympiad preparation. Just give us a quick mention if you use our content in presentations or assignments.

If you need to use our content commercially for some reason, just reach out to us and we can probably work something out. Note that fair use of the content is completely fine!

</div>
</div>
