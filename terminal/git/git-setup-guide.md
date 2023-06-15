# Git Setup Guide

This setup guide covers several aspects of getting started with Git and/or continuing with Git on a Mac computer.

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

Your instructor will add you to a private repository. This is so that you can tell if you authenticated to GitHub correctly. If you did, then you'll be able to clone the repository successfully.

**Once they've added you**, you should get an email inviting you to join a repository as a collaborator, and you can follow these steps to get added to the repository:

1. **Find the email**. If you have trouble finding the email, it should have a "from" field that's the private repo's owner's username (ask your instructor if you're not sure) and a "subject" field  with the private repo's owner's username and "invited you to".
6. **Click the link** in the email that says **"View invitation"**.
7. That will take you to a page where you can **click "Accept invitation"**.

### Install GitHub's Git Credential Manager

Now that you're on the repo, we can get you authorized to GitHub using Git Credential Manager.

8. Now they can go back to their terminal and install Git Credential Manager. They can enter the commands `brew tap microsoft/git` followed by `brew install --cask git-credential-manager-core`. It may ask them for their password, which can throw them off, since terminals don't show password input.
9. Then they can clone down the private repo with `git clone`, which will open a window asking if they want to sign in. Once they say they do, it will then open their default browser, and by signing in (or being signed in already) they will automatically be authorized to GitHub.
