# Git Solo Exercise - Prepping To Interview Someone

In this assignment, you'll **write questions** as if you were **interviewing a peer**.

More importantly, you'll **practice your Git and GitHub skills**.

## Learning Objectives

After this assignment, students will be able to:

- Edit a file with Visual Studio Code.
- Have some familiarity with Git.
- Have some familiarity with GitHub.
- **Use** (but **not** memorize) the basic Git workflow.
- Push their changes to GitHub.

## Instructions

1. Switch to your browser.
2. Go to [GitHub's homepage](https://www.github.com).
3. Create a new repository. There should be a green button that says "New" on the left, as of this writing. If not, you'll have to figure out how to do so!
4. On the next page, where you create a repo,  enter "git-solo-exercise" as a name for the repository.
5. Do not create it with a readme or any other option. This is the default, so go right from naming the repo to clicking "Create repository" at the bottom.
6. It should take you to a page with an address like "https://www.github.com/[your-username]/git-solo-exercise". The page should have many terminal commands for you to enter, but **we'll give you the right ones here**.
7. Switch to your terminal.
8. If you haven't already, create a `dev` directory in Documents using `mkdir`.
9. Navigate to your `dev` directory with `cd`.
10. Create a directory called `git-solo-exercise`.
11. Navigate into it with `cd`.
12. Initialize it as a git repository with `git init`.
13. Create a file called `readme.md`—`touch` is a good command to use, here.
14. **Open the file or directory in Visual Studio Code**.
	- If you have the `code` command set up, you can simply run `code .` to open the current directory in VSC—`.` is a shortcut in the terminal for the current directory
	- If not, you can launch or switch to Code, then click the File menu at the top, then Open, and navigate to the directory `git-solo-exercise` or the file `readme.md`.
	- If you opened the whole directory, now open the `readme.md` file in VS Code—you should be able to see the file in VS Code on the left side of the screen, though a good tool for opening files is the shortcut Command-p, which will let you type in the name of any file in your current project to open it or switch to it.
15. In `readme.md`, write "Questions For An AnnieCannons Student" as the first line of the document. If you want it to appear as a big heading on GitHub, add a `# ` to the start, so that the title is "# Questions For An AnnieCannons Student".
16. Save the changes! (Or turn auto-save on in the File menu so this is done for you automatically.)
17. Switch to the terminal.
18. Add the changes using `git add readme.md`.
19. Commit. You can enter `git commit -m "[commit message goes here]"` in your terminal, replacing the brackets and their contents with a message. Don't forget the spaces and the closing quotes. You can enter **any message you like**, but a typical one here would be "Initial commit."
20. Switch to your browser.
21. Copy the address of your GitHub repository to your clipboard.
22. Switch back to the terminal
23. Add a connection to the GitHub server's repository by entering the command `git remote add origin [url]`, where the brackets and their contents are the address in your clipboard from the previous step.
24. Now you can push your new commit to GitHub using `git push origin main`.
	- Optionally, switch to your browser to confirm this worked—reload the GitHub repo page and you should see the title appear in the `readme.md` file.
25. Switch back to your `readme.md` document in VS Code.
26. On a new line, write a **question** that you might ask another student to get to know them better.
27. Save the file if you don't have auto-save turned on.
28. Switch back to your terminal.
29. Add the change with `git add readme.md`.
30. Commit the changes with `git commit -m "[commit message goes here]"`. Try to use the message to describe the change you just made!
31. Push to GitHub again with `git push origin main`.
32. Repeat steps 25-31 until you have **5** questions. Think about what commit messages to enter as you describe what it is you've changed!
33. Switch to your browser to confirm that the repository on GitHub has **all 5 questions** in its `readme.md` file.
  - If it has only 4 questions, you probably left off steps 29-31 for the last question!
  - If it doesn't have any, hit up your help channel to see if someone can help you figure out what command you missed!
34. Once you've confirmed that they're all in GitHub, turn in your assignment by submitting the URL for your GitHub repo on Canvas.
