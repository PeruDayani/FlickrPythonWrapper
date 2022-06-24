# FlickrPythonWrapper
A iPython notebook to fetch, manipulate and store data from the Flickr API.

## Setup
1. Install Required libraries:
- pip install json
- pip install flickrapi
- pip install csv

2. Create an account on Flickr.com and get your API keys. Copy-paste them into the corresponding code block.

## Overview
Flickr API: https://www.flickr.com/services/api/
We first use the flickr.photos.search (https://www.flickr.com/services/api/flickr.photos.search.html) endpoint to get a list of image ID's corresponding to a search query. Eg: For a search query of 'Delhi, Street' all pictures on Flickr containing tags 'Delhi' and 'Street' were returned in paginated format.  
We then used the flickr.photos.getInfo (https://www.flickr.com/services/api/flickr.photos.getInfo.html) endpoint to get all data attributes associated with each image.
All the data collected is stored in a photos_{search terms}_raw_page_{number}.csv file and cleaned filtered data is stored in photos_{search terms}_clean_page_{number}.csv
