<h2 class="c-project-heading--task">Let the user edit the summary</h2>

Add a function that hides the summary and shows the form again when the user clicks Edit.

--- task ---

Open `scripts.js` and add the `changeSummary()` function below `displaySummary()`.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 25
line_highlights: 26-29
---
// Function to edit summary
function changeSummary() {
  characterDetails.style.display = "flex";
  summary.style.display = "none";
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Create a superhero, click Edit, and confirm the form appears again so you can change the details.

--- /task ---
