# Create and Clone a Repository
A **repository** is like a folder that stores code for a project. First, create a server repository in GitHub, then clone it locally!

>_Note: Before creating a repository, make sure you have a GitHub account and have properly verified your email address_

## Creating a repository

1. Go to [github.com/new](https://github.com/new)
1. Enter a name for the repository
1. Optionally, enter a description for the repository
1. Select the privacy settings for the repository
1. Click the **Create Repository** to create the repository!

## Cloning the repository
Once you have your own repository, you can clone it on your local machine to play around with it.  A **clone** is a copy of a repository that lives on your computer instead of on a website's server somewhere.

>_Note: Before cloning the repository, make sure to install Git (for [Mac](https://git-scm.com/download/mac) or [Windows](https://gitforwindows.org/))_

1. Navigate to your GitHub repository on the web
1. On the right side of your repository page, click the **Clone or download** button
    - Make sure you are on the **Clone with HTTPS** menu
1. Click the _copy_ icon to copy your repository URL to your clipboard  
    ![](https://i.imgur.com/D1iXTDp.png)

Depending on which tool you are using, follow the instructions in one of the sections below to complete the cloning process.

### Option 1: Cloning in Visual Studio Code
If you have installed Git on your machine, Visual Studio Code has built-in Git tools you can use.

1. Open Visual Studio Code
1. Press `Ctrl`+`Shift`+`P` to open the Command Palette
1. Type in ">Git: Clone" and press `Enter` to execute the command  
    ![](https://i.imgur.com/WEoYQer.png)
1. Paste in your repository URL and press `Enter` to confirm  
    ![](https://i.imgur.com/UZHIFN0.png)
1. Navigate to a suitable location for your repository folder, and click the **Select Repository Location** button  
    ![](https://i.imgur.com/ELgHyHy.png)
1. Once your repository is cloned, a popup should appear in the lower right corner of the window. Click the **Open Repository** button to open a new instance of VS Code with the newly cloned repository
    ![](https://i.imgur.com/rKdgz2p.png)

### Option 2: Cloning via the Command Line
If you have Git Bash installed on your machine (or another shell), you can use that for all Git commands.

1. Open your shell application (e.g. Git Bash)
1. Change your directory to wherever you'd like the repository to live
    ```bash
    cd /path/to/folder/
    ```
1. Use the `clone` command to clone the repository (paste in the repository's url after `clone`)
    ```bash
    git clone https://github.com/YOUR_REPO_URL.git
    ```

## Next Steps
That's it! Now you have a local clone of your repository. Next, [push some changes](PushChanges.md) to the repository!