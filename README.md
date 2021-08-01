# python-api-challenge

This project analyzes data from the Weather API and uses the Google Maps API to map the data:

* [The Open Weather API](https://openweathermap.org/) tracks daily weather data and forecasts, historical data, etc.
* [Google Cloud Map APIs](https://console.cloud.google.com/google/maps-apis) is used for mapping weather data

For more information see the analysis in the `WeatherPy.ipynb` and `VacationPy.ipynb`  Jupyter Notebooks respectively.

## Prerequisites

To run this project the following tools are needed:

* Python (tested with v3.85, earlier versions may work as well, but have not been tested)
* Jupyter Notebooks and/or Jupyter Labs
* Anaconda is recommended though library dependencies can be installed individually as well.

## Usage

* Clone the respository
* Rename `api_keys.py.sample` to `api_keys.py`. Add your own API keys. 
* Open and run the `WeatherPy.ipynb` and `VacationPy.ipynb` respectively from Jupyter Notebook or Jupyter Labs. Note running `VacationPy.ipynb` without running `WeatherPy` first will map existing data from an existing `city_weather.csv`. For more current data, overwrite the `city_weather.csv` using the first cells in the `WeatherPy.ipynb` notebook.

## Known Issues

* In some cases data from previous Jupyter cells are used to calculate values in the current cell. As such make sure to run all above cells to obtain the correct output
* Displaying maps in Jupyter Labs can have issues. The user sees an error saying `Error displaying widget: model not found`. Various resources on the web point to solutions (eg. upgrading versions, rebuilding labs, etc), but none seemed to work. If you have issues the work around seems to be to use Jupyter Notebook instead.

## References

### WeatherPy References

The WeatherPy analysis made use of the following concepts and links in addition to the Pandas/Plotly documentation.

#### Matplotlib Markers

* https://matplotlib.org/stable/api/markers_api.html

#### Empty Column Types Reference

* https://stackoverflow.com/questions/36462257/create-empty-dataframe-in-pandas-specifying-column-types

#### Date Conversion and Formatting

* https://stackoverflow.com/questions/42400529/convert-seconds-to-datetime-without-dropping-the-microsecond-precision-using-p
* https://www.programiz.com/python-programming/datetime/strftime
* https://stackoverflow.com/questions/54350585/python-convert-2-digit-4-digit-year

### VacationPy References

* TBD