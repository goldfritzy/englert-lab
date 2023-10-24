# ⚙ Edit the site

This approach requires experience with Git and using command-line interfaces, but is better for when you're doing larger edits, when you want to work on your changes privately before pushing them, and when you want to iterate rapidly and not wait for pull request previews to update.

[Make changes with Git](https://www.google.com/search?q=git+basics) on your command line. In summary:

1. Decide how you'll be making changes:
   1. Make changes directly to the `main` branch of your website repo (_publishes changes immediately_).
   2. Make changes to a branch (e.g. `add-joshua-bio`) of your website repo (_allows previewing changes before publishing_).
   3. Make changes to a fork of your website repo (_allows previewing changes before publishing_).
2. [Clone](https://docs.github.com/en/free-pro-team@latest/github/creating-cloning-and-archiving-repositories/cloning-a-repository) the appropriate repo to your computer and switch to the appropriate branch.
3. Edit the cloned site on your computer with your favorite [text/code editor](https://code.visualstudio.com/).
4. Commit and push the changes.
5. If working from a branch or fork, make a pull request to your main website repo and merge when ready to publish.

### On Your Computer (Locally) (Method Two - GitHub Client)

A more "user-friendly" approach is to use the GitHub desktop client, which makes it easier to track individual changes made on a local machine. Below is a brief overview of the instructions in order to develop on the GitHub client.

1. Download the[ GitHub Desktop Client](https://desktop.github.com/).
2. Log-in with your GitHub account
3. Inside the GitHub App, click on "clone repository", then click on "englertlab/englert-lab".
4. Press "Clone". This will download the files of the website onto your local machine.
5. Click "For my own purposes".

{% hint style="info" %}
You can access the Englert Lab repository either through the dedicated Englert Lab Development account, or by adding yourself as a collaborator and using your own personal GitHub account.
{% endhint %}

{% hint style="info" %}
The local path of the repository doesn't matter, just as long as you remember where it is on your machine.
{% endhint %}

### Editing the Site Locally through a Code Editor (VS Code)

Feel free to use any code editor you are comfortable using, for these purposes, I will be demonstrating the basics with my own code editor I used in creating this website.



1. Download and install the [Visual Studio Code](https://code.visualstudio.com/) application.
2. Open Visual Studio Code
3. Click File>Open Folder
4. Navigate to the local directory where you cloned the Git repo to.
5. You will see a pop-up window which asks if you trust the authors of the folder. Click "Yes".
6.  You will now see all files which are a part of the Englert Lab Website.



&#x20;

{% hint style="info" %}
When installing VS Code, leave all options default unless you know what you are doing
{% endhint %}
