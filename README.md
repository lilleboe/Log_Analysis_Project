## Overview
The Log Analysis Project is part of the [Udacity](http://udacity.com) Nanodegree Full Stack Web Developer program. 
It is a python program that runs reports against a psql database located on a VM.

## Table of contents

- [Requirements](#requirements)
- [Instructions](#instructions)


## Requirements

Download and install the following software and files:
- Python is required to be installed on the system that will run the project. The project was created using Python version 2.7.13; however, it should also work on later versions. [Download Python](https://www.python.org/ftp/python/2.7.13/)
- Download and install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- Download and install [Vagrant](https://www.vagrantup.com/)
- Download the [news](https://d17h27t6h515a5.cloudfront.net/topher/2016/August/57b5f748_newsdata/newsdata.zip) data
- Clone Udacity's [repositiy](https://github.com/udacity/fullstack-nanodegree-vm): 

The following python file is required for the project to run correctly.
- reportrunner.py

## Instructions

After obtaining the files, downloading and installing the software you are ready to run your reports.  In your vagrant shell and in the same directory your reportrunner.py script is located run this command:
> python reportrunner.py

The output of running that command will produce three reports that answer the following questions:
- What are the most popular three articles of all time?
- Who are the most popular article authors of all time?
- On which days did more than 1% of requests lead to errors?

The reports are in the following format:
`
============================================================
Most popular three articles of all time
------------------------------------------------------------
Candidate is jerk, alleges rival -- 342102 views
Bears love berries, alleges bear -- 256365 views
Bad things gone, say good people -- 171762 views
============================================================
`
