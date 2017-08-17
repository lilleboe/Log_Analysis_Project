## Overview
The Log Analysis Project is part of the [Udacity](http://udacity.com) Nanodegree Full Stack Web Developer program. 
It is a python program that runs reports against a psql database located on a VM.

## Table of contents

- [Requirements](#requirements)
- [Instructions](#instructions)
- [Customizations](#customizations)
- [Enhancements](#enhancements)


## Requirements

Download and install the following software and files:
- Python is required to be installed on the system that will run the project. The project was created using Python version 2.7.13; however, it should also work on later versions. [Download Python](https://www.python.org/ftp/python/2.7.13/)
- Download and install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- Download and install [Vagrant](https://www.vagrantup.com/)
- Download the [news](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip) data
- Clone Udacity's [repositiy](https://github.com/udacity/fullstack-nanodegree-vm). This contains the Vagrant config file.

The following python file is required for the project to run correctly.
- reportrunner.py

## Instructions

After starting up Vagrant navigate to the location of your newsdata.sql file.  Here you are going to load the database with the proper tables and data.  Run this command:
> psql -d news -f newsdata.sql

You should be ready to run your report.  In the same directory your reportrunner.py script is located run this command:
> python reportrunner.py

The output of running that command will produce three reports that answer the following questions:
- What are the most popular three articles of all time?
- Who are the most popular article authors of all time?
- On which days did more than 1% of requests lead to errors?

The reports are in the following format:
```
============================================================
Title (question being answered)
------------------------------------------------------------
data row 1
data row 2
...
data row n
============================================================
```

## Customizations

Within the reportrunner.py file's main function, you can add more queries for further reporting by appending information to both the printInfo and queries lists.  The printInfo list adds the title and any text to be added to the end of each row.  The queries list contains just that, queries to be sent to the database.

## Enhancements

A list of out of scope updates/features that may be implemented at a later date:
- Queries saved in another database, text file, etc instead of hard coded in the python
- Output of the queries saved in various formats (text, excel, etc.)
- Front end that provides available reports and recieves results displayed to the browser.
