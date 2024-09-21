# Webpage Accessibility

## Overview

This project consists of adjusting the provided webpage for better accessability and readability. We explore and implement various practices that allow this webpage to be viewed by sight and hearing impaired individuals as well as making it screen reader compatible.

**To view the webpage:**

Clone the repository locally.

Navigate to and open the cloned repository.

Start the live preview plugin on VSCode or live preview plugin in your IDE of choice.

Navigate to ```http://127.0.0.1:3000/index.html``` in your browser or view the webpage in the live preview window.

## Accessibility Lab Answers

**Color:**

- The contrast ratio tested for the provided foreground and background colors together provided me with a 2.79:1 ratio which fails all of the WCAG 2 guidelines. The provided background color for the comments section provided a contrast ratio of 12.13:1 which adheres to WCAG 2 guidelines. Both backgrounds were changed to white to increase readability.

![Alt text](/img/contrast_test.png)

**Semantics:**

- Personally for me, navigating the website using Tab was functional, starting from the tabs at the top and moving right then down the body section to the music player and comments section then back to the links on the right in the side panel. Shift + Tab went to previous elements, spacebar played media, and the enter key selected the tabbed element.

- During this section there were a few misspelled words like "encourage", "naturally", and "behavior".

- Font size was set in HTML rather than using header tags and adjusting the CSS styling afterwards.

- Breaks were used instead of paragraph tags.

- The nav section should be updated to use the nav tag instead of a div with class name "nav".

**Images:**

- Images could be improved for screen readers by adding proper and descriptive alt text which were not done in the original HTML.

**The audio player:**

- The audio clip could be improved for deaf and hard of hearing by providing a transcript below it.

- For browsers that don't support HTML audio, you can provide download links for the audio files instead.

**The Forms:**

- To add a label that is only accessible by screen readers we can use an ARIA label.

- You can achieve association with labels by using the label tag with a for such as label for="comments".

**Show/Hide Comment Control:**

- You can make the div tab selectable by adding tabindex="0".

- I put the toggle comment logic into it's own function, kept the comments hidden by default which I believe is not working properly because we are not waiting for the HTML code to load before javascript is ran. I then added an action listener for a key down event for the enter key to submit.

**The Table:**

- The table headers were set using td tags instead of header tag th.

- The table tag does not have a summary added to it, so I have added one for clarity and accessibility.

**Other potential improvements:**

- One potential improvement that could be made would be to add a custom color selector for the foreground and background so users can adjust the colors to their preferred liking.

- Another potential improvement would be to set the webpage up to load all of the HTML elements first before then performing the Javascript. This would require some restructuring of the javascript file but could be worthwhile depending on how much script will be ran on the webpage.

## Sources and Credits

- Contrast Checker: https://webaim.org/resources/contrastchecker
- Aria Labels: https://stackoverflow.com/questions/26032089/in-html-how-can-i-have-text-that-is-only-accessible-for-screen-readers-i-e-fo
- HTML Tables: https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics
