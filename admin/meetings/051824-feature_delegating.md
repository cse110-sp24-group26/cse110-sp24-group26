# Meeting Minutes

## Meeting Information

**Meeting Date/Time:** May 18 2024, 1:00PM - 2:00PM  
**Meeting Purpose:** Development kickoff  
**Meeting Location:** Zoom  
**Note Taker:** Jason  

## Attendees

**Attended**:

- Manu
- Jason
- Angel
- Pranav
- Angelo
- Suhaib
- Luis
- Santiago
- Ekin
- Viann

**Missing**:

- N/A

## Agenda Items

### CI/CD Pipeline

- When creating feature, first create issue, then create branch
- Develop and test locally
- Push onto remote feature branch
- Submit pull request to staging branch, checks done automatically
- Get one person to review, merge into staging
- Test locally, submit pull request to main, get approved by 2 other people

### App Foundation/Structure

- Cypress directory is where all tests are
- Src is where the main project is where there's documentation and a readme, giving overview of how it's designed
- Single page app, so only one index.html file
- Message and event-based programming
- Subfolders containing scripting and styling for sections of the page
- Everything is done on native web components

### Planning/Delegating

- *Make sure you're doing everything with proper conventions, Think about tests but don't have to implement them because still early and might be futile*
- *Create your own branches from STAGING*
- **Calendar minimap: Ekin and Jason**
  1. By Monday, get a very basic calendar down (just able to scroll it and dates and whatever)
  2. Load tag content to dynamically render a given date
  3. Add event handling; when a date is clicked publish open date event, subscribe to tag change event to update a given date based on its tag
  4. Handle mobile layout of sidebar + dark theme toggle
  5. CSS to make it look good
- **Search + database: Luis, Manu, Pranav**
  - Manu: Handles main database
  - Pranav + Luis: work on html/js of the search results, plus the search querying
- **Tags and categories: Angelo and Viann**
  1. By monday, get just toggle on and off of tags working
  2. Later on, get it so you can add and remove tags (somehow)
  3. Even more later on, get it so syncs up with the database and general events
  4. Finally, get css working
- **Tabs: Angel**
  1. By Monday, probably get basic rendering of tabs and code structure
  2. At some point, get event handling working: whenever an open tab event is clicked, the tab list should update to mark it as selected and add it to the list if not already present. Conversely, if a tab is selected, then it should be the one publishing the openTab event so that main editor can react. Finally, it should subscribe to tagChanged events so it can update the individual tab colors
  3. Handle CSS styling and overflow and what not
- **Entries/Editor: Suhaib, Santiago**
  1. By Monday, get line numbers working?
  2. From there get event handling/life cycling working (initial page load, querying and  saving to database, responding to open Tab events)
  3. Get markdown syntax working 
  4. Css styling and making it look pretty

## Action Items

- **Tags Team**:
  - [ ] Due: Following Monday || Make tags and get toggling working
- **Calendar Team**:
  - [ ] Due: Following Monday || Get a basic calendar down, be able to navigate between months and days, representing real dates
- **Editor/Entries Team**
  - [ ] Due: Following Monday || Angel gets basic rendering of tabs, suhaib gets line numbering working
- **Database/Search team**
  - [ ] Due: Following Monday || Manu gets database working, pranav and luis get mock search ui working
