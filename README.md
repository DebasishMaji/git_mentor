# Git mentor

First lets understand what's version control system and why it is necessary. And obviously how Git comes into picture.

Version Control System:

    Whenever people and teams collaborate on projects together some questions become very evident
    
    1. Which changes were made?
    2. Who made the changes?
    3. When were the changes made?
    4. Why were changes needed?
    
    Version Control System tracks the history of changes here and can answer the above questions.
    

Distributed Version Control System:

    DVCSs allow full access to every file, branch, and iteration of a project, and allows every user access to a full and self-contained history of all changes.
    
    Don’t need a constant connection to a central repository. Developers can work anywhere and collaborate asynchronously from any time zone.
    
    Git is a distributed version control system (DVCS) commonly used for open source and commercial software development.

A World without Version Control System:

    # team members are subject to redundant tasks
    # slower timelines
    # multiple copies of a single project
   

Why Git?

    Git lets developers see the entire timeline of their changes, decisions, and progression of any project in one place
    
    Using branches, developers can safely propose changes to production code.
    
    Git makes it possible to align experts across a business to collaborate on major projects
    

Terminology:
    
    Repository:
    A Git project that contains a collection of files and folders along with each file's revision hostory.

    Commits:
    snapshot of file hostory appeanrs in a particular time.
    
    Branches:
    Lightweight movable pointer to one of the commits(You can visualize commits as a linked-list relationship and relate branch to it).
    
GitHub Flow:

    1. Create a branch
    2. Add commits
    3. Open a pull request
    4. Discuss and review code
    5. Merge
    6. Deploy
 
Git Commands:
    
    git init: Intialize a new Git repo
    
    git clone: Creates a local copy of a project that already exists remotely
    
    git add: stages a change
    
    git commit: saves the snapshot to the project history and completes the change-tracking process
    (Anything that’s been staged with git add will become a part of the snapshot with git commit)
    
    git status: shows the status of changes as untracked, modified, or staged
    
    git branch: shows the branches being worked on locally
    
    git merge: combines changes made on two distinct branches (merges lines of development together)
    
    git pull: updates the local line of development with updates from its remote counterpart
    
    git push: updates the remote repository with any commits made locally to a branch.
    
    
Helpful Operations:

   Install Git:
        Git can be installed from
        http://git-scm.com/ for all platforms.
        
   Configure tolling:
        Configure user information for all local repositories

        git config --global user.name "[name]" (Sets the name you want attached to your commit transactions)
    
        git config --global user.email "[email address]" (Sets the email you want attached to your commit transactions)

    Create repositories:
        Start a new repository or obtain one from an existing URL

        git init [project-name] (Creates a new local repository with the specified name)
        
        git clone [url] (Downloads a project and its entire version history)
       
   Make changes:
        Review edits and craft a commit transaction
    
        git status (Lists all new or modified files to be committed)

        git diff (Shows file differences not yet staged)
        
        git add [file] (Snapshots the file in preparation for versioning)
        
        git diff --staged (Shows file differences between staging and the last file version)
        
        git reset [file] (Unstages the file, but preserves its contents)
        
        git commit -m"[message description]" (Records file snapshots permanently in version history)
        
        
   Group Changes:
        Name a series of commits and combine completed efforts

        git branch (Lists all local branches in the current repository)
        
        git branch [branch-name] (Creates a new branch)
        
        git checkout [branch-name] (Switches to the specified branch and updates working directory)
        
        git merge [branch-name] (Combines the specified branch’s history into the current branch)
        
        git branch -d [branch-name] (Deletes the specified branch)
        
   Review history:
        Browse and inspect the evolution of project files
    
        git log: Lists version history for the current branch

        git log --follow [file] (Lists version history for the file, including renames)
        
        git diff [first-branch] ... [second-branch] (Shows content differences between two branches)
        
        git show [commit] (Outputs metadata and content changes of the specified commit)


   Save fragments:
        Shelve and restore incomplete changes

        git stash (Temporarily stores all modified tracked files)
        
        git stash pop (Restores the most recently stashed files)
        
        git stash list (Lists all stashed changesets)
        
        git stash drop (Discards the most recently stashed changeset)
        
   Redo commits:
        Erase mistakes and craft replacement history

        git reset [commit] (Undoes all commits after [commit], preserving changes locally)
        
        git reset --hard [commit] (Discards all history and changes back to the specified commit)
        
   
   Synchronized changes:
        Register a remote (URL) and exchange repository history

        git fetch [remote] (Downloads all history from the remote repository)
        
        git merge [remote]/[branch] (Combines the remote branch into the current local branch)
        
        git push [remote] [branch] (Uploads all local branch commits to GitHub)
        
        git pull (Downloads bookmark history and incorporates changes)
        
        
   Note: "Learn Git Branching" is the most visual and interactive way to learn Git on the web. Must explore 
   https://learngitbranching.js.org/.
   
   Note: Explore how Git commands affect the structure of a repository within your web browser. Must explore 
   http://git-school.github.io/visualizing-git/.
   
   Note: More advanced concepts will be added soon.