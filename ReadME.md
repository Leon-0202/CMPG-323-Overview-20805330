## Table of contents

- [Repositories](#repositories)  
- [Project and Repository Context](#project-and-repository-context)  
- [Branching Strategies](#branching-strategies)  
- [gitignore Files](#gitignore-files)
- [Storage of Credentials and Sensitive Information](#storage-of-credentials-and-sensitive-information)
- [References](#references) 

## Repositories
Repositories to be created and used for each project:  
- CMPG-323-Overview-20805330: Used primarily for Project 1 - Agile & Scrum, but also serves as a supporting repository for the other projects.  
- CMPG-323-Project02-20805330: Used for Project 2 - API Development.
- CMPG-323-Project03-20805330: Used for Project 3 - Standards & Patterns.
- CMPG-323-Project04-20805330: Used for Project 4 - Testing & RPA.
- CMPG-323-Project05-20805330: Used for Project 5 - Reporting & Monitoring.

## Project and Repository Context
A repository is essentially a storage location (similar to a folder) that stores related files and documentation. A project is a management tool that helps improve visualization and organization of tasks such as issues and pull requests (Khillar, 2021).
![alt text](http://cdn.differencebetween.net/wp-content/uploads/2021/03/GitHub-Repository-vs-Project.jpg)  
(Table used from http://www.differencebetween.net/technology/difference-between-github-repository-and-project/#:~:text=GitHub%20Repository%20vs.%20Project:%20Comparison%20Chart)

## Branching Strategies
Branching strategies to be used for each project:
- Project 1:  
Since the only file that needs to be edited for Project 1 is the README.md file, and seeing how it won't involve any code, it will be hot-fixed on the main branch.
- Project 2 to 5:  
Innitially, a remote repository will be created for a project.  Then a local repository will be created by cloning the remote repository to a specified directory.

Whenever a new feature is to the be added to the project, or whenever existing code needs to be updated/changed, a new branch will be created and checked out on the local repository. The main branch will then be pulled from the remote repository to the newly created branch (feature branch) on the local repository. It is here where the relevant code will be added/changed. The new code and files will then be added to the staging area, and then be subsequently committed to the local repository (still on the feature branch, not the main branch), along with a descriptive message describing the changes made. The branch will then be pushed to the remote repository.  

From the remote repository, a pull request will be created.  The changes will reviewed, a proper description will be provided, and if automatically possible, merged into the main branch.  If not, the merge conflict will first be resolved before merging the feature branch into the main branch.  After the merge request is completed, the feature branch will subsequently be deleted.  

## gitignore Files

## Storage of Credentials and Sensitive Information

## References
Khillar, S. (2021) “Difference between GitHub repository and Project | Difference between,” Difference Between [Preprint]. Available at: http://www.differencebetween.net/technology/difference-between-github-repository-and-project/#:~:text=GitHub%20Repository%20vs.%20Project:%20Comparison%20Chart. (Accessed: 08 August 2023).
