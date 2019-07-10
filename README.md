# Bielinski - Schema for Templates

**Creation Date:** 2019.06.18  
**Updated:** 2019.07.09  
**Version:** 1.0.1  
  
	
## Description
Code that will be used in templates to include schema.org data on
the Bielinski website.


## Use
Code should be placed into the CMS templates and auto-populated with
data pulled from the house/condo/apartment.


## Examples
`home-condo.json` shows sample for [The Arabella](https://www.bielinski.com/new-homes/buy-a-redihome/RediHome-Details.aspx?p=7083)  
`apartment.json` shows sample for [River Park Place](https://www.bielinski.com/Apartments/River-Park-Place.aspx)

## Changelog
**v1.0.2** - (Date: 2019.07.10)  
Removed `publicAccess` from `apartment.json`  
Changed `address` to use text rather than `PostalCode` in`apartment.json`  
No schema for Townhomes so using:  
```
"@additionalType" : {"Townhouse": "https://www.wikidata.org/wiki/Q1202402"},
"@type" : "Townhouse",
```	

**v1.0.1** - (Date: 2019.07.09)  
Made change to `hasMap` URL to work with latitude and longitude.  

**v1.0.0** - (Date: 2019.06.18)  
Initial creation and validation of the schema.org scripts.  
Validated with Google's schema checker.  