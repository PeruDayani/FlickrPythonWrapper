# FlickrPythonWrapper
A iPython notebook to fetch, manipulate and store data from the Flickr API.

## Setup
1. Install Required libraries:
```
pip install csv
pip install json
pip install flickrapi
```
2. Create an account on Flickr.com and get your API keys. Copy-paste them into the corresponding code block.
```
# API Keys
api_key = "INSERT_YOUR_KEY_HERE"
api_secret = "INSERT_YOUR_SECRET_HERE"
```

## Overview
1. Flickr API: https://www.flickr.com/services/api/
2. We first use the [flickr.photos.search](https://www.flickr.com/services/api/flickr.photos.search.html) endpoint to get a list of image ID's corresponding to a search query. Eg: For a search query of 'Delhi, Street' all pictures on Flickr containing tags 'Delhi' and 'Street' were returned in paginated format. 
3. We then used the [flickr.photos.getInfo](https://www.flickr.com/services/api/flickr.photos.getInfo.html) endpoint to get all data attributes associated with each image.
4. All the data collected is stored in a photos_searchTerms_raw_page_number.csv file and cleaned filtered data is stored in photos_search terms_clean_page_number.csv
