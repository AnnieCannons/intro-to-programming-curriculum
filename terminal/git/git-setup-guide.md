# Git Setup Guide

This setup guide covers several aspects of getting started with Git and/or continuing with Git on a Mac computer.

It is highly recommended that you install Git **after class**. It can take a while, especially with the Homebrew portion, and especially on a slow connection. Devote a half hour of uninterrupted time to it, though some of this can be spent away from your computer while Homebrew downloads.


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

## Github Authentication

Now that you have Git, you can manage your version control locally on your computer. However, to upload your projects to GitHub or collaborate with anyone on there, you'll need to authorize your computer to do so. (Security is taken _very_ seriously when it comes to the server your app's code lives on!)

So in the next step, we'll add a Personal Access Token (or PAT) for GitHub, first on their servers, then on our machine.

We're generally going to follow the steps outlined in the **Creating a personal access token (classic)** on GitHub. **Make sure not to follow the "fine-grained personal access token" steps**. They're fine steps, but they're different and slightly more complicated than what's described below. 

### Personal Access Token Creation On GitHub

1. In the browser, log into your Github account.
2. Follow the steps outlined in the **Creating a personal access token (classic)** on GitHub,  to [create your Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#creating-a-personal-access-token-classic) **with the following specific directions**:
    a. Under "Expiration", select “No expiration”
    b. For "Select scopes", please check the following boxes. Some will check boxes under themselves—this is what we want.
        1. "repo" 
        2. every box that starts with the word "admin" 
        3. "user"
        4. "delete_repo"
3. Follow all other steps outlined in GitHub's directions, finishing with pressing the "Generate token" button, but you do _not_ need to do the last step to work with an organization that uses SAML single sign-on. **Once you have clicked "Generate token", do not close the tab.**
4. It's _very_ important that you now **copy the code** to your clipboard **without closing the tab or window**, and paste it into a text file—a note in the Pages app is a good place for it. The code should start with `ghp` and be in a green rectangle. You can copy it to your clipboard automatically by pressing the blue squares after the code, one of the universal symbols for a clipboard. Put that code somewhere you can find it—a Pages note is a good place for this—although if you lose it, you can follow the steps in this section from the beginning.

### Logging Into GitHub With Your Personal Access Token
