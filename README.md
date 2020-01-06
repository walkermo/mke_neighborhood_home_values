# mke_neighborhood_property_value_analysis

This project uses Python and R to examine what variables influence median single-family property values of Milwaukee census tracts. It then seeks to compare a model's predicted value for a given tract to its actual value to get a sense of what neighborhood might be considered undervalued or overvalued. Although imperfect, city appraisal data is used for home values because it is the most comprehensive, publicly available dataset for all homes in Milwaukee. It also comes with the benefit of identifying a home's Census tract, which makes it easy to join with Census economic and demographic data as a well the police department's crime data.

The processing, cleaning and joining of the various datasets is done in the process_data.ipynb jupyter notebook.

The analysis and modeling is done in the analysis.Rmd file, which outputs the final analysis.html file.

This analysis includes the following datasets:
* Milwaukee master property file (Not uploaded here because of its size, though it can be [downloaded here from the city's data portal](https://data.milwaukee.gov/dataset/mprop))
* Crime incident data (Not uploaded here because of its size, though it can be [downloaded here from the city's data portal](https://data.milwaukee.gov/dataset/wibr))
* Educational attainment (U.S. Census)
* Household income (U.S. Census)
* Race and ethnicity (U.S. census)
* Milwaukee vacant properties (Can be downloaded from [the city's open data portal](https://data.milwaukee.gov/dataset/accelavacantbuilding))
* A Milwaukee County census-tract level GEOJSON file was created from a Wiscononsin tract-level shapefile downloaded from the Census website.

And while this might go without saying, there are certainly additional variables likely influencing property values that data used here doesn't account for.