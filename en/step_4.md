<h2 class="c-project-heading--task">Add form elements</h2>

Add the inputs your user will use to design their superhero.

--- task ---

In `character.html` give the Superhero character details section the id `"character-details"` 

Then add form elements so the user can:
- type a superhero name
- choose an ability
- write an origin story

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 22
line_highlights: 23-36
---
    <main>
      <section id="character-details"> <!--Superhero character details-->
        <label for="name-text">Superhero Name:</label>
        <input type="text" id="name-text">

        <label for="ability-choice">Ability:</label>
        <select id="ability-choice">
          <option value="">Choose an option</option>
          <option value="Flying">Flying</option>
          <option value="Invisibility">Invisibility</option>
          <option value="Time travel">Time travel</option>
        </select>

        <label for="origin-text">Origin Story:</label>
        <textarea id="origin-text" placeholder="Add your superhero origin story!"></textarea>
      </section>
    </main>
--- /code ---

</div>

--- /task ---

--- task ---

Add a `<button>` element with the event `onclick="displaySummary()"` below the origin story `div`. 

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 35
line_highlights: 37
---

        <label for="origin-text">Origin Story:</label>
        <textarea id="origin-text" placeholder="Add your superhero origin story!"></textarea>
        <button onclick="displaySummary()">Create</button>
      </section>

--- /code ---

</div>

--- /task ---


--- task ---

Add a new `<section>` element with the attribute `id="summary-section"`.

<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 35
line_highlights: 36-38
---
      
    </section>
    <section id="summary-section">
      <h2>Superhero Summary</h2>
      <p id="summary-paragraph"></p>
    </section>
    
--- /code ---

</div>

--- /task ---

--- task ---

Open `scripts.js`.

Use the `querySelector()` method to find:
+ The summary section element and assign it to the constant `summary`
+ The character details section element and assign it to the constant `characterDetails`

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 5
line_highlights: 9-11
---
// Create constants for superhero form
const summary = document.querySelector("#summary-section");
const characterDetails = document.querySelector("#character-details");

const characterName = document.querySelector("#name-text");
const characterAbility = document.querySelector("#ability-choice");
const characterOrigin = document.querySelector("#origin-text");
    
--- /code ---

</div>

--- /task ---

--- task ---

Use the `querySelector()` to find the `<p>` element with the attribute `id="summary-paragraph"`.

Assign the element to the constant `summaryParagraph`.

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 13
line_highlights: 15
---
    
// Function to display summary
function displaySummary() {
  const summaryParagraph = document.querySelector("#summary-paragraph");

}
    
--- /code ---

</div>

--- /task ---

--- task ---

Update the `.textContent` of the `summaryParagraph`.

**Notice:** The text content is inside backticks ``` ` ` ``` instead of using `" "` or `' '`.

<div class="c-project-code">

--- code ---
---
language: js
filename: scripts.js
line_numbers: true
line_number_start: 13
line_highlights: 17-19
---
    
// Function to display summary
function displaySummary() {
  const summaryParagraph = document.querySelector("#summary-paragraph");

  summaryParagraph.textContent = `Your superhero name is ${characterName.value}. 
  Their ability is ${characterAbility.value}. 
  Their origin story is ${characterOrigin.value}.`;

}
    
--- /code ---

</div>

--- /task ---

--- task ---

**Test:** Open the character page and check you can type a name, choose an ability, and write an origin story.

--- /task ---