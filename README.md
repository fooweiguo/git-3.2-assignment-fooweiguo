# What is GitHub Authentication?
When accessing GitHub accounts, most fundamentally usernames and passwords are
required. However when a person links his Github account with organisations for
example, it is important to secure repositories to protect organisations'
information as well as to prevent any malicious modifications to the
repositories that can compromise privacy and security. Therefore GitHub
Authentication has 2FA (2 Factor Authentication) method that links an account
with the device. Thus when a user logs in with his username and password, he
will be prompted to also key in a 6-digit passcode from his authenticator. This
will allow GitHub verify that the login is done from a correct device. 

A user is also required to authenticate when he performs remote modifications of
the GitHub repositories such as git clone, git add, git push etc. For this to
happen, the user is required to generate a SSH key-pair and upload his public
key onto his user security settings. 

# 15 Github Commands. 

## 01. git clone
To replicate and download the repository to local machine. 

## 02. git checkout -b branch_name
To create a repository branch and enter into the branch.

## 03. git add .
To add working directory on local machine to staging area. 

## 04. git commit -m "[Message]"
To transfer the directory on local machine from staging area to localrepo, with
message of the commit.

## 05. git push --set-upstream origin branch_name
To transfer the directory from localrepo to the branch named "branch_name" of
the remote repository.

## 06. git pull
To update directory on the local machine with latest changes to the remote
repository.

## 07. git log
To show a list of commits.

## 08. git branch
To show a list of branches and the branch that the user is currently in.

## 09. git merge destination_branch
To integrate changes from another branch, while still in this branch, into the
destination_branch.

##  10. git remote set-url origin git@github.com:OWNER/REPOSITORY.git
To change from remote's URL from HTPPS to SSH.

## 11. git rebase -i HEAD~N
To edit the commit message in the git log file. Takes all of the commits from
the branch you're going to rebase and replays them onto the end of the branch
you're rebasing onto.

## 12. git fetch
Fetch down all the branches from that Git remote.

## 13. git reset
clear staging area, rewrite working tree from specified commit.

## 14. git diff branchB...branchA
Show the difference of what is in branchA that is not in branchB.

## 15. git rm [file]
Delete the file from project and stage the removal for commit.


# What are the 4 GitHub commands that you think you will use the most in the
# real project.

 I think that I will use the following commands the most in the real projects:
	
	1. git checkout -b branch_name
	2. git add .
	3. git commit -m "message_block"
	4. git push --set-upstream origin branch_name 

Explanation: In the DevOps role, there will be many branches created from the
main branch. This is to allow different developers to work on various parts of
the same project, some of them with overlapping parts. without affecting the
main branch. Otherwise if all the developers work on the same main branch at the
same time, there will be a lot of conflicting versions of the software in the
repository, making debugging and roll-back of the codes almost impossible to
carry out if anything goes wrong. Thus the git checkout command allows
developers to create a sub-branch away from the main branch so that they can
implement new features and perform debugging. Once these are done, they will
perform git add to save the changes to the staging area of the sub-branch. Then
they can do a git commit to add a message to inform the approver of the changes
made. Finally the git push command will push the directory from the staging area
to the sub-branch in the remote repository. The approver will then be notified
of the pull requests from the sub-branch, and he/ she will decide whether to
allow or reject merging changes from the sub-branch to the main branch. This
controlled way of making changes to the main branch will be very useful,
especially when doing capstone projects, since we will be working with a team of
several members, each working on different things. 
