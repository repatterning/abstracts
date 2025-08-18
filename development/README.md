<br>

The repository's development notes.

<br>

## Materials

Launch an interactive environment via

```shell
docker run --rm -i -t -p 8000:8000 -w /app 
  --mount type=bind,src="$(pwd)",target=/app materials
```

Subsequently, launch a web server, i.e., `mkdocs server`, via

```shell
mkdocs serve -a 0.0.0.0:8000
```

<br>

### Remote Development

For this Python project/template, the remote development environment requires

* [Dockerfile](../.devcontainer/Dockerfile)
* [requirements.txt](../.devcontainer/requirements.txt)

An image is built via the command

```shell
docker build . --file .devcontainer/Dockerfile -t materials
```

On success, the output of

```shell
docker images
```

should include

<br>

| repository | tag    | image id | created  | size     |
|:-----------|:-------|:---------|:---------|:---------|
| materials  | latest | $\ldots$ | $\ldots$ | $\ldots$ |


<br>

Subsequently, run an instance of the image `materials` via:

```shell
docker run --rm -i -t -p 8000:8000 -w /app 
  --mount type=bind,src="$(pwd)",target=/app materials
```

<br>

Herein, `-p 8000:8000` maps the host port `8000` to container port `8000`.  Note, the container's working environment,
i.e., `-w`, must be inline with this project's top directory.  Additionally, visit the links for more about the flags/options $\rightarrow$

* --rm: [automatically remove container](https://docs.docker.com/engine/reference/commandline/run/#:~:text=a%20container%20exits-,%2D%2Drm,-Automatically%20remove%20the)
* -i: [interact](https://docs.docker.com/engine/reference/commandline/run/#:~:text=and%20reaps%20processes-,%2D%2Dinteractive,-%2C%20%2Di)
* -t: [tag](https://docs.docker.com/get-started/02_our_app/#:~:text=Finally%2C%20the-,%2Dt,-flag%20tags%20your)
* -p: [publish the container's port/s to the host](https://docs.docker.com/engine/reference/commandline/run/#:~:text=%2D%2Dpublish%20%2C-,%2Dp,-Publish%20a%20container%E2%80%99s)
* --mount type=bind: [a bind mount](https://docs.docker.com/engine/storage/bind-mounts/#syntax)
* -v: [volume](https://docs.docker.com/engine/storage/volumes/)

<br>

Get the name of a running instance of ``materials`` via:

```shell
docker ps --all
```

**Never deploy a root container**.

<br>

### Remote Development & Integrated Development Environments

An IDE (integrated development environment) is a helpful remote development tool.  The **IntelliJ
IDEA** set up involves connecting to a machine's Docker [daemon](https://www.jetbrains.com/help/idea/docker.html#connect_to_docker), the steps are

> * **Settings** $\rightarrow$ **Build, Execution, Deployment** $\rightarrow$ **Docker** $\rightarrow$ **WSL:** {select the linux operating system}
> * **View** $\rightarrow$ **Tool Window** $\rightarrow$ **Services** <br>Within the **Containers** section connect to the running instance of interest, or ascertain connection to the running instance of interest.

<br>

**Visual Studio Code** has its container attachment instructions; study [Attach Container](https://code.visualstudio.com/docs/devcontainers/attach-container).


<br>
<br>


## References

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
* [Amazon EMR Release Guide](https://docs.aws.amazon.com/emr/latest/ReleaseGuide/emr-780-release.html)

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
* [Intrinsic Functions](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-join.html)

<br>
<br>

<br>
<br>

<br>
<br>

<br>
<br>
