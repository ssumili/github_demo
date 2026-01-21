# Simple Command-Line To-Do List (A GitHub Demo Project)

![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

This is a simple, command-line to-do list application written in Python. I've created it to serve as a hands-on project for learning the fundamental concepts and workflows of Git and GitHub.

The application itself is simple so that we can focus on the version control process and other features of GitHub rather than complex code.

## Features

*   **View To-Do List:** Displays all the current items in your to-do list.
*   **Add Item:** Adds a new task to your list.
*   **Mark Item as Completed:** Removes a task from the list once it's done.
*   **User-Friendly Menu:** A simple, numbered menu for easy navigation.

## Prerequisites

Before you begin, ensure you have the following installed on your system:
*   [Python](https://www.python.org/downloads/) (version 3.6 or higher)
*   [Git](https://git-scm.com/downloads/)

## How to Run the Application

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd <repository-name>
    ```
3.  **Run the Python script:**
    ```bash
    python todo.py
    ```
    You will then see the main menu and can start interacting with the application.

## Learning Git & GitHub with This Project

This repository is a perfect sandbox for practicing core version control skills. Follow these steps to simulate a real development workflow.

### 1. Initial Setup: Creating the Repository

First, you need to get the project on your local machine and connect it to GitHub.

*   **Initialize Git:** If you are starting from scratch, navigate into your project folder and run `git init`.
*   **Make your first commit:** Add all the project files and make your first "save".
    ```bash
    git add .
    git commit -m "Initial commit: Add basic to-do list application"
    ```
*   **Connect to GitHub:** Create a new repository on GitHub.com and follow the instructions to "push an existing repository from the command line".
    ```bash
    git remote add origin <your-github-repo-url>
    git push -u origin main
    ```

### 2. The Basic Workflow: Making a Change

Every time you make a change, you should commit it. Let's try changing the welcome message in `todo.py`.

*   **See the status:** Check which files have been modified.
    ```bash
    git status
    ```
*   **Stage your changes:** Prepare the modified files for a commit.
    ```bash
    git add todo.py
    ```
*   **Commit your changes:** Save the changes with a descriptive message.
    ```bash
    git commit -m "Docs: Update welcome message for clarity"
    ```
*   **Push to GitHub:** Upload your commit to the remote repository.
    ```bash
    git push
    ```
    Now, check your repository on GitHub to see the new commit!

### 3. Branching: Working on a New Feature

You should never work directly on the `main` branch. Let's create a new branch to add a "Remove Item" feature.

*   **Create and switch to a new branch:**
    ```bash
    git checkout -b feature-remove-item
    ```
*   **Modify the code:** Open `todo.py` and add the logic for removing an item from the list. Don't forget to add a new option to the menu.
*   **Commit your new feature:**
    ```bash
    git add todo.py
    git commit -m "Feat: Add ability to remove items from list"
    ```
*   **Push the new branch to GitHub:**
    ```bash
    git push origin feature-remove-item
    ```

### 4. Collaboration: Creating a Pull Request (PR)

A Pull Request is how you propose your changes and ask for them to be merged into the main codebase.

1.  Go to your repository on GitHub.
2.  You will see a prompt to create a **Pull Request** for the `feature-remove-item` branch. Click it.
3.  Give your PR a title and description, explaining what you've done.
4.  Click "Create Pull Request".

This is the point where a team would review your code, leave comments, and discuss the changes before merging.

### 5. Merging and Cleaning Up

Once the Pull Request is approved, you can merge it.

1.  On the GitHub Pull Request page, click the **"Merge pull request"** button.
2.  Now that the feature is part of the `main` branch, you can switch back to your local `main` branch and pull the changes down.
    ```bash
    git checkout main
    git pull origin main
    ```
3.  You can also delete the feature branch, as it's no longer needed.
    ```bash
    git branch -d feature-remove-item
    ```

## Contributing

Contributions are welcome! This is a learning project, so feel free to fork the repository, try adding a new feature on a branch, and open a pull request.

Some ideas for new features:
*   Save the to-do list to a `.txt` or `.csv` file.
*   Add priority levels (e.g., High, Medium, Low) to tasks.
*   Allow editing of existing to-do items.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.