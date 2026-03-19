<h2 class="c-project-heading--task">Light mode theme</h2>

--- task ---
Add a light mode switch and remember the user’s preference.
--- /task ---

--- task ---
When the switch changes:
- toggle a `light-mode` class on the `<body>`
- save the switch state in `localStorage`
- restore it when the page loads
--- /task ---

<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 55
line_highlights: 1-21
---
// Create the constant for light mode
const lightModeSwitch = document.querySelector("#lightModeSwitch");

// Light mode function
function changeLightMode(){
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

--- task ---
**Test:** Turn on light mode, refresh the page, and check light mode stays on.
--- /task ---