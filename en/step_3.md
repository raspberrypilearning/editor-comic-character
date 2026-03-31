<h2 class="c-project-heading--task">Show the current year</h2>

Use JavaScript to fill the `copyrightYear` span with the current year automatically.

### Step 1

Open `scripts.js` and create a `Date` object before setting the footer text.


<div class="c-project-code">

--- code ---
---
language: javascript
filename: scripts.js
line_numbers: true
line_number_start: 1
line_highlights: 2-3
---
// Update Copyright Year function
const currentDate = new Date();
document.querySelector("#copyrightYear").innerText = currentDate.getFullYear();
--- /code ---

</div>

<h2 class="c-project-heading--task">Test</h2>

### Step 2

Click Run and confirm the current year appears in the footer on both pages.
