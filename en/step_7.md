<h2 class="c-project-heading--task">Check user input</h2>

--- task ---
Warn the user if they miss an important part of the form.
--- /task ---

--- task ---
Create an alert message that appears if the user leaves the name, ability, or origin story blank.
--- /task ---

<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 31
line_highlights: 2-23
---
// Function to check the character details form 
const alertBox = document.querySelector("#alert");

function checkForm(){

  var alertMessage = "";

  if (characterName.value == ""){
    alertMessage = "Please enter a name"; 
  } else if (characterAbility.value == "") {
    alertMessage = "Please choose an ability";
  } else if (characterOrigin.value == "") {
    alertMessage = "Please write the origin story";
  } 
  
  if (alertMessage != ""){
    alertBox.innerText = alertMessage;
    alertBox.style.display = "block";
  } else {
    alertBox.style.display = "none";
    displaySummary();
  }
}
--- /code ---

</div>

--- task ---
**Test:** Try clicking **Create** with one field blank and check the correct warning message appears.
--- /task ---