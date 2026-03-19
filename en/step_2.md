<h2 class="c-project-heading--task">Add the footer to the home page</h2>

Add a copyright message to the footer of `index.html` so the home page has space for the current year.

--- task ---

Open `index.html` and add a paragraph inside the empty `<footer>`.

--- /task ---

<div class="c-project-code">

--- code ---
---
language: html
filename: index.html
line_numbers: true
line_number_start: 32
line_highlights: 33
---
    <footer>
      <p>Ⓒ <span id="copyrightYear"></span> Malik Johnson - All Rights Reserved</p>
    </footer>
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

--- task ---

Click Run and confirm the footer now shows a copyright message on the home page, even though the year is still blank.

--- /task ---
