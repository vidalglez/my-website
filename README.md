# my-website

this is a really awesome website

These are some useful commands for git:

To review your remote repos that your local project is pointing: $git remote -v

To update remote repo name to yout local: $git remote set-url [remote_branch] [github_project.git]

Example:
$git remote set-url origin https://github.com/vidalglez/website.git

To review information for our remote repo and see if project name matches: $git remote show [branch_name]

Example:
$git remote show origin

To push changes to remote repository: git push -u [remote repo] [branch]

To perform merge in yourlocal: my-website (master) $ git merge [branch_to_merge]

Example: my-website (master) $ git merge remove-ipsum

To list all your branches: $ git branch -a

To delete a branch: $ git branch -d [nameofbranch]

To look for death branches and remove references: $ git fetch -p
