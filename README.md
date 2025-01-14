# CSS Specificity Bug: Unexpected Font Size Inheritance

This repository demonstrates a subtle bug in CSS related to specificity and inheritance.  A `<span>` element nested within a paragraph inherits a `font-size` from a distant ancestor element instead of its direct parent.  This is counter-intuitive and can lead to unexpected styling issues in web applications.

The `bug.css` file contains the erroneous CSS code, while `bugSolution.css` provides a corrected version.

The root cause is a specificity conflict in which a more general selector with higher specificity overrides the more specific but less specific selector.  The solution involves carefully adjusting the CSS to ensure that the intended styles are applied correctly based on the intended inheritance patterns.

This issue highlights the importance of understanding CSS specificity and inheritance to avoid unexpected styling behavior.