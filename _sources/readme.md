# Data Science Cookbook

This repository is a collaborative project created for the purpose of learning about Git and Github, with special focus on collaborative workflows. Each participant will contribute to our collaborative **Data Science Cookbook** by providing a single recipe of some food that they like. The goal is to learn how to use Git and Github effectively, while also creating a useful resource for everyone involved.

## Contribution Guidelines

### Initialization

- Each of you will be added as a **collaborator** to the repository in the beginning of our class. Please please provide me with your github username or the email address that you used for your Github account.
- **Clone the central repo** to your local machine.

### Making Contributions

- **Create a New Branch**: Create a branch for your specific contribution. Name it after the git term you are explaining, e.g., `git branch add`.
- **Switch to New Branch**: Switch to your branch, e.g. `git switch add`.
- **Copy the Template**: You'll find a `template.md` in the directory. Copy this file and rename it according to the recipe that you are adding. For example, if you are adding a recipe for "Pasta", name it `pasta.md`.
- **Edit the File**: Follow the format specified in `template.md` to fill out your ingredients and instructions. You can also note additional information, such as cooking time, or personal hints and tricks.
- **Commit Your Changes**: Commit your changes with speaking commit messages.
- **Push Your Changes**: Push your branch to the central repository. If you are pushing your branch for the first, you need to use the --set-upstream flag, e.g., `git push --set-upstream origin <your_branchname>`. For follow-up pushes, you can simply use `git push`. 
- **Submit a Pull Request**: Go to the respective branch of the central repository, and make a pull request to the main branch for integration and review.

### Review Process and Merging
- Each pull request should be reviewed by at least one person before it can be merged into the main branch. 
- You may ask one of your classmates (your neighbour, your professor, ...) to review your pull request. You could also assign a reviewer in the pull request interface on Github.
- Reviewers should check for accuracy and clarity.
- Pull requests can be merged once they have been approved.
- In this simple setup, conflicts are unlikely, since everyone is working in a separate file. 
- However, should any merge conflict arise (e.g. if simultaneous edits are made to the README file), then try to resolve the conflict (either locally or on Github).