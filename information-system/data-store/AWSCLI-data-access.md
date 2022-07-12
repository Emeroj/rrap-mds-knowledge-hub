---
layout: default
title: Data access to S3 with AWS CLI 
nav_order: 9
grand_parent: Information System
parent: Data store
---

{: .no_toc }

# Data access to S3 with AWS CLI 

<details  open markdown="block">
  <summary>
    Table of contents
  </summary>
{: .text-delta }
* TOC
{:toc}
____
</details>

## Overview

TO DO

### Setting up the AWS CLI v2
In order to use the AWS CLI for uploading (and downloading) you will need to install it first. Please see [this page](./setting-up-the-aws-cli.html){:target="\_blank"} for instructions on how to setup the AWS CLI v2 on your system.


### Uploading files
Once the AWS CLI is installed copy the AWS access credentials you require (LINUX, Windows CMD or Powershell) by clicking on the **Click to copy** button.  
Paste the credentials into your AWS CLI terminal.  
Navigate to the location of your dataset (the XXXXX should be the folder where your dataset is)   
`aws s3 sync dataset/ s3://dev-rrap-storage-bucket/XXXXX/10378-1-1687302/`   
Verify that the files were uploaded correctly by running the following command and verifying the contents are accurate:  
`aws s3 ls s3://dev-rrap-storage-bucket/XXXXX/10378-1-1687302/`  

|                                 Uploading large files                                    |
| :---------------------------------------------------------------------------------:      |
| <img src="../../assets/images/data_store/uploadLargeFilesStep1.png" alt="drawing" width="600"/> |



___