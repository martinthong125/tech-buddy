# Meeting 1

1. Need to have proper setup of systems and softwares to ensure productivity and high speed.
2. Installed WSL2 with Ubuntu, Homebrew, using Homebrew, installed Python + boto3 (pip3), Terraform, Docker (including desktop), GitHub desktop.
3. For Python - focus on list, dict and func. # Quite comfortable with them.
4. Installed the different extensions for VS.
5. Tried Bing Chat (5 queries per chat, an alternate to ChatGPT) and bookmarked it on Browser.
6. Superpower - installed 'Oh My Zsh' from https://ohmyz.sh
7. Configured Powerlevel10k, which is a powerful prompt customization tool for ZSH, also added plugins=(git zsh-autosuggestions zsh-syntax-highlighting) for terminal: auto suggestion and highlighting. Also explored available themes.
8. How to use alias # https://github.com/martinthong125/notes/blob/main/Linux/alias.md
e.g., t1='terraform init'.
9. Using argparse in Python - hello2.py # https://github.com/martinthong125/notes/blob/main/Python/hello2.py 
10. Created a new gmail account for all tech uses and a new GitHub account.
11. Ensure to remove the random numbers at the end of personal LinkedIn link unless the numbers have relevant meaning to job search.
12. Open VS Code from terminal using 'code .' # https://www.freecodecamp.org/news/how-to-open-visual-studio-code-from-your-terminal

---

# Meeting 2

1. Docker can be used to improve collaboration among developers, build applications, servers and even VMs. 
2. Git is used for local version control, while GitHub is remote collaboration platform.
3. To push to GitHub successfully, commit needs to take place first.
4. Using 'git log': 1) After committing and before pushing: latest commit shows (HEAD -> update-doc); 2) After both committing and pushing: latest commit shows (HEAD -> update-doc, origin/update-doc), the addition of 'origin/update-doc' is because push has occured to the origin (remote) repository.
5. git add . is the same as git add./ , it adds all files under the current directory. When cd-ed into a sub-folder and using 'git add .', only the files in that sub-folder will be added, or can use 'git add sub-folder/' to achieve the same result without cd-ing.
6. git push, if having any error, can add '-f' as your local repository branch is always the single source of truth.
7. 'git pull origin main' - ensure to checkout to the local repository's branch having the same name as the origin branch specified, otherwise may get 'divergent branches and need to specify how to reconcile them' message. Note that the pulling on CLI is different than pulling on GitHub (where it has a confirm option before merging) as merging happens directly, can consider using 'git fetch' and 'git merge' to allow for reviewing of changes before merging.
8. 'git commit --amend --no-edit' - to amend only the last commit done.
9. Also explored additionally how to amend older or multiple commit messages, though this is discouraged: 
https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/changing-a-commit-message
10. in MS VS, no need git init as there is green color - master (branch name).
11. 'git restore -staged .' - to unstage all files. 
12. 'git branch -a' # list all branches in local and origin (remote) repository. Can use 'git ls-remote --heads origin' to list only the remote branches.
13. 'git remote -v' to list all sites for 'fetch' and 'push' in the remote repositories.
14. Researched on the below to understand more:
[ Difference between Git Clone and Fork ]
Git Clone: This command is used to create a copy of a Git repository on your local machine. When you clone a repository, you get an exact copy of the entire project, including its history, branches, and files. It establishes a connection between your local copy and the original repository, allowing you to pull in updates and changes made to the original repository.

Fork: Forking is a feature used on hosting platforms like GitHub, GitLab, and Bitbucket. It creates a personal copy of someone else's repository under your account. Essentially, it's a clone of the repository, but it's not on your local machine—it exists on the hosting platform. Forking allows you to freely **experiment** with changes without affecting the original repository. You can make changes in your forked repository, commit them, and even create a pull request to propose those changes back to the original repository.

In essence, a git clone brings a copy of a repository to your local machine, while forking creates a copy on the hosting platform, allowing for collaborative development and contribution without directly affecting the original project.

