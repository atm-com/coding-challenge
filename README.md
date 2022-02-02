# ATM Coding Challenge
We are going to build backend, frontend, or data tooling for a publically available Geo resolution API, [GeoJS](https://www.geojs.io/docs/v1/endpoints/geo/). We will use this API to retrieve the country and city associated with any IP address.

We are looking for the following
- Design choices
- Coding style, quality, and readability
- Testing
- Documentation around design trade-offs you made, or any other considerations you want to call out
- Bonus: Edge cases and completeness

This should not take you more than 2 hours. When you are done, push your solution to a public Github repository (preferred) or share a .zip file.

## Backend Challenge
Build a REST API (Ruby on Rails preferred) that allows users to submit IP addresses. Fetch the country & city from GeoJS and store the results in a server memory cache. The IP addresses and their data do _not_ need to be persisted to a database. A second end point should allow users to see all previously queried IP addresses alongside relevant data. The user should also be able to filter these IP addresses by country & city. Each API should return JSON.

## Frontend Challenge
Build a standalone frontend app using [GatsbyJS](https://www.gatsbyjs.com/) that allows users to input an IP address. You can retrieve the country & city from GeoJS and show them on the page. The page should show all the input IP addresses and the country & city associated with them.

## Data Engineer
Build a python script that reads a list of IP addresses from a file. Fetch the country & city from the GeoJS endpoint and write out these IP addresses to file by city & country. Each file name will be the country name (or city name if its by city), and will have a list of IPs that belong to that city.
