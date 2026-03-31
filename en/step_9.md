<h2 class="c-project-heading--task">Add a light mode switch to the home page</h2>

Add a switch to `index.html` so the home page has a control for changing the colour theme.

--- task ---

Open `index.html` and add the switch container inside the header, below the navigation links.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 25
line_highlights: 25-31
---
      <div class="switch-container">
        <label class="switch">
          <input onchange="changeLightMode()" type="checkbox" id="lightModeSwitch">
          <span class="switch-slider"></span>
        </label>
        <span class="switch-label material-symbols-outlined">light_mode</span>
      </div>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Click Run and confirm a switch appears in the home page header, even though it does not change the colours yet.

--- /task ---
