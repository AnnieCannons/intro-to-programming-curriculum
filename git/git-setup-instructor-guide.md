1. Have them install Homebrew and Git. Possibly outside of class time, as this can be a real time-sink if you do it in class.
2. Have them configure Git using the [class-gitconfig](https://github.com/abbreviatedman/class-gitconfig) repo.
3. Have them get a GitHub account with their personal-professional emails.
4. Collect their GH usernames (which is a good thing to have on file!).
5. Add each of those usernames as a collaborator on a private repo. Each of them should get an email inviting them to join as a collaborator. If they have trouble finding the email, it should have a "from" field that's the private repo's owner's username and a "subject" field  with the private repo's owner's username and "invited you to".
6. They should each click the link in the email that says "View invitation".
7. That will take them to a page where they can click "Accept invitation".
8. Now they can go back to their terminal and install Git Credential Manager. They can enter the commands `brew tap microsoft/git` followed by `brew install --cask git-credential-manager-core`. It may ask them for their password, which can throw them off, since terminals don't show password input.
9. Then they can clone down the private repo with `git clone`, which will open a window asking if they want to sign in. Once they say they do, it will then open their default browser, and by signing in (or being signed in already) they will automatically be authorized to GitHub.
