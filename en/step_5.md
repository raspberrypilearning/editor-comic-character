<h2 class="c-project-heading--task">Show the superhero summary</h2>

Use JavaScript to turn the form answers into a superhero summary when the user clicks Create.

### Step 1

Open `scripts.js`, store the form elements in constants, and create a `displaySummary()` function that updates the paragraph and swaps the visible section.


<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 5
line_highlights: 6-7,9-11,14-15,17-19,21-23
---
// Create constants for superhero form
const summary = document.querySelector("#summary-section");
const characterDetails = document.querySelector("#character-details");

const characterName = document.querySelector("#name-text");
const characterAbility = document.querySelector("#ability-choice");
const characterOrigin = document.querySelector("#origin-text");

// Function to display summary
function displaySummary() {
  const summaryParagraph = document.querySelector("#summary-paragraph");

  summaryParagraph.textContent = `Your superhero name is ${characterName.value}. 
  Their ability is ${characterAbility.value}. 
  Their origin story is ${characterOrigin.value}.`;

  characterDetails.style.display = "none";
  summary.style.display = "flex";
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

### Step 2

Fill in the form, click **Create**, and confirm the form disappears while the summary section shows the details you entered.
