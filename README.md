# 473projectfinal
## Project goal
The ultimate goal of this project was to show all we've learned on Python, which we showed through plotting weather maps, comparing forecast data to verification data, and calculating the mean absolute error of model runs, among other things.

All of this was made possible by the several libraries that were imported, which include pandas, matplotlib, cartopy, xarray, and, perhaps most importantly, Herbie. These libraries streamlined the processing of weather data and made the process much easier and more accessible to those who are just learning Python.
## What does the code do?
### Milestone 1
Herbie was used to fetch an ECMWF forecast dataset (run at 2024-01-13 00z) as well as a verification dataset to be used for plotting. A custom colormap was used to plot the forecast and verification (as well as the difference) of the 500 mb heights at 0, 72, 144, and 240 hours. An attempt was made at obtaining a reanalysis dataset to use as the verification dataset, but we were unsuccessful.

### Milestone 2
Using the same ECMWF dataset, a new parameter (300 mb winds) was obtained and an xarray was created. At the KUNV grid point, a plot of the forecast error vs the forecast hour was created to show the decreasing acccuracy of the model with time. Plots of the CONUS were also created to show the short-range (fhr 6-60), medium-range (fhr 66-144), and long-range (fhr 152-240) mean absolute error across the US, to show what regions and/or events the model had the least/most trouble forecasting. A line chart of the Root Mean Square Error was also created to show the average error across the CONUS at each forecast hour. All of this was analyzed for 00z on 2024-01-13. This same process was repeated for another parameter (2m temperature), another run (12z on 2024-01-13), and another model (the GFS). When comparing the RMSE of the ECMWF and the GFS, it was found that for this time period, the GFS had an overall higher error than the ECMWF.
