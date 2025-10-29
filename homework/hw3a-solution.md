# HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.
### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`
## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL:   
  https://github.com/maramshqair-AU/py4eda-work.git  

- Output of `git remote -v`:   
  origin  https://github.com/maramshqair-AU/py4eda-work.git (fetch)  
  origin  https://github.com/maramshqair-AU/py4eda-work.git (push)  

- The output of `git log --oneline`:   
  892d5b0 (HEAD -> main, origin/main) Add hw3a solution document  
  61fca7e Initial commit: Add README and .gitignore  
## Questions
### Reflections:
**Question 1**  
a) Before using Git, I used to save multiple versions of my files (e.g., simulation files) with numbers to mark the latest version. It was tough. After a while I couldn’t remember the differences between versions, especially when the simulation model was complicated. Although I can’t apply Git directly to simulation binaries, the Git workflow is very organized and convenient. I’ll look for ways to keep key model inputs, scripts, and notes in Git so I can modify things without the fear of breaking the main work. Git lets me see exactly what changed and when, roll back if something goes wrong, and attach clear commit messages so the history tells the story of my decisions. Finally, connecting to GitHub also gives me a safe backup and makes it easy to collaborate or review changes later  
b) As I mentioned in part a, I often lost track of changes while modifying simulation models. A clear Git commit history would have solved this. I’d keep the model inputs, parameter files, and helper scripts in Git, then commit regularly with short messages. With this history, I could 1) see exactly which change produced a result, 2) compare runs by diffing parameters and scripts, and 3) roll back when a change breaks the model.  
  
**Question 2**  
a) It’s important to keep class_repo and my_repo separate so my changes don’t conflict with the instructor’s updates. Keeping the class repo as a clean, read-only reference lets me pull new materials anytime without mixing them with my edits.  
b) I will keep each in a separate repository. For a group project, the repo should be shared with the team so everyone can pull updates, work on it, and push changes, keeping all of us on the same track. My individual assignments will stay in my own repo. The class reference materials will live in a separate read-only repo so I can pull updates without mixing them with my work.  
  
**Question 3**  
a) Of course, the second message is more useful because it’s more informative and specific. Looking back at the log later, this kind of message makes it easy to find the right commit and remember exactly what changed at each step.  
b) For a project that lasts weeks, I’d commit each time I finish one clear step that works by itself (Example commit: “clean missing values”). I think the unit of work should be one idea per commit, with a short message that says what changed and why.  
  
### Graduate Questions  
**Question 1**  
a) Committing README.md and .gitignore first, then hw3a-solution.md later keeps the history clean. The first commit says “set up the repo and ignore junk,” the second says “add my homework.” If I dumped everything in one commit, I’d lose that separation, it will be harder to review and track.  
b) I’d commit the data-loading code when it actually works without errors. I’d wait on the half-done analysis function until it works before committing it. I’d make a tiny commit for the comment typo right away. I’d commit the README if it already matches what the project does right now. The staging step helps because I can choose only the finished files (to include and leave the unfinished so each commit stays clean and clear.  
c) git status tells me mainly what changed, what’s staged, and what’s untracked. I try to use it all the time, especially before and after staging and committing to double-check that I’m committing exactly what I intend.  
  
**Question 2**  
a) Distributed means every clone is complete. My laptop’s copy of the repo has all files and the full history, so I can commit and view changes offline. Later I sync with GitHub. Google Drive or Dropbox have central cloud folder that syncs files. It doesn’t track real commits. If my colleague and I edit a file, we get conflicted copies. With Git, each one of us has a full history, can work offline, and Git can merge changes cleanly.  
b) Because I can keep working and committing even with no internet. My laptop has the full history, so it’s fast, I can roll back if something breaks, and my work stays private until I’m ready to share. When I’m online, I push once to back up and sync. This enables simple workflows like making small commits, pushing to back up and sync, and rolling back if something breaks.  
c) git clone makes a local copy of a remote repo on GitHub. git pull gets new commits from that remote. git push sends my local commits up to the remote. I can pull from class_repo but not push because it’s the instructor’s read-only repo and I don’t have write permission. In my_repo, I am the owner, so I have write access and can both pull and push.  
  
**Question 3**  
a) I’ll commit small, finished steps like a new script, a cleaned notebook, and an updated README. This way I show my process without sharing messy unfinished steps in the final view.  
b) A portfolio README should be a quick tour and say what the project is in one sentence, show how to run it in 2–3 steps, point to the first thing to open, and maybe include one picture or result so people see something right away. An open-source README is different. It’s longer and more technical, with install details, examples and options.  
c) My portfolio should simply show the projects and publications I’m proud of, the stuff I want employers to see, each with a one-line summary, an easy way to view/run, and links to PDFs/posters. The habits to keep it strong include making regular commits with clear messages, keep a clean layout, and  add a short README for each project.  
 



