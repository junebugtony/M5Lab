# Accessibility

## Overview

TODO: Write a project description

## Sources and Credits

- Contrast Checker: https://webaim.org/resources/contrastchecker

## Accessibility Lab Answers

**Color:**

- The contrast ratio tested for the provided foreground and background colors together provided me with a 2.79:1 ratio which fails all of the WCAG 2 guidelines. The provided background color for the comments section provided a contrast ratio of 12.13:1 which adheres to WCAG 2 guidelines. Both backgrounds were changed to white to increase readability.

![Alt text](/img/contrast_test.png)

**Semantics:**

- Personally for me, navigating the website using Tab was functional, starting from the tabs at the top and moving right then down the body section to the music player and comments section then back to the links on the right in the side panel. Shift + Tab went to previous elements, spacebar played media, and the enter key selected the tabbed element.

- During this section there were a few misspelled words like "encourage", "naturally", and "behavior".

- The table headers were set using td tags instead of header tag th.

- Font size was set in HTML rather than using header tags and adjusting the CSS styling afterwards.

- Breaks were used instead of paragraph tags.

**Images:**

- Images could be improved for screen readers by adding proper and descriptive alt text which were not done in the original HTML.