# Documentation on Data Creation for Mapping Black Boston Project

## Finding Address for an Individual or Entity
1. Find the Boston Directory for the apporpriate year.
2. Search for the individual's name in directory. For businesses, there is a Business Director. There are often also sections for churches, schools, etc.
3. Record the listed address, using middle initials or details when necessary. 

## Finding Lat/Long for an Address
1. If you are unfamiliar with the street in the address, search for it in Google Maps or Open Street Map. If the street is in the same place as it was at the time of this address, go to step 3. If not, go to step 2.
2. Using the Boston Directory for the year of this address, find the street in the Streets section. This section is usually near the beginning. It lists all the streets and alleys and describes their location. Use this info to find the street on the McIntyre or another map closer to that year.
3. Load the tiles for the McIntyre or earlier map into QGIS as an xyz layer as well as an appropriate atlascope layer.
4. Find a control point for an address you know on this street. This may be an address already in the spreadsheet, an address verified through one of the sources below, or an address you can gather from the Streets section of a Boston Directory.
5. If this numbering matches the numbering on the atlascope layer, use that numbering to locate your street address. Go to step 7.
6. If this numbering does not match the numbering on atlascope, estimate the location based on other control points and the building footprints on the McIntyre map. For addresses in Beacon Hill, use the path-wise census data to help count the number of buildings between cross streets.
7. Right click to copy the WGS84 coordinates.
8. Copy and paste the lat/long into the columns of pois.csv.

## Useful resources for finding control points
- [Numbering for Washington Street in 1851](https://archive.org/details/bd-1851/page/60/mode/1up)
- [Numbering for some downtown streets in 1851])https://archive.org/details/bd-1851/page/61/mode/1up)
- [Kathryn Grover and Janine V. da Silva, "Historic Resource Study, Boston African Ameican National History Site," 31 December 2002](https://www.nps.gov/parkhistory/online_books/bost/hrs.pdf)

## Finding Lat/Long for Schools
1. Using the [1847 Reports of the Annual Visiting Committees of the Public Schools](https://archive.org/details/annualreport1847bost), identify the street on which the school was listed.
2. Load the atlascope and McIntyre xyz layers into QGIS. 
3. Using the atlascope layers, see if the school was still on that street in the 1860s or 1870s. 
4. If so, compare that location to what if any information is on the 1852 McIntyre map. If not, work directly from the McIntyre map.
5. Right click to copy the WGS84 coordinates.
6. Copy and paste the lat/long into the columns of pois.csv.

## Getting IIIF links
1. Visit https://digital.bodleian.ox.ac.uk/manifest-editor/#/?_k=5v9mdg
2. Copy in the IIIF manifest link: 
- Example: https://iiif.lib.harvard.edu/manifests/drs:486018367
- https://iiif.lib.harvard.edu/manifests/ids:1042518
3. If it’s a book, navigate to the right page
4. Under canvas metadata, go to Image URI. If you want the full picture, copy the whole link. If you want to zoom in to a particular crop, copy the whole link that ends right before /full 
- Example https://ids.lib.harvard.edu/ids/iiif/486018377/full/full/0/default.jpg copy just https://ids.lib.harvard.edu/ids/iiif/486018377
- Paste that link into the end of the URL for the IIIF Image Manipulation Tool: https://jbhoward-dublin.github.io/IIIF-imageManipulation/index.html?imageID=https://ids.lib.harvard.edu/ids/iiif/486018377
- Crop to the area of your choice
- Copy the link at the bottom of the page. This is the link to put in the Airtable.

- Digital commonwealth: https://www.digitalcommonwealth.org/search/commonwealth:668305767/manifest


# Example h1

- example bullet points
- example bullet points

## Example h2 

1. example ordered list
2. example ordered list

*italics*
**bold**

> aside

![picture alt text](documentation-images/example.png)

[hyperlink display text](www.google.com)