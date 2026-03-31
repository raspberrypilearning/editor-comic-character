<h2 class="c-project-heading--task">Add a light mode switch to the home page</h2>

--- task ---

Open `index.html` and paste this switch container inside the header, just after `</nav>` and before `</header>`.

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
      <nav class="navbar" id="nav">
        <a href="index.html">HOME</a>
        <a href="character.html">CREATE CHARACTER</a>
      </nav>
      <div class="switch-container">
        <label class="switch">
          <input onchange="changeLightMode()" type="checkbox" id="lightModeSwitch">
          <span class="switch-slider"></span>
        </label>
        <span class="switch-label material-symbols-outlined">light_mode</span>
      </div>
    </header>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Click Run and confirm a switch appears in the home page header, even though it does not change the colours yet.

--- /task ---
