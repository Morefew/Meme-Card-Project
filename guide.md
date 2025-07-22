# Git & GitHub Collaborative Meme Card Project Guide

Para leer esta guía en ESPAÑOL haz clic [aquí](guia.md)

## Welcome!

Welcome to the **Git & GitHub Collaborative Meme Card Project**! This project is a fun and practical way to learn the essentials of collaborative code development using Git for version control and GitHub for hosting and teamwork. Your goal is to contribute a unique "Meme Card" to a shared web page. The difficulty is **beginner-friendly**, designed to introduce fundamental concepts without overwhelming complexity. The final product will be a single, static HTML page showcasing a collection of all participants' meme cards, a tangible result of our collective effort!

## Who is This For?

Let's see how well you use GIT and GitHub collaboratively?

Level 1: Beginner
- I can clone repositories (git clone), make changes, and push them with git add, git commit, and git push.
- I can create files and folders, but I don't usually work with branches or resolve conflicts.
- I primarily work in my own repository or on the main branch.

Level 2: Intermediate
- I work with branches (git branch, git checkout, git merge) and make pull requests on GitHub.
- I can update my branch with changes from the remote repository using git pull and resolve simple conflicts.
- I participate in code reviews, assign issues, and use comments to collaborate.

Level 3: Advanced

- I can handle collaborative workflows such as fork & pull requests, interactive rebases (git rebase -i), cherry-picking, and squash merges.
- I resolve complex conflicts and maintain remote and local branches (Git remote, Git fetch, and Git prune).
- I automate processes with GitHub Actions, manage releases, and participate in repository administration.

This project is open to anyone who wants to participate but is ideal for level 1 developers who want to understand how programmers collaborate on code using Git and GitHub.

### Prerequisites:

- **Basic Computer Literacy:** Familiarity with using a computer, navigating file systems, and opening applications.
- **Text Editor:** Access to a code editor like VS Code, Sublime Text, Atom, or Notepad++.
- **Web Browser:** A modern web browser like Chrome, Firefox, Edge, or Safari.
- **Internet Access:** To connect to GitHub and download necessary tools.
### Requirements:
- **Git Installed:** Git command-line tools must be installed on your computer.
- **GitHub Account:** You'll need a free GitHub account.
### Experience Level Expected:
- **No prior Git or GitHub experience is required.** This guide and the project are designed to be your first step into version control collaboration.
- **Basic HTML/CSS knowledge is helpful but not strictly necessary.** We'll provide enough guidance for you to create your card.
## Approximate Time of Completion
Expect to spend approximately **2-4 hours** on this project. This includes setting up your environment, creating your card, understanding the Git workflow, and participating in the pull request process.
## Project Structure and Learning Objectives
The project involves a simple static web page built with HTML and CSS. Each participant will add their own "Meme Card" to this page.

### Learning Objectives:
By completing this project, you will:
- Understand the **purpose of version control** with Git.
- Learn how to **clone a repository** from GitHub.
- Practice **creating and switching Git branches** for isolated development.
- Gain experience with **staging and committing code changes**.
- Learn how to **push your local changes to a remote GitHub repository**.
- Master the process of **creating and managing Pull Requests (PRs)** on GitHub.
- Understand the importance of **code review** and how to respond to feedback.
- Experience **resolving merge conflicts** (if they arise).
- Contribute to a **collaborative coding project** from start to finish.
## The Feature Branching Workflow

### Description
The **Feature Branching Workflow** is a standard practice in professional development. Instead of everyone working directly on the main project code, each new feature or task gets its own dedicated branch. This isolates your work, preventing you from disrupting the main codebase or other ongoing development. Once your feature is complete and reviewed, it's merged back into the main branch. This keeps the main codebase stable and clean.

## GIT Conventional Commits

### Description
**Conventional Commits** provide a lightweight convention on top of commit messages. It's a structured way to write commit messages that makes project history more readable, helps automate changelog generation, and aids in automatic versioning. A typical Conventional Commit message looks like this:

`type(scope): subject`
`[optional body]`
`[optional footer]`

For this project, we'll primarily focus on the `type` and `subject`.
- **`type`**: Describes the kind of change. Common types include:
    - `feat`: A new feature
    - `fix`: A bug fix
    - `docs`: Documentation only changes
    - `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
    - `refactor`: A code change that neither fixes a bug nor adds a feature
    - `test`: Adding missing tests or correcting existing tests
    - `chore`: Other changes that don't modify src or test files (e.g., build process, tooling)
- **`subject`**: A very brief description of the change.

**Example Commit Messages:**
`feat: add meme card styles`
`fix: change style display type of main div of meme card`
`feat: add image to meme card`
## Process
The following steps outline the typical process for contributing your meme card. Remember to consult the provided links for detailed instructions if you encounter difficulties.

- ### Step 1: **Fork and Clone the Repository**
    - **Fork:** On GitHub, find the main project repository and click the "Fork" button to create your own copy.
    - **Clone:** `git clone https://docs.github.com/articles/fork-a-repo`
    
- ### Step 2: **Create a New Feature Branch**
        - `git checkout -b feature/[your-github-alias]-card` (e.g., `git checkout -b feature/jane-doe-card`)
        
- ### Step 3: **Add Your Meme Card**
    - Open `index.html` in your text editor. 
    - Add a new `div` for your card, including your GitHub alias, a `div` for the meme image, and a `div` for the description.
    - For your meme image, you will use a **link (URL) to an externally hosted image**. You can use services like Imgur, Cloudinary, GitHub Gist (for small images), or any other public image hosting platform. Ensure the image is publicly accessible via a direct URL.`
    - Inside your `<div>` for the meme image, use an `<img>` tag with the **src attribute pointing to your external image URL** (e.g., `<img src="https://i.imgur.com/your-meme.jpg" alt="Your Meme Description">`).
    - Add your card-specific CSS styles to `styles.css.
        
- ### Step 4: **Stage and Commit Your Changes**
    - `git add .` (to stage all modified files, including your image)
    - `git commit -m "feat: add [your-github-alias]'s meme card"`
    
- ### Step 5: **Push Your Branch to GitHub**
    - `git push origin feature/[your-github-alias]-card`
    
- ### Step 6: **Open a Pull Request (PR)**
    - Go to your forked repository on GitHub.
    - Click "Compare & pull request."
    - Ensure the base branch is `main` and the compare branch is your feature branch.
    - Provide a clear title (e.g., `feat: Add [Your Name]'s Meme Card`) and a brief description.
        
- ### Step 7: **Address Feedback and Resolve Conflicts**
    - Monitor your PR for comments from reviewers. Make any requested changes locally.
    - `git add .` then `git commit -m "fix: address review comments"`
    - `git push`
    - If there are merge conflicts, `git pull origin main` into your feature branch, resolve conflicts manually in your editor, then `git add .`, `git commit -m "fix: resolve merge conflicts"`, and `git push`.
        
- ### Step 8: **Merge Your Pull Request**
    - Once your PR is approved and all checks pass, it will be merged into the `main` branch.
        
- ### Step 9: **(Optional) Clean Up**
    - `git checkout main`
    - `git pull origin main`
    - `git branch -d feature/[your-github-alias]-card` (deletes local branch)
    - Go to GitHub and delete the remote branch.

## List of Links

- **Installing Git:**
    - [Git Downloads](https://git-scm.com/downloads)

- **Creating a GitHub Account:**
    - [Join GitHub](https://github.com/join)

- **Basic Git Commands:**
    - [Git Handbook - GitHub Guides](https://guides.github.com/introduction/git-handbook/)
    - [Git Cheat Sheet](https://training.github.com/downloads/github-git-cheat-sheet/)

- **Understanding Pull Requests:**
    - [About pull requests - GitHub Docs](https://www.google.com/search?q=https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-with-pull-requests/about-pull-requests)
    
- **Resolving Merge Conflicts:**
    - [Resolving a merge conflict on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)
    - [How to resolve a Git conflict - Atlassian](https://www.atlassian.com/git/tutorials/using-branches/merge-conflicts)
    
- **Conventional Commits:**
    - [Conventional Commits Specification](https://www.conventionalcommits.org/en/v1.0.0/

- **Image Hosting Services:**
	- [Imgur](https://imgur.com/) (simple, widely used for sharing)
	- [Cloudinary](https://cloudinary.com/) (more robust, but might be overkill for a simple meme)
	- [GitHub Gist](https://gist.github.com/) (you can upload images to a public gist and use the raw URL)

## [Glossary of Terms and Ideas](glossary.md)
Click the title above for the glossary.


## Final Thoughts and Encouragement
Learning Git and GitHub is one of the most valuable skills for any aspiring programmer. It opens doors to collaborative projects, open-source contributions, and managing your own code effectively. Don't be discouraged if you encounter challenges; it's part of the learning process! Every conflict resolved and every pull request merged is a step forward. You've got this!
