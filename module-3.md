# Module 3: Deploying a Workload

> [!NOTE]
> In this lesson you will deploy a Workspace workload.

## Lesson 1: Deploying a workload

### Step 1
Select **"Workloads"**.

<img alt="module-3-image-01" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-01.png" />

### Step 2 

Click **"NEW WORKLOAD"**.

<img alt="module-3-image-02" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-02.png" />

### Step 3 

We will create a workspace. Click **"Workspace"**.

<img alt="module-3-image-03" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-03.png" />

### Step 4 

Ensure your project is selected.

<img alt="module-3-image-04" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-04.png" />

### Step 5 

Give the workspace a name. For example, **jupyter-notebook"**.

<img alt="module-3-image-05" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-05.png" />

### Step 6 

Click **"Continue"**.

<img alt="module-3-image-06" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-06.png" />

### Step 7

You'll now notice you see all of the environments that have been made available to your project (remember the scope). 

Select the **"jupyter-example"** environment.

<img alt="module-3-image-07" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-07.png" />

### Step 8 

Scroll down and select the **"small-fraction"** Compute resource. This will give the workload a 10% fraction of a GPU.

<img alt="module-3-image-08" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-08.png" />

> [!TIP]
> **Use Case**  
> As mentioned in Module 2, using a fraction of a GPU when suitable, rather than a whole one, means that _**less resource is wasted**_.  

### Step 9 

Expand "Data sources". 

<img alt="module-3-image-09" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-09.png" />

### Step 10 

Select the git data source you just created.

<img alt="module-3-image-10" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-10.png" />

### Step 11 

Click **"Create Workspace"**.

<img alt="module-3-image-11" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-11.png" />

<br/>

## Lesson 2: Validating the Workload

### Step 12 

Select your new workload.

<img alt="module-3-image-12" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-12.png" />

### Step 13 

Click **"show details"**.

<img alt="module-3-image-13" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-13.png" />

### Step 14 

Under the Event History section here you will see all the steps we are taking within Kubernetes. This can help you troubleshoot issues that arise before the container starts running.

<img alt="module-3-image-14" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-14.png" />

Feel free to explore other tabs.

### Step 15 

Wait for the status to be "Running". Click **"Connect"**.

<img alt="module-3-image-15" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-15.png" />

### Step 16 

Click **"Jupyter"**.

<img alt="module-3-image-16" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-16.png" />

### Step 17 

If required, please sign in using your credentials.

<img alt="module-3-image-17" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-17.png" />

### Step 18 

This takes you to the Jupyter Notebook url we created as part of the ingress rule. You are now working within your new workload. 

Select **"terminal"**.

<img alt="module-3-image-18" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-18.png" />

### Step 19 

Type `nvidia-smi`. This will show the GPU config. 

> [!IMPORTANT]
> You can see we are only seeing 10% of the H100 80GB GPUs memory.

<img alt="module-3-image-19" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-19.png" />

### Step 20 

Now Double-click the **"github"** folder.

<img alt="module-3-image-20" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-20.png" />

### Step 21 

Double-click **"GenerativeAIExamples.git"**. 

Within here you will see the contents of the github repo we set in the data source we created earlier have been copied over ready to work with.

<img alt="module-3-image-21" src="https://github.com/leewaileongjames/runai-lab/blob/main/images/module-3-image-21.png" />


