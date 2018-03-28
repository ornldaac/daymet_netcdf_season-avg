# Python Methods to Derive a Seasonal Mean from Daymet Data - Reading/Writing netCDF

*Author: ORNL DAAC*  
*Date: February 28, 2018*  
*Contact for ORNL DAAC: uso@daac.ornl.gov*  

### Keywords: Daymet, Python, netCDF, THREDDS

## Overview

These tutorials demonstrate how to use the Python netCDF4 and numpy modules to work with a dataset in netCDF file format using N-dimensional array objects. Python numpy array methods are shown that open and subset a temporal range from a gridded multidimentional netCDF file. The example uses data from the maximum temperature variables of a dataset (Daymet) that contain daily gridded meteorologic data. In the first tutorial, a summer average maximum temperature is created and the results saved into a new netCDF file. A second tutorial condenses introductory information and demonstates how to loop through more than one year of data.


![Max Temp Avg, Summer 2016, GSMNP](NCSS_GSMNPsubset.png)

## Source Data

Spatial subsets of the North American Daymet dataset daily data: https://daymet.ornl.gov.

For these tutorials, spatial subsets were obtained from the ORNL DAAC's THREDDS netCDF Subset Service (NCSS). A tutorial of the NCSS is available [here](https://daymet.ornl.gov/web_services.html) under the "Gridded Subsets" tab: . 

You can download the 2015 maximum temperature Daymet subset data used in these tutorials by pasting the following HTTP GET NCSS Request URL into a browser:\
https://thredds.daac.ornl.gov/thredds/ncss/ornldaac/1328/2015/daymet_v3_tmax_2015_na.nc4?var=lat&var=lon&var=tmax&north=36.61&west=-85.37&east=-81.29&south=33.57&disableProjSubset=on&horizStride=1&time_start=2015-01-01T12%3A00%3A00Z&time_end=2015-12-31T12%3A00%3A00Z&timeStride=1&accept=netcdf

Daymet subset data for 2016 can be downloaded by updating the URL above to the 2016 dataset path and changing to 2016 in the time_start and time_end parameters.

## Prerequisites

Python 2.7 or later. Python modules: netCDF4, numpy, matplotlib, pylab, datetime

## Procedure

You can access the two tutorials here:
[Tutorial 1](daymet_netCDF_season-avg.ipynb)
[Tutorial 2](daymet_netcdf_season-avg-loopyrs.ipynb)