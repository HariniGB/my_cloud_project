
Poto Booth Website
==================

Poto Booth is a cloud born 3 tier web application, that provides the end users a secured environment to upload, download, view and modify their image files in cloud. This application is entirely build on Amazon Web Services (AWS) like EC2, ELB, Lambda, AutoScaling Group, RDS (PostgreSQL), CloudFront, S3, S3 Transfer Acceleration, R53, CloudWatch, SNS and Route 53.

[![Poto Booth demo](https://i.imgur.com/co7enBZ.png)](https://www.youtube.com/watch?v=3VDgBgRh1Xs&feature=youtu.be)

## Table of content

- [Details](#details)
- [Introduction](#introduction)
    - [Feature List](#feature-list)
- [Demo](#demo)
    - [Login/Sign-up](#login)
    - [Upload](#upload-a-new-image-to-cloud)
    - [View](#view-image-details-in-list-page)
    - [Download](#download-from-cloud-front-faster)
    - [Update](#update-both-contents-and-image-file)
- [Links](#links)

## Details

|Title | Detail|
|---|---|
| University | [SJSU UNIVERSITY]( http://www.sjsu.edu/) |
| Domain | [AWS CLOUD TECHNOLOGIES](https://aws.amazon.com/)|
| Developer | [HARINI BALAKRISHNAN](https://www.linkedin.com/in/harini-balakrishnan/) |

## Introduction
Poto booth is a cloud born 3 tier web application, that provides the end users a secured environment to upload, download, view and modify their image files. This application provides features like cloud based object storage, security and efficient file management. This application also maintains a relationship between the user and the file they uploaded by tracking details like which user uploaded, updated the image file at what time. Main idea behind this application is to build unlimited storage space to upload image files, download those files with faster data retrieval from public internet, maintain the file details in a database and perform all these operations with user authentication. As a developer, I wanted to build an application that is highly scalable, highly available, load balanced with auto recoverable with 24x7 monitoring services. But I also wanted to develop this application with simple workflows and processes without costing more money. Keeping these featured in my mind, I decided to build this application using AWS Cloud services. By deploying this application in cloud-based infrastructure like Amazon Web Services (AWS), the application got instant advantages like auto scaling, on-demand provisioning, full automation and multiple integrated services. By using AWS cloud services, I was able to implement additional features like versioning of storage which keeps track of the updates in the image files by default, cross-region replication that makes the stored files available in different Availability Zones (AZs) and supports faster data transfer.

### Feature List
- Model—Vie—Controller (MVC) based web application to allow users to upload new file with maximum size of 10MB per file and store the image files in the cloud.
- Allow users to browse their uploaded image files in the home page with low latency.
- Keep track of the file’s contents and allow users to update the image file details. 
- Users can delete their files which will also delete their files from cloud storage.
- Provide the file related content’s to the users for their reference in the view page.
- Allow users to download the image files with low latency and faster data delivery.
- Notify the admin when a user uploaded a image file to the cloud with an email.
- 24x7 monitoring service for all the features with all logs and metrics maintenance.
- Maintain the cloud storage in multiple secured locations (Availability Zones) for data recovery and faster retrieval. This also enhances maintaining versions of the storage
- Configure the cloud storage with different types of archived storage based on the frequency of data usage and confidentialities. This is in-build in AWS S3 storage.
- Deploy the entire application in cost effective and auto-scaling cloud compute with proper load balance ti manage millions of user requests and auto recovery.
- Register this application with a Domain Name to make it available in public internet.
- Throughout the development and production, track the health of the application and notify the admin in case of emergency and alarm the situation for safety.

## Demo
### Login

* In Web::Page, root page (display no images unless logged in)
* Click on the Login option in the navigation pane or Sing-up if new user.
* Provide emailID and password
* Click "Login" 

![Login](https://i.imgur.com/XbaWvw9.png)

### Upload a new image to cloud

* In the home page click 'Add new photo' button
* Provide Title and Description
* Press 'Submit' button.
* Uploaded successflly in the cloud AWS S3

![Upload new image form](https://i.imgur.com/n4bUEMu.png)

### View image details in list page

* In the home page click on any image tha that you want to view
* Left side, the image file
* Righr side, the image related details
* You can Edit/ Delete the file from this form
* The images are retrieved from S3 via AWS CloudFront distribution Edge Location

![View the image details](https://i.imgur.com/YMEB4Uz.png)

### Download from cloud front faster

* In the home page click on any image tha that you want to download
* Click the 'Downlaod' button
* Th image will be downloaded in your local machine in the 'Downloads' folder

### Update both contents and image file

* In the home page click on any image tha that you want to Update
* Click 'Edit' 
* You can Update Title, Description and the image file itself by uploading a new file instead.

![Update your image file](https://i.imgur.com/61kh5zN.png)

## Links

* [Web site](https://www.youtube.com/watch?v=3VDgBgRh1Xs&feature=youtu.be)
* [Documentation](https://github.com/HariniGB/my_cloud_project/blob/master/README.md)
* [Source code](https://github.com/HariniGB/my_cloud_project/)
