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

    ![image](https://github.com/user-attachments/assets/668a7b64-788f-4bdf-b659-ea556a8d061b)

## Working in both R and python
- Once your integrated development environment (IDE - usually Rstudio, Pycharm, VSCode) is set up and you are in the working directory (e.g., in R this will be in the same directory as the Rproject that you created) there is general workflow for integrating your code and GitHub
1. **Clone your remote repository**

    - only need to do this once
    - most IDEs have a place to access the terminal
    - type: ```git clone https://github.com/YourName/SpecificRepo```
    - The URL can be found in the GitHub repository and copied by clicking the button to the right of the URL (boxed in red)
       
        ![image](https://github.com/user-attachments/assets/afa0ae40-6024-4741-a38d-f63dffc90677)

2. **Create your working branch**

    - When working in your local repository after you clone you will have made a copy of the master/main branch. To edit your code, you should create a local branch. This will be named according to the task (e.g., creating_plots will be the branch you develop plots in).  
    - Commands in the terminal to use in this case:  
      - **To look at all available branches**: ```git branch``` (the branch highlighted green or starting with an asterix (*) is the branch you are currently on)
      - **To create a new branch**: ```git branch your_branch_name```
      - **To switch branches**:  ```git checkout your_branch_name``` 

3. **Pushing work from local branch to remote repository**
    - Once you have finished the current task you are working and are done with the branch you must add, commit and push to the remote repository.
    - Type in the terminal:  
      - ```git add “filename.R”``` to add speficic files to the commit
      - ```git commit -m “this is your informative commit message”``` to commit with an informative commit message
      - ```git push origin your_branch_name``` to push from a specific branch to remote repo

4. **Merging changes you pushed to GitHub**
    - Go to GitHub and view pull requests 
    - Confirm and merge pull request
    - Note: Where messages are suggested but not required are good places to describe the specific changes you made to the code. This is a good way of documenting just in case you would like to go back and review what has done.
        
8. **Updating your local master/main branch**
    - After updating you remote main you should update your local main  
      - Change your local branch to the local master/main branch (see instructions above)  
      - Once in branch, pull from remote repo with ```git pull```
    - To continue working in the branch you previously created, switch local branch to the one you want to work in and type: ```git merge Master/Main``` 

## Commenting your code properly 
An important best practice to follow is clear and concise commenting of your code. Functions in both R and Python should have specific headers.  
In R:  
  - Install the ```Roxygen``` package  
  - When inside the function:
    - Windows: ctrl + alt + shift + R
    - Mac: command + option + shift + R  

In Python:  
  - Inside your function type 3 quotation marks (e.g., ''')  
  - This will create a Docstring that looks like this:  
    <img width="611" alt="image" src="https://github.com/user-attachments/assets/51c5dd0b-7f0a-4add-b658-1f441be42be0">

  - Inside of your functions or even if you have no functions you should document your code. General sections should have a short comment what the task being accomplished is and each loop or conditional statement should have a comment. 

    ![image](https://github.com/user-attachments/assets/0877e3c4-e578-486d-b71c-3760ab388b2b)
