# Assignment Documentation

## Day 1 – Easy Level

### Git Version
git version 2.39.5 (Apple Git-154)

### Git Config Commands Used
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"

## Day 1 – Medium Level

### Git vs GitHub
- **Git** is a local version control tool installed on your computer. It tracks file changes offline.
- **GitHub** is an online platform that stores your Git repositories in the cloud and enables collaboration.

### .gitignore entries
Ignored: node_modules/, .env, .vscode/

### git log --oneline output
c300a09 Add logs and uploads folders with .gitkeep placeholders
b47d866 Add .gitignore and ASSIGNMENT.md with Git vs GitHub explanation
283870f Initial commit: Add README.md with Git and GitHub introduction

## Day 1 – Advanced Level

### Branch Rename Command
git branch -m feature/day-1-practice day-1-practice-done

### Merge Conflict Explanation
I created two branches that both modified `day-1/conflict-test.md` differently.
When I ran `git merge conflict-branch` on main, Git couldn't auto-merge them and
marked the conflict with `<<<<<<<`, `=======`, and `>>>>>>>` markers.
I resolved it by clicking "Accept Both Changes" in VS Code, then staged and committed the resolution.
## Day 2 – Easy Level

### git diff
The diff shows lines added (marked with +) and removed (marked with -)
since the last commit. It compares the working directory against the last committed state.

### git stash
Used `git stash` to temporarily save unstaged changes.
`git stash list` showed: stash@{0}: WIP on main: 8ffe929 Complete Day 1 advanced tasks documentation
Used `git stash apply` to restore the changes back.
### Tags
Created tag: v1.0
`git tag` output: v1.0

## Day 2 – Medium Level

### Rebase
Created feature/day-2-practice branch, added day-2/notes.md, then rebased onto main.
Rebase replays commits on top of another branch keeping history clean and linear.

### git reflog – Why it's useful
`git reflog` records every movement of HEAD, including resets, merges, and checkouts.
It's useful for recovering lost commits — even after a `git reset --hard` you can
find the commit hash in reflog and restore it.