# Spatial CIMIS Parser

This package provides a python API to access gridded Spatial CIMIS data in a tidy tabular format.

### Motivation

The California Department of Water Resources offers a [great API](http://et.water.ca.gov/Rest/Index) to access data from the CA Irrigation Management System (CIMIS). This API provides access to CIMIS station data as well as Spatial CIMIS data by coordinate (lat/lon), street address, and zip code.

For some applications, it is more useful to have access to the raw grid of Spatial CIMIS readings accross the entire state of California, and that's where this package comes in. This python package pulls the grid files (.asc) from the [Spatial CIMIS FTP server](http://cimis.casil.ucdavis.edu/cimis/) and reformats them as tidy tabular data into a `pandas` DataFrame.
