<h2 class="c-project-heading--task">Add copyright text</h2>

Show the current year automatically in the footer.

--- task ---

Create a `Date` in JavaScript, then write the year into the `<span>` with the id `copyrightYear`.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 1
line_highlights: 2-3
---
// Update Copyright Year function 
const currentDate = new Date();
document.querySelector("#copyrightYear").innerText = currentDate.getFullYear();
--- /code ---

</div>

--- task ---

**Test:** Run your code and check the footer displays the current year.

--- /task ---