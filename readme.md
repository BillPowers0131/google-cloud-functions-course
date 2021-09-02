# Google Cloud Functions Course
## Starting a new project in Google Cloud
To start a new project go to the [Google Cloud Platform console](https://console.cloud.google.com/home/dashboard?project=cloud-functions-course-324509&authuser=1)
## Creating a Virtual Environment
First we have to install ``python3-venv`` with the following command:
```
sudo apt isntall python3-venv
```
The we execute the following command:
```
python -m venv venv
```
To activate the virtual environment we issue the following command:
```
source venv/bin/activate
```
In order to add new packages to our venv we issue the following command:
```
pip install -r requirements.txt
```
## Deploying our function
First we have to set our project ID with the following command:
```
gclooud config set project [YOUR PRO?JECT ID]
```
Then we deploy our function wiht this command:
```
gcloud function deploy [FUNCTION NAME] --runtime python38 --trigger-http

