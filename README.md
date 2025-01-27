# How-To-Use-Git-And-Github
A guide on how to utilize Git &amp; Github for all your software needs!

# Contents
  - [What is Git?](#what-is-Git?)
  
  - [What is Github?](#what-is-Github?)
  
  - [How to Upload Your Projects onto Github (Full Guide)](#how-to-push-your-Projects-onto-Github)
  
     - [All the Git commands](#All-the-Git-commands-to-push-your-project-onto-Github)
  
  - [How to Update existing Repositories with Git (Full Guide)](#How-to-Update-existing-Repositories-with-Git)

     - [All the Git commands](#All-the-Git-commands-to-update-your-Github-repository)

  - [Downloading code from Github Repositories](#Downloading-code-from-Github-Repositories)

  - [How to View Github Repositories in VS Code](#View-Github-Repositories-in-VS-Code)

  - [Bash Commands you Should Know](#Bash-Commands-you-Should-Know)


## What is Git?
- Git is the most widely used version control system that is used today. It is utilized for tracking changes in computer files and coordinating work on those files among multiple people. It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files.

- With git, you can easily see what other people on your team are working on, view your previous changes to the code, and you can rollback to your previous code. 

- Git is also what programmers use to push code onto Github through their command prompt or terminal. Instead of uploading files onto Github manually, programmers use git to simply push their code or any other files online through a couple commands. 

- Read more about Git [here](https://www.freecodecamp.org/news/what-is-git-and-how-to-use-it-c341b049ae61/)

  - ### Download Git [here](https://git-scm.com/downloads)

## What is Github?
- Github is world's hub for open-source software. It is where you can view other people's projects, publish your own projects, and get inspiration for future projects. If you are working for a company and your responsibilities involve programming, you will most likely be using Github to collaborate with other team members on a codebase.

- The main feature of Github is repositories, and within them, you can view all the source code and files for a given project. 

- You can also **fork** repositories from one user’s account to another. This enables you to take a project that you don’t have write access to and modify it under your own account. If you make changes you’d like to share, you can send a notification called a **pull request** to the original owner. That user can then, with a click of a button, merge the changes found in your repo with the original repo.

## How to Upload your Projects onto Github

- By uploading your projects onto Github, you can easily keep track of all the changes to your files and source code and have the ability to go back to a previous version of your project. It can serve as a backup for files since it is all hosted online and it is a great way to showcase your talents to other developers and contribute to an open-source community. 

- To get started, first make sure all the files from your project are in a separate folder in a specified location E.g. Desktop

- Then, create a new repository on your github account. Name the project whatever you like and give it a good description

- Make sure you **don't** add a README file, as this will change up the following steps. Then, create the repository

- You will now see a quick setup screen, which is indicating that you have successfully created a repository

- To push the files from your project onto this repository, navigate to the project's location on your device through
 the command prompt (Windows) or terminal (Mac). Getting familiar with the command line interface is imperative for working 
 with git and software in general. To get familiar with CLI commands, read more [here](https://programminghistorian.org/en/lessons/intro-to-bash)
 
 - If your project folder is on your desktop, navigate to your desktop directory by running `cd desktop` on your command prompt or terminal. Then, run `cd` followed by the name of your project folder.

- Next, run `git init`, this initializes an unversioned folder to be ready for use with git 

- After that, run `git status`, this shows you the state of the files in your folder

- Now, run `git add -A`, this tells git that you want to include these files in your next commit (update)

- Run `git commit -m "First commit"`, this is setting up all your files to be pushed onto Github. Note: In the future, you would want to add a description for each commit to indicate what you have changed for the project. Each commit should be detailed in explaining what changed from before. 

- Then, run `git remote add origin URL`, where URL represents the specific URL for your project. This URL can be copied from the page of your repository, see highlighted in the screenshot below. So for me, I would run `git remote add origin https://github.com/faizancodes/Test.git` 

![image](https://user-images.githubusercontent.com/43652410/111018415-aa3e5480-8386-11eb-89c8-a5762919f458.png)

- Lastly, run `git push -u origin master` to push your files onto github. If you have done this successfully, you should see your files uploaded on your github repository!

 ### This is how your command prompt or terminal should look if you have executed all the commands correctly: 
![image](https://user-images.githubusercontent.com/43652410/111018455-d659d580-8386-11eb-91d4-4e77705f1e5c.png)

  ## All the Git commands to push your project onto Github
  
  **NOTE: Commands surrounded with brackets [] are specific to you**

  ```
  cd [Project Location]
  git init
  git status
  git add -A
  git commit -m "First commit"
  git remote add origin [URL]
  git push -u origin master
  ```
  
# How to Update existing Repositories with Git

  - Git makes it very simple and quick to update your repositories with just a few commands. This is especially useful if you made several changes to multiple files in your project and want to push them onto Github. Uploading / doing these changes manually without git would be very tedious and time consuming.

  - First, navigate to your project folder's location by running `cd [Folder Location]`. If the folder is on your desktop, you would run `cd desktop` and then `cd [Project Name]`, with project name being the name of your project folder

  - Next, run `git init`, this sets the files up to be ready for use 

  - Then, run `git add -A`, this stages all the files for the next commit

  - After that, run `git status`, this shows you all the changes to the files you made

  - Run `git commit -m "Commit"`, this prepares all the files to be pushed. This is where you would specify what changes you made to the files within the quotes, you would replace "commit" with a description of what you modified. 

  - Lastly, run `git push -u origin master`, which pushes all your files to github. 

  ### If you executed all the commands successfully, your command prompt or terminal should look like this:

  ![image](https://user-images.githubusercontent.com/43652410/111020813-6eab8680-8396-11eb-9843-7fb71d085540.png)
  
  - You will then see the files in your github repository have been updated based on your modifications

  ## All the Git commands to update your Github repository
  
  **NOTE: Commands surrounded with brackets [] are specific to you**

  ```
  cd [Project Location]
  git init
  git add -A
  git status
  git commit -m "Commit"
  git push -u origin master
  ```
  
# Downloading code from Github Repositories

  - There are two ways to download all the files from a github repository. 
  
  - For the first and preferred way, make sure you have git downloaded from [here](https://git-scm.com/downloads) 
  
    - Then, go the repository you want to download the files from and click on the green button that says 'Code' 

    - You want to copy the URL in the menu that pops up (as shown below), for this repository, the URL is https://github.com/SJUSATA/How-To-Use-Git-And-Github.git. The URL will simply be the URL for the repo except with `.git` at the end

    <img src="https://user-images.githubusercontent.com/43652410/111021589-83d6e400-839b-11eb-8877-867393b024dc.png">

    - Then, you want to open your command prompt or terminal and run `git clone [URL]`, with URL being the URL you just copied. For example, for this repo you would run `git clone https://github.com/SJUSATA/How-To-Use-Git-And-Github.git`

    - If done correctly, your command prompt or terminal should look like this:

    ![image](https://user-images.githubusercontent.com/43652410/111021473-87b63680-839a-11eb-865a-f81bcd8b9802.png)

    - Now, all the files have been downloaded onto your computer within a folder named the same as the repository. You can access this folder by navigating to its specified location.

    - Since I cloned the repository while in my desktop directory, the folder is located within my desktop folder. 

    - The name of the repository I cloned is called `sonnet` so to navigate to its folder, I would run `cd sonnet` and now I can execute certain files (check the repository's README file for instructions on how to run the program)

    - You can also simply view the files in your file explorer / finder as well. For me, I would have to simply find the `sonnet` folder within my desktop folder and I can then view all the files inside 

  - The second way to download all the files from a repository, which only recommended if git is not working for you, is to simply click the 'Download ZIP' option after you click on the green 'Code' button which is shown above 

    - This downloads a zip file containing all the files within the repository, which you then have to unzip to access the files. 
  
# View Github Repositories in VS Code

  - With [Github1s](https://github.com/conwnet/github1s), you can load any Github repository in a VS Code environment, where you can then develop your project in the cloud

  - To view any repo within VS code, simply add `1s` after `github` in the URL for the repo, for example, view this repo in VS Code: https://github1s.com/SJUSATA/How-To-Use-Git-And-Github

# Bash Commands you Should Know

 -  `cd [Folder]`  Change directory to specified folder

 - `cd ..`  Navigate to parent folder

 - `pwd` Print working directory

 - `mkdir [Folder Name]` Create a folder with a specified name 

 - `ls`  List of all the files in your current directory
