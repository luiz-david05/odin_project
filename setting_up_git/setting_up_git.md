#### Setting up git

1. Install git on your machine. You can download it from [here](https://git-scm.com/downloads).

2. Open your terminal and type `git --version` to check if git is installed.

3. Set up your git username and email by typing the following commands in your terminal:

```bash
git config --global user.name "Your Name"
git config --global user.email "
```

4. Check if your username and email are set up correctly by typing `git config --global --list`.

5. Create a new repository on GitHub. You can follow the instructions [here](https://docs.github.com/en/github/getting-started-with-github/create-a-repo).

6. Clone the repository to your local machine by typing `git clone <repository-url>` in your terminal.

7. Change directory to the cloned repository by typing `cd <repository-name>`.

8. Create a new file in the repository by typing `touch <file-name>`.

9. Add the file to the staging area by typing `git add <file-name>`.

10. Commit the changes by typing `git commit -m "Add new file"`.

11. Push the changes to the remote repository by typing `git push origin master`.

12. Check the status of the repository by typing `git status`.

13. Check the commit history by typing `git log`.

14. Create a new branch by typing `git checkout -b <branch-name>`.

15. Switch back to the master branch by typing `git checkout master`.

16. Merge the branch into the master branch by typing `git merge <branch-name>`.

17. Delete the branch by typing `git branch -d <branch-name>`.

18. Update your local repository by typing `git pull origin master`.

19. Resolve any merge conflicts by editing the conflicting files.

20. Add the resolved files to the staging area by typing `git add <file-name>`.

21. Commit the changes by typing `git commit -m "Resolve merge conflicts"`.

22. Push the changes to the remote repository by typing `git push origin master`.

23. Congratulations! You have successfully set up git and GitHub on your machine.