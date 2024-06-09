## Development Pipeline
1. During team meetings or on Slack, decide what needs to be worked on in terms of bugs, features, documentation, etc and create issues list
2. For each issue in the list, open an issue accoridng to one of several provided templates. If applicable make sure to assign the person working on that feature in the issue itself
3. Create a new branch for the issue from the issue page so that it is automatically linked and make sure to name the branch according to the conventions below 
4. Add issues to the team board by going to the backlog tab and following the given steps:
    -  Click Add item near the bottom of the "todo" section
    - Input "#" to bring up the repositories and select "final-project"
    - Then search for the brand new issue and select it to add it to the board
5. Develop on the branch and test locally, make sure to update the issue to "in progress" on team board
6. Push on the branch and submit a pull request to staging
7. GitHub actions will ensure that nothing goes wrong in terms of linting and testing
8. Have a manual review by at least one other person
9. Merge into staging
10. Have two other people manually review the staging branch to ensure no unexpected merge conflicts
11. Merge into main, update the issue to "done" on the team board
12. GitHub actions will build the documentation and website
13. Repeat for next issue from step 2 onwards

## Local Building
1. Clone [project repository](https://github.com/cse110-sp24-group26/final-project) locally
2. Use `serve src` serve the application on localhost (install [serve](https://www.npmjs.com/package/serve) if you don't have it already)
3. Use `npm update` to update install all dev dependencies
4. Use `npm test` to run the tests

## Other Info
See [README.md](https://github.com/cse110-sp24-group26/final-project/blob/main/README.md) for full information on our convention guides 
and other quirks of contribution.
