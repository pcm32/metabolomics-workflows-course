# Portal practical

Prepared by Sijin He and Pablo Moreno

## Overview

1.- Access the Phenomenal Portal on https://portal.phenomenal-h2020.eu/. 

2.- The PhenoMeNal Portal consists on three main parts, displayed in this order in the main page: 

 - Cloud Research Environment Deployment
 - App Library
 - Documentation

3.- On the left, under "Test drive our Cloud Research Environment", click on "Galaxy Workflow" button, it will take you to the PhenoMeNal Public Galaxy instance.
![images/test-drive-button.png]

4.- Go back to the Portal tab.
![images/browser-tab-porta.png]

## Login and Cloud deployment

5.- Now, to the right, click on "Create Cloud Research Environment" blue button. This will take you to the login page, where our single sign on (SSO) will allow you to register with Google, LinkedIn, Orcid or your academic account (provided is recognized by Elixir).
![images/cre-creation-button.png]

6.- On the login page, click on the "SSO" button. It will ask you to choose an identity provider, choose one and proceed to authenticate with it. The first time it will ask you to register Elixir, follow this registration process. After that, you might need to open again the Portal URL https://portal.phenomenal-h2020.eu/ and click on "Create Cloud Research Environment" if you had to go through the Elixir registration. This only happens when registering. Alternatively, you might see a Welcome with your name on it, please click "Continue".
![images/sso-button.png]

7.- Once we login, you should see the ELSI requirements and terms & conditions, which can be viewed by clicking the links. Then, you will need to agree with the terms & conditions as well as with the ELSI requirements for the Portal before you can continue. 
![images/terms-and-conditions.png]

8.- You will now be able to select from the available cloud providers to run a deployment. You will only be able to do this if you have an account with credits on Amazon AWS or Google GCE cloud services currently. 
![images/available-cloud-providers.png]

9.- **Optional** - Deployment with AWS: 

9.1.- If you have AWS credentials, as the demonstrator, click on "Select" on the Amazon AWS box.
![images/amazon-aws-box.png]

9.2.- Select a Region, paste your Access Key and your Secret Access Key. Then press "Next"
![images/amazon-regions.png]
![images/amazon-access-keys.png]

9.3.- In order to secure your Galaxy instance, the system requires that you set an email and password (and confirm it). This will be used as well for your Jupyter and Kubernetes Dashboard credentials. Please add now an email and password (and confirm it) in the fields. Please don't use any sensitive passwords. Then press "Next", and confirm in the following part pressing "Deploy". The deployment will start.
![images/amazon-galaxy-auth.png]

9.4.- Optional point: if you really want to see what is going behind the scenes, and get all the Infrastructure as code logs, head over to https://portal.tsi.ebi.ac.uk/, press login at the upper right corner, and then login using the SSO button. Once logged in, go to menu and choose "Deployments". You should see a "Phenomenal VRE" deployment with a progress circle. Click on that card, and then move to the lowest part of the new page, click there on the "eye" icon next to "Deployment logs", and enjoy your logs! 

Skip to point 10 for the Public instance, or to point 14 for the App Library, then come back here.

9.5.- Later on (around 20 minutes), check whether the deployment is ready on the Portal's depoyment page. If it says ready (or if the progress bar is done and you see "Installation complete", click on it), you will be able to click on the "Galaxy" button, which will take you to the deployed CRE Galaxy frontend. On that instance, you should be able to login with the pre-set email and passowrd.

9.6.- You can now try one of the PhenoMeNal workflow tutorials available at https://portal.phenomenal-h2020.eu/help under "User tutorials", or play with individual tools.

9.5.- To destroy your instance, go to https://portal.phenomenal-h2020.eu/cloud-research-environment, press "More" and then "Destroy". Please make sure that the instance has been destroyed in AWS later on, specially if there are errors.

## Public instance account 

10.- Open a new PhenoMeNal portal tab https://portal.phenomenal-h2020.eu/, and click on CRE.
![images/cre-button.png]

11.- On the PhenoMeNal Cloud, click on "Register". Enter your email, password (and confirm the password). Then press "Register" again.
![images/pheno-cloud-register.png]

12.- Press "Login", it should take you to the Galaxy Public instance page. On the upper right, click on "Login or register", select "Login" on the pull down menu.
![images/galaxy_register.png]

13.- You can now try one of the PhenoMeNal workflow tutorials available at https://portal.phenomenal-h2020.eu/help under "User tutorials", or play with individual tools.

## App Library

14.- Open a new PhenoMeNal portal tab https://portal.phenomenal-h2020.eu/, and click on App Library at the top.

15.- App library is a catalogue of containerised tools. 

16.- On the left hand side, there is a filter which helps users to filter applications according to the characteristics of the applications, such as functionality, approaches, and instrument data types. For example, we can select MS, which will show a list of applications that are related to MS. 

17.- Select only NMR on the filter, which shows a list of applications that contains MS or NMR. When we click rnmr, we will see all information relating to this application, including, website, version, git repo, features, description, screenshots of the application, installation, usage instruction, and publication.

18.- Besides using filters, we can also use text-based search to look for a specific application, for example, we can look for metabolights labs uploader, by typing in “metabolights”, we are able to find the application. When we click the logo of the application, users will be redirected to a page of the application.

## Help

19.- Open a new PhenoMeNal portal tab https://portal.phenomenal-h2020.eu/ (or use an existing one), and click on Help at the top.

20.- At the top of the help page, there is a search bar which allows users to search for documentations

21.- For example, we can search for "Galaxy". Choose the first result, take a look.

22.- Additionally, topics are organized under three major sets: User Documentation, Developer Documentation and User Tutorials. The last one focuses on workflows to be run inside the CRE.










