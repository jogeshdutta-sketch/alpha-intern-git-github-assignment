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

