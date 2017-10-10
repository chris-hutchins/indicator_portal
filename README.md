# Process for updating NHS Digital Indicator Portal datasets for data.gov.uk

At present the following domains are included: NHSOF, CCGOIS, POMI.
Each month, the portal is updated. DGU can harvest the metadata for these domains, as long as there is an associated json file.
The indicator portal produces xml schemas for each indicator, so the general process is to convert the xml schemas into a json file capable of being read by DGU.
This is acheived by the following steps:
1. Combine the xml schemas for the individual indicators within each domain , so that there is one schema per domain
2. Utilise Google Refine to convert this xml to a json file
3. Save the json file to github
4. Refresh the harvests within DGU.


## 1. Combine the xml schemas
