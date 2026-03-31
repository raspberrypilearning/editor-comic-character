<h2 class="c-project-heading--task">Add the footer to the home page</h2>

### Step 1

Open `index.html` and add this paragraph inside the empty `<footer>` so the home page has space for the current year.


<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 37
line_highlights: 38
---
    <footer>
      <p>Ⓒ <span id="copyrightYear"></span> Malik Johnson - All Rights Reserved</p>
    </footer>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

### Step 2

Click Run and confirm the footer now shows a copyright message on the home page, even though the year is still blank.
