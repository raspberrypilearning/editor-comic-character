## Check the form before creating

Warn the user when they miss a field so the summary is only created after the form is complete.

Open `character.html` and `scripts.js` to add the warning area and the `checkForm()` function.

Code snippet 1 updates the form so the Create button runs `checkForm()` and there is a place to show the warning.

```html filename="character.html" line_numbers="true" line_number_start="33" line_highlights="35-36"
        <label for="origin-text">Origin Story:</label>
        <textarea id="origin-text" placeholder="Add your superhero origin story!"></textarea>
        <div id="alert"></div>
        <button onclick="checkForm()">Create</button>
      </section>
      <section id="summary-section">
```

Code snippet 2 adds the JavaScript that checks each field before showing the summary.

```javascript filename="scripts.js" line_numbers="true" line_number_start="31" line_highlights="32,34,36,38-44,46-52"
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
```

## Now run your code

Click Create with one field left blank and confirm a warning appears instead of the summary, then fill every field in and confirm the summary appears.
