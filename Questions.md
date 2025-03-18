## What is the keyboard interaction missing?

The original accordion component was missing the following keyboard interactions:

Focus Navigation: Users cant not navigate through the accordion buttons when using the tab key because there were no proper focus styles or keyboard support.

Expand/Collapse: The accordion sections could not be toggled when pressing enter or space keys, which is a common accessibility requirement.

## What is the ARIA missing?

The original accordion component was missing key ARIA attributes required for accessible accordions:

"aria-expanded": This attribute was missing on the buttons to indicate a section was either expanded (true) or collapsed (false).

"aria-controls": This attribute was not used to link each button to the corresponding content, allowing screen readers to associate the button with the collapsible region.

"role="region"": The content sections didnt include region role to mark them as landmark regions for the screen readers.

"aria-labelledby": This was missing on the content sections to associate them with the corresponding buttons for screen reader users.
