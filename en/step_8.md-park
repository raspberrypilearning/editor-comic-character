<h2 class="c-project-heading--task">Check the form before creating</h2>

Warn the user when they miss a field so the summary is only created after the form is complete.

--- task ---

Open `character.html` and `scripts.js` to add the warning area and the `checkForm()` function.

--- /task ---

Code snippet 1 updates the form so the Create button runs `checkForm()` and there is a place to show the warning.

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 33
line_highlights: 35-36
---
        <label for="origin-text">Origin Story:</label>
        <textarea id="origin-text" placeholder="Add your superhero origin story!"></textarea>
        <div id="alert"></div>
        <button onclick="checkForm()">Create</button>
--- /code ---

</div>

Code snippet 2 adds the JavaScript that checks each field before showing the summary.

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 31
line_highlights: 32-34,36,38-44,46-52
---
// Function to check the character details form
const alertBox = document.querySelector("#alert");

function checkForm() {

  var alertMessage = "";

  if (characterName.value == "") {
    alertMessage = "Please enter a name";
  } else if (characterAbility.value == "") {
    alertMessage = "Please choose an ability";
  } else if (characterOrigin.value == "") {
    alertMessage = "Please write the origin story";
  }

  if (alertMessage != "") {
    alertBox.innerText = alertMessage;
    alertBox.style.display = "block";
  } else {
    alertBox.style.display = "none";
    displaySummary();
  }
}
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Click Create with one field left blank and confirm a warning appears instead of the summary, then fill every field in and confirm the summary appears.

--- /task ---
