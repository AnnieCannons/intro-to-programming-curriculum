# Git Pair Exercise - Actually Interviewing Someone

In this assignment, you'll **write questions** for a peer... _and_ they will answer them!

More importantly, you'll **practice your Git and GitHub skills**.

### Learning Objectives

After this assignment, students will be able to:

- Add collaborators to their GitHub repositories.
- Explain the process for pushing and pulling.
- Have some familiarity with the commands for pushing and pulling, but **not** have them memorized.
- Know where to look for further resources.

### A Git Cheatsheet

There is no perfect cheatsheet out there, but with only **one exception**, this one from GitHub matches our workflow.

**The exception**: Please note that for pushing and pulling, we'll be using the fuller version of those commands:

- `git push origin main`
- `git pull origin main`

Here is |GitHub's Git Cheatsheet|(https://training.github.com/downloads/github-git-cheat-sheet/).

### If Your Branch Is called "master" Instead

**If you haven't pulled in the class gitconfig**, then your **branch** will still be **master**.

In that case, the commands will be `git push origin master` and `git pull origin master` for you.

You can fix this and avoid using a terrible slavery metaphor using the directions in the [class gitconfig](https://github.com/abbreviatedman/class-gitconfig) repository. This will also get **rid of** many **lengthy git warnings** that clutter your terminal, _and_, with the `code` command installation (here are [the directions for setting up that command](https://code.visualstudio.com/docs/setup/mac#_launching-from-the-command-line)), allow you to shorten the `git commit -m "[commit message]"` to just `git commit`, and then write your commit messages in VS Code. This makes it _far_ easier to work on your commit messages!

### Assignment Instructions

For these instructions, we'll refer to **partner 1** and **partner 2**. Pick one to be (it doesn't matter much which), and any instructions that are targeted at that partner will be for you.

Each partner should **share their screen** when they are the ones following instructions. When the instructions ask you to switch, **switch whose screen is being shared**. This way you **can always work together to do the steps**, seeing the same actions and results as you go and **solving problems together**.

##### Setup

_These steps are for partner 1._

