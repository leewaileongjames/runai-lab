# Module 2 - Creating Workload Assets

## Lesson 1: Environment Assets

> [!NOTE]
> In this lesson you will learn what an environment asset is and what can be configured within it.

### Step 1

Click **"Workload manager"**.

<img alt="module-2-image-01" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-01.png" />

This is where your workloads are managed. When using the UI, we use assets to abstract Kubernetes away from the end user.

### Step 2

Select **Environments** first.

<img alt="module-2-image-02" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-02.png" />

An Environment is built around a _**container image**_. Any accessible container image can be used in an environment. These environments are essentially templates providing the tools, libraries and frameworks to perform a function and can be tailored to a specific step of the AI lifecycle. There are 3 types of workloads that can be configured in an environment: 
1. A **Workspace** which is an interactive workload, usually for IDE environments like Jupyter.
2. A **Training** workload which is a traditional batch workload used for training models
3. The **Inference** workload which is for running models in production.

### Step 3

Select the jupyter-example environment.

<img alt="module-2-image-03" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-03.png" />

Click **"Edit"**. _Do not make any changes, we will just view the configuration._

<img alt="module-2-image-04" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-04.png" />

### Step 4

You can set the container image being used in the environment here. 

<img alt="module-2-image-05" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-05.png" />

### Step 5

Expand the **"Tools"** section.

<img alt="module-2-image-06" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-06.png" />

The tools section is for configuring the ingress rules NVIDIA Run:ai will create for you when deploying from this environment. For example a URL for Jupyter Notebook or maybe a port for SSH connectivity with tools such as Pycharm or VSCode. 

### Step 6 

Now expand the **"Runtime settings"**.

<img alt="module-2-image-07" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-07.png" />

This is where you can configure the startup command and arguments as well as any environment variables. This section is editable at the point of deployment too, allowing you to specify your own scripts etc.

### Step 7

Select **"Cancel"**.

<img alt="module-2-image-08" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-08.png" />

<br/>

## Lesson 2: Compute Resource Assets

> [!NOTE]
> In this lesson you will learn what a compute resource asset is and what can be configured within it.

### Step 8

Select **"Compute resources"**.

<img alt="module-2-image-09" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-09.png" />

A Compute resource is a block of compute, cpu, memory and gpu that can be allocated to a workload.

### Step 9

Select the **"small-fraction"** resource. 

<img alt="module-2-image-10" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-10.png" />

Click "Edit". _Do not make any changes, we will just view the configuration._

<img alt="module-2-image-11" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-11.png" />

Here you can see you can configure the amount of gpu, cpu and memory. For the GPU, when 1 device request is set, you can configure a percentage of the GPU. This allows you to _**run multiple workloads on a single GPU**_ and can be very efficient for interactive IDE environments in particular.

### Step 10

Scroll down and click **"cancel"**.

<img alt="module-2-image-12" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-12.png" />

## Lesson 3: Data Source Asset

> [!NOTE]
> In this lesson you will learn what an data source asset is and what can be configured within it.

### Step 11

Select **"Data sources"**.

<img alt="module-2-image-13" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-13.png" />

### Step 12

Click **"new data source"**.

<img alt="module-2-image-14" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-14.png" />

Here you can see all the different types of data sources you can add. 

### Step 13

Select **"Git"**.

<img alt="module-2-image-15" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-15.png" />

### Step 14

Click the **blue logo** next to the scope section here.

<img alt="module-2-image-16" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-16.png" />

Select your project.

<img alt="module-2-image-17" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-17.png" />

### Step 15

Click **"Apply"**.

<img alt="module-2-image-18" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-18.png" />

### Step 16

Give the data source a **name**.

<img alt="module-2-image-19" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-19.png" />

### Step 17

For the **"Repository URL"** field add `https://github.com/NVIDIA/GenerativeAIExamples.git`

<img alt="module-2-image-20" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-20.png" />

### Step 18 

Expand the **"Credentials"** field.

<img alt="module-2-image-21" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-21.png" />

Select "None".

<img alt="module-2-image-22" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-22.png" />

### Step 19

Click the **"Container path"** field and Type `/home/jovyan/github`

<img alt="module-2-image-23" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-23.png" />

### Step 20

Click **"create data source"**.

<img alt="module-2-image-23" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-2-image-24.png" />

> [!TIP]
> We will be using this data source in **Module 3**.
