# Layered Architecture

## Description
- Organised in horizontal layer with each having its own specific role
- Seperation of concerns between each layer
- Usually have 3 or more layers such as Presentation layer, Business Layer, Database layer



## Concepts
- Have layers of isolation between each layers
  - A change in one layer usually does not affect the other layers, or minor impact to the other layers
  - Benefits from isolation reduce independecy in the program
 
## Consideration of implementation
- Good as a general-purpose pattern
- Need to make sure to not fall into an architecture sinkhole anti-pattern
  - Too many layers with little or no processing in the layer
- There may be request that falls into the sinkhole
    - Use the 80-20 rule to guage

## Overall statistics of the program
- Low ability to respond to changes
  - Monolithic structure + Tight coupling of components lead to high time consumption to make changes
- Low ease of deployment
  - Small change to one small component may lead to redeployment of the entire application 
- High testability
  - As each component is within individual layer, easy to test the specific layer function
- Low Performance
  - Inefficient as need to go through multiple layers
- Low scalability
  - Possible to scale by splitting the layered architecture into seperate physical deployment, but overall granularity too broad, expensive to scale
- High ease of development
  - Not complex to implement as well known, due to [conway's law](https://en.wikipedia.org/wiki/Conway%27s_law)
