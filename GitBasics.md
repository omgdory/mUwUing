As for how I did this, I personally like to make PRs as follows: THIS IS ALL FOR COMMAND LINE BTW IDK HOW DESKTOP APP WORKS
    1) Make an issue detailing what I'm going to work on
    2) Assign myself that issue and, from GitHub's website itself, create a branch for that issue
    3) On my local text editor/IDE (I use VSCode personally) I will:
        3a) git fetch origin (updates the branches available)
            You can run 'git branch' to see what branches currently exist
        3b) git checkout [name of new branch you just made on GitHub]
    4) Just work and as you work, add the files changed and removed to staging by using git add
        You can then just make a git commit to "save" your changes to the added files on your branch LOCALLY
    5) To get your local changes on that branch to the remote one on GitHub, you'd have to 'git push'
        That just pushes your changes from the local machine to the remote version of the branch
        After you do that, you can actually do 'git pull' to get those changes onto another machine. Really useful.
        Think about it like working on a Google Doc and you 'save' by doing a git commit -> git push
        And when you log into another computer to work on that same doc, you do git pull to get the most recent version.
    
    6) Rinse and repeat steps 4-5 until you are done working on your issue/feature, then you can finally open what's called a pull request.
        You do this by finishing one last set of steps 4 and 5, and then navigating to GitHub on a web browser.
        You will be met with an option to open a pull request to merge your most recent changes to your branch into main.
        You will then write up some details for your PR, it will get reviewed/approved by somebody else, and hopefully merged in.
    That is all for creating a PR

As for reviewing PRs:
    On GitHub, at least Web version, you can see a Pull Requests tab on the top of the repository
    There will be the listed PRs to review and merge in. You can just click on one, and then click on the "Code" tab.
    Review the code, test it by checking out the branch being merged in and running stuff locally.
    If everything looks good, then feel free to go back to the main tab for that PR and approve it at the bottom to merge in.
    
    IF WHEN YOU'RE REVIEWING THE CODE, HOWEVER, SOMETHING IS OFF OR YOU'D LIKE TO REQUEST CHANGES TO THE CODE, YOU CAN CLICK ON A LINE OF CODE
    AND LEAVE A COMMENT THUS STARTING A PR REVIEW.

    This is a lot harder to explain via text tbh so it'll make more sense when you review my PR and have access to the actual tools. 
    Lmk if you have any questions :like:

As for when I'm working on a branch from an issue, before every major work session I like to:
    1) Checkout the main branch to pull any changes since my last session.
        1a) git checkout [name of main branch, in this case 'main']
        1b) git pull (while on main branch), can also do git fetch and git merge
        1c) git checkout [name of branch you were working on]
        1d) git merge --no-ff main [this merges the changes on main into your branch]
This keeps everything updated as you work on your branch and people update main.