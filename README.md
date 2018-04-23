# HackaTrain 2018 Contest

Repository used for the HackaTrain Contest assignment. It contains the explanation of what is required to be delivered and the assets needed to complete the assignment.

## Assignment

> **As a** Hackatrain contestant<br/>
**I want** to have an easy, standardized way of importing location files<br/>
**So that** the location datastore is kept up-to-date

## Narrative

At Parkmobile a large part of the work we do revolves around having an accurate and up-to-date datastore of parking locations. Luckily we do not have to drive around cities to count the number of parking locations, we get lists of the parking locations delivered to us!
Unfortunately our clients highly rely on their Microsoft Office environments, meaning we get these lists of parking locations delivered as CSV files.

This is where **you** come in!

We are looking for a simple, yet effective way, to import these CSV files into our datastore, removing the chances of human mistakes in the process where ever we can.

### Requirements / Acceptance criteria

- All CSV asset files must be imported and processed
- Each row of location data must end up in the datastore
- The solution must at least expose the datastore REST API so it can be easily used by the import process
- Provide proof that your solution works

### Information Security Requirements

The datastore is completely shielded of from outside access for security reasons. We therefore need to expose a REST API to accept incoming changes.

### Technical intake

- Until the datastore is finalized by the IT/DBA department we should provide a mock for the datastore, so we can start with the assignment
- How to deal with invalid data?

## Scope

- Import all CSV asset files
- Import Excel files (out of scope for now)
- Mocked datastore

## Tasks

- Process CSV asset files
- Move data into datastore
- Create tests
- Write documentation

## Documentation

- Technical Specification
- Argument your design decisions
- Provide instructions on how-to run your solution

## References

- <https://www.hackatrain.nl/toa/>
- <https://en.wikipedia.org/wiki/Comma-separated_values>
- <https://en.wikipedia.org/wiki/Application_programming_interface>
- <https://en.wikipedia.org/wiki/Swagger_(software)>
