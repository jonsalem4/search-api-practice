## Actions taken

- Verified tools

  - Checked Git is installed. It is (git version 2.49.0).
  - Winget installation of GitHub CLI failed due to missing sources and needing admin elevation, so I pivoted to a portable install that doesn’t require admin.
  - Downloaded the latest GitHub CLI portable zip, extracted it to a temp folder, and verified it works (gh version 2.82.1).

- Created the local project

  - Made a new folder: c:\Users\jelsa\AttackVentures\Testing-New-Libraries-and-APIs\Testing Search APIs\search-api-practice
  - Added a minimal README and .gitignore to get you started.
  - Initialized a git repo on the main branch, added files, and committed.

- Authenticated to GitHub

  - Launched the browser-based login via GitHub CLI and completed device-code auth. Logged in as jonsalem4.

- Created and wired the GitHub repo
  - Attempted to create the repo via CLI; it indicated the name already existed on your account (likely created during the first attempt).
  - Verified the remote was already set to https://github.com/jonsalem4/search-api-practice.git.
  - Pushed the local main branch to origin and set upstream. Everything is up-to-date.

## Result

- Local project: c:\Users\jelsa\AttackVentures\Testing-New-Libraries-and-APIs\Testing Search APIs\search-api-practice
- GitHub repository: https://github.com/jonsalem4/search-api-practice
- Remote set: origin -> https://github.com/jonsalem4/search-api-practice.git
- Initial commit pushed on main.

## What I did at each step (explained)

1. Check Git and GitHub CLI

- Why: Needed to ensure I can create a repo and push code.
- What: Verified git; winget install of gh required admin. Used a portable gh instead (no admin required).
- Outcome: gh available and working.

2. Create local project folder

- Why: To initialize a working directory for the repo.
- What: Created a folder named search-api-practice under your provided path.
- Outcome: New local folder is ready.

3. Add initial project files

- Why: Having a README and .gitignore is standard and helpful for a first commit.
- What: Created README.md with a short description and a simple .gitignore for Python/Node/VS Code/OS clutter.
- Outcome: Clean starting point for the repository.

4. Initialize local git repo

- Why: To start tracking files and prepare to push to GitHub.
- What: Ran git init -b main; added files; committed “chore: initial commit.”
- Outcome: Local git repository with main branch and first commit.

5. Create GitHub repo and push

- Why: To host the code remotely and collaborate/track history.
- What: Authenticated with GitHub via gh auth login; attempted repo creation (the name existed already), verified remote, and pushed main.
- Outcome: Repo exists on GitHub and local is connected as origin; main is pushed.

6. Verify and share repo URL

- Why: To confirm everything is wired correctly.
- What: Retrieved the origin URL to confirm it points to the right repo.
- Outcome: Confirmed URL: https://github.com/jonsalem4/search-api-practice.git

## Try it

- Open the repo in your browser:

  - https://github.com/jonsalem4/search-api-practice

- Your local path is ready. You can add files and push changes. Typical flow:
  - Add or edit files in the folder.
  - Commit and push:
    ```powershell
    git add .
    git commit -m "feat: add first script"
    git push
    ```

## Notes

- I handled the GitHub CLI install without admin by using a portable build. If you want gh available globally, we can later install the MSI or fix winget sources with admin rights.
- The repository name appeared to already exist under your account when I tried to create it via CLI. Since the remote was already set to that URL, I verified it and pushed successfully.

Completion summary:

- All todos finished: local project created, files added, git repo initialized, GitHub repo connected, and initial commit pushed. If you’d like me to add a basic script scaffold or a minimal README section describing goals for the search API exploration, I can do that next.

Made changes.
