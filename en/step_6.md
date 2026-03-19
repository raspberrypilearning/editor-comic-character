<h2 class="c-project-heading--task">Change the summary</h2>

--- task ---
Let the user go back and edit their superhero choices.
--- /task ---

--- task ---
Create a function that hides the summary section and shows the form again.
--- /task ---

<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 25
line_highlights: 2-5
---
// Function to edit summary
function changeSummary() {
  characterDetails.style.display = "flex";
  summary.style.display = "none";
}
--- /code ---

</div>

--- task ---
**Test:** Show the summary, then use your “Edit” button and check the form appears again.
--- /task ---