### **Steps to Upload a Project to GitHub Using Git Bash**

1. **Initialize a Local Git Repository**:
    
    - Navigate to your project folder:
        
    
        `cd /path/to/your/project`
        
    - Initialize a Git repository in this folder:
        
        
        `git init`
        
        - This creates a hidden `.git` folder in your project directory and tells Git to start tracking the project.
        -


1. **Add Files to the Staging Area**:
    
    - Check the status of your files:
        
    
        `git status`
        
    - Add specific files to the staging area:
        
    
        `git add <file>`
        
        Or add all files:

        `git add .`
        
        - The staging area is like a "preview" of what will be committed.
        -
1. **Commit the Changes**:
    
    - Save the changes in the repository with a descriptive message:
        
        
        `git commit -m "Initial commit"`
        
        - The commit message should describe what changes you’ve made. "Initial commit" is typically used for the first commit.
        -
1. **Create a Repository on GitHub**:
    
    - Go to your GitHub account and create a new repository:
        - Click on the **New** button.
        - Provide a name for your repository (e.g., `my-project`).
        - Don’t initialize it with a README file since you’re uploading an existing project.
        - 
1. **Link the Local Repository to the Remote Repository**:
    
    - Copy the repository URL from GitHub (it will look something like `git@github.com:username/my-project.git`).
    - Add the remote origin (link your local repo to the GitHub repo):
        

        `git remote add origin <repository-URL>`
        
        Example:
        
        `git remote add origin git@github.com:username/my-project.git`
        
6. **Push the Changes to GitHub**:
    
    - Push your local commits to the remote repository:
        
        `git push -u origin main`
        
        - The `-u` flag sets the remote `origin` and branch `main` as the default for future pushes.
        -
        -By default, Git creates a branch named `master` when you run `git init`, but modern GitHub repositories use `main`

---

### **Full Example**:

Here’s how it looks in a full session:


`cd /path/to/your/project          # Navigate to your project folder git init                          # Initialize Git in the folder git add .                         # Stage all files git commit -m "Initial commit"    # Commit with a message git remote add origin git@github.com:username/my-project.git  # Link to GitHub git push -u origin main           # Push to GitHub`

---

### **Key Commands Summary**:

- `git init`: Initializes a Git repository in your project folder.
- `git add <file>` or `git add .`: Stages files for commit.
- `git commit -m "<message>"`: Saves changes with a description.
- `git remote add origin <repository-URL>`: Links the local repo to GitHub.
- `git push -u origin main`: Pushes your changes to GitHub's `main` branch.