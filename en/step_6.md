## Let the user edit the summary

Add an Edit button and a function that hides the summary and shows the form again when the user clicks it.

Open `character.html` and `scripts.js` to add the Edit button and the `changeSummary()` function.

Code snippet 1 adds the Edit button to the summary section.

```html filename="character.html" line_numbers="true" line_number_start="37" line_highlights="40"
      <section id="summary-section">
        <h2>Superhero Summary</h2>
        <p id="summary-paragraph"></p>
        <button onclick="changeSummary()">Edit</button>
      </section>
```

Code snippet 2 adds the JavaScript that shows the form again when Edit is clicked.

```javascript filename="scripts.js" line_numbers="true" line_number_start="25" line_highlights="26-29"
// Function to edit summary
function changeSummary() {
  characterDetails.style.display = "flex";
  summary.style.display = "none";
}
```

## Now run your code

Create a superhero, click Edit, and confirm the form appears again so you can change the details.
