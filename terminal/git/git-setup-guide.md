# Git Setup Guide

This setup guide covers several aspects of getting started with Git and/or continuing with Git on a Mac computer. After you're done, you'll have some of the most popular and powerful tools in a developer's tool belt.

## Git Installation

### Step 1: Install Homebrew

We'll use Homebrew to install Git. This will give you the most up-to-date version of Git, as well as make it easy to update or uninstall it. It's also _very_ useful to have Homebrew, and we'll be using it to install other things in this course.

1. This [Homebrew link](https://brew.sh/) has the code you'll need under its "Install Homebrew" section. Click the clipboard symbol to its right to copy the one line of code, then paste into Terminal and it return.
2. It will ask you for your account's password. Enter it, but note that **it will not show you typing as you type your password**. There will be **no cursor** as you type. But if you type in your password correctly and hit return, the installation will proceed.
3. It may ask you to hit RETURN to confirm its creation of folders. Do so!
4. Homebrew installation will take some time to complete, especially over slower connections. If this happens to you, go take a break!
5. **You'll know installation is done when you get back to a "command prompt"**. You'll see the line "Installation successful!" in bold next to an arrow. You'll see similar messages below it with "Homebrew is run entirely by unpaid volunteers"—it is—and "Next steps"—which we'll follow now.
6. Under that "Next steps" heading, there are **two important commands** to finish installation of Homebrew. One should start with something _like_ `(echo; echo`, and the other, on the next line, starts with something _like_ `eval "$(`. (If neither is exactly like that, don't panic! They'll match those starts pretty closely.) You'll copy-paste these into the terminal **one at a time**. So first you'll copy the entire line that starts with `(echo; echo`, paste it into your terminal, and hit return. Then you'll copy the entire line that starts with `eval "$(`, paste that into your terminal, and hit return.
7. You'll know you're done when entering the command `brew --version` into your terminal gives you any output _that does not include_ `command not found: brew`. If it tells you `command not found`, it's likely that you didn't copy and paste the commands from the previous step. If you think you did so, copy and paste them again. If `brew --version` still gives you `command not found`, then ask in Slack!

### Step 2: Use Homebrew To Install Git

Now that we have Homebrew, this is fairly easy!

1. Run `git --version`, taking note of what number it gives you. This is just to check later that you have a newer version.
2. Run `brew install git`. If it gives you output that includes `command not found: brew`, then you should follow the last couple of steps from the Homebrew installation settings.
3. Once it's done installing (and it shouldn't take long), **open a new terminal window** (Command-n will do so), type in `git --version`, hit return, and make sure that the output is a number greater than you had before. If so, you're done!

### Step 3: Configuring Git

We'll follow the steps in [this repository](https://github.com/abbreviatedman/class-gitconfig). This will give us a basic setup for Git, cutting down on the time we need to explain configuration or make you configure it yourself, while still providing the understanding of how to configure it in the future.

## Github Authentication

Now that you have Git, you can manage your version control locally on your computer. However, to upload your projects to GitHub or collaborate with anyone on there, you'll need to authorize your computer to do so. (Security is taken _very_ seriously when it comes to the server your app's code lives on!)

### Get A GitHub Account

Sign up for a new account on [GitHub](https://www.github.com) **with your professional personal email** (not your AnnieCannons one). It's a fairly easy signup process, though you _will_ have to:

1. check your email for a confirmation code, and then 
2. enter it back in on GitHub

### Send Us Your GitHub Username

However your instructor asks for it, get us your GitHub username. This is **very important** for the next step!

### Accept Your GitHub Collaboration Invitation

Your instructor will add you by GitHub username to a private repository. This is so that you can tell if you authenticated to GitHub correctly. If you did, then you'll be able to clone the repository successfully.

**Once they've added you**, you should get an email inviting you to join a repository as a collaborator, and you can follow these steps to get added to the repository:

1. **Find the email**. If you have trouble finding the email, it should have a "from" field that's the private repo's owner's username (ask your instructor if you're not sure) and a "subject" field  with the private repo's owner's username and "invited you to".
2. **Click the link** in the email that says **"View invitation"**.
3. That will take you to a page where you can **click "Accept invitation"**.

### Install GitHub's Git Credential Manager

Now that you're on the repo, we can get you authorized to GitHub using Git Credential Manager.

1. Let's go back to the terminal and install Git Credential Manager. The first step is to enter the command `brew tap microsoft/git` in the terminal, then hit return.
2. Then enter the command `brew install --cask git-credential-manager-core` and press return. It _may_ ask you for their password, which would be your **password to your computer**. It may still not show your input as you type your password.
2. Now it's time to **clone down the private repo** and make sure you're authorized. Enter the command `git clone [repo url]`, with the `[repo url]`portion replaced with the url your instructor will give you.
3. It will now ask you if you want to sign in with your browser, which you do.
4. It should switch you to your default browser and ask you to **sign into GitHub**, if you're not signed in already.
5. Then it will ask if you want to authorize to GitHub. You do!
6. Once you've authorized to GitHub, your browser will tell you you're done, and you can **switch back to your terminal**. It should have output that includes a line starting with "Cloning into", some lines starting with "remote" and some more lines starting with "Receiving".

**If you got the output from the last step**, then _you're all set_ to work in the cloud and collaborate with anyone in the world through GitHub.

**If you _didn't_ get that output**, then ask your instructor. I'm sure they'll help.

## Final Thoughts

 Believe it or not, we've worked to cut a _lot_ of steps out of installing all these standard code collaboration tools (wait... this could have been _more_ difficult??). Setting up Homebrew, Git, and GitHub is famously an _awful lot_. And as new developers, this is especially challenging. But it's a necessary step since so much of what we do now lives under version control and in the cloud.
 
 If you got stuck, we'll _always_ help you get unstuck, whether it's in code or with tech support needs.
 
 If you finished all of the above, then congratulations, you now have all the tools you need to work with each other's code, turn in _your_ code to the instructors, start new side projects and store them in the cloud, contribute to open source projects, and so much more.
 
 Well done!
