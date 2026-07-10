## Show the current year

Use JavaScript to fill the `copyrightYear` span with the current year automatically.

Open `scripts.js` and create a `Date` object before setting the footer text.

```javascript filename="scripts.js" line_numbers="true" line_number_start="1" line_highlights="2-3"
// Update Copyright Year function
const currentDate = new Date();
document.querySelector("#copyrightYear").innerText = currentDate.getFullYear();
```

## Now run your code

Click Run and confirm the current year appears in the footer on both pages.
