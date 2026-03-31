<h2 class="c-project-heading--task">Build the character form</h2>

### Step 1

Open `character.html` and replace the empty `<section>` with this superhero form and summary section.


<div class="c-project-code">

--- code ---
---
language: html
filename: character.html
line_numbers: true
line_number_start: 28
line_highlights: 28-47
---
    <main>
      <section id="character-details"> <!--Superhero character details-->
        <label for="name-text">Superhero Name:</label>
        <input type="text" id="name-text">
        <label for="ability-choice">Ability:</label>
        <select id="ability-choice">
          <option value="">Choose an option</option>
          <option value="Flight">Flying</option>
          <option value="Invisibility">Invisibility</option>
          <option value="Time travel">Time travel</option>
        </select>
        <label for="origin-text">Origin Story:</label>
        <textarea id="origin-text" placeholder="Add your superhero origin story!"></textarea>
        <button onclick="displaySummary()">Create</button>
      </section>
      <section id="summary-section">
        <h2>Superhero Summary</h2>
        <p id="summary-paragraph"></p>
      </section>
    </main>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

### Step 2

Click Run, open `character.html`, and confirm you can see a name field, an ability menu, an origin story box, and a Create button.
