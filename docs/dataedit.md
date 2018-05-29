# Update Application Data

TransitSphere was designed with exensibility in mind, especially for end-users, making it very easy to make changes to the data inside the application and rebuild the project. Instead of using a database, a simple online spreadsheet was used to hold all the information.

?> Currently the information is curated in [this Google Sheets file](https://docs.google.com/spreadsheets/d/1-aBL2tsKYet1vlc4ESGTYoNmt7wzVoDdmzv3PKZWjkU/) 

## Card Content

Each asset class in the application holds each of these attributes below.

| layer | head | text | anchor | extra | extext |
| ------|------|------|--------|-------|--------|
| contains ID of layer |  header text  |  primary card content  |  anchor to navigation   |   subheading     |  secondary text | 
| Bike_Ped | Bicycle and Pedestriand System | The Bicycle and Pedestrian System asset class serves ... | bike_ped | Accessible Seattle For Everyone | SDOT's Curb Ramp and Accessible Route Planner ... |
| ... | ... | ... | ... | ... | ... |

## Budget Data

Each asset the SDOT manages is also part of chart infographic within the application. The data for each asset is in the format below:

| Asset | Inventory | Replacement Value | Data Confidence | Good | Fair | Poor | Unknown | Asset Class | Asset Number |
|-------|----------:|------------------:|-----------------|-----:|-----:|-----:|--------:|-------------|-------------:|
|Bike & Pedestrian System | | 5,449.00 | | | | | | | 7 |
|Bicycle Racks | 3,301 | 2.20 | High | 978.00 | 0.01 | 0.01 | 0.01 | BIKE & PEDESTRIAN SYSTEM |
|Kiosk | 150 (e) | 1.10 | Low | 0.00 | 0.00 | 0.00 | 1.00 | BIKE & PEDESTRIAN SYSTEM |	
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |

The first line provides data for the asset class, which merely has _Replacement Value_ data for this entry. This is used in the highest level of the visualization. Data following the asset class is complete, utilizing all columns and will populate the 2nd and 3rd degress of nesting within the visualization.


## Configuration

To change/swap out the spreadsheet to hold the information you can simply edit the value of `sheets` in the `project.json` file.

```js
<!-- project.json -->
{
  "title": "SDOT Web Companion",
  "description": "",
  "url": "https://github.com/ibromley/sdot-webcomp/",
  "sheets": ["1-aBL2tsKYet1vlc4ESGTYoNmt7wzVoDdmzv3PKZWjkU"],
  "production": true,
  "embedded": false
}
```

!> Be sure to remember to [publish](https://support.google.com/docs/answer/37579) this file to the web, or else the grunt task will fail!