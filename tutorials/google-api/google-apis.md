# Google APIs

## Google developer account

First, you need to create an account: [Google developers](https://developers.google.com/profile/u/me)


## Google APIs Explorer

The Google APIs Explorer is a tool available on most [REST API](https://en.wikipedia.org/wiki/Representational_state_transfer) reference documentation pages that lets you try Google API methods without writing code:

- [Open Google APIs Explorer](https://developers.google.com/apis-explorer) 


We will use Google's Drive API v3 as an example.


## Google Drive API v3

We want to create a Python command-line application that makes requests to the Drive API by using OAuth 2.0 for authorization.


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
pip install --upgrade google-api-python-client google-auth-httplib2 google-auth-oauthlib googleapiclient pandas
```

### Configure the OAuth consent screen

When you use OAuth 2.0 for authorization, Google displays a consent screen to the user including a summary of your project, its policies, and the requested authorization scopes of access.


:::{note}
 If you don't know required consent screen information, you can use placeholder information.
:::

Follow these instruction: [Configure OAuth consent & register your app](https://developers.google.com/workspace/guides/configure-oauth-consent)

### Python quickstart


Next, go to the [Python quickstart](https://developers.google.com/drive/api/quickstart/python) and complete the instructions for step 1, 3, 4 and 5:

1. Set up your environment (choose user type external)
1. Install the client library (we already completed this step)
1. Set up the sample.
1. Run the sample.