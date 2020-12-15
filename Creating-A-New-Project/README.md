# Git and Github Starter Cheatsheet

#### To create a new local repo and connect it to github:
<!-- -->
<br/>

1. Create the repo on github.
<!-- -->
<br/>

2. Navigate to the directory on your machine where you want to create the repo at.
<!-- -->
<br/>

3. Create a folder in the directory you navigated to in step 2 with the same name as the repo you created on github in step 1.
<!-- -->
<br/>

4. Navigate to the folder you created in step 3.
<!-- -->
<br/>

5. Create or add the files and folders that you want to add to the repo in the folder you're currently in.
<!-- -->
<br/>

6. Right-click on an empty space in the folder and click **Git Bash Here** from the context menu that appears. A terminal window running **git-bash** should open shortly after.
<!-- -->
<br/>

7. Type in `git init` after the prompt and press enter.
> This initializes a local git repo in your current directory.
<!-- -->
<br/>

8. Type in `git add .` after the prompt and press enter.
> This adds all the newly added or created files and folders from step 3 to the staging area. This is where new files and folders that were changed or added to the repo are placed in order to be later committed as changes to the repo.
<!-- -->
<br/>

9. Type in `git status` after the prompt and press enter.
> This is used to check the files that have been added to the staging area.
<!-- -->
<br/>

10. Type in `git commit -m "Any message you want"` after the prompt, replace **Any message you want** with a message that you want to associate with the commit and press enter.
> This makes commits to the repo with commit messages. This means that the files in the staging area are now added as changes to the repo and a checkpoint is created. This checkpoint is like a point in history that you can return to if you make any subsequent changes to the repo that you want to revert.
<!-- -->
<br/>

11. Type in `git remote add origin link` after the prompt, replace **link** with the link to the github repo and press enter.
> This this connects the repo on your machine to the one on github with a **remote** by adding the link to the github repo as the **remote URL** under an alias called **origin** to the repo on your machine.
<!-- -->
<br/>

12. Now type in `git push -u origin master` after the prompt and press enter.
> This should push the changes that were committed to your local repo to the one on github.
<!-- -->
<br/>

13. At this stage, if everything went according to plan, the repo on your machine should be connected to the one on github. Now, anytime you make changes to the repo on your machine that you want to commit to the github repo, use the `git add .`, `git commit -m "Any message you want"` and the `git push -u origin` commands in their respective order as described in steps 8, 10 and 12 respectively.
<!-- -->
<br/>

#### Hope this helps
