# COVID-19-twitter-tracker
School project for web mining course

## Summary
This final project would entail mining twitter for COVID-19 related tweets, and comparing the volume of tweets with the current number of cases as well as the number of deaths from COVID-19 in the country of origin. The aim of this project is to either establish or refute the connection between tweet volume and infection rate, and discern whether tweets about COVID-19 are reactionary or possibly predictive in some way, or otherwise unconnected.
## Data
Data will be sourced from twitter using tweepy to keep things simple and manageable, and will cover a dictionary of tags related to COVID-19. Tweets will be normalized by population and twitter usage within a country to ensure countries with higher average tweet volumes in general are not inflated.
COVID-19 infection data will be retrieved using an existing API (which incidentally seems to use Beautiful Soup) that aggregates Chinese city level infection, and outside country level infection reports.
The major variables that are going to be used for analysis will be the change in tagged tweets by country (normalized to twitter use per capita) and change in reported COVID-19 cases and deaths by country (possibly per capita). Granularity of the time step is uncertain at this time.
## Visualization
Ideally I’d like to create a web based interactive map, that compares a map of COVID-19 cases/deaths with a map of related tweets, with a timeline that can be scrubbed through. This will most likely use Google Charts’ geomap visualization.
### Possible Challenges
* Assessing tweet volume and origin at a large scale may be computationally difficult
* Access to COVID-19 infection data may be inaccurate or unreliable updated

Inspired by Influenza prediction using twitter:
https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.468.4738&rep=rep1&type=pdf
