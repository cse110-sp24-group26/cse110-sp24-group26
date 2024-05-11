# Meeting Minutes

## Meeting Information

**Meeting Date/Time:** May 10th 2024, 6:00PM - 7:00PM  
**Meeting Purpose:** Finish CI/CD assignment, Discuss tool choices  
**Meeting Location:** Zoom  
**Note Taker:** Jason

## Attendees

**Attended**:

- Manu
- Jason
- Pranav
- Viann
- Ekin
- Angel
- Suhaib

**Missing**:

- Luis
- Santiago
- Angelo

## Agenda Items

- **Dicuss testing framework choice**
  - Jest: Everyone has experience, well-rounded, simple
  - Cypress: Easy to learn, integrable, some cool functions
  - Descision doesn't matter to much
  - Going with Cypress to do unit tests, e2e tests, and component tests
  - Testing locally and upon pull requests
- **Discuss database choice**
  - IndexedDB: requires no dependencies, easy search, storing file blobs
  - Not using local storage
- **Discuss non functional features**
  - Performance
    - Load within 1s on 2015pc 3G internet?
    - Small bundle size, less than 5KB?
    - Shouldn't use more file storage space than necessary
  - Accessiblity
    - Works in an offline and mobile environment
    - Doesn't depend too much on javascript, graceful degradation
    - Doesn't depend on external fonts, has backup fonts
    - Keyboard navigatable, dark mode, colorblind mode???
    - Works on different devices
    - Uses proper HTML semantic tags
- **Finish CI/CD assignment**
  - Create Github Issue
  - Test locally
  - Push to feature branch
  - Pull request to dev branch, needs one approval and passing github actions
  - Pull requests need 3 ppl approval to merge into main
  - Diagram in repo
- **Discuss Github Issues and Commits**
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

## Action Items

- **Manu**:
  - [ ] Due: End of the day || Finish CI/CD stuff, inform TA
- **Jason**:
  - [ ] Due: End of tomorrow || Push meeting minutes, send recap and action items, documentation assignment
- **Everyone**
  - [ ] Due: End of the day || Finish filling out the when2meet

## Other Notes & Information

N/A
