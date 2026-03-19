<h2 class="c-project-heading--task">Upgrade your project</h2>

--- task ---
Make one improvement to your superhero builder.
--- /task ---

--- task ---
Add a few more abilities to the `<select>` menu so users have more choices.
--- /task ---

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 32
line_highlights: 8-10
---
        <select id="ability-choice">
          <option value="">Choose an option</option>
          <option value="Flight">Flying</option>
          <option value="Invisibility">Invisibility</option>
          <option value="Time travel">Time travel</option>
          <option value="Super speed">Super speed</option>
          <option value="Water breathing">Water breathing</option>
          <option value="Teleportation">Teleportation</option>
        </select>
--- /code ---

</div>

--- task ---
**Test:** Reload the character page and check your new abilities appear in the dropdown list.
--- /task ---