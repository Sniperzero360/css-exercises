# CSS Exercise #6

This exercise explores specificity and rule order in cascade. There are bugs in the specificity or rule order elements of the CSS files that we need to fix by adding, removing, or editing selectors for a declaration block, or by moving declaration blocks around. There is no need to edit the HTML file or any of the actual styles in the CSS.

The "cascade" is what determines what rules actually get applied to our HTML. There are different factors that cascade uses to determine this.

## Specificity

- A CSS declaration that is more specific will take precedence over less specific ones
- Inline styles have the highest specificity compared to selectors
- Each type of selector has its own specificity level that contributes to how specific a declaration is.
- ID Selector (most specific selector) > Class Selector > Type Selector
- Specificity will only be taken into account when an element has multiple, conflicting declarations targeting it, sort of like a tie-breaker.
- When there is no declaration with a selector of higher specificity, a rule with a greater number of selectors of the same type will take precedence over another rule with fewer selectors of the same type.

## Inheritance

Inheritance refers to certain CSS properties that, when applied to an element, are inherited by that element’s descendants, even if we don’t explicitly write a rule for those descendants.

- Typography-based properties (color, font-size, font-family, etc.) are usually inherited, while most other properties aren’t.

## Rule Order

Whichever rule was the last defined is the winner.