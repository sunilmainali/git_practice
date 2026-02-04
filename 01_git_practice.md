# Git Practice

## Setup
```bash
echo "# git_practice" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/sunilmainali/git_practice.git
git push -u origin main
```

## Workflow
working files -> (git add) -> staging area -> git commit/push -> repository

## Quick commands
```bash
git remote -v
git status
```

## Commit message conventions
- feat: new features added
- fix: bug fixing
- refactor: refactored code that neither fix a bug nor add a feature
- docs: update the documentation
- perf: performance improvements
- style: Formatting only (indentation, remove extra lines)
- chore: project maintenance (update packages, remove unused packages)

## .gitignore
The .gitignore file tells Git which files and folders should not be tracked or uploaded to the repository. It is important because it keeps the project clean by ignoring unnecessary, auto-generated, large, or sensitive files like cache, datasets, and passwords. This helps maintain security, reduces repository size, and makes collaboration easier.

## Git branching (local)
1. `git branch <branch>`
2. `git checkout <branch>`
3. Make changes
4. `git add <filename>`
5. `git commit -m "commit message"`

To merge locally:
- `git checkout main`
- `git merge <branch>`
- `git branch -d <branch>`

## Git branching (remote)
- `git push origin <branch>`
- Create a pull request to merge into `main`
- After remote merge: `git pull origin main`

## Resolving merge conflicts
When conflicts occur during merge, open the conflicted files, resolve the differences, `git add` the resolved files, and `git commit` to finish the merge. Use `git status` to help locate conflicts.
