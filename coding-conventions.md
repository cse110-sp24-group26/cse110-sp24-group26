# Coding Conventions

## HTML, CSS, JS

- Tab size: 4 spaces
- Lines less than 100 characters
- pascalCase
- Same line curly braces
- Every function is documented, summary for complex files and funcctions with additional comments for complex logic, present tense
- Include examples in comments for complex functions
- Code is as self-documented as possible
- Avoid hard-coded values, use variables for constants

## Git

- Feature branch for every feature, merge that into staging/development branch, approved by someone other than you
- Merging into main requiring two approvals
- Commit early and often, every commit does one thing
- Commit messages should mention what the commit is for, then add details in description/body, present tense
- Make github issues for every single thing we do
- **Github Issues and Commit Templates**
  - Commit template:

  ```Markdown
  # Title: Type of commit (issue adressed), Summary, imperative, start upper case, don't end with a period
  # No more than 50 chars. #### 50 chars is here:  #

  # Remember blank line between title and body.

  # Body: Explain *what* and *why* (not *how*).
  # Wrap at 72 chars. ################################## which is here:  #
  ```
  
  - Issue templates:

    - Feature:

    ```Markdown
    # Summary of feature
    # Expected difficulties
    # Reference/example of similar feature from another app
    ```

    - Bug:

    ```Markdown
    # Summary of Issue
    # Expected Behavior
    # Current Behavior
    # Steps to reproduce (How is the bug displayed)
    ```

    - Documentation:

    ```Markdown
    # Affected modules
    # Summary of Documentation necessary
    ```

    - DevOps:

    ```Markdown
    # Type of DevOps
    # Current behavior
    # New behavior
    ```

    - Testing:

    ```Markdown
    # Type of testing
    # Affected modules
    # Example test cases
    ```
