# Git Flow for Creating a New Branch, Adding, Committing, and Merging to Main

## 1. Start in the Main Branch

Assuming you are currently on the `main` branch, pull the latest changes from the remote repository:

```bash
git pull origin main
```
## 2. Create New Branch
Create a new branch for your feature or bug fix. Replace feature-branch with an appropriate and descriptive branch name:
```bash
git checkout -b feature-branch
```
## 3. Make Changes
Make the necessary changes to your code, add new files, or modify existing ones.

## 4. Stage Changes
Stage the changes you want to include in the commit:
```bash
git add .
```

## 5. Commit Changes
Commit the changes with a descriptive commit message:

```bash
git commit -m "Add a descriptive commit message"
```

## 6. Push Changes to Remote
Push your changes to the remote repository:
```bash
git push origin feature-branch
```

## 7. Open a Pull Request
If you are working in a collaborative environment, open a pull request on the Git repository hosting service (like GitHub or GitLab) to merge your changes into the `main` branch.

## 8. Review and Merge
Review your changes, address any feedback, and once approved, merge the changes into the `main` branch.

## 9. Switch Back to Main
After merging, switch back to the main branch:

```bash
git checkout main
```
## 10. Pull Latest Changes
Pull the latest changes from the remote repository to ensure you have the most up-to-date main branch:

```bash
git pull origin main
```