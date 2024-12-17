# Project Report

## Author

ALFIYA - 24BSDS104

## Project Title

Server Management for Content Management System

## Introduction

A content management system (CMS) is software that helps users create, manage, store, and modify their digital content. 
This all-encompassing system is a one-stop-shop to store content—such as apps, images, and websites—in a user-friendly interface ,
that is customizable to an organization’s needs and their employees.

##Examples of a CMS

There are many different CMS options available. Each has its own purpose and relevant features to meet the organization’s needs.
Below are a few of the systems offered:

WordPress: Originally was a web content management system that was built to publish blogs, but has extended into many other areas.
The open source management system can be used for websites, professional portfolios, e-commerce stores and more.

Drupal: The open source CMS is used by many companies around the globe to build and maintain their websites.
The user interface is easily accessible and allows you to create and publish unlimited content.

Squarespace: Unlike the CMSs mentioned above, Squarespace is an all-in-one content management system, meaning with a single subscription the
owner can do it all without needing third-party integrations.This is a popular CMS for small businesses online and in-store.

Joomla: This CMS is another open source system to build websites and online applications.It is SEO-friendly and features unlimited designs 
and built-in multilingual capabilities.

Shopify: This e-commerce platform wouldn’t be able to function without its CMS.The platform is built for businesses that want to create 
online stores.They are then able to edit and manage different content types through one software system.

Adobe Experience Manager: The “marketer-and developer-friendly” software has a combination of CMS and DAM features. It’s fitting for 
businesses looking for one platform to handle their content management, digital asset management, digital enrollment, forms, and more.

Salesforce CMS: This hybrid CMS allows organizations to create and deliver content to any device and customize as the customer sees fit. 
The software is multi-language and can be run on the web or on an app.

Wix: The web-based platform is software that creators and businesses use to make and manage their own websites without needing to know how 
to code. The platform provides advanced SEO features and marketing tools.


## Commands Used

##Directory Creation & Organization

  cd ALFIYA/
  mkdir CloudComputing_Project
  ls
  cd CloudComputing_Project/
  clear
  mkdir cms_server
  ls
  cd cms_server/
  mkdir Wordpress Joomla Drupal Shopify
  ls
  cd Wordpress/
  mkdir themes plugins uploads logs
  ls
  cd ..
  cd Joomla/
  mkdir themes plugins uploads logs
  ls
  cd ..
  cd Drupal/
  mkdir themes plugins uploads logs
  ls
  cd ..
  cd Shopify/
  mkdir themes plugins uploads logs
  ls
  cd uploads
  mkdir images videos documents
  ls
  cd ..
  cd Drupal/
  cd uploads/
  mkdir images videos documents
  ls
  cd ..
  cd Joomla/
  cd uploads/
  mkdir images videos documents
  cd ..
  cd Wordpress/
  cd uploads/
  mkdir images videos documents
  ls
  cd ..
  ls -all
  ls -l
  cd Drupal/
  ls -all
  cd ..
  cd Wordpress/
  cd uploads
  cd images/

## Below are the commands used during the project development:

## Move and Rename Files:
  touch logo.png
  mv ./Wordpress/uploads/images/logo.png ./Joomla/
  mv ./plugin_old.zip ./plugin_updated.zip
  ls
## Navigation & Listing Files:
  cd ..
  ls -R - To list all subdirectories and files
## File Permissions Management:
  touch db_config.php
  chmod 600 db_config.php
  ls -l - To list all the properties of the file
## Backup Files:
  mkdir Backup
  cp -r ./cms_server/Wordpress/uploads/ ./Backup/
  ls
## Removing Files & Directories:
  rm file_name  - to remove files
  rmdir test - to remove test directory
## Creating a Script for File Generation:
  touch image_{1..50}.jpg
## Exploring File History:
  history 20 - to view the history of 20 commands
  history | grep mv - Search the history for commands related to file manipulation, such as moving or renaming uploads.
## System Monitoring:
  uptime - server's uptime
  top - View system load and resource usage statistics, focusing on PHP and MySQL performance during peak traffic.
  echo "top - 16:29:16 up  6:39,  2 users,  load average: 0.05, 0.30, 0.34
  Output :Tasks: 331 total,   1 running, 329 sleeping,   0 stopped,   1 zombie
  %Cpu(s):  0.7 us,  0.2 sy,  0.0 ni, 99.0 id,  0.1 wa,  0.0 hi,  0.0 si,  0.0 st
  MiB Mem :   3348.4 total,    492.2 free,   1536.8 used,   1319.5 buff/cache
  MiB Swap:   8582.0 total,   7426.2 free,   1155.7 used.   1335.1 avail Mem"
  top - 16:29:16 up  6:39,  2 users,  load average: 0.05, 0.30, 0.34
  Tasks: 331 total,   1 running, 329 sleeping,   0 stopped,   1 zombie
  %Cpu(s):  0.7 us,  0.2 sy,  0.0 ni, 99.0 id,  0.1 wa,  0.0 hi,  0.0 si,  0.0 st
  MiB Mem :   3348.4 total,    492.2 free,   1536.8 used,   1319.5 buff/cache
  MiB Swap:   8582.0 total,   7426.2 free,   1155.7 used.   1335.1 avail Mem
## Ping Test & Network Verification:
  ping example.com - Verify network connectivity 
## Search for Specific Files or Content:
  grep -r wp-config.php - Search for a specific file
  grep -r "define('DB_NAME')" - search for a specific string
## Create a Directory for Each CMS Instance:
  mkdir cms_wordpress cms_joomla cms_drupal
  chmod 766 cms_drupal/ - Assign permissions so that each directory is accessible only by the respective CMS administrator.
  chmod 766 cms_joomla/
  chmod 766 cms_wordpress/
## Create a Script for Directory Cleanup:
  touch emptyfile.sh
  nano emptyfile.sh
  rmdir documents videos - empty directories
  chmod 700 emptyfile.sh - to give permission to execute
  ./emptyfile.sh
## File Sorting & Management:
  du - to sort image file according to size
  ls -las :to Create a report listing the largest and smallest files
##  File Type Identification:

  find . -type f \( -iname "*.jpg" -o -iname "*.mp4" -o -iname "*.pdf" \) : Identify and list files of specific types in the "uploads" 
  directory, such as .jpg for images, .mp4 for videos, and .pdf for documents.
## File Compression and Archive:

  tar -czvf joomla_themes_backup.tar.gz themes : Compress the "themes" directory of the Joomla instance into a single archive file named 
  "joomla_themes_backup.tar.gz".

  tar -tzvf joomla_themes_backup.tar.gz : to list the contents of the archive.

