# Google APIs

You need to login to [Google developers](https://developers.google.com/profile/u/me)


## Google APIs Explorer

The Google APIs Explorer is a tool available on most REST API reference documentation pages that lets you try Google API methods without writing code:

- [Open Google APIs Explorer](https://developers.google.com/apis-explorer) 


We will use Google's Drive API v3 as an example.


## Google Drive API v3

We want to create a Python command-line application that makes requests to the Drive API.


### Set up Anaconda environment

First we need to setup a new Anaconda environment where we will use `pip` to install packages (not conda):


```bash
conda create -n drive python=3.9 pip 
```


### Install the Google client library

Activate your environment:

```bash
conda activate drive
```

Install some libraries for Python:


```bash
pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib pandas
```

### Python quickstart


Next, go to the (Python quickstart)[https://developers.google.com/drive/api/quickstart/python] and complete the instructions for step 1, 3, 4 and 5:

1. Set up your environment (choose user type external)
1. Install the client library (we already completed this step)
1. Set up the sample.
1. Run the sample.

