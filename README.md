## Google Cloud - Configuring a Centos 7 Workstation (GNOME GUI)

### Description

This guide is focused on creating a Centos 7 workstation specific to the google cloud platform. 

The purpose of this workstation is to have a linux (centos) based workstation from which to create custom
images, for use on GCP (Google Cloud Platform).

This guide is part of a series of guides aimed at setting up an Openshift Cluster on GCP, leveraging a 
custom RHEL 7.7 server image, and setting up the infrastructure to deploy Openshift on GCP.

##### Additional Guides

- [Creating a custom RHEL 7.7 Server Image on GCP](https://github.com/chainlynx/google-cloud-rhel-image) 
- [Deploying Openshift Enterprise on GCP](https://github.com/chainlynx/google-cloud-openshift-ocp)
- [Deploying Openshift OKD on GCP](https://github.com/chainlynx/google-cloud-openshift-okd)

### Prerequisites

- You will need a Google Account
- Your Google Account will need a project and billing setup
- SSH Public Key Added to Metadata
    - See: [Managing SSH keys in metadata](https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys)

### Steps

- [Creating a Centos 7 Instance on GCP](Creating-Centos7-Instance-GCP.md)
- [Installing / Configuring GNOME](Installing-Configuring-GNOME.md)
- [Installing / Configuring a VNC Server](Installing-Configuring-VNC.md)



