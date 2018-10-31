# Spatial CIMIS Parser

This package provides a python API to access gridded Spatial CIMIS data in a tidy tabular format.

### Motivation

The California Department of Water Resources already offers an [API](http://et.water.ca.gov/Rest/Index) to access data from the CA Irrigation Management System (CIMIS). The existing API provides access to 

* **CIMIS station** data by station
* **Spatial CIMIS** data by 
    - coordinate (lat/lon)
    - street address
    - zip code

However, for some applications it is more useful to have access to the raw grid of Spatial CIMIS readings accross the entire state of California. 


### Details

This python package pulls the grid files (.asc) from the [Spatial CIMIS FTP server](http://cimis.casil.ucdavis.edu/cimis/) and reformats them as tidy tabular data in a `pandas` DataFrame for easy analysis.
