# Pokemon-API-Scripts
Two scripts to ingest data from the Pokemon API, particularly species evolution data and endpoint counts.

## get_endpoint_counts.ipynb
This script reads all API services (endpoints) available within the Pokemon API and counts how many objects there are for each service.
My approach was to save the endpoint data within a list and leverage Pandas to convert it to dataframe for easier manipulation. I then iterated over the list to access the count object and stored the results in a new dataframe.

## pikachu_evolutions.ipynb
This script accesses heavely nested JSON objects - the species evolutions and their URLs. My approach was to locate the index of the specific evolution within the parent object and access the evolution and URL. Repeat this process for the next evolutions.


