# Rules for Successful Assignment Submissions

## _Rule 1_

### **Deploy Early**

Before you even open VS Code it is important to make sure you set yourself up for a smooth assignment submission process by having a deployed version of your GitHub repository. When you are ready to start an assignment follow the following steps:

1. Create your repository on GitHub by using the template for the assignment
2. Log in to Netlify and select `Add new site` then `Import an existing project`
3. Select `GitHub` as your Git provider and then select the repository you'd like to deploy
4. Make sure the `Branch to deploy` is `main`
5. Click `Deploy site` and on the next page copy the randomly generated site name (_ex: crunchy-chinchilla-e02af8_)
6. Go back to GitHub and add a link to your Netlify deployment to the `About` section (_The format for the address is:_ **https://** _random-site-name_ **.netlify.app**
   )

## _Rule 2_

### **Don't work on the main branch**

The main branch is sacred. When developing your application the `main` branch will always represent the "released" or "finished" version of your code. As you are developing your app you should work on a `dev` (development) branch so that any changes you make won't be released to the world until you have explicitly told it to do so (by merging to your main branch). A good workflow is as follows:

1. Clone your repo and `cd` into the directory of the repo
2. Open your project using `code .`
3. Check out a new branch `git checkout -b dev`
4. Get to work building your app!

## _Rule 3_

### **ACP Frequently**

During the development of your app it will flip-flop between stages of working and being completely broken. It is important to capture all the times it is "working" (even if not finished) in a commit. Committing often is an important habit to develop because it captures a snapshot of your progress over time as your app adds features and functionality. It is also a way to "revert" your code back to a point where you knew it was working just in case you break everything. The steps to making a commit are:

1. (A) Add or "stage" all the files you changed `git add -A`
2. (C) Commit the changes `git commit -m 'brief message'`
3. (P) Push the commit to GitHub `git push origin dev`

## _Rule 4_

### **Avoid turning in a Pull Request with failing CI**

Continuous Integration (aka CI) is the practice of merging all developers' code into a shared mainline (your `main` branch in these assignments). CI is often guarded by a set of automated tests that check to make sure your code meets the minimum quality requirements that were determined by the product managers. If it doesn't pass the tests, it shouldn't be merged into `main`.

1. ACP to create your Pull Request on GitHub
2. View the Pull Request on GitHub
3. Next to each commit you will see either a small `x` (failing) or a green `✓` (passing)
4. If failing, click the `x` and then click `Details` to view information on what made the CI fail
5. Fix the issues in your code and then ACP again

Note: In order for your assignments to be graded the PR you submit in Canvas must have passing CI, but you can still submit as long as have a comment in your Canvas submission indicating that you are aware it is failing and an explanation as to why you believe it is failing.

=====================================

## _Submission checklist_

Ask yourself:

1. Is my `main` branch deployed to Netlify?
2. Did I put a link to my deployed site in the About section of my GitHub repo?
3. Was my work completed on a `dev` branch?
4. Did I `ACP` often as I progressed through the assignment?
5. Is my PR passing CI? (Leave a note in your submission if not passing)
6. Did I copy the link to my PR for my submission?
7. If this was a re-submission, did I tell my TA?
