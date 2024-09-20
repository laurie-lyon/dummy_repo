# From GitHub to your Local Computer
Notes from Lozupone Lab GitHub SOP

## Vocab used here
- **Remote Repository**: the repository of code that you see in GitHub
- **Local Repository**: the repository of code (file) that you see on your local computer
- **Working Directory**: the file on the computer where the scripts that you are working on are located
- **Master/Main Branch**: the official branch containing the most recent collection of all code. When cloning a GitHub Repo it is the branch that is cloned - will be named EITHER *main* or *master*
- **Working Branch**: the branch that a task is being completed in - used to not interfere with the official main code


## Coding in R
- When coding in R, create an **Rproject** for every project that you do
- Creating an Rproject makes a separate environment for every set of scripts in development
- To do this go to the top right corner of Rstudio and click *New Project, make a new directory and name the project (example below)

- ![image](https://github.com/user-attachments/assets/668a7b64-788f-4bdf-b659-ea556a8d061b)

## Working in both R and python
- Once your integrated development environment (IDE - usually Rstudio, Pycharm, VSCode) is set up and you are in the working directory (e.g., in R this will be in the same directory as the Rproject that you created) there is general workflow for integrating your code and GitHub
1. **Clone your remote repository**
     - only need to do this once
     - mose IDEs have a place to access the terminal
     - type: ```git clone https://github.com/YourName/SpecificRepo```
     - The URL can be found in the GitHub repository and copied by clicking the button to the right of the URL (boxed in red)
        ![image](https://github.com/user-attachments/assets/afa0ae40-6024-4741-a38d-f63dffc90677)

2. **Create your working branch**
3. **Pushing work from local branch to remote repository**
4. **Merging changes you pushed to GitHub**
5. **Updating your local master/main branch**
  
## Commenting code properly 
