- What was the most challenging part of this assignment? Did you find HTML and CSS easy or difficult to work with?
    - The most challenging aspects of this assignment were implementing the grid layout and writing the logic to compare the user's input against the correct answers. CSS layout was particularly difficult—the grid items wouldn't stay aligned, and small CSS tweaks often broke the page structure. Additionally, I found it confusing at first to manage the HTML syntax, specifically when assigning and targeting the right IDs and classes for the input elements.


- How did you build the puzzle grid, and what other options did you consider?
    - I built the puzzle with CSS Grid: one `.puzzle` container uses `display: grid` and `grid-template-columns: repeat(5, 1fr)` to hold 25 squares (17 open and 8 blocked), and an `@media` query shrinks them from 100px to 56px so the grid fits on a phone. Each open square holds an `<input type="text" maxlength="1">` with an `aria-label`, so visitors can click or tab into it and type one letter. To check answers, every input has a `pattern` with the correct letter, and the `:valid` and `:invalid` pseudo-classes turn the square green or pink. 
    I also considered an HTML `<table>`, but tables are meant for data rather than layout, and Flexbox with `flex-wrap`, but I would have had to calculate every square's width myself. I chose CSS Grid because one line of CSS creates all five columns and places every square automatically.


- What did you take into account when designing the site? Is there anything you are particularly proud of?
    - I write my own design document at first, and keep those points in mind. I wanted all four pages to feel like one site, so they share the same font, light background, centered layout, and navbar, and the text pages use the same white cards with rounded borders. Every page has a viewport tag, and `@media` queries shrink the puzzle squares and reshape the navbar so nothing scrolls sideways at 320px. I am most proud that the puzzle checks answers with only HTML and CSS, using `pattern` with `:valid` and `:invalid`, because at first I did not know this was possible without JavaScript. Even this idea was inspired by AI, I am still proud of that I deploy it successfully on my page.



- Given more time or resources, what would you add?
    - If more time is given, I would add background picture for the pages, instead of using plain white.
Besides, I also plan to add a validation feature for the puzzle. If the user prompts with all correct answer, I want the page to generate a dynamic pattern design, showing `Congratulations` or `Navigate to next level`.



- How many hours did you spend on this assignment? (obviously just a sentence is sufficient)
    - Around 20 hr.



- If you used code or design from anywhere online (including AI), say so here. If you imported a font or icon library, or adapted an existing puzzle, note that as well
    - I use Claude to generate the answer and clue in the puzzle for me. Besides, I also ask Claude to guide me to properly use '@media' and give me hints in validating user's answer ,and using `placeholder` to keep the grid white before the user make any input or delete their input.