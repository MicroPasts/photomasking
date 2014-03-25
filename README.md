PyBossa photo masking application
=================================

This application has three files:

*  createTasks.py: for creating the application in PyBossa, and fill it with some tasks.
*  template.html: the view for every task and deal with the data of the answers.
*  tutorial.html: a simple tutorial for the volunteers.

![alt screenshot](http://i.imgur.com/ag9QvLf.png)

Testing the application
=======================

You need to install the pybossa-client first (use a virtualenv):

```bash
    $ pip install -r requirements.txt
```
Then, you can follow the next steps:

*  Create an account in PyBossa
*  Copy under your account profile your API-KEY
*  Run python createTasks.py -u http://crowdcrafting.org -k API-KEY
*  Open with your browser the Applications section and choose the FlickrPerson app. This will open the presenter for this demo application.

Documentation
=============

We recommend that you read the section: [Build with PyBossa](http://docs.pybossa.com/en/latest/build_with_pybossa.html) and follow the [step by step tutorial](http://docs.pybossa.com/en/latest/user/tutorial.html).

Adding pictures from a folder in an S3 bucket
=============================================

This application supports public S3 buckets. Adding pictures/photos from
a folder in a S3 bucket is as simple as the following command:

```bash
    $ python createTasks.py -s server -k api-key -x -b "folder/in/s3/"
```

**NOTE**: This application uses the [pybossa-client](https://pypi.python.org/pypi/pybossa-client) in order to simplify the development of the application and its usage. Check the [documentation](http://pythonhosted.org/pybossa-client/).


LICENSE
=======

Please, see the COPYING file.
