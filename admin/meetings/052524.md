# Meeting Minutes

## Meeting Information

**Meeting Date/Time:** May 25th 2024, 1:00PM - 2:02PM  
**Meeting Purpose:** First Sprint check-in  
**Meeting Location:** Zoom  
**Note Taker:** Jason  

## Attendees

**Attended**:

- Manu
- Jason
- Ekin
- Viann
- Suhaib
- Santiago
- Angel
- Pranav
- Luis

**Missing**:

- Angelo

## Agenda Items

### Review Minutes

https://canvas.ucsd.edu/courses/54609/assignments/778821

### Standup

- Calendar Team
  - Dates can be changed by navs or dropdown
  - Highlighting today's date
  - CSS effects with hovering and clicking
  - To do: Consistency with keeping track of current date and function call to communicate to the rest of the app, refactor code
- Tabs
  - Added basic functionality for adding tabs
  - displays a label for the date opened
  - Some styling for functionality
  - To do: Coordinate with calendar team
- Editor
  - Line numbers working, but a little overcomplicated so needs refactoring
  - Bold syntax highlighting
  - To do: Make headings a different color, add italics, change to monospace font, merge buttons with syntax highlighting
- Tags
  - Tags togglable and styled
  - To do: tag renaming
- Etc
  - Talk to Manu for integration details

### Retrospective

- What to Improve:
  - Going a biy below pace, integrating things a bti faster, but we can catch up pretty easily
  - Integration even though it's conceptually simple, will get messy, especially with styling
  - Haven't gone over fine details on how the different feature teams will come together for the final product
  - Make a markdwn file for a feature later on to explain its functionality at a high level.
  - Some teams aren't communicating with each other that much, at the very least tell each other what you're doing, your progress, what you guys need to work on, your approaches
  - Talk more and plan in the beginning
  - How different parts of the app are going to communicate with each other
  - Integration:
    - Message-based, calendar publishes an open tab event, tab opens a tab, editor opens cotnent, tags update which are toggled
    - Clicking another tab also publishes another open tab event, and calendar will also change the current highlighted date
    - Changing a tag updates the database, possibly, the tab list and calendar date can reflect these tag changes

### Merge into staging and Main

- Everyone submits a pull request into staging from respective feature branches
- Close corresponding issues
- Good work that there are no linting errors
- Approved pull request from staging into main, building website and documentation, successful!!!
- Fix editor

### Check-In Video

- Manu handles steps 1 2 and 4, fully integrating all the snippets
- Every subteam has one person making a snippet showcasing the feature, flexible with time

### Assign tasks for next week/sprint

- Calendar
  - Integrating with events
  - Experimenting tag colors on calendar
- Tags
  - Integrating with events
- Tabs
  - Integrating with events
  - Close button
- Search Team
  - UI
  - Database function
- Editor
  - Integrating with events and database rest of the app
  - Handle Markdown later on
- Manu
  - More comments and documentation with events
  - integration of css

## Other Notes & Information

N/A
