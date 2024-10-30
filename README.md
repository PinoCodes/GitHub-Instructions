# GitHub-Instructions
## Connecting to the repository and uploading the project

This guide will help you open the terminal, connect to a GitHub repository, and download the project locally on your computer. When I first started working with Git, it was difficult for me to find information that was useful to me personally. Therefore, I decided to make my own detailed checklist on how to upload projects. 

### 1. Open the Terminal

- **On macOS**: Press `Command + Space`, type **Terminal**.
- **On Windows**: Press `Win + R`, type **cmd** or **PowerShell**.(you can also download Git Bush, it may be easier to use)

### 2. Clone the Repository

In the terminal, use the following command to clone the repository and create a local copy:


`git clone git@github.com:your_account/repository_name.git`

**Example**: git clone git@github.com:PinoCodes/ML-Labs.git

### 3. Navigate to the Project Folder

Once cloned, navigate to the project directory:
`cd repository_name`

### 4. Create a New Branch

If you’d like to work in a separate branch, create and switch to it:
`git checkout -b branch_name`

### 5. Add and Commit Changes
After making changes, add the files and create a commit:
 
 `git add .`
 
 `git commit -m "Description of changes"`

### 6. Push Changes to GitHub

To push changes to your GitHub repository, run:
`git push origin branch_name`
If you’re working on main, replace branch_name with main.

## Connecting to GitHub via SSH

To securely connect to GitHub, you can use SSH keys. Follow these steps to set it up:

### 1. **Check for existing SSH keys**:  
   Open your terminal and enter the following command:

   `ls -al ~/.ssh`
This will display a list of files in the .ssh directory. Look for files named id_rsa and id_rsa.pub. If these files exist, you already have SSH keys generated.

### 2.	Generate a new SSH key (if you don’t have one):
If you don’t have SSH keys, you can generate a new one with the following command. Make sure to replace <your_email@example.com> with your GitHub email address:
