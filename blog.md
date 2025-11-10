---
layout: home
title: Home, Refactored
subtitle: process optimization for every space
---

<div class="scroll-container" id="scrollContainer">
  <a href="../2025-08-01-projector"><img src="/assets/img/projector-icon.jpg" alt="Projector" width="300" height="300"></a>
  <a href="../2025-07-15-scarves"><img src="/assets/img/scarves-icon.jpg" alt="Scarves" width="300" height="300"></a>
  <a href="../2025-05-12-kid-bedroom"><img src="/assets/img/kidbedroom-icon.jpg" alt="Kid Bedroom" width="300" height="300"></a>
  <a href="../2025-04-12-living-room"><img src="/assets/img/livingroom-icon2.jpg" alt="Living Room" width="300" height="300"></a>
  <a href="../2025-03-15-master-bedroom"><img src="/assets/img/masterbed-icon.jpg" alt="Master Bedroom" width="300" height="300"></a>
  <a href="../2025-03-01-wardrobe"><img src="/assets/img/wardrobe-icon2.jpg" alt="Wardrobe" width="300" height="300"></a>
  <a href="../2024-09-20-laundry"><img src="/assets/img/laundry-icon2.jpg" alt="Laundry Room" width="300" height="300"></a>
  <a href="../2024-08-15-entry-closet"><img src="/assets/img/entryway-icon.jpg" alt="Entry Closet" width="300" height="300"></a>
  <a href="../2024-06-26-laundry"><img src="/assets/img/laundry-icon.jpg" alt="Utility Room" width="300" height="300"></a>
  <a href="../2024-03-31-jars"><img src="/assets/img/jars01.jpg" alt="Labeled Jars" width="300" height="300"></a>
  <a href="../2024-02-01-storage-unit"><img src="/assets/img/storageunit-icon.jpg" alt="Storage Unit" width="300" height="300"></a>
  <a href="../2023-06-01-fireplace"><img src="/assets/img/fireplace-icon2.jpg" alt="Fireplace" width="300" height="300"></a>
  <a href="../2022-12-30-toys"><img src="/assets/img/toys-icon.jpg" alt="Toys" width="300" height="300"></a>
  <a href="../2022-09-01-kids-artwork"><img src="/assets/img/artwork-icon.jpg" alt="Artwork" width="300" height="300"></a>
  <a href="../2022-06-25-bathroom-reno"><img src="/assets/img/bathroom-icon.jpg" alt="Downstairs Bathroom" width="300" height="300"></a>
  <a href="../2022-01-18-linens"><img src="/assets/img/linens-icon.jpg" alt="Linen Closet" width="300" height="300"></a>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  const container = document.getElementById('scrollContainer');

  // --- RANDOMIZE IMAGE ORDER ---
  const children = Array.from(container.children);
  const shuffled = children.sort(() => Math.random() - 0.5);
  container.innerHTML = '';
  shuffled.forEach(child => container.appendChild(child));

  // --- AUTO-SCROLL ---
  let scrollSpeed = 0.5;
  let isPaused = false;

  function canScroll() {
    return container.scrollWidth > container.clientWidth;
  }

  function autoScroll() {
    if (!isPaused && canScroll()) {
      container.scrollLeft += scrollSpeed;
      if (container.scrollLeft + container.clientWidth >= container.scrollWidth - 1) {
        container.scrollLeft = 0;
      }
    }
    requestAnimationFrame(autoScroll);
  }

  container.addEventListener('mouseenter', () => isPaused = true);
  container.addEventListener('mouseleave', () => isPaused = false);
  container.addEventListener('touchstart', () => isPaused = true);
  container.addEventListener('touchend', () => isPaused = false);

  setTimeout(autoScroll, 300);
});
</script>


**The backstory.** Part of what draws me to Computer Science research is my general love of thinking about optimal solutions given a set of 
constraints, and testing out (and measuring the success of) new ideas :balance_scale: :chart_with_upwards_trend:. I like playing strategy board games :chess_pawn:, 
grouping errands to minimize travel time and distance :world_map: :stopwatch:, and packing *exactly* without excess :briefcase:.
Unrelated: I'm also sensitive to visual overcrowding and cannot concentrate when my surroundings are messy or disorganized :face_with_spiral_eyes:.

**The catalyst.** Enter two baby boys across [three](https://www.who.int/news-room/spotlight/why-we-need-to-talk-about-losing-a-baby) [rough pregnancies](https://en.wikipedia.org/wiki/Hyperemesis_gravidarum) 
during my postdoc and a worldwide pandemic imprisoning our family of 4 in a tiny urban apartment 
*with no childcare options or any outside help for more than half a year*. 
You get it. [Maybe](https://www.americanprogress.org/article/covid-19-pandemic-forcing-millennial-mothers-workforce/).

**The outcome.** Planning, executing, and iteratively refactoring organization solutions to enable everyone in the family to 
*independently find and use their stuff* safely and *put it away themselves* was essential for life but also, turns out, an 
[essential form of selfcare for me](https://www.nature.com/articles/s44220-024-00268-4). 
Our friends have been so delighted by some of my systems that they've encouraged me to share my ideas with you all. Hope you enjoy!

---