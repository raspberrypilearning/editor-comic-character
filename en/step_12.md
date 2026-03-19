<h2 class="c-project-heading--task">Control the hero slider</h2>

Use JavaScript to move the hero slider backwards and forwards when the navigation buttons are clicked.

--- task ---

Open `scripts.js` and add the slider list, the current index variable, and the `changeHero()` function.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 77
line_highlights: 78-81,83-90,92,94
---
// Change Hero function
const heroSlides = document.querySelectorAll(".hero-slide");
var currentHeroIndex = 0;

function changeHero(direction) {

  heroSlides[currentHeroIndex].classList.remove("active");
  currentHeroIndex = currentHeroIndex + direction;

  if (currentHeroIndex < 0) {
    currentHeroIndex = 2;
  } else if (currentHeroIndex > 2) {
    currentHeroIndex = 0;
  }

  heroSlides[currentHeroIndex].classList.add("active");
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Click the left and right hero buttons on the home page and confirm the active image changes each time, wrapping back to the start when needed.

--- /task ---
