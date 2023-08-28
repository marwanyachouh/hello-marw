### Detailed Practice for Code Changes:

1. **Sync with Main Branch**
   - Ensure you have the latest version of the `main` branch.
     ```bash
     git checkout main
     git pull
     ```

2. **Create a New Branch for Your Feature/Change**
   - Use descriptive names for your branch, indicating the purpose (feature, bugfix, etc.).
     ```bash
     git checkout -b feature/descriptive-name
     ```

3. **Make Your Code Changes**
   - Edit, add, or remove files as needed for your task.

4. **Stage & Commit Your Changes**
   - Add the changes you've made to the staging area.
     ```bash
     git add .
     ```
   - Commit these changes with a meaningful message.
     ```bash
     git commit -m "Descriptive commit message about your changes"
     ```

5. **Stay Updated with Main**
   - Before pushing, pull the latest changes from the `main` branch to ensure compatibility and reduce merge conflicts.
     ```bash
     git pull origin main
     ```

6. **Push Your Branch to GitHub**
   - This will push your branch and changes to the remote repository.
     ```bash
     git push -u origin feature/descriptive-name
     ```

7. **Create a Pull Request (PR)**
   - Use the GitHub interface to open a pull request. This is a formal way to propose your changes and get them reviewed.

8. **Address Feedback**
   - If your team reviews PRs, there might be feedback or requested changes.
   - Make any required changes in your branch and then stage, commit, and push those changes.
     ```bash
     git add .
     git commit -m "Addressed review feedback"
     git push origin feature/descriptive-name
     ```

9. **Merge Your Changes**
   - Once approved, use the GitHub interface to merge your PR into the `main` branch.

10. **Clean Up: Delete the Feature Branch Locally**
   - After merging, it's a good practice to delete your feature branch locally to avoid clutter.
     ```bash
     git checkout main
     git branch -d feature/descriptive-name
     ```
     If you receive an error about the branch not being fully merged (and you're certain that all changes have been merged or are no longer needed), you can use:
     ```bash
     git branch -D feature/descriptive-name
     ```

11. **Clean Up: Delete the Feature Branch Remotely**
   - This will delete the branch from the GitHub repository.
     ```bash
     git push origin --delete feature/descriptive-name
     ```

This detailed workflow ensures you're always working with the latest code, reduces potential merge conflicts, and keeps your Git history and branches organized.
