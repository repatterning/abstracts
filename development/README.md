<br>

<b>Notes</b>


## References

### SEPA, etc.

Scottish Environment Protection Agency (SEPA):
* [Application Programming Interface](https://timeseriesdoc.sepa.org.uk/api-documentation/)
* [Query Service](https://timeseries.sepa.org.uk/KiWIS/KiWIS?datasource=0&service=kisters&type=queryServices&request=getrequestinfo)
* [Water Levels](https://www.sepa.org.uk/environment/water/water-levels/)
  * [Water Levels](https://waterlevels.sepa.org.uk/)
* [Catchment boundaries for Scotland based on Scottish Environment Protection Agency (SEPA) catchments (WGS84) 2023](https://data.cefas.co.uk/view/21970)
* [Environmental Data](https://www.sepa.org.uk/environment/environmental-data/)
* [Geospatial Standards Register](https://www.gov.uk/government/publications/uk-geospatial-data-standards-register/national-geospatial-data-standards-register)
* [Access Control](https://timeseriesdoc.sepa.org.uk/api-documentation/before-you-start/what-controls-there-are-on-access/)
* [Quality Codes](https://timeseriesdoc.sepa.org.uk/api-documentation/before-you-start/how-data-validity-may-change/)
* [Gauge Height](https://waterdata.usgs.gov/blog/gage_height/)
  * [The Reference Point](https://www.usgs.gov/media/images/gage-datum-reference-point)

<br>

Time Series Modelling & Analysis:
* [Forecasting Principles & Practice: Stationarity](https://otexts.com/fpp2/stationarity.html)
* [Stationarity, De-trending, Tests](https://www.statsmodels.org/dev/examples/notebooks/generated/stationarity_detrending_adf_kpss.html)
* [Model Identification for Southern Oscillations Data](https://www.itl.nist.gov/div898/handbook/pmc/section4/pmc4461.htm)
* [Robust de-trending, re-referencing, outlier detection, and inpainting for multichannel data](https://pmc.ncbi.nlm.nih.gov/articles/PMC5915520/)
* [Using ARIMA and ETS models for forecasting water level changes for sustainable environmental management](https://www.nature.com/articles/s41598-024-73405-9)
* [Partial Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/pmc/section4/pmc4463.htm)
* [Auto-correlation Plot](https://www.itl.nist.gov/div898/handbook/eda/section3/autocopl.htm): For investigating questions such as (From <abbr title="National Institute of Standards and Technology">NIST</abbr>)
  * Is an observation related to an adjacent observation?
  * Is an observation related to an observation twice-removed? (etc.)
  * Is the observed time series white noise?
  * Is the observed time series sinusoidal?
  * Is the observed time series autoregressive?
* [Statistical forecasting: notes on regression and time series analysis](https://people.duke.edu/~rnau/411home.htm)
  * [Identifying the order of differencing in an ARIMA model](https://people.duke.edu/~rnau/411arim2.htm)
  * [Identifying the numbers of AR or MA terms in an ARIMA model](https://people.duke.edu/~rnau/411arim3.htm)

<br>

Extra:
* [Natural Logarithm Transformations](https://www.bridgetext.com/log-transforming-time-series-data-in-r)
* [Time Formatting Codes](https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes)
* [statsmodels.tsa.stattools.pacf](https://www.statsmodels.org/dev/generated/statsmodels.tsa.stattools.pacf.html)
* [statsmodels.graphics.tsaplots.plot_pacf](https://www.statsmodels.org/dev/generated/statsmodels.graphics.tsaplots.plot_pacf.html)
* [python: hub.docker.com](https://hub.docker.com/_/python/)

<br>

### Linux Distributions

* [ubuntu man pages](https://manpages.ubuntu.com/manpages/trusty/man1/)

<br>

### Time

* [Epoch Time](https://unixtime.org)
* [UNIX Time Converters](https://time.is/Unix_time_converter)
* [Time Durations](https://en.wikipedia.org/wiki/ISO_8601#Durations)

<br>

### Actions

* [docker/login-action](https://github.com/docker/login-action/releases)
* [docker/metadata-action](https://github.com/docker/metadata-action/releases)
* [aws-actions/configure-aws-credentials](https://github.com/aws-actions/configure-aws-credentials/releases)
* [aws-actions/amazon-ecr-login](https://github.com/aws-actions/amazon-ecr-login/releases)

<br>

### DASK & Amazon EMR (Elastic MapReduce)

In brief:
* [GPU](https://docs.dask.org/en/stable/gpu.html)
* [Deploying on Amazon EMR](https://yarn.dask.org/en/latest/aws-emr.html)
  * [Quick Start: dask-yarn](https://yarn.dask.org/en/latest/quickstart.html)
  * [A bootstrap for EMR](https://github.com/dask/dask-yarn/blob/main/deployment_resources/aws-emr/bootstrap-dask)
  * [Create bootstrap actions to install additional software with an Amazon EMR cluster](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-bootstrap.html)
  * [step](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-spark-submit-step.html)

Packaging for deployment:
* [venv-pack2](https://pypi.org/project/venv-pack2/)
* venv-pack &rarr; [venv-pack](https://pypi.org/project/venv-pack/), [documentation](https://jcristharif.com/venv-pack/)
* docker & virtual environments &rarr; [docker & venv](https://coderivers.org/blog/docker-with-python-venv/), [Activate python virtualenv in Dockerfile](https://bobcares.com/blog/activate-python-virtualenv-in-dockerfile/)

Beware of Python versions:
* [Amazon EMR Release Guide](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-780-release.html)




<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
