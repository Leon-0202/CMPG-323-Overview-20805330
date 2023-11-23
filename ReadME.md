## Table of contents

- [Repositories](#repositories)  
- [Project and Repository Context](#project-and-repository-context)  
- [Branching Strategies](#branching-strategies)  
- [gitignore Files](#gitignore-files)
- [Storage of Credentials and Sensitive Information](#storage-of-credentials-and-sensitive-information)
- [Burndown Chart](#burndown-chart)
- [Training Completed](#training-completed)
- [References](#references) 

## Repositories
Repositories to be created and used for each project:  
### CMPG-323-Overview-20805330: Used primarily for Project 1 - Agile & Scrum, but also serves as a supporting repository for the other projects. 

### CMPG-323-Project2-20805330: Used for Project 2 - API Development.
#### The API can be accessed on Azure with the following link:
https://restfullapi.azurewebsites.net/index.html
#### The WebAPI was created as, and makes use of the following core features:  
- Created as an ASP.NET Core Web API, using .NET 6.0 
- Makes use of a SQL Server Database, hosted on Azure
- The DbContext, model, and controller classes were scaffolded using Entity Framework Core
- Uses Swagger support
- Implements authentication to secure its endpoints 

#### The following minor features were also implemented:
- Data Transfer Objects are used to facilitate input and output of data
- JsonPatchDocuments are used when PATCHing existing records in the database

### CMPG-323-Project3-20805330: Used for Project 3 - Standards & Patterns.
#### The webapp can be accessed on Azure with the following link:
https://cmpg323-project3-webapp.azurewebsites.net/
#### The Web Application was created as, and makes use of the following core features:  
- Created as an ASP.NET Core Web Application, using .NET 6.0 
- Makes use of a SQL Server Database, hosted on Azure
- Follows the repository design pattern
- Includes a servide layer
- The design pattern layers are implemented between projects
  
### CMPG-323-Project4-20805330: Used for Project 4 - Testing & RPA.
#### Automation Process Overview
The UiPath User Acceptance Testing automation process has some of the following core features:
- It tests CRUD operations.
- It first adds all the records for a selected entity (e.g., Customer), then edits all records, and then deletes all records.
- The user can select which entities to test during a run.
- The automation process logs the user in at the start of a run, and logs the user out at the end of the run.

### CMPG-323-Project5-20805330: Used for Project 5 - Reporting & Monitoring.

## Project and Repository Context
A repository is essentially a storage location (similar to a folder) that stores related files and documentation. A project is a management tool that helps improve visualization and organization of tasks such as issues and pull requests (Khillar, 2021).  
![alt text](https://3ba1f5b2.rocketcdn.me/wp-content/uploads/2021/03/GitHub-Repository-vs-Project.jpg)  
(Table used from http://www.differencebetween.net/technology/difference-between-github-repository-and-project/#:~:text=GitHub%20Repository%20vs.%20Project:%20Comparison%20Chart)  

So GitHub project CMPG-323-Project-20805330 will be used as an overview to help manage the flow of the tasks of the Github repositories for the five different projects, each of which will be linked to the project.  

![Projects_Repositories](https://github.com/Leon-0202/CMPG-323-Overview-20805330/assets/110893659/7d703558-ebc6-4ce7-aa7b-49c0e36d1e78)  

## Branching Strategies
Branching strategies to be used for each project:
- Project 1:  
Since the only file that needs to be edited for Project 1 is the README.md file, and seeing how it won't involve any code, it will be hot-fixed on the main branch.
- Project 2 to 5:  
Innitially, a remote repository will be created for a project.  Then a local repository will be created by cloning the remote repository to a specified directory.

Whenever a new feature is to the be added to the project, or whenever existing code needs to be updated/changed, a new branch will be created and checked out on the local repository (if the remote repository is ahead of the local repository, the main branch will first be pulled from the remote repository). It is in this local working directory where the relevant code will be added/changed. The new code and files will then be added to the staging area, and then be subsequently committed to the local repository (still on the side branch, not the main branch), along with a descriptive message describing the changes made. The branch will then be pushed to the remote repository.  

From the remote repository, a pull request will be created.  The changes will reviewed, a proper description will be provided, and if automatically possible, merged into the main branch.  If not, the merge conflict will first be resolved before merging the side branch into the main branch.  After the merge request is completed, the side branch will subsequently be deleted.  

## gitignore Files
Visual Studio 2022 will be used as an IDE for the projects. Therefor, for each project's GitHub repository, a gitignore file will be added for Visual Studio.  This is so that Git does not track the .vs related Visual Studio files, and they do not get committed to the repository.  

## Storage of Credentials and Sensitive Information
No credentials or sensitive information will be stored in any of the repositories on GitHub.  Instead, the it will be stored locally (with redundant backups accross multiple devices/drives), and made available as needed.  

## Burndown Chart
![BurndownChart](https://github.com/Leon-0202/CMPG-323-Overview-20805330/assets/110893659/265a3160-78a7-4bca-8c1a-cb9844496217)  

## Training Completed
### Agile/Scrum
- 2023/08/07; Growing Agile; Scrum Basics; Certificate; https://growingagile.thinkific.com/courses/scrumbasics  
- 2023/08/09; Mindluster; Basics of Agile; Certificate; https://www.mindluster.com/certificate/8729

### Source Control
- 2023/08/01; Mindluster; Git/GitHub; Certificate; https://www.mindluster.com/certificate/268
- 2023/08/09; LearnMS; Introduction to Git; Badge; https://learn.microsoft.com/en-us/training/modules/intro-to-git/

### API
- 2023/08/15; LearnMS; Create a web API with ASP.NET Core Controllers; Badge; https://learn.microsoft.com/en-us/training/modules/build-web-api-aspnet-core/
- 2023/08/17; Mindluster; Swagger ASP NET Core; Certificate; https://www.mindluster.com/certificate/5807

### Cloud
- 2023/08/19; LearnMS; Describe cloud computing; Badge; https://learn.microsoft.com/en-us/training/modules/describe-cloud-compute/
- 2023/08/19; LearnMS; Describe the benefits of using cloud services; Badge; https://learn.microsoft.com/en-us/training/modules/describe-benefits-use-cloud-services/
- 2023/08/19; LearnMS; Describe cloud service types; Badge; https://learn.microsoft.com/en-us/training/modules/describe-cloud-service-types/

### Design Patterns & Standards
- 2023/09/06; Mindluster; Design Patterns in C; https://www.mindluster.com/certificate/5908
- 2023/09/09; Mindluster; Design Patterns and Best Practices; https://www.mindluster.com/certificate/6957
- 2023/09/19; Mindluster; Design Design Patterns in Java; https://www.mindluster.com/certificate/4051

### Robotic Process Automation
- 2023/10/02; Mindluster; UiPath for Beginners; https://www.mindluster.com/lesson/99261
- 2023/10/03; Meet the UiPath Platform; https://academy.uipath.com/courses/meet-the-uipath-platform
- 2023/10/04; Build Your First Process; https://academy.uipath.com/courses/build-your-first-process-v202110
- 2023/10/04; A Day in the Life of an RPA Developer; https://academy.uipath.com/courses/a-day-in-the-life-of-an-rpa-developer-
- 2023/10/09; Variables and Arguments in Studio; https://academy.uipath.com/courses/variables-and-arguments-in-studiov202110

## References
Khillar, S. (2021) “Difference between GitHub repository and Project | Difference between,” Difference Between [Preprint]. Available at: http://www.differencebetween.net/technology/difference-between-github-repository-and-project/#:~:text=GitHub%20Repository%20vs.%20Project:%20Comparison%20Chart. (Accessed: 08 August 2023).
