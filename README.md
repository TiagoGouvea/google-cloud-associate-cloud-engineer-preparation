# Google Cloud Associate Cloud Engineer preparation

This is a list of useful contents to be used while studying to [Associate Cloud Engineer](https://cloud.google.com/certification/cloud-engineer) certification.

I got the idea to organize content like that from [João Vitor Guimarães](https://twitter.com/joaovitor) Medium [post](https://medium.com/@joaovitor/associate-cloud-engineer-study-guide-cf7e74da1bb6).

It's not a ready document, I'm writing as I study, and pushing here (weekly preferably).

:ballot_box_with_check: Partially studied  
:white_check_mark: Fully studied

# Study log
- April 26th, 2020 - Spent around 3 hours studying
- April 25th, 2020 - Having studied around 40% of the content, took the [practice exam](https://cloud.google.com/certification/practice-exam/cloud-engineer) and got 11 of the 23 questions right. Proportional, I guess. :)  
- April 19th, 2020 - Spent around 4 hours studying
- April 5th, 2020 - Started to study. Spent around 3 hours studying the basic concepts (many of that I already knew)

# My study plan

## 1. Setting up a cloud solution environment :white_check_mark:

*   1.1 Setting up cloud projects and accounts :white_check_mark:
    *   Creating projects
        *   [gcloud projects create](https://cloud.google.com/sdk/gcloud/reference/projects/create)
    *   Assigning users to predefined IAM roles within a project
        *   [gcloud projects add-iam-policy-binding](https://cloud.google.com/sdk/gcloud/reference/projects/add-iam-policy-binding)
        *   [Understanding policies | Cloud IAM Documentation](https://cloud.google.com/iam/docs/policies)
        *   [Policy | Cloud IAM Documentation](https://cloud.google.com/iam/docs/reference/rest/v1/Policy)
    *   Managing users in Cloud Identity (manually and automated)
        *   [Overview | Cloud Identity](https://cloud.google.com/identity/solutions/overview)
        *   [Automate user provisioning across cloud apps | Cloud Identity](https://cloud.google.com/identity/solutions/automate-user-provisioning)
    *   Enabling APIs within projects
        *   [Listing Services | Service Usage Documentation](https://cloud.google.com/service-usage/docs/list-services)
        *   [Enabling and Disabling Services | Service Usage Documentation](https://cloud.google.com/service-usage/docs/enable-disable)
    *   Provisioning one or more Stackdriver workspaces
        *   [Workspaces | Cloud Monitoring](https://cloud.google.com/monitoring/workspaces/)
        *   [https://cloud.google.com/monitoring/workspaces/create](https://cloud.google.com/monitoring/workspaces/create)
*   1.2 Managing billing configuration :white_check_mark:
    *   Creating one or more billing accounts
        *   [Create, modify, or close your Cloud Billing account](https://cloud.google.com/billing/docs/how-to/manage-billing-account)
    *   Linking projects to a billing account
        *   [gcloud beta billing projects link](https://cloud.google.com/sdk/gcloud/reference/beta/billing/projects/link)
    *   Establishing billing budgets and alerts
        *   [Set budgets and budget alerts | Cloud Billing](https://cloud.google.com/billing/docs/how-to/budgets)
    *   Setting up billing exports to estimate daily/monthly charges
        *   [Export Cloud Billing data to BigQuery](https://cloud.google.com/billing/docs/how-to/export-data-bigquery)
*   1.3 Installing and configuring the command line interface (CLI), specifically the Cloud SDK (e.g., setting the default project) :white_check_mark:   
    *   [gcloud command-line tool overview](https://cloud.google.com/sdk/gcloud)
    *   [Installing Google Cloud SDK](https://cloud.google.com/sdk/install)
    *   [gcloud config set](https://cloud.google.com/sdk/gcloud/reference/config/set)


### 2. Planning and configuring a cloud solution

*   2.1 Planning and estimating GCP product use using the Pricing Calculator :white_check_mark:
    *   [Google Cloud Platform Pricing Calculator](https://cloud.google.com/products/calculator/)
    *   [Google Cloud Platform on a shoestring budget (Google I/O '18)](https://www.youtube.com/watch?v=N2OG1w6bGFo&feature=youtu.be)
*   2.2 Planning and configuring compute resources :white_check_mark:
    *   Selecting appropriate compute choices for a given workload (e.g., Compute Engine, Google Kubernetes Engine, App Engine, Cloud Run, Cloud Functions)
        *   [Deciding between Compute Engine, Container Engine, App Engine and more (Google Cloud Next '17)](https://www.youtube.com/watch?v=g0dN8Hkh5H8)
        *   [Get to know Google App Engine](https://www.youtube.com/watch?v=2PRciDpqpko)
        *   [https://cloud.google.com/run](https://cloud.google.com/run)
        *   [Quickstarts | Cloud Run Documentation](https://cloud.google.com/run/docs/quickstarts)
        *   [The Good and the Bad of Google Cloud Run](https://read.acloud.guru/the-good-and-the-bad-of-google-cloud-run-34455e673ef5)
        *   [Cloud Functions](https://cloud.google.com/functions/?&utm_source=google&utm_medium=cpc&utm_campaign=latam-BR-all-pt-dr-bkws-all-all-trial-b-dr-1008075-LUAC0008673&utm_content=text-ad-none-none-DEV_c-CRE_429691579873-ADGP_BKWS+%7C+Multi+~+Compute+%7C+Functions-KWID_43700046780193860-kwd-808554695722-userloc_1001575&utm_term=KW_%2Bgoogle%20%2Bfunctions-ST_%2BGoogle+%2BFunctions&gclid=CjwKCAjwg6b0BRBMEiwANd1_SG94_8UoelcnURy-YK5XEbBVIhUgR-MuUrch1iX3BJGDKQlu-K2P8hoClRwQAvD_BwE&gclsrc=aw.ds)
    *   Using preemptible VMs and custom machine types as appropriate
        *   [Preemptible VM instances | Compute Engine Documentation](https://cloud.google.com/compute/docs/instances/preemptible)
        *   [Machine types | Compute Engine Documentation](https://cloud.google.com/compute/docs/machine-types)
*   2.3 Planning and configuring data storage options :white_check_mark:
    *   Product choice (e.g., Cloud SQL, BigQuery, Cloud Spanner, Cloud Bigtable)
        *   [BigQuery documentation](https://cloud.google.com/bigquery/docs)
        *   [Cloud Spanner | Automatic Sharding with Transactional Consistency at Scale](https://cloud.google.com/spanner)
        *   [Cloud Bigtable](https://cloud.google.com/bigtable)
    *   Choosing storage options (e.g., Standard, Nearline, Coldline, Archive)
        *   [https://cloud.google.com/storage/docs/introduction](https://cloud.google.com/storage/docs/introduction)
        *   [Storage classes | Cloud Storage](https://cloud.google.com/storage/docs/storage-classes)
*   2.4 Planning and configuring network resources. Tasks include:
    *   Differentiating load balancing options
    *   Identifying resource locations in a network for availability
    *   Configuring Cloud DNS

### 3. Deploying and implementing a cloud solution

*   3.1 Deploying and implementing Compute Engine resources. Tasks include:
    *   Launching a compute instance using Cloud Console and Cloud SDK (gcloud) (e.g., assign disks, availability policy, SSH keys)
    *   Creating an autoscaled managed instance group using an instance template
    *   Generating/uploading a custom SSH key for instances
    *   Configuring a VM for Stackdriver monitoring and logging
    *   Assessing compute quotas and requesting increases
    *   Installing the Stackdriver Agent for monitoring and logging
*   3.2 Deploying and implementing Google Kubernetes Engine resources. Tasks include:
    *   Deploying a Google Kubernetes Engine cluster
    *   Deploying a container application to Google Kubernetes Engine using pods
    *   Configuring Google Kubernetes Engine application monitoring and logging
*   3.3 Deploying and implementing App Engine, Cloud Run, and Cloud Functions resources. Tasks include, where applicable:
    *   Deploying an application, updating scaling configuration, versions, and traffic splitting
    *   Deploying an application that receives Google Cloud events (e.g., Cloud Pub/Sub events, Cloud Storage object change notification events)
*   3.4 Deploying and implementing data solutions. Tasks include:
    *   Initializing data systems with products (e.g., Cloud SQL, Cloud Datastore, BigQuery, Cloud Spanner, Cloud Pub/Sub, Cloud Bigtable, Cloud Dataproc, Cloud Dataflow, Cloud Storage)
    *   Loading data (e.g., command line upload, API transfer, import/export, load data from Cloud Storage, streaming data to Cloud Pub/Sub)
*   3.5 Deploying and implementing networking resources. Tasks include:
    *   Creating a VPC with subnets (e.g., custom-mode VPC, shared VPC)
    *   Launching a Compute Engine instance with custom network configuration (e.g., internal-only IP address, Google private access, static external and private IP address, network tags)
    *   Creating ingress and egress firewall rules for a VPC (e.g., IP subnets, tags, service accounts)
    *   Creating a VPN between a Google VPC and an external network using Cloud VPN
    *   Creating a load balancer to distribute application network traffic to an application (e.g., Global HTTP(S) load balancer, Global SSL Proxy load balancer, Global TCP Proxy load balancer, regional network load balancer, regional internal load balancer)
*   3.6 Deploying a solution using Cloud Marketplace. Tasks include:
    *   Browsing Cloud Marketplace catalog and viewing solution details
    *   Deploying a Cloud Marketplace solution
*   3.7 Deploying application infrastructure using Cloud Deployment Manager. Tasks include:
    *   Developing Deployment Manager templates
    *   Launching a Deployment Manager template

### 4. Ensuring successful operation of a cloud solution

*   4.1 Managing Compute Engine resources :ballot_box_with_check:
    *   Managing a single VM instance (e.g., start, stop, edit configuration, or delete an instance)
        *   [gcloud compute instances start](https://cloud.google.com/sdk/gcloud/reference/compute/instances/start)
        *   [gcloud compute instances list](https://cloud.google.com/sdk/gcloud/reference/compute/instances/list)
        *   [gcloud compute instances describe](https://cloud.google.com/sdk/gcloud/reference/compute/instances/describe)
        *   [gcloud compute instances stop](https://cloud.google.com/sdk/gcloud/reference/compute/instances/stop)
        *   [gcloud compute instances delete](https://cloud.google.com/sdk/gcloud/reference/compute/instances/delete)
        *   [gcloud compute instances update](https://cloud.google.com/sdk/gcloud/reference/compute/instances/update)
    *   SSH/RDP to the instance
        *   [Connecting to instances | Compute Engine Documentation](https://cloud.google.com/compute/docs/instances/connecting-to-instance)
    *   Attaching a GPU to a new instance and installing CUDA libraries
        *   [Adding or removing GPUs | Compute Engine Documentation](https://cloud.google.com/compute/docs/gpus/add-gpus)
    *   Viewing current running VM inventory (instance IDs, details)
        *   [gcloud compute instances describe](https://cloud.google.com/sdk/gcloud/reference/compute/instances/describe)
    *   Working with snapshots (e.g., create a snapshot from a VM, view snapshots, delete a snapshot)
        *   [Creating persistent disk snapshots | Compute Engine Documentation](https://cloud.google.com/compute/docs/disks/create-snapshots)
        *   [Creating scheduled snapshots for persistent disk](https://cloud.google.com/compute/docs/disks/scheduled-snapshots)
        *   [gcloud compute snapshots list](https://cloud.google.com/sdk/gcloud/reference/compute/snapshots/list)
        *   [Restoring and deleting persistent disk snapshots](https://cloud.google.com/compute/docs/disks/restore-and-delete-snapshots)
        *   [Best practices for persistent disk snapshots](https://cloud.google.com/compute/docs/disks/snapshot-best-practices)
    *   Working with images (e.g., create an image from a VM or a snapshot, view images, delete an image)
        *   [Images | Compute Engine Documentation](https://cloud.google.com/compute/docs/images)
        *   [gcloud compute images create](https://cloud.google.com/sdk/gcloud/reference/compute/images/create)
        *   [gcloud compute images list](https://cloud.google.com/sdk/gcloud/reference/compute/images/list)
        *   [gcloud compute images delete](https://cloud.google.com/sdk/gcloud/reference/compute/images/delete)
    *   Working with instance groups (e.g., set autoscaling parameters, assign instance template, create an instance template, remove instance group)
    *   Working with management interfaces (e.g., Cloud Console, Cloud Shell, GCloud SDK)
*   4.2 Managing Google Kubernetes Engine resources. Tasks include:
    *   Viewing current running cluster inventory (nodes, pods, services)
    *   Browsing the container image repository and viewing container image details
    *   Working with node pools (e.g., add, edit, or remove a node pool)
    *   Working with pods (e.g., add, edit, or remove pods)
    *   Working with services (e.g., add, edit, or remove a service)
    *   Working with stateful applications (e.g. persistent volumes, stateful sets)
    *   Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
*   4.3 Managing App Engine and Cloud Run resources. Tasks include:
    *   Adjusting application traffic splitting parameters
    *   Setting scaling parameters for autoscaling instances
    *   Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
*   4.4 Managing storage and database solutions. Tasks include:
    *   Moving objects between Cloud Storage buckets
    *   Converting Cloud Storage buckets between storage classes
    *   Setting object life cycle management policies for Cloud Storage buckets
    *   Executing queries to retrieve data from data instances (e.g., Cloud SQL, BigQuery, Cloud Spanner, Cloud Datastore, Cloud Bigtable)
    *   Estimating costs of a BigQuery query
    *   Backing up and restoring data instances (e.g., Cloud SQL, Cloud Datastore)
    *   Reviewing job status in Cloud Dataproc, Cloud Dataflow, or BigQuery
    *   Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
*   4.5 Managing networking resources. Tasks include:
    *   Adding a subnet to an existing VPC
    *   Expanding a subnet to have more IP addresses
    *   Reserving static external or internal IP addresses
    *   Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)
*   4.6 Monitoring and logging. Tasks include:
    *   Creating Stackdriver alerts based on resource metrics
    *   Creating Stackdriver custom metrics
    *   Configuring log sinks to export logs to external systems (e.g., on-premises or BigQuery)
    *   Viewing and filtering logs in Stackdriver
    *   Viewing specific log message details in Stackdriver
    *   Using cloud diagnostics to research an application issue (e.g., viewing Cloud Trace data, using Cloud Debug to view an application point-in-time)
    *   Viewing Google Cloud Platform status
    *   Working with management interfaces (e.g., Cloud Console, Cloud Shell, Cloud SDK)

### 5. Configuring access and security

*   5.1 Managing identity and access management (IAM) :white_check_mark:
    *   Viewing IAM role assignments
        * [gcloud projects get-iam-policy](https://cloud.google.com/sdk/gcloud/reference/projects/get-iam-policy)
        * [gcloud organizations get-iam-policy](https://cloud.google.com/sdk/gcloud/reference/organizations/get-iam-policy)
    *   Assigning IAM roles to accounts or Google Groups
        * [gcloud projects add-iam-policy-binding](https://cloud.google.com/sdk/gcloud/reference/projects/add-iam-policy-binding)
        * [gcloud projects set-iam-policy](https://cloud.google.com/sdk/gcloud/reference/projects/set-iam-policy)
        * [gcloud projects remove-iam-policy-binding](https://cloud.google.com/sdk/gcloud/reference/projects/remove-iam-policy-binding)
    *   Defining custom IAM roles
        * [Better Practices for Cloud IAM (Cloud Next '18)](https://www.youtube.com/watch?v=ZMC8Ng3E3LQ)
        * [Google Cloud: IAM and Organization Node](https://www.youtube.com/watch?v=etxbSda_ZAU)
        * [Understanding IAM custom roles](https://cloud.google.com/iam/docs/understanding-custom-roles)
        * [gcloud iam roles](https://cloud.google.com/sdk/gcloud/reference/iam/roles/)
        * [Creating and managing custom roles](https://cloud.google.com/iam/docs/creating-custom-roles)
        * [REST Resource: projects.roles](https://cloud.google.com/iam/docs/reference/rest/v1/projects.roles)
        * [gcloud iam roles update](https://cloud.google.com/sdk/gcloud/reference/iam/roles/update)

*   5.2 Managing service accounts  :white_check_mark:
    *   Managing service accounts with limited privileges
        * [Service accounts](https://cloud.google.com/compute/docs/access/service-accounts)
    *   Assigning a service account to VM instances
        * [Creating and enabling service accounts for instances](https://cloud.google.com/compute/docs/access/create-enable-service-accounts-for-instances)
    *   Granting access to a service account in another project
        * [Cross project management using service account](https://stackoverflow.com/questions/35479025/cross-project-management-using-service-account)
*   5.3 Viewing audit logs for project and managed services.
