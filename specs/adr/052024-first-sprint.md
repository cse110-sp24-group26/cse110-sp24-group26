# First Sprint Designs

## Context and Problem Statement

For our first sprint, we had a couple of people write the boilerplate code. We then split into teams to work on each feature. After out first meeting/standup for the sprint, we needed to iron out some of the design sepcifics for each feature.

## Considered Options

* Tags: User can create as many tags as they want.
* Tags: There are a hardcoded number of tags.
* Tags: Use ShadowDOM
* Tags: Do not use ShadowDOM
* Calendar: Label tags on days using color
* Editor: Use vanilla HTML/JS
* Editor: Use Eternal Dependencies

## Decision Outcome

Chosen option: "Tags: Hardcoded number of tags (6)", because implementing deleting tags will be difficult and it will allow us to hardcode the colors as well.

Chosen option: "Tags: Do not use ShadowDOM", because it is unecessary and simplifies code/design. It may also lead to some technical problems.

Chosen option: "Calendar: Label tags on days using color", because we can use a small amount of color to represent a tag. We do not need to display any more information. It alsow works well since we are ahrd coding colors.

Chosen option: "Editor: Use vanilla HTML/JS", because we want to simplify and have more control over our design and it is unecessary. 
