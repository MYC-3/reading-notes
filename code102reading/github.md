# Reading 3 - Revisions and the Cloud

Git is a Distributed Version Control System (DVCS) that makes it easy for a development team to collaborate on a project by keeping a history of changes to files.
This allows for an easy way to revert a file to a previous version in case of a mistake.

## Cloning repository to your local computer:
1. Copy clone URL from GitHub
2. In the terminal, move to the location you want to store your repository (`Users/Username/projects/codefellows/code102`)
3. Type `git clone ` followed by the clone URL into the terminal
4. Move into the repository with `cd` command in terminal
5. `code .` will open repository in VSCode
6. Make changes and save

## ACP Steps (syncing local changes to GitHubs):
1. `git add nameoffile`
2. `git commit -m "your commit message. keep it appropriate"`
3. `git push origin main`

## Git terminal commands cheat sheet

Command | Explanation
--------|------------
`git clone repositoryURL` | creates a copy of your repository in your current location
`code .` | opens repository in VSCode
`git status` | checks status. Informs you of what has been changed/is ready to commit
`git add nameoffile` | ADD step of ACP. Add the files that have been changed.
`git add .` | Adds all files that have been changed.
`git commit -m "message goes here"` | COMMIT step of ACP. Keep your messages appropriate they are public
`git push origin main` | PUSH step of ACP. Syncs all changes to GitHub.


[Back to HOME](README.md)