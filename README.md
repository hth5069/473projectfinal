# 473projectfinal
## Project goal
The ultimate goal of this project was to show all we've learned on Python, which we showed through plotting weather maps, comparing forecast data to verification data, and calculating the mean absolute error of model runs, among other things.

All of this was made possible by the several libraries that were imported, which include pandas, matplotlib, cartopy, xarray, and, perhaps most importantly, Herbie. These libraries streamlined the processing of weather data and made the process much easier and more accessible to those who are just learning Python.
## What does the code do?
### MS1
Herbie is used to fetch an ECMWF forecast dataset (run at 2024-01-13 00z) as well as a verification dataset to be used for plotting. A custom colormap is used to plot the forecast and verification (as well as the difference) at 0, 72, 144, and 240 hours.
