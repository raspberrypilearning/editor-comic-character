<h2 class="c-project-heading--task">Add a light mode switch to the character page</h2>

Add the same switch to `character.html` so both pages have the same theme control.

--- task ---

Open `character.html` and add the switch container inside the header, below the navigation links.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 20
line_highlights: 20-26
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

Open `character.html` and confirm the same switch now appears in that page header as well.

--- /task ---