1. Switch to your browser.
2. Go to [GitHub's homepage](https://www.github.com).
3. Create a new repository. There should be a green button that says "New" on the left, as of this writing. If not, you'll have to figure out how to do so!
4. On the next page, where you create a repo,  enter "git-pair-exercise" as a name for the repository.
5. Do not create it with a readme or any other option. This is the default, so go right from naming the repo to clicking "Create repository" at the bottom.
6. It should take you to a page with an address like "https://www.github.com/[your-username]/git-pair-exercise". The page should have many terminal commands for you to enter, but **we'll give you the right ones in a moment**.
7. Click the "settings" button. It's near the top of the repository's page, in a row of buttons that begins with "Code". (If you're zoomed in or in a small window there may be a "..." at the right of "Code"—click on it and a menu will drop down with "Settings" as an option.)
8. Click the "Collaborators" button, which should be on the left side. It may ask you for your password again at this point.
9. Click the "Add people" button.
10. Enter the username for your partner here.
11. Click the "Add [username] to this repository" button.
12. Go back to your repo's homepage by pressing the "Code" button, which should be near the top left of the app.
13. Switch to your terminal.
14. If you haven't already, create a `dev` directory in Documents using `mkdir [filepath]`. What's the path to give `mkdir`? Depends on where you are.
15. Navigate to your `dev` directory with `cd [path to dev directory]`.
16. Create a directory called `git-pair-exercise` by entering the command `mkdir git-pair-exercise`.
17. Navigate into it with `cd git-pair-exercise`.
18. Initialize it as a git repository with `git init`.
19. Create a file called `readme.md` using the command `touch readme.md`.
20. Open the file or directory in Visual Studio Code.
	- If you have the `code` command set up, you can simply run `code .` to open the current directory in VSC—`.` is a shortcut in the terminal for the current directory
	- If not, you can launch or switch to Code, then click the File menu at the top, then Open, and navigate to the directory `git-pair-exercise` or the file `readme.md`.
	- If you opened the whole directory, now open the `readme.md` file in VS Code—you should be able to see the file in VS Code on the left side of the screen, though a good tool for opening files is the shortcut Command-p, which will let you type in the name of any file in your current project to open it or switch to it.
21. Switch to your browser.
22. Make sure you're at the "Code" tab of your repository—click the "Code" button if not!
23. Copy the address of your GitHub repository to your clipboard.
24. Switch back to the terminal
25. Add a connection to the GitHub server's repository by entering the command `git remote add origin [url]`, where the brackets and their contents are the address in your clipboard from the previous step.

##### Your First Commit

1. In `readme.md`, write "Interview With [your partner's name]" as the first line of the document, replacing the brackets and their contents with your partner's name. If you want this first line to appear as a big heading on GitHub, add a `# ` to the start, so that the title is "# Interview With [your partner's name]" (note the space after the `#` symbol).
2. Save the changes! (Or turn auto-save on in the File menu so this is done for you automatically.)
3. Switch to the terminal.
4. Add the changes using `git add readme.md`.
5. Commit. You can enter `git commit -m "[commit message goes here]"` in your terminal, replacing the brackets and their contents with a message. Don't forget the spaces and the closing quotes. You can enter **any message you like**, but a typical one for adding a file would be "Initial commit."
6. Now you can push your new commit to GitHub using `git push origin main`.
   - Optionally, switch to your browser to confirm this worked—reload the GitHub repo page and you should see the title appear in the `readme.md` file.
	
##### Adding A Question 

1. Switch back to your `readme.md` document in VS Code.
2. On a new line, write a **question** for your partner.
3. Save the file if you don't have auto-save turned on.
4. Switch back to your terminal.
5. Add the change with `git add readme.md`.
6. Commit the changes with `git commit -m "[commit message goes here]"`. Try to use the message to describe the change you just made!
7. Push to GitHub again with `git push origin main`.

##### Setup For The Other Partner

Now it's the other partner's turn!

_These steps are for partner 2._

1. If you haven't already, create a `dev` directory in Documents using `mkdir [filepath]`. What's the path to give `mkdir`? Depends on where you are.
2. Navigate to your `dev` directory with `cd [path to dev directory]`.
3. Clone down your partner's repository. Get the web address ( otherwise known as a "URL") from your partner for their repository, then clone it down with `git clone [repo url]`.
4. Navigate into it with `cd [repo name]`. The repo name is _probably_ `git-pair-exercise`, but your partner may have named it differently—it should be the last part of the URL you cloned, everything after their username and the `/`. If you can't find it, run `ls` to see what you just cloned down, and navigate into directory.
5. Open the file or directory in Visual Studio Code.
   - If you have the `code` command set up, you can simply run `code .` to open the current directory in VSC—`.` is a shortcut in the terminal for the current directory
   - If not, you can launch or switch to Code, then click the File menu at the top, then Open, and navigate to the directory `git-pair-exercise` or the file `readme.md`.
   - If you opened the whole directory, now open the `readme.md` file in VS Code—you should be able to see the file in VS Code on the left side of the screen, though a good tool for opening files is the shortcut Command-p, which will let you type in the name of any file in your current project to open it or switch to it.

##### Answering The First Question And Asking The Next

_These steps are for partner 2._

1. You should see an unanswered question in the `readme.md` file in VS Code.
2. Write an answer to the question. It will show up better on GitHub if you add an extra blank line between the question and answer, but this is optional.
3. Write a **new question** for your partner to answer. It will show up better on GitHub if you add an extra blank line between the previous answer and this new question, but this is optional.
4. Save the changes! (Or turn auto-save on in the File menu so this is done for you automatically.)
5. Switch back to your terminal.
6. Add the change with `git add readme.md`.
7. Commit the changes with `git commit -m "[commit message goes here]"`. Try to use the message to describe the change you just made!
8. Push to GitHub again with `git push origin main`.

##### The General Workflow

_These steps are for partner 1 _first_, but after that you will take turns doing this general workflow._

1. Switch to your terminal.
2. Enter the command `git pull origin main`.
3. Switch to VS Code.
4. You should see the answer to your previous question, as well as a new question for yourself!
5. Answer the question, then enter a new question for your partner.
6. Save the changes! (Or turn auto-save on in the File menu so this is done for you automatically.)
7. Switch back to your terminal.
8. Add the change with `git add readme.md`.
9. Commit the changes with `git commit -m "[commit message goes here]"`. Try to use the message to describe the change you just made!
10. Push to GitHub again with `git push origin main`.

##### Keep Alternating That General Workflow

Switch to partner 2 and repeat steps 1-10 from The General Workflow, then switch again and repeat. Do this for each partner for at least 5 questions, but for as many as you want to do for practice!

##### Turning In

What you'll submit on Canvas is **the URL of the repository on GitHub**. It does _not_ matter **whether it's on your account or your partner's**—you will **both** turn in the **same** URL.
