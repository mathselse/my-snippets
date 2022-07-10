# Google Kubernetes Engine (GKE)
## Enable Service  
### Enable GKE service

    $ gcloud services enable container.googleapi.com
### Enable IAM service

    gcloud services enable iam.googleapis.com
### Enable Resource Manager Service
    gcloud services enable cloudresourcemanager.googleapis.com
    
## Clusters
### Create a cluster with default machine
1. Enable GKE services
2. Create the cluster  

        $ gcloud container clusters create <cluster-name> --num-nodes 2 --enable-autoscaling --min-nodes 1 --max-nodes 5 --zone us-central1-a

### Create a cluster with selected machine

    gcloud containter clusters create <cluster-name> --zone <zone> -m <machine-name>