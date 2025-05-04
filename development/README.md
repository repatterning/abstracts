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

Core
* [docker/login-action](https://github.com/docker/login-action/releases)
* [docker/metadata-action](https://github.com/docker/metadata-action/releases)
* [aws-actions/configure-aws-credentials](https://github.com/aws-actions/configure-aws-credentials/releases)
* [aws-actions/amazon-ecr-login](https://github.com/aws-actions/amazon-ecr-login/releases)

Extra
* [Dockerfile](https://docs.docker.com/reference/dockerfile/)
* [requirements.txt](https://pip.pypa.io/en/stable/reference/requirements-file-format/)

<br>

### DASK & Amazon EMR (Elastic MapReduce)

[EMR Pricing](https://aws.amazon.com/emr/pricing/)

In brief:
* [GPU](https://docs.dask.org/en/stable/gpu.html)
* [Deploying on Amazon EMR](https://yarn.dask.org/en/latest/aws-emr.html)
  * [Quick Start: dask-yarn](https://yarn.dask.org/en/latest/quickstart.html)
  * [A bootstrap for EMR](https://github.com/dask/dask-yarn/blob/main/deployment_resources/aws-emr/bootstrap-dask)
  * [Create bootstrap actions to install additional software with an Amazon EMR cluster](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-bootstrap.html)
  * [step](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-spark-submit-step.html)
  * [Configure Docker for use with Amazon EMR clusters](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-docker.html)
  * [EMR & Custom Images](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/docker-custom-images-steps.html)

Packaging for deployment:
* [venv-pack2](https://pypi.org/project/venv-pack2/)
* venv-pack &rarr; [venv-pack](https://pypi.org/project/venv-pack/), [documentation](https://jcristharif.com/venv-pack/)
* docker & virtual environments &rarr; [docker & venv](https://coderivers.org/blog/docker-with-python-venv/), [Activate python virtualenv in Dockerfile](https://bobcares.com/blog/activate-python-virtualenv-in-dockerfile/)

Beware of Python versions:
* [Amazon EMR Release Guide](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-780-release.html)

For Cloud Formation:
* [Intrinsic Functions](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-join.html)

<br>
<br>

### RAPIDS & Spark & EMR

* [Use the Nvidia RAPIDS Accelerator for Apache Spark](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-spark-rapids.html)
* [RAPIDS Accelerator for Apache Spark Deployment Guide](https://docs.nvidia.com/ai-enterprise/deployment/spark-rapids-accelerator/latest/emr.html)
* [NVIDIA AI Enterprise with RAPIDS Accelerator Deployment Guide](https://docs.nvidia.com/ai-enterprise/deployment/spark-rapids-accelerator/latest/index.html)
* [rapids.ai & Amazon EMR](https://docs.nvidia.com/ai-enterprise/deployment/spark-rapids-accelerator/latest/emr.html)
* [rapids.ai, EMR, EKS](https://aws.amazon.com/blogs/containers/run-spark-rapids-ml-workloads-with-gpus-on-amazon-emr-on-eks/)
* [Quickstart](https://docs.nvidia.com/spark-rapids/user-guide/latest/qualification/quickstart.html)
* Images: **a.** [rapids.ai & EMR](https://gallery.ecr.aws/emr-on-eks/spark/emr-7.0.0-spark-rapids), **b.** [EMR](https://gallery.ecr.aws/emr-on-eks?page=1)
* [Amazon EMR & Dockerfile](https://github.com/awslabs/data-on-eks/blob/main/ai-ml/emr-spark-rapids/examples/xgboost/Dockerfile)
* [cutting cost](https://developer.nvidia.com/blog/accelerated-data-analytics-faster-time-series-analysis-with-rapids-cudf/)
* [Getting Started: Amazon EMR, Python, Spark](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-gs.html#emr-getting-started-plan-and-configure)

<br>
<br>

### Amazon & GPU Tasks

* [Amazon ECS task definitions for GPU workloads](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html)
* [Run Amazon ECS or Fargate tasks with Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/connect-ecs.html)
* [Amazon ECS task definitions for GPU workloads](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html)
* [Launch a GPU container instance for Amazon ECS](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/gpu-launch.html)
* [Amazon ECS-optimized Linux AMI](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html)
* [Amazon ECS container agent configuration](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-config.html)
* [Amazon ECS increases the CPU limit for ECS tasks to 192 vCPUs](https://aws.amazon.com/about-aws/whats-new/2025/02/amazon-ecs-increases-cpu-ecs-tasks/)
* [Container Definitions](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#container_definitions)<br>Environment: cpu &rarr; <blockquote>The total amount of CPU reserved for all the containers that are within a task must be lower than the task-level cpu value.</blockquote>

<br>

BATCH
* [BATCH: Use a GPU workload AMI](https://docs.aws.amazon.com/batch/latest/userguide/batch-gpu-ami.html)
* [Run AWS Batch workloads with Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/connect-batch.html)

<br>

TEMPLATES
* [Create launch templates](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/quickref-ec2-launch-templates.html)
* [awscli ec2](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html#cli-aws-ec2)

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
