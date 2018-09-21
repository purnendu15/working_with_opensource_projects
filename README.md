# working_with_opensource_projects
#### PUSHING TO OPEN SOURCE REPOSITORY ####

1. Identify the repository
For e.g airship-in-a-bottle

1-1) For this to your local github repository.
- go to your github repo and search for "airship-in-a-bottle"
and fork it.

2. Create a github ssh key and upload
https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/

3) Clone with SSH.
git clone git@github.com:purnendu15/airship-in-a-bottle.git

4) Make you changes.

5) Sync your fork

5-1)https://help.github.com/articles/configuring-a-remote-for-a-fork/
In the above step the command for upstream addition is:

https://help.github.com/articles/syncing-a-fork/
$ git remote -v
$ git remote add upstream https://github.com/openstack/airship-in-a-bottle.git
$ git remote -v 
You can see the difference
Note: It is the parent repository	

https://help.github.com/articles/syncing-a-fork/

6) git commit -am "Commit Message"
Note: the "a" will stage all changes.
If you want specific files just -m "Commit Message" <filename>

7) git push origin master

7-1) this will push to my local repository

7-2)Do a pull request there.

7-3) Next steps only if the pull request is accepted.

8) git fetch upstream
9) git checkout master
10) git merge upstream/master <this updates the changes from step 7-3>
11) git push origin master<this will update your local repository>

Ref: https://www.atlassian.com/git/articles/git-forks-and-upstreams
Ref: https://dont-be-afraid-to-commit.readthedocs.io/en/latest/git/remotes.html

