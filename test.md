

# Working with Git

> What is Git

- This is a version control or source control system
- Lets you manage the changes you've made to files
- like a time machine where you can make changes in the history of your project
- you can set checkpoints also called as "Commits"
- There is a term called "Branching" which lets you create multiple versions of something.
- There is a term called "merging" which enables you to syncronise multiple projects into one. 

> What do you need to use git.

- Git. (latest version)
- Installer from the website 
- for windows: terminal called "gitbash" and "hyper"
- Node JS

>Using Git


1. Git is managed by multiple people so you need to tell it who is making the changes to the files by Git Config command

		 git config --global user.name "Your Name"
		 git config --global user.email "your email"

3. Select a folder to you want to be managed by git
	- Open the folder in VScode which has inbuilt terminal, where you choose "git bash" if you don't have others

4. Open the terminal
	- type "git bash" to initialize the repo. it makes a invisible folder ".git" which manages all the folder. 
	- using "ls -la" command shows you all the files and that ".git" folder.

5. Staging files
	- A storing area, where you can store files which you want to commit later on 
	 - Makes you an entry to which you can come back
	 - Done by `git add "file name"` or `git add --A`/` git add --all` to add all files

6. Adding a message after making changes
	- You use `git commit -m "your message"` To insert a message so that you remember it when you come back to this. 
	- You can check the logs by `git log`






# working with GitHub


> what is github

- It is a online service to let developers work together. also called as a social coding website
- Similar to Git. 

It has 
- Cloud repository
- collaborative development
- project management 

>working with Github

- set up a remote, to tie your local repo to remote repo
- Push changes from your local repo to remote repo
- Pull changes from the repo to your local machine 


>process


- Install git. and a git gui
- Install windows terminal
- Install oh-my-posh

- Create git repo
- copy the git repo's link via code->https->copy link.
- open the windows terminal by searching "terminal" and type `git clone {copied link}`
- open the repo in terminal by `cd {repo name}`
- Check branches with `git branch --all`
- Create branch with `git branch {branchname}`
- switch to the new branch with `git checkout {branchname}`
- To open VScode directly from the terminal `code .`


- In the terminal
	- Define who you are with
		- ```git config --global user.email  {your email}
		- `git config --global user.name {your name}
	- Make changes in the  code when you open the editor via `code .`
	- when done, close the terminal and do `git add readme.md/{file name}`
	- next step is to commit that you made changes with a message by `git commit --m {message}`
	- Finally you push the changes from local to remote, by `git push --set-upstream origin {branch name}`
	- and hopefully you've updated it all in github
