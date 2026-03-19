<h2 class="c-project-heading--task">Hero image slider</h2>

--- task ---
Let the user click buttons to move through hero images.
--- /task ---

--- task ---
Create a function that:
- removes the `active` class from the current slide
- updates the slide index
- adds `active` to the new slide
--- /task ---

<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 77
line_highlights: 2-18
---
// Change Hero function
const heroSlides = document.querySelectorAll('.hero-slide');
var currentHeroIndex = 0;

function changeHero(direction) {

  heroSlides[currentHeroIndex].classList.remove("active");
  currentHeroIndex = currentHeroIndex + direction;

  if (currentHeroIndex < 0){
    currentHeroIndex = 2;
  } else if (currentHeroIndex > 2) {
    currentHeroIndex = 0;
  }

  heroSlides[currentHeroIndex].classList.add("active");

}
--- /code ---

</div>

--- task ---
**Test:** Click the next/previous buttons and check the hero image changes (and loops at the ends).
--- /task ---