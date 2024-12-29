# Tailwind CSS JIT Mode: Unexpected Behavior with @apply and Responsive Modifiers

This repository demonstrates an uncommon bug encountered when using `@apply` directives within responsive modifiers in Tailwind CSS's JIT mode.  The issue arises from the order of operations within JIT and how it handles the cascading of styles with responsive directives.

## Bug Description

The primary problem is that `@apply` directives, when used inside responsive modifiers, do not always behave predictably.  Styles might be overridden unexpectedly, or might not be applied at all.

## Reproduction

1. Clone this repository.
2. Run `npm install` (or your preferred package manager) to install Tailwind CSS.
3. Open `bug.html` in your browser. Observe the unexpected styling behavior.

## Solution

The recommended solution is to avoid nesting `@apply` directives inside responsive modifiers.  Instead, apply styles directly or utilize a more straightforward approach to achieve the same responsive styling effect.  See `bugSolution.html` for a corrected implementation.