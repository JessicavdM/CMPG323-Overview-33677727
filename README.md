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

# Project 1 Burndown Chart
This burndown chart is for 8 August to 17 August.
![burndow sprint 2](https://user-images.githubusercontent.com/83065167/184940761-4ed5cdab-19ef-4bb8-9863-0b9de59178a7.png)
