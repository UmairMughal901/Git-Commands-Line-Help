<!-- <h2></h2>  <p></p> -->
<h2>How to initialize folder for git tacking</h2>
<p>git init</p>

<h2>If you want to revert changes made to your working copy, do this</h2>
<p>git checkout .</p>


<h2>If you want to revert changes made to the index (i.e., that you have added), do this. Warning this will reset all of your unpushed commits to master!:</h2>
<p>git reset</p>


//If you want to revert a change that you have committed, do this:

git revert <commit 1> <commit 2>

//If you want to remove untracked files (e.g., new files, generated files):

git clean -f

//Or untracked directories (e.g., new or automatically generated directories):

git clean -fd

//That's because Git can't merge the changes from the branches into your current master. Let's say you've checked out branch master, and you want to merge in the remote branch other-branch. When you do this:

$ git pull origin other-branch

//Simply track your remote branches explicitly and a simple git pull will do just what you want:

git branch -f remote_branch_name origin/remote_branch_name
git checkout remote_branch_name

git branch -f new_local_branch_name upstream/remote_branch_name

#set a new remote

git remote add my_awesome_new_remote_repo git@git.assembla.com:portfolio/space.space_name.git


#Verify new remote

git remote -v

> my_awesome_new_remote_repo  git@git.assembla.com:portfolio/space.space_name.git (fetch)
> my_awesome_new_remote_repo  git@git.assembla.com:portfolio/space.space_name.git (push)

<h2>Generating a new SSH key</h2>

<p>ssh-keygen -t ed25519 -C "your_email@example.com"</p>
