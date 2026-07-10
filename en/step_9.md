## Add a light mode switch to the character page

Open `character.html` and paste this switch container inside the header, just after `</nav>` and before `</header>`.

```html filename="character.html" line_numbers="true" line_number_start="25" line_highlights="25-31"
      <nav class="navbar" id="nav">
        <a href="index.html">HOME</a>
        <a href="character.html">CREATE CHARACTER</a>
      </nav>
      <div class="switch-container">
        <label class="switch">
          <input onchange="changeLightMode()" type="checkbox" id="lightModeSwitch">
          <span class="switch-slider"></span>
        </label>
        <span class="switch-label material-symbols-outlined">light_mode</span>
      </div>
    </header>
```

## Now run your code

Open `character.html` and confirm the same switch now appears in that page header as well.
