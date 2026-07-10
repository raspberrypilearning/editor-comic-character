## Control the hero slider

Use JavaScript to move the hero slider backwards and forwards when the navigation buttons are clicked.

Open `scripts.js` and add the slider list, the current index variable, and the `changeHero()` function.

```javascript filename="scripts.js" line_numbers="true" line_number_start="77" line_highlights="78-79,81,83-90,92-93"
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
```

## Now run your code

Run your code, then open `index.html`.

Click the left and right hero buttons on the home page and confirm the active image changes each time, wrapping back to the start when needed.
