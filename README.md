# CSS Specificity Gotcha: Unexpected Style Overriding

This repository demonstrates a subtle issue related to CSS selector specificity and the order of rules within a stylesheet.  It highlights a scenario where the order of selectors does not affect the final specificity decision which may be counter-intuitive to some developers.

The `bug.css` file contains the problematic CSS, while `bugSolution.css` offers a clearer way to write such CSS to prevent unexpected outcomes.

**Key Concepts:**

* **CSS Specificity:**  Understanding how the browser determines which style rules to apply when conflicts arise.  The order of CSS rules does not influence specificity directly, although it plays a role in the case of equal specificity.
* **Selector Specificity:** Different selectors have different weights (IDs have higher weights than classes, and classes have higher weights than element selectors).
* **Cascading Style Sheets:** CSS operates on a cascading system where later rules can override earlier ones, but only if they have higher or equal specificity. 