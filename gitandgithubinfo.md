# Command Line

In this part we are going to learn some commands that will help us to have a better performance.

## Create and delete directories

`mkdir [Directory Name]`
__mkdir__ is an abreviation for "make directory", we only have to give a name for this and it will be created.

`rmdir [Directory Name]`
This other command is used to remove the directory specified, __rmdir__ is also an abreviation and it means "remove directory" 


## Navigate

`cd`
If we use __cd__ followed by the route that we want to go, it will take us there. 


## Compare

`cmp`
This command is used to compare two files and it can tell if the two files are completely identical or not.


## Find files

`find [Route] [Name or extension]`
This one can be used if we are looking for a specific file, we just have to specify the location of the file in the __Route__ and then type the name of the file in the __Name or extension__ part.

For example:
__find /OneDrive/example-username/ -filename_example__


## Create and edit files

`nano`
This is the command that we will use when we want to create a file, it is quite easy and simple to use because we only have to type __nano__ followed by the name we want to give to the file.


## Get the state of the computer

`lscpu`
This is the command used in Linux to check the state of the computer.


# Git Commands

In this section, we will learn the basic commands that we can use on git.

## Configuration

As we know, we have to set the workspace in order to have a complete configuration, for this, we can use some commands to set default values:

`$ git config --global user.name "Your name"` 
This will set the name that will be attached to the commits done afterwards. For example $ git config --global user.name "Your name" 

`$ git config --global user.email "Your email"`
This is similar to the previous one, but in this case we are going to use our email instead of the name, it is shown in commits and tags.


## Starting a project

After doing the initial configuration, we have to start the project by using this tools:

`$ git init [project name]`
This command will create a local repository inside a directory that we already have.

`$ git clone [project url]`
This other command will clone or download a project from a remote repository.


## Basic workflow commands to stage and commit

Once we have started the project, we have to know the correct commands that will help us to work correctly.

`$ git status`
This is one of the commands that we could use the most because it will show the status of the directory in use, showing us created, modified or deleted files.

`$ git add [file]`
This command will be applied when you want to stage your files which are ready to be committed.

`$ git diff [file]`
This one can show changes between the directory in use and the staging area.

`$ git diff --staged [file]`
This other shows changes between the local repository and the staging area.

`$ git reset [file]`
This command will reverse our repository to a previous saved state.

`$ git stash`
This command is useful when you don't want to take the current changes to the staging area, and instead, you will add them to a stash.

`$ git stash pop`
This one will apply again the changes previously saved into the stash to the directory in use.

`$ git commit`
With this, we will create a new commit of the changes located in the staging area, we can add a message by using `-m "Your message"` below the command.

`$ git rm [file]`
If you want to remove or undo something from the directory in use or add something to the staging area, you can use this command to make this happen.


## Branches

When we work with a team, we will probably need to do some changes, but it is important to not affect the script from the others, and for this we have the next commands:

`$ git branch [-a]`
This will show a list of the local branches.

`$ git checkout [-b][branch_name]`
It takes us from the directory in use to the specified branch. If the branch does not exist yet, __[-b]__ will create it

`$ git merge [from name]`
With this, we will join or merge 2 branches, the one specified in __[from name]__ to the current branch

`$ git branch -d [name]`
After joining 2 branches, the branch that has been merged to the other can be removed with this command


## Reviews

If we want to see who has done changes or committed in a project, we can use this command:

`$ git log [-n count]`
This will list all the commits specified using __n__ as the limit that we want
