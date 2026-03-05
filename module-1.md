# Module 1: Explore Cluster and Configure Quotas

## Lesson 1: Exploring the Cluster

> [!NOTE]
> In this lesson we will explore the cluster within the NVIDIA Run:ai interface.

### Step 1

From your web browser, navigate to the [runai](https://runai.jp-isv.sg-cna.com/) lab.

<br/>

### Step 2

Login using the credentials provided to you.

<img alt="module-1-image-02" src="" />

<br/>

### Step 3

Click **Resources**.

<img alt="module-1-image-03" src="" />

<br/>

### Step 4

Now click **"Nodes"**. You will see the GPU nodes that are registered to the Run:ai cluster.

<img alt="module-1-image-04" src="" />

<img alt="module-1-image-05" src="" />

<br/>

Here you will see the GPU nodes.

> [!NOTE]
> Please note these GPUs are _**fake**_ and you will not be able to run real GPU workloads.

<br/>

> [!TIP]
> **Use Case!**  
> With NVIDIA Run:ai a single control plane can manage multiple clusters in multiple locations. This provides your organization a centralized AI platform, regardless of which cluster you wish to deploy workloads on or their location.

<br/>

## Lesson 2: Configuring Departments

> [!NOTE]
> In this lesson we will learn about Departments and configuring their Quota.

### Step 5

Click **"Organization"**.

<img alt="module-1-image-06" src="" />

### Step 6

Click **"Departments"**. A department is the top hierarchical level within a cluster.

<img alt="module-1-image-07" src="" />

### Step 7

Select **"department-xx"**. `xx` is your student ID.

<img alt="module-1-image-08" src="" />

### Step 8

Click **"Edit"**.

<img alt="module-1-image-09" src="" />

### Step 9

A Department allows you to configure a resource quota (GPU/CPU/Memory) which is a guaranteed amount of resource when it needs it. However with NVIDIA Run:ai's over-quota option, another Department can utilise this resource if you are not, until you need access to it again. This ensures high utilization across the cluster and faster job completion. 

Now select the `GPU Devices` field.

<img alt="module-1-image-10" src="" />

Set it to "0.5".

<img alt="module-1-image-11" src="" />

### Step 10 

Click "Apply".

<img alt="module-1-image-12" src="" />

### Step 11 

Ensure that department over quota is _**disabled**_.

<img alt="module-1-image-13" src="" />

### Step 12 

Click "SAVE".

<img alt="module-1-image-14" src="" />

> [!TIP]
> No workloads run directly in a Department, this is a hierarchal level for permissions and quota only, a bit like a resource pool.

<br/>

## Lesson 3: Creating and Configuring Projects

> [!NOTE]
> In this lesson you will create a project and configure it with a quota.

### Step 13 

Select **"Projects"**.

<img alt="module-1-image-15" src="" />

### Step 14

A **Project** is a child of a **Department** and where workloads actually run. 

Click **"New Project"**.

<img alt="module-1-image-16" src="" />

### Step 15 

Ensure that the project is assigned to your department (`department-xx`). 

<img alt="module-1-image-17" src="" />

<img alt="module-1-image-18" src="" />

Click **"Apply"**.

<img alt="module-1-image-19" src="" />

### Step 16

Name the project **"project-xx"** where `xx` is your student ID.

<img alt="module-1-image-20" src="" />

### Step 17

Next select the GPU devices option and set it to **"1"**. 

You can see this quota is coming out of the parent department's quota.

<img alt="module-1-image-21" src="" />

### Step 18

Click **"Apply"**.

<img alt="module-1-image-22" src="" />

### Step 19

Click **"Create Project"**.

<img alt="module-1-image-23" src="" />

