# --------------------- Jenkins Assignment 3 ----------------------

## Step 1

```bash
Go to your browser and search for Google Devlopers Console >> Go to APIs & Services
```

## Step 2

```bash
Go to Select a project  click on 'Create New Project' 
```
![project](/uploads/e04d2e7ebe8fb5835e61a3d4c0da511c/project.png)

## Step 3

```bash
Give Project Name, here I will use “Jenkins-demo” and create a project.
```

## Step 4 

```bash
Now click on on the “Credentials” Tab on the left slide bar & now click on “Configure Consent Screen”
```

## Step 5 

```bash
Go to the OAuth consent screen tab .Enter App name “Jenkins” & your 'Email address' Then Enter Details in 'Authorized domain 1' DNS in Authorized domains then save them
```


## Step 6

```bash
Then Go to “Credentials Tab” click on  'Create Credentials' select 'OAuthClientID' Then Select Application type 'Web Application' give the name “JenkinsSSO”
```
![oth1](/uploads/7fdcd962042856f9cb20aa496a52559d/oth1.png)

![oth2](/uploads/a3bccb8efdab1dcf4be7e619a3b8ff09/oth2.png)

## Step 7

```bash
Now Enter DNS details in 'Authorized JavaScript origins' Then Enter DNS details again in 'Authorized redirect URIs' By click on 'Add URL' with additional content in 'securityRealm/finishLogin' for example 'http://ec2-13-127-65-117.ap-south-1.compute.amazonaws.com:8080/securityRealm/finishLogin' and save them.
```
![cred](/uploads/c86080384d9114fc4b825d43c23b699a/cred.png)

## Step 8

```bash
Now  After above step some Credentials are generated 'client ID' and 'Client_Secret' you can copy or download them
```

## Step 9  [Configure Jenkins]

```bash
Go to Manage Jenkins >> Manage Plugins >> Available plugins and Download "Google Login Plugin"
```
![plugin](/uploads/f5823e4285406a40a2e4c14e964d23ae/plugin.png)

## Step 10 

```bash
Now go to 'Configure Global Security' Change security realm to >> 'Login with Google' and Paste the 'Client ID' and 'Client secret' generated in Create Credential Step and Save them.
```
![config](/uploads/30e69ce3324c36c6253dc2a29e81e20f/config.png)

## Step 11 

```bash
And last task is Go to 'manage jenkins' >> 'Configure System'  >> Jenkins locations, and paste the DNS in that column
and save them and now every thing is done just logout and try login by google
``` 
![url](/uploads/5236ccb23e578099b8049096d477c710/url.png)
![image__4_](/uploads/25192895f7a1a3fb8f9add7a89ef71d6/image__4_.png)
