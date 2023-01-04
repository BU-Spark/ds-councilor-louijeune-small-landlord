##Overall goal
-----------------------

Build an inventory of the affordable units. 

We want to focus on the quality of the data. It's okay to miss some properties, but knowing where it comes from and representing it as accurately as possible is important.

- This means being clear on definitions, where datasets come from.

##Datasets
--------------------------

[Property Assessment Database](https://data.boston.gov/dataset/property-assessment/resource/4b99718b-d064-471b-9b24-517ae5effecc)

Our primary database of rental properties.

[Boston Assessors Database](https://data.boston.gov/dataset/property-assessment/resource/4b99718b-d064-471b-9b24-517ae5effecc)

This has addditional helpful information, we can use it as an extension of the Property Assessment dataset. NOTE: Next week, Tom will help us work with this dataset depending on what we want to do with it.

[Income restricted housing dataset](https://data.boston.gov/dataset/income-restricted-housing)

An inventory of income-restricted units in Boston, which we will use to start as a fairly comprehensive list of these properties. These properties are "income-restricted" which is one definition of ours for affordable properties. 

[Neighborhoods Shape file](https://bostonopendata-boston.opendata.arcgis.com/datasets/3525b0ee6e6b427f9aab5d0a1d0a1a28_0/explore?location=42.312295%2C-71.056800%2C12.58)

##TODO
---------------------------

1. Geocode with geopy, Mapbox, or Google maps API.

2. We want to look only at *rental units* because these will be properties that are rented *from landlords*. We don't look at people who own their property and live in them themselves.

3. Group by neighborhood over ZIP.

4. Look at properties in the rental properties dataset, filter out affordable properties, filter out large properties (> 6 units). What's left is small rental properties that *could* be rented out affordably.
