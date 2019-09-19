## Google Cloud - Configuring a Centos 7 Workstation

### Description

This guide is focused on creating a Centos 7 workstation specific to the google cloud platform. 

The purpose of this workstation is to have a linux (centos) based workstation from which to create custom
images, for use on GCP (Google Cloud Platform).

This guide is part of a series of guides aimed at setting up an Openshift Cluster on GCP, leveraging a 
custom RHEL 7.7 server image, and setting up the infrastructure to deploy Openshift on GCP.

######Additional Guides

- [Creating a custom RHEL 7.7 Server Image on GCP](https://github.com/chainlynx/google-cloud-rhel-image) 
- [Deploying Openshift Enterprise on GCP](https://github.com/chainlynx/google-cloud-openshift-ocp)
- [Deploying Openshift OKD on GCP](https://github.com/chainlynx/google-cloud-openshift-okd)

### Prerequisites

- You will need a Google Account
- Your Google Account will need a project and billing setup

### Quick Start

######Creating a Centos 7 instance

1. Login to your google account at https://cloud.google.com/
2. In the top right, select "Console" or navigate to https://console.cloud.google.com
3. Select your desired project, or create a new project.
4. Go to the VM Instances page (https://console.cloud.google.com/compute/instances)
5. At the top, select **Create Instance**
   - Specify a **Name** for your instance: 
        - Example: ***centos-desktop***
   - Optionally, change the **Region** and **Zone** for this instance
        - Example: Region: ***us-east1***, Zone: ***us-east1-b***
   - Select a **Machine configuration** for your instance
        - Example: ***n1-standard-2 (2 vCPUs, 7.5 GB memory)***
   - In the **Boot disk** section, click **Change** to configure your boot disk 
        - Select the **CentOS 7** image from the list of images under the ***OS Images*** tab.
        - Select your preferred **Boot disk type** and **Size** towards the bottom of the list.
            - Example: Boot disk type: ***Standard persistent disk***, Size (GB): ***200*** 
        - Click **Select** when finished to complete the Boot disk selection.
   - To add network tags and optionally select or add a network interface
        - In the **Management, Security, Disks, Networking, Sole Tenancy** section.
        - Select the **Networking** tab.
        - Add a **Network tag**.
            - Example: ***vnc-server***
        - Leave the **default** network interface.
        - (Optionally) You can change this network interface to use a custom interface. 
   - Finally, click **Create** to start your new instance.
        - Note: You can leave the rest of the settings to their defaults for the purpose of this example. 

###### Install / Configure the GNOME GUI on your instance


