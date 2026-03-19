<h2 class="c-project-heading--task">Save the light mode choice</h2>

Use JavaScript and local storage to switch the page theme and remember the user’s choice.

--- task ---

Open `scripts.js` and add the light mode switch constant, the `changeLightMode()` function, and a `DOMContentLoaded` listener.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 55
line_highlights: 56,58-60,62,64-65,67-68,70-73,75
---
// Create the constant for light mode
const lightModeSwitch = document.querySelector("#lightModeSwitch");

// Light mode function
function changeLightMode() {
  var isLightMode = lightModeSwitch.checked;

  document.body.classList.toggle("light-mode");

  localStorage.setItem("lightMode", isLightMode);
}

// Check local storage
document.addEventListener("DOMContentLoaded", function () {

  if (localStorage.getItem("lightMode") == "true") {
    document.body.classList.toggle("light-mode");
    lightModeSwitch.checked = true;
  }

});
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Run your code, then turn on light mode, refresh the page, and confirm the lighter colours stay enabled with the switch still checked.

--- /task ---
