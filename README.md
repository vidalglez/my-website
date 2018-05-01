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

To review if there is a remote branch that doesn't exist in local: $ git fetch

To delete remote branch once you removed from your local($ git branch -d 'update-readme' ): $ git push [remote_branch] :[removed_branch]

Example: 
my-website (master) $ git branch -d 'update-readme'
Deleted branch update-readme (was 972336c).
my-website (master) $ git push origin :update-readme
To https://github.com/vidalglez/website.git
 - [deleted]         update-readme

To revivew Github graphs: $ git log --oneline --graph

When a conflict is detected pulling changes from remote you can use: 
$ git mergetool

The only detail will be that you need to install and configure a mereg tool like p4merge or beyondcompare

To list all the tags generated in your local: $ git tag

To create a new tag: $ git tag [name of tag] [target branch]

To show details for a specific tag: $ git show [name of tag]

To create a new annotateg tag: $ git tag -a [tag name] -m "Details for the tag" [commit id]
Example $ git tag -a v0.1-alpha -m "Release 0.1 (Alpha)" 5976df4

To push a tag to remote repo: $ git push [local remote branch] [tag name]
Example: $ git push origin stable

If there are multiple tags in local repo, to push all of them to remote repo: $ git push --tags

