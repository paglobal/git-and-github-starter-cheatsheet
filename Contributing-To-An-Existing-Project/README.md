# Git and Github Starter Cheatsheet

#### To contribute to an existiing repo on github:
<!-- -->
<br/>

1. Fork the repo. This can be done by clicking the fork button while in the original repo on github and choosing where to fork it (eg.your github account).
<!-- -->
<br/>

2. After the repo has been forked to the specified location (eg.your github account), click on the green button that says **Code**.
<!-- -->
<br/>

3. Copy the link the dropdown menu that appears.
<!-- -->
<br/>

4. Navigate to the directory you want to clone to repo to on your local machine.
<!-- -->
<br/>

5. Right-click on an empty space in the folder and click **Git Bash Here** from the context menu that appears. A terminal window running **git-bash** should open shortly after.
<!-- -->
<br/>

7. Type in `git clone link` after the prompt, replace **link** with the link to your forked version of the github repo (the one you copied in step 3) and press enter.
> This should clone your forked version of the github repo into your current directory.
<!-- -->
<br/>

8. After cloning the repo, navigate to the local repo directory on you machine. To do this, type in `cd repo-name`, replace **repo-name** with the name of the repo you cloned in step 7, and press enter.
<!-- -->
<br/>

9. Now go to github and navigate to the original repo (the one you forked).
<!-- -->
<br/>

10. Click on the green button that says **Code** and copy the link from the dropdown menu that appears.
<!-- -->
<br/>

11. Afterwards, move to the terminal window, type in `git remote add upstream link`, replace **link** with the link to the original repo (the one you copied in step 10) and press enter.
> This this connects the repo on your machine to the original repo (the one you forked) with a **remote** by adding the link to the original repo as the **remote URL** under an alias called **upstream** to the repo on your machine.
<!-- -->
<br/>

12. At this stage, the original repo has been forked to the specified location (eg. your github account) and a local version of the repo has been created on your machine and linked to the original repo (the one you forked) with a remote called **upstream** and your forked version of the repo on github with a remote called **origin**. Follow the subsequent steps to contribute to the original repo.
<!-- -->
<br/>

13. Assuming this hasn't already been done, open your local repo directory, right-click on an empty space in the folder and click **Git Bash Here** from the context menu that appears. A terminal window running **git-bash** should open shortly after.
<!-- -->
<br/>

14. Type in `git checkout master` to checkout your local master branch.
<!-- -->
<br/>

15. Type in `git pull upstream master` and press enter to pull any new changes (if any) from the master branch of the original repo (the one you forked) to your local repo (the one on your machine).
<!-- -->
<br/>

16. Type in `git push origin master` and press enter to push the new changes (if any) to the master branch of your forked version of the repo on github.
<!-- -->
<br/>

17. Type in `git branch branch-name`, replace **branch-name** with your branch name of choice and press enter to create a new branch form your local master branch. You can skip this step if you already have a branch you are working on.
<!-- -->
<br/>

18. Type in `git checkout branch-name`, replace **branch-name** with the name of the branch you are working on and press enter to checkout the branch.
<!-- -->
<br/>

19. Work on the branch by making changes to the repo.
<!-- -->
<br/>

20. When you are done making the changes, use `git add .` and `git commit -m "Any message you want"` to stage and commit the changes respectively.
<!-- -->
<br/>

21. Afterwards, type in `git push origin branch-name`, replace **branch-name** with the name of the branch you worked on and press enter.
> This should push the changes that were committed to your local repo to your forked version of the repo on github.
<!-- -->
<br/>

22. Submit a pull request on github.
<!-- -->
<br/>

23. If the pull request you made in step 22 gets accepted, delete the branch you made the changes on (from step 17). To do this, type in `git branch -d branch-name`, replace **branch-name** with the name of the branch and press enter to delete the branch. Delete the corresponding branch on your forked version of the repo on github too.
<!-- -->
<br/>

24. If the pull request you made in step 22 gets rejected for because it needs more work, repeat the process starting from step 18.
<!-- -->
<br/>

25. Anytime you, want to make a change to the original repo, follow the steps outlined in the guide starting from step 14.
<!-- -->
<br/>

#### Hope this helps
