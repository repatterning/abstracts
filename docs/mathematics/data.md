# Data

## Sources

The data sources:

<table style="width: 85%; margin-left: 35px; vertical-align: top; font-size: .7rem;">
  <colgroup>
      <col span="1" style="width: 18.5%;">
      <col span="1" style="width: 43.5%;">
  </colgroup>
  <thead><tr style="text-align: left"><th>&nbsp;</th><th>Notes</th></tr></thead>
  <tr><td><abbr title="Scottish Environment Protection Agency">SEPA</abbr> Hydrometric Data</td>
      <td><a href="https://timeseriesdoc.sepa.org.uk" target="_blank"><abbr title="Scottish Environment Protection Agency">SEPA</abbr> API</a> &rarr;<br><a href="https://timeseriesdoc.sepa.org.uk/api-documentation/" target="_blank">application programming interface documentation</a>, <a href="https://timeseries.sepa.org.uk/KiWIS/KiWIS?datasource=0&service=kisters&type=queryServices&request=getrequestinfo" target="_blank">query service</a>, water levels (<a href="https://www.sepa.org.uk/environment/water/water-levels/">1</a>, <a href="https://waterlevels.sepa.org.uk/">2</a>), <a href="https://timeseriesdoc.sepa.org.uk/api-documentation/before-you-start/what-controls-there-are-on-access/">access controls</a>, <a href="https://timeseriesdoc.sepa.org.uk/api-documentation/before-you-start/how-data-validity-may-change/">river level data quality codes</a>, <a href="https://www.sepa.org.uk/environment/environmental-data/"><abbr title="Scottish Environment Protection Agency">SEPA</abbr> Environmental Data</a>, <a href="https://www.gov.uk/government/publications/uk-geospatial-data-standards-register/national-geospatial-data-standards-register">geospatial standards register</a>, <a href="https://waterdata.usgs.gov/blog/gage_height/">gauge height</a>, <a href="https://www.usgs.gov/media/images/gage-datum-reference-point">gauge datum reference point</a></td></tr>
  <tr>
    <td>Granular Catchment Polygons</td>
    <td><abbr title="Centre for Environment Fisheries and Aquaculture Science">cefas</abbr>, catchment boundaries (<a href="https://data.cefas.co.uk/view/21969" target="_blank">1</a>, <a href="https://data.cefas.co.uk/view/21970" target="_blank">2</a>)</td>
  </tr>
</table>

<br>

## Weather Warnings & Meteorological Office

[Meteorological Office Warnings Services](https://weather.metoffice.gov.uk/guides/warnings):

* [RSS feeds](https://weather.metoffice.gov.uk/guides/rss)[^materials-and-rss]
* [email alerts](https://www.metoffice.gov.uk/about-us/news-and-media/media-centre/subscribe-to-email-alerts)
* [National Severe Weather Warnings Service Public API](https://metoffice.github.io/nswws-public-api)

<br>

## Exploratory Analysis Methods

* [Partial Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/pmc/section4/pmc4463.htm).  [Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/eda/section3/autocopl.htm): For investigating questions such as[^auto-correlation]
    1. _Is an observation related to an adjacent observation?_
    2. _Is the observed time series white noise?_
    3. _Is the observed time series sinusoidal?_
    4. _Is the observed time series autoregressive?_

* [Statistical forecasting: notes on regression and time series analysis](https://people.duke.edu/~rnau/411home.htm)
    1. [Identifying the order of differencing in an ARIMA model](https://people.duke.edu/~rnau/411arim2.htm)
    2. [Identifying the numbers of AR or MA terms in an ARIMA model](https://people.duke.edu/~rnau/411arim3.htm)

* De-trending, etc.
    1. [Stationarity, De-trending, Tests](https://www.statsmodels.org/dev/examples/notebooks/generated/stationarity_detrending_adf_kpss.html)
    2. [Robust de-trending, re-referencing, outlier detection, and inpainting for multichannel data](https://pmc.ncbi.nlm.nih.gov/articles/PMC5915520/)

* [Model Identification for Southern Oscillations Data](https://www.itl.nist.gov/div898/handbook/pmc/section4/pmc4461.htm)

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>

[^materials-and-rss]: [Materials & RSS](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/#rss)
[^auto-correlation]: From NIST [Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/eda/section3/autocopl.htm)

<br>
<br>
