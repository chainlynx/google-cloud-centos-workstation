## Google Cloud - Configuring a Centos 7 Workstation (GNOME GUI)

### Description

This guide is focused on creating a Centos 7 workstation specific to the google cloud platform. 

The purpose of this workstation is to have a linux (centos) based workstation from which to create custom
images, for use on GCP (Google Cloud Platform).

This guide is part of a series of guides aimed at setting up an Openshift Cluster on GCP, leveraging a 
custom RHEL 7.7 server image, and setting up the infrastructure to deploy Openshift on GCP.

### Prerequisites

- You will need a Google Account
- Your Google Account will need a project and billing setup
- SSH Public Key Added to Metadata
    - See: [Managing SSH keys in metadata](https://cloud.google.com/compute/docs/instances/adding-removing-ssh-keys)

### Steps

- [Creating a Centos 7 Instance on GCP](Creating-Centos7-Instance-GCP.md)
- [Install / Configure the GNOME GUI and VNC Server](Installing-Configuring-GNOME.md)

### Follow on Guides 

- This guide is a pre-requisite to creating custom RHEL images for use on GCP. To create a RHEL 7.7 Image, you need a Linux machine to create the image. To deploy Openshift Enterprise on GCP, you need to setup your cluster nodes based on the RHEL image. 
- **Note**: You can use the default RHEL 7 images available on GCP, however these include their own subscription to RH, and thus incur an additional $40 charge per instance. So it's cheaper to create a custom image and attach it to your RH subscription without using the default GCP RHEL images.
  
  
- [Creating a custom RHEL 7.7 Server Image on GCP](https://github.com/chainlynx/google-cloud-rhel-image) 
- [Deploying Openshift Enterprise on GCP](https://github.com/chainlynx/google-cloud-openshift-ocp)

### Additional Guides

- **Note**: Deploying Openshift OKD on GCP does not require a custom RHEL image as no RH subscription is required for your nodes. The walkthrough for OKD uses Cento 7 instead of RHEL 7.7, so the prerequisites for a custom RHEL image are not needed for OKD.


- [Deploying Openshift OKD on GCP](https://github.com/chainlynx/google-cloud-openshift-okd)


