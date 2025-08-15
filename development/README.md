<br>

## Project Notes

Weather Warnings
* [Warnings](https://weather.metoffice.gov.uk/guides/warnings)
* [RSS feeds from the Met Office](https://weather.metoffice.gov.uk/guides/rss)

<br>
<br>
<br>

## Development

### NGINX

* [docker hub](https://hub.docker.com/_/nginx)
* [docker nginx](https://toxigon.com/setting-up-nginx-with-docker)
* [docker nginx](https://www.uptimia.com/questions/how-to-run-nginx-in-the-foreground-within-a-docker-container#implementing-the-solution-in-docker)
* [extra help](https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44)
* [more](https://www.socketxp.com/iot/remote-access-nginx-web-server-from-internet/)
* [nginx -g 'daemon off;'](https://www.thecoderscamp.com/nginx-g-daemon-off/)
* [Dockerfile](https://github.com/devasthali-os/nginx-base/blob/master/Dockerfile)
* [conf](https://nginx.org/en/docs/beginners_guide.html#conf_structure)
* [MIME (Multipurpose Internet Mail Extensions) Types](https://server.hk/blog/14461/)
* [MIME Types](https://www.slingacademy.com/article/nginx-mime-types-the-complete-guide/)
* [load error example](https://www.slingacademy.com/article/nginx-error-cannot-load-css-js-files/)

<br>

### live server

* [live server](https://itnext.io/dockerizing-modern-web-apps-cd9667eebf44)
* [github](https://github.com/tapio/live-server)
* [npm](https://www.npmjs.com/package/live-server)

<br>

### vim & vi

* [vi](https://linuxsimply.com/cheat-sheets/vi/)
* [vim](https://vim.rtorr.com)
* [vim](https://www.redhat.com/en/blog/beginners-guide-vim)

<br>

### JavaScript Modules

* [Modules](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)
* [Modules](https://javascript.info/modules)
* [Module Errors](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors/import_decl_module_top_level#importing_in_a_non-module_script)
* [SCRIPT](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script)

<br>

### JavaScript

* [fetch](https://javascript.info/fetch)
* [1](https://wpdean.com/css-dropdown-menus/), [2](https://jsfiddle.net/cL2x7/), [3](https://www.geeksforgeeks.org/how-to-creating-html-list-from-javascript-array/)
* High Charts
  * [data grouping](https://www.highcharts.com/docs/stock/data-grouping)
  * [the date formats](https://api.highcharts.com/class-reference/Highcharts.Time#dateFormat)

  
<br>
<br>
<br>

## References

### SEPA, etc.


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

### GitHub Actions

Core
* [docker/login-action](https://github.com/docker/login-action/releases)
* [docker/metadata-action](https://github.com/docker/metadata-action/releases)
* [aws-actions/configure-aws-credentials](https://github.com/aws-actions/configure-aws-credentials/releases)
* [aws-actions/amazon-ecr-login](https://github.com/aws-actions/amazon-ecr-login/releases)

<br>

Extra
* [Dockerfile](https://docs.docker.com/reference/dockerfile/)
* [requirements.txt](https://pip.pypa.io/en/stable/reference/requirements-file-format/)
* [docker run](https://docs.docker.com/reference/cli/docker/container/run/)


<br>

### DASK & Amazon EMR (Elastic MapReduce)

[EMR Pricing](https://aws.amazon.com/emr/pricing/)

<br>

In brief:
* [GPU](https://docs.dask.org/en/stable/gpu.html)
* [Deploying on Amazon EMR](https://yarn.dask.org/en/latest/aws-emr.html)
  * [Quick Start: dask-yarn](https://yarn.dask.org/en/latest/quickstart.html)
  * [A bootstrap for EMR](https://github.com/dask/dask-yarn/blob/main/deployment_resources/aws-emr/bootstrap-dask)
  * [Create bootstrap actions to install additional software with an Amazon EMR cluster](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-bootstrap.html)
  * [step](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-spark-submit-step.html)
  * [Configure Docker for use with Amazon EMR clusters](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-docker.html)
  * [EMR & Custom Images](https://docs.aws.amazon.com/emr/latest/EMR-on-EKS-DevelopmentGuide/docker-custom-images-steps.html)

<br>

Packaging for deployment:
* [venv-pack2](https://pypi.org/project/venv-pack2/)
* venv-pack &rarr; [venv-pack](https://pypi.org/project/venv-pack/), [documentation](https://jcristharif.com/venv-pack/)
* docker & virtual environments &rarr; [docker & venv](https://coderivers.org/blog/docker-with-python-venv/), [Activate python virtualenv in Dockerfile](https://bobcares.com/blog/activate-python-virtualenv-in-dockerfile/)

<br>

Beware of Python versions:
* [Amazon EMR Release Guide](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-780-release.html)

<br>

For Cloud Formation:
* [Intrinsic Functions](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-join.html)

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

### Amazon & GPU Tasks

* [Release Notes: Deep Learning Amazon Machine Image](https://docs.aws.amazon.com/dlami/latest/devguide/appendix-ami-release-notes.html)
* [Specialized Configurations with Docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/docker-specialized.html)
* [Amazon ECS task definitions for GPU workloads](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html)
* [Run Amazon ECS or Fargate tasks with Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/connect-ecs.html)
* [Amazon ECS task definitions for GPU workloads: Instances List](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-gpu.html)
* [Launch a GPU container instance for Amazon ECS](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/gpu-launch.html)
* [Amazon ECS-optimized Linux AMI](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-optimized_AMI.html)
* [Amazon ECS container agent configuration](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/ecs-agent-config.html)
* [Amazon ECS increases the CPU limit for ECS tasks to 192 vCPUs](https://aws.amazon.com/about-aws/whats-new/2025/02/amazon-ecs-increases-cpu-ecs-tasks/)
* [Container Definitions](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_definition_parameters.html#container_definitions)<br>Environment: cpu &rarr; <blockquote>The total amount of CPU reserved for all the containers that are within a task must be lower than the task-level cpu value.</blockquote>

<br>

BATCH
* [BATCH: Use a GPU workload AMI](https://docs.aws.amazon.com/batch/latest/userguide/batch-gpu-ami.html)
* [Run AWS Batch workloads with Step Functions](https://docs.aws.amazon.com/step-functions/latest/dg/connect-batch.html)
* [Getting started with Amazon EC2 orchestration](https://docs.aws.amazon.com/batch/latest/userguide/getting-started-ec2.html)
  * [Example: chaos gears](https://chaosgears.com/blog/gpu-jobs-on-aws-batch)
  * [retry strategy](https://docs.aws.amazon.com/batch/latest/userguide/job_retries.html)
  * [retry strategy: evaluate on exit](https://docs.aws.amazon.com/batch/latest/userguide/job_definition_parameters-copy.html#retryStrategy-evaluateOnExit)
* [Jobs stuck in a RUNNABLE status](https://docs.aws.amazon.com/batch/latest/userguide/job_stuck_in_runnable.html)
* [Batch job stuck in RUNNABLE status](https://repost.aws/knowledge-center/batch-job-stuck-runnable-status)

<br>

TEMPLATES
* [Create launch templates](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/quickref-ec2-launch-templates.html)
* [awscli ec2](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html#cli-aws-ec2)
* [user data & cloud init](https://cloudinit.readthedocs.io/en/latest/explanation/format.html#mime-multi-part-archive)
* [user data & launch templates](https://docs.aws.amazon.com/batch/latest/userguide/launch-templates.html)
* [Amazon EC2 launch template examples](https://docs.aws.amazon.com/batch/latest/userguide/launch-template-examples.html)


<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
