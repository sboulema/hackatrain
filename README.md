# hackatrain
Repository used for the HackaTrain Contest

# Assignment

As a ParkNow backend developer I want to have a quick, easy, standardized way of importing zone files so that our zone datastore is easily kept up to date.

## Narrative
At ParkNow a large of part of the work we do revolves around having an accurate and updated datastore of parking zones. Luckily we do not have to drive around cities to count the number of parking zones, we get lists of parking zones delivered to us!
Unfortunately governments highly rely on their Microsoft Office environments, meaning we get the list of parking zones as CSV files.
This is where you come in!

We are looking for a quick and easy way to import these CSV files into our datastore, removing the chances of human mistakes in the process.

## Requirements / Acceptance criteria
- CSV file must be imported
- Each row must be inserted into the datastore
- Import tool must expose its own REST API so it can be easily used

## Information Security Requirements
The datastore is completely shielded of for security reasons and only exposes a REST API to make changes.

## Technical intake
- Until the datastore is finalized by the IT department we should mock the REST API it exposes so we can start with our assignment.

## Scope
- CSV import file - in scope
- Excel import file - out of scope for now

## Tasks
- Import CSV file
- Insert data into datastore
- Test
- Documentation

## Documentation
-

# References

- https://www.hackatrain.nl/toa/
