# Tailwind CSS @apply Directive Silent Failure
This repository demonstrates a subtle bug in Tailwind CSS where using the `@apply` directive with a non-existent class results in no error or warning, making debugging challenging.  The absence of any feedback makes it difficult to identify typos or missing classes.

## Reproducing the Bug
1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the div element lacks the expected styling because `my-nonexistent-class` does not exist.

## Solution
The solution involves carefully checking for typos in your class names and ensuring that all classes referenced by `@apply` are correctly defined in your Tailwind configuration.  More robust build processes with linters or dedicated Tailwind plugins could help catch these errors earlier in the development process.