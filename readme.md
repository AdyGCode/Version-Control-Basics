# Version Control (VC) Demo

## Who am I

Configure git to use your name and email address for commit tracking.

Edit the config file using...
`git config --global --edit`

Or we can do this at the command line:

`git config --global user.name "YOUR NAME"`
`git config --global user.email "YOUR EMAIL ADDRESS"`

git config --global user.name "Ady G"
git config --global user.email "Adrian.Gould@nmtafe.wa.edu.au"

Check the settings using `git config --list`


## Create a new project for VC

- Get to the location for the project
- Make the project folder: `mkdir PROJECT-NAME`
- Change into the folder: `cd PROJECT-NAME`
- Create a `README.MD` file:
  - Linux/cmder `touch ReadMe.md` then `pico ReadMe.md`
  - PC: `notepad ReadMe.md`
- Add brief outline of project to ReadMe.md
- Save and Exit editor

- Initialise VC: `git init`
- Rename to main using `git branch -m main`

## Showing the Status of the Repo

Use the command `git status` to see what has been added, deleted, or changed.

## Add file(s) to "waiting area"

`git add FILENAME`
for example:
`git add ReadMe.md`

To add multiple files, list them after the add (spaces between file names)

To add a complete folder use:
`git add FOLDER_NAME`

To add everything (apart from ignored files) use:
`git add .`

## Committing Files to VC

Commiting files into history/version control:

`git commit -m "COMMIT MESSAGE"`


## Show the change history

Use the command `git show`


## Remote Repository on GitHub
- Go to GitHub, login to your account
- Locate the + and click to create a new repository
- This will then show you the commands to add the remote to your repo and push the data up!

```shell
git remote add origin https://github.com/AdyGCode/Version-Control-Basics.git

git branch -M main

git push -u origin main
```

In the future, you will only need to do a `git add`, `git commit` and then `git push` to upload the changes you have made.

