## Street Layers

Building a reliable historical geocoder for pre-1860s Boston requires careful, manual attention to detail, due to the lack of high-resolution map resources from that time, as well as the idiosyncratic ways nature of street development in Boston. 

Contained here are `course-street-grid` and `streets-complete`. 

The folder `course-street-grid` contains files from a first attempt at vectorizing streets from an 1852 map of Boston. This is a good basis for creating a geocoder, but more work is still required. Many of the line directions are backwards, the line segments are too long and not fine enough to run a successful geocoding process, and the file contains no start and end numbering for each segment.
- `McIntyre-first-draft.geojson` is the first draft of this historic street network file, abstracted from the [1852 McIntyre map in the Harvard digital collections](https://digitalcollections.library.harvard.edu/catalog/990093967530203941)
- `Match-test-1852.geojson` is an attempt to programmatically add the highest and lowest instance of addresses from the [1850 Directory of the City of Boston](https://catalog.hathitrust.org/Record/000499337). This yielded some results, but due to the lack of resolution in the original vectorized street grid, the results are not as precise as we would like them to be.
- `McIntyre-1852-working.geojson` is a cleaned up version of `McIntyre-first-draft`, and what we are using for doing large-scale GIS work on a small number of historically-relevant streets on Beacon Hill and in the West End. If you are involved in this project **this is the file to use** as a basis for geocoding. 

The folder `streets-complete` contains actionable street segments for this large-scale work, each of which have been historically verified across a number of sources, including NPS site reports, the Boston City Census, as well as other primary and secondary sources. 