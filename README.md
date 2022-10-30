# CMPG323-Overview-33677727
## Project Repositories
### Project 1
In this Project the 'CMPG323-Overview-33677727' repository was created. This repository will be used to provide an overview of all the Projects and as a source reposiroty for the 'CMPG 323 Project Progress Tracking' Kanban project.  
### Project 2
This Project will create a 'CMPG323-Project2-33677727’ repository to store and work on the main parts of Project 2. It will also make use of the 'CMPG323-Overview-33677727' repository in order to keep the 'CMPG 323 Project Progress Tracking' Kanban project up to date.
### Project 3
This Project will create the 'CMPG323-Project3-33677727’ repository and will fork the existing GitHub repository. This project will also use repository classes that will contain data access operations. Project 3 will also use the 'CMPG323-Overview-33677727' repository in order to keep the 'CMPG 323 Project Progress Tracking' Kanban project up to date.
### Project 4
This Project will create a 'CMPG323-Project4-33677727’ repository. This Project will require the cloning of the 'CMPG323-Project3-33677727’ repository (as Project 4 will be working with the web application developed in Project 3). Project 4 will also make use of the 'CMPG323-Overview-33677727' repository in order to keep the 'CMPG 323 Project Progress Tracking' Kanban project up to date.
### Project 5
This Project will create the 'CMPG323-Project5-33677727’ repository. Project 5 will require the cloning of the 'CMPG323-Project4-33677727’ repository. It will also make use of the 'CMPG323-Overview-33677727' repository to keep the 'CMPG 323 Project Progress Tracking' Kanban project up to date. 

## Project and Repository Context and Integraion
![project integration](https://user-images.githubusercontent.com/83065167/184691813-7af65395-a819-4ce8-82e5-357bd7301ec3.png)

The 'CMPG 323 Project Progress Tracking' Kanban project will be used to track the progress and plan the work and tasks for all the CMPG 323 Projects as well at the POE. All the Projects together will be treated as one big project (tracked by the 'CMPG 323 Project Progress Tracking' Kanban project). This will create a central planning area for the whole semester and will allow for easy managing and overviewing of all the projects and sprints. One big managing project will also allow for a smoother transition from sprint to sprint and project to project as some projects overlap within certain sprints. Each individual Project will have its own repository and will be separate from other Projects but will still be within the big overarching project. All the Projects will be linked through the 'CMPG323-Overview-33677727' repository except for the POE which will take information from all the projects and repositories.

## Branching Strategy
### Project 1
This project does not require the use of source control and therefore does not need a branching strategy.
### Project 2 and 4
Because  these projects will have lots of smaller functions and methods and won't be implementing big features, a variation on the GitHub Flow branching strategy will be used. There will be no release branch, but there will be feature branches that stems directly from the main branch. Once the feature is complete the branch will be merged back into the main branch. There will also be a hotfix branch for small fixes that may be needed on the main branch.
<br/>Branches:
* main
* feature
* hotfix
### Project 3 and 5
These projects will need a development branch and thus a version of the GitFlow branching strategy will be used. All features will be developed on a feature branch which stems from the development branch. Once the feature is complete the feature branch will be merged with the development branch. Once the development branch is ready to be realeased, the branch will be merged with the main branch.There will also be a hotfix branch for any small fixes that the main branch may need.
<br/>Branches:
* main
* development
* feature
* hotfix

## Use of .gitignore Files
Because the API keys and secrets will be stored outside of GitHub no security key files or API keys will be added to te .gitignore files for any of the Projects. The only files that will be added to a .gitignore file will be any system-specific files that may be encountered in Project 3,4 and 5. Project 1 and 2 will not make use of a .gitignore file.

## Storage of Credentials and Sensitive Information
For Project 2 and 3, specifically, no credentials are to be stored on GitHub. All credentials and sensitive information pretaining to any of the Projects will be stored in an Azure Key Vault (Azure Key Vault is a cloud service for securely storing and accessing any information that must be tightly controlled). By keeping all sensitive information seperate from the GitHub repositories (which will all be public) the information can be kept secure and no third party will be able to gain access to any of the systems.
<br/><br/>





# Project 1 Information
## Burndown Chart
This burndown chart is for 8 August to 17 August.
![burndow sprint 2](https://user-images.githubusercontent.com/83065167/184940761-4ed5cdab-19ef-4bb8-9863-0b9de59178a7.png)
<br/><br/><br/>



# Project 2 Information
Project repository: CMPG232Project2-33677727
## Use the API
Enter the folllowing URL to access the API:
<br/> https://connectedoffice33677727.azurewebsites.net/swagger/index.html

## Authentication Aspects
To use the Zone and Category endpoints a user must be an admin user. A normal user can use the Devices endpoints and the Authentication endpoints. A user must login to recieve a token (use user name and password to login), be sure to copy this token with no "" marks. Click on the lock to the right of the endpoints and type in "Bearer \<token>" to use the endpoints. 

## Endpoints
#### Authenticate
* Create a user(POST/api/Authenticate/register)
* Create an admin user (POST/api/Authenticate/register-admin)
* Log in and recieve a token (POST/api/Authenticate/login)
#### Categories
* Get all Categories (GET/api/Categories)
* Get a specified Category entry by id (GET/api/Categories/{id})
* Create a new Category (POST/api/Categories)
* Update an existing Category (PATCH/api/Categories/{id})
* Delete an existing Category (DELETE/api/Categories/{id})
#### Zones
* Get all Zones (GET/api/Devices)
* Get a specified Zone entry by id (GET/api/Devices/{id})
* Create a new Zone (POST/api/Devices)
* Update an existing Zone (PATCH/api/Devices/{id})
* Delete an existing Zone (DELETE/api/Devices/{id})
#### Devices
* Get all Devices (GET/api/Zones)
* Get a specified Device entry by id (GET/api/Zones/{id})
* Create a new Device (POST/api/Zones)
* Update an existing Device (PATCH/api/Zones/{id})
* Delete an existing Device (DELETE/api/Zones/{id})

## API manager Screen Shots
![image](https://user-images.githubusercontent.com/83065167/190157686-da3f3a49-7425-4ce9-b1ca-3d6d01bdb12c.png)

![image](https://user-images.githubusercontent.com/83065167/190157559-0a65ad7c-bf4c-40b5-9277-86f010c64903.png)
<br/><br/><br/>



# Project 3 Information
Project repository: CMPG323Project3-33677727
The Web App developed for this project is meant to store information on IoT devices. The App allows you to store informaton on the Category of the Device (Name, Description and Date Created), on the Zone the Device is located in (Name, Description and Date Created) as well as information on the IoT Device itself (Name, Status, Is Active, Date Created, Category and Zone). The Web App makes use of a database hosted on Azure to store the information and the Web App is also hosted on Azure.

This Web App makes use of the MVC architecture pattern and uses Views, Models and Controllers. The Controller makes use of Repositories. A Generic Repository is used for all Database Context access operations. Each class is also given their own Repository which their controller uses to access the datbase indirectly.

## Using the Web App
To access the Web App hosted on Azure the following link can be used:
https://devicemanagementwebapp33677727.azurewebsites.net

<br/>![image](https://user-images.githubusercontent.com/83065167/193046327-e7b366fb-17d8-439d-b376-7d1cb4e62755.png)

To use the Web app you can Register your own account or use the provided Login credentials. Once you have logged in three new tabs will become avaliable to you, namely Zones, Categories and Devices. 

<br/>![image](https://user-images.githubusercontent.com/83065167/193046489-bb5d723b-6a0d-4eb7-aa31-43e6edc15dcb.png)

You can then Add, Edit, Delete and View Zones, Categories and Devices on the Web App. The Web App is quite user friendly and there should be little difficulty navigating to the different sections. Once you have added, edited or deleted all the Zones, Categories and Devices you want, you can then log out using the logout button on the menu tab.


<br/>![image](https://user-images.githubusercontent.com/83065167/193046724-4fccc45b-2aea-479f-b23b-8460a2f450a2.png)


## Security
To ensure that no credential are avaliable or present in the Project 3 repository, all the files that contain sensitive information or that may contain credentials have been added to the gitignore file. This was done after the repository was forked and before any work was done to ensure no credential are present in earlier commits of the project.

## Project Accesability
Because this project was forked from another reopsitory it was not possible to make the repositry private as all forked repositories must be public.
<br/><br/><br/>




# Project 4 Information
Project repository: CMPG323Project4-33677727

## How to Use the Automation
Once you click the play button in UIpath Orchestrator or run the process from UIpath Assistant you will be prompted to select an excel file to test the Web Page against.
Once you have selected an excel File the automation will run and test everything on the https://connectedoffice-devicemanagement.azurewebsites.net web page (including logging in) and when it is done it will have printed the results of the testing in the "Test Results" tab of the selected excel file. Do not use the mouse or keyboard while the automation is running, go make yourself some tea instead :)

## Excel File Requirements
The sheets of the excel file must be in the order that the records must be created (Devices can't be created if there aren't any Zones or Categories). 
<br/>
![image](https://user-images.githubusercontent.com/83065167/198303970-c65a271f-2323-4ee6-b4c1-1459ce1eb6b1.png)
<br/>
The last sheet in the excel file must have he name "Test Results" and must have a list of the ID of all the test data as well as the following headings: Create Test Passed, Read Test Passed, Update Test Passed, Delete Test Passed. (Is case sensitive). 
<br/>
![image](https://user-images.githubusercontent.com/83065167/198305557-f4572bfd-0262-4ab6-88e6-f799e0a1495a.png)
<br/>
Each sheet will be used to test an entity (Zone, Category or Device) in the Web page. The columns of the tables in excel must match the lables in the web page. The first column of these sheets must also be and ID column (case sensitive).
<br/>
![image](https://user-images.githubusercontent.com/83065167/198304816-0fa51809-e782-4d50-9430-753ab54c7684.png)
<br/>
![image](https://user-images.githubusercontent.com/83065167/198305001-9587d73a-4534-43e2-82f8-01abaa157bf0.png)
<br/>
An example of an acceptable excel file is in this repo under "Connected Office Test Data".



