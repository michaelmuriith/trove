# Coding Standards

## File Naming
- Use descriptive, PascalCase file names for classes and modules.
  - For example, `UserProfileService.ts`.

## Variable Naming
- Use self-descriptive names for variables, functions, and classes.
  - Choose names that clearly convey the purpose and usage of the code element.
  - For example, use `userProfileData` instead of `data` or `temp`.
  - Function names should indicate actions and start with a verb.
    - For example, `getUserProfile()`, `calculateTotalAmount()`.

## Indentation
- Use 2 spaces for indentation. Avoid tabs.

## Braces and Spacing
- Use braces for control structures (if, loops, functions) even for one-liners.
- Place opening braces on the same line as the control structure.
- Use a space after keywords like `if`, `else`, `for`, `while`.
  - For example:
    ```typescript
    if (condition) {
        // code here
    } else {
        // code here
    ```

## Comments
- Use meaningful comments. Comments should explain why the code is doing something if the code isn't self-explanatory.
  - For example, complex algorithms, important decisions, or workarounds.
- Avoid redundant comments that simply restate the code.
- Comments should be placed above the code they explain and indented at the same level as the code.

---

**End of Standards**
