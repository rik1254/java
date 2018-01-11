# java

Follow these steps to get git properly running

#Delete old repo
rm -rf repo_name

#Check current user name and email linked
git config --global --list

#If different, do
git config --global user.email your_email_address
git config --global user.name you_user_name

#Clone new repo
git clone https://github.com/rik1254/java.git

#Checkout the master branch
git checkout master
(This should just say already on master)
(There should already be a directory in there)

#Test by making a branch
git checkout -b name_of_your_branch

#Push your new branch
git push -u origin name_of_your_branch

#Go get git website if the new branch has stuck

#Change branch back to master
git checkout master

#Check all branches
git branch
(This should show master and your branch)

#Delete your branch
#You have to delete the remote (github) version and your local version

#Local version
git branch -f name_of_your_branch
#Remote version
git push origin --delete name_of_your_branch
