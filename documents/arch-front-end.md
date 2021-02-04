## Front End Architecture

### Brainstorming - Front End and UI

#### User Scenario
- Where I live right now- how bad will it be 20 years from now
- I want to see an overlay  of all the layers
- I want to see a combination of layers
- I want to know how to interpret what I'm being shown, a blurb would be nice
- No jargon, use simple language

#### Layers/ Data
All data represented as layers (color overlay/ icons/ text) on top of map. The map itself will not be altered 
(example - https://vancouver.ca/green-vancouver/sea-level-rise.aspx)


Some data represents events that are harmful in any context, these are medium - extreme weather events. 
Remaining data is context based, it is describing a part of the climate which at a reagional level would have different implications than at the global and climate level

Category: negative outcomes, weather events
- droughts
- floods
- hurricanes
- fires
- earthquakes
- tsunamis

Category: neutral, context based data
- temperature
- precipitaion
- humidity
more criteria TBD

Note: these categories are only to help with the designing of UX, 
not categories that will be used on the web app. On the webapp, we may list all options at the same level (no nesting)
show limitation in data - NA vs global

#### Feature: Map options
- Display a map
- A heading / title saying what the user is currently looking at
- Take an input for a city to focus the map on that region
- Display option for timeframes available
- The user can select between the current and the time frames to see the differencs
- List of criteria to add data layers for, on  the map
- When map is depicting future scenario, show an animation icon that allows the user to see current-> selected year, criteria animated.

#### Feature: User Education
- Side panel - with a blurb for the user. for example: additional rainfall and what that means reagionally and globally
- Each criteria should have a hover over box

#### Feature: Dropped Pins
- Top 10 cities - most affected by climate change (using over all livibility)
- Top 10 most resilent cities

#### Logic / Data units
- Select units to show
- Select what metric to show the difference in
  - rate of change
  - base unit
  - percentage change
- For each prediction - display probability and confidence (depends directly on the data used). Where to show this is TBD


#### Interesting but Out-Of-Scope

1. What will current city feel like in 10 years in terms of another present day city?
- User centers on city X
- User selects prediction timeframe of Y years
- Algorithm to compare the future conditions of city X and match with conditions of a current city
- Display the result to the user
- "In 10 years Austin, TX will have the climate of San Antonio, TX"

2. Ocean chemisty changes 
- Research - is there data available that's raw with clear models that we use to predict events and changes that can be shown to the user?
- Is there data available that uses this ocean chemistry data and predicts other climate trends it will contribute to?

