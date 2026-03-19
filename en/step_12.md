<h2 class="c-project-heading--task">Challenge</h2>

--- task ---
Personalise the summary message so it matches your character and your story.
--- /task ---

--- task ---
Edit the summary text template so it sounds more like a comic book caption (you decide the style).
--- /task ---

<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 13
line_highlights: 5-7
---
// Function to display summary
function displaySummary() {
  const summaryParagraph = document.querySelector("#summary-paragraph");

  summaryParagraph.textContent = `🌟 Meet ${characterName.value}!
Power: ${characterAbility.value}
Origin: ${characterOrigin.value}`;
  ...
}
--- /code ---

</div>

--- task ---
**Test:** Create a character and check your new summary style appears exactly the way you intended.
--- /task ---