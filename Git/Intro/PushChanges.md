# Push Changes
When you want to store a change on your remote repository, you will have to **push** those changes up. When you push your changes, they will appear on the server. This is possible using VS Code or the command line.

## Option 1: Adding, Committing, and Pushing in Visual Studio Code
If you have Git installed, Visual Studio Code has some built-in tools that make it easy to interact with your repository. First, make sure you have opened the proper root-level folder for your local repository clone.

To view the various source control options, click the Source Control icon on the left menu:  
![](https://i.imgur.com/jm8aCAA.png)

Then, if you make a change to one of the files in your local repository, it will appear in the source control pane.

### Stage (add) the changes for commit
If you have a change and you are ready to commit it, you first have to **add** or **stage** the change for commit. In the source control pane, click the _plus_ icon next to the file to add it to the commit:  
![](https://i.imgur.com/dtSdJny.png)

### Updating the Git User
Update the git configuration so that it contains the proper user e-mail.

1. Open a new terminal in VS Code by selecting `Terminal` -> `New Terminal` from the top menu  
    ![](https://i.imgur.com/Ah0ogIi.png)
1. In the terminal pane, find the dropdown on the right side to select the shell type and choose **Select Default Shell**  
    ![](https://i.imgur.com/YDPvuRn.png)
1. If using Windows, select **Git Bash** from the list  
    ![](https://i.imgur.com/ZRRh4Ja.png)
1. If using Mac or Linux, select the preferred shell
1. In the terminal pane, click the `+` to create a new terminal  
    ![](https://i.imgur.com/Nkudw3L.png)
1. Enter the following command, swapping `email@example.com` for your GitHub e-mail address
    ```bash
    git config --global user.email "email@example.com"
    ```

Now, it should be possible to commit to the local repository without issue.

### Commit the change
After you have added the change, it will be _staged_ for commit. From there, you simply have to commit it!

1. Type a **commit message** in the box describing your change
1. Click the _checkmark_ icon to complete the commit  
    ![](https://i.imgur.com/WRwINED.png)

Once your change is committed, your local repository will include the change. The next step is to sync the change with the remote repository, so it's actually in GitHub.

### Push the change
Visual Studio Code has an interesting tool for pushing changes up to the remote repository. Instead of simply pushing changes, it actually _synchronizes_ the local and remote repositories. This means that it pushes any commit changes up, and also pulls down any changes from the server that may exist. For now, you'll only use the tool to push, but it works for pulling too.

To push your changes up, use the **Synchronize Changes** button on the blue bar at the bottom of the window:  
![](https://i.imgur.com/d2PY1qT.png)

_Note: This may be a **Publish Changes** button with a cloud and an arrow instead, depending on the repository_

Once you click that button, you may have to enter your credentials. After that, your changes should exist in the server repository! You can go to your repository on GitHub and make sure the changes are there.

## Option 2: Adding, Committing, and Pushing via the Command Line
First, make sure your present working directory is your repository's folder. Then, use the commands below to interact with git.

### Status
To see the current status of your local repository, you can use the `git status` command:

```bash
git status
```

### Add all changes in the repository
This command will take any changes you currently have, and stage them for commit:

```bash
git add .
```

### Commit all changes
Once all of your changes are staged for commit, you can use the `git commit` command to commit them. Replace `COMMIT MESSAGE HERE` with a message regarding your changes:

```bash
git commit -m "COMMIT MESSAGE HERE"
```

### Push all changes
Once your changes are committed, you can push them up to the server repository. Use the `git push` command to accomplish this:

```bash
git push
```

Note: you will have to enter your credentials in order to push to the server repository. After that, your changes should exist in the server repository! You can go to your server repository on GitHub and make sure the changes are there.