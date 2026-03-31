<h2 class="c-project-heading--task">Let the user edit the summary</h2>

Add an Edit button and a function that hides the summary and shows the form again when the user clicks it.

### Step 1

Open `character.html` and `scripts.js` to add the Edit button and the `changeSummary()` function.


Code snippet 1 adds the Edit button to the summary section.

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 37
line_highlights: 40
---
      <section id="summary-section">
        <h2>Superhero Summary</h2>
        <p id="summary-paragraph"></p>
        <button onclick="changeSummary()">Edit</button>
      </section>
--- /code ---

</div>

Code snippet 2 adds the JavaScript that shows the form again when Edit is clicked.

<div class="c-project-code">

--- code ---
---
language: javascript
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

### Step 2

Create a superhero, click Edit, and confirm the form appears again so you can change the details.
