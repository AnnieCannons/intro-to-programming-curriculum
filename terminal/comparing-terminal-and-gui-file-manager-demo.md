# Demo - Comparing GUI File Manager And The Terminal

The purpose of this instructor demonstration is to show how a graphical file manager and a terminal are showing the same information.

## Opening The File Manager And The Terminal

Open the file manager ("Finder" on macOS) and the terminal ("Terminal" on macOS).

Ask your students to follow along _only_ in the file manager as you do this. You'll slow things down too much if they're using the terminal, _unless_ you combine this with learning terminal commands.

This demo could also work to repeat it later with the students following along, once they're ready to learn some terminal commands.

## Show `ls` and `pwd`.

1. Enter `ls` in the terminal and show that it has the same files and folders as shown in the file manager.
2. Ask, "now what folder are we in?" The answer is "your home folder", but you can _also_ show that you can find it by command-clicking the title bar.
3. Now show that `pwd` shows the same thing as the title-bar file manager path.

## Show `mkdir` and `touch`.

### `mkdir`

1. Navigate to the Documents folder by double-clicking in the file manager. `cd` into the directory in the terminal. Show `ls` and  `pwd` and that they still match the file manager's output.
2. Create a folder with the file manager and a different one with `mkdir`.  `ls` and show the file manager to show their equivalence. `cd` into one directory and run `pwd`, showing the equivalent in the Finder.

### `cd`

1. `cd` up a level with `..` and discuss that `..`is a shortcut for "the current directory's parent". Do the same in the file manager.
2. `cd` up several levels, following along in the file manager.
3. Then `cd` down several levels, following along in the file manager, ending up in the _other_ directory you made with `mkdir`.
4. Finally, demonstrate the speed with which you can navigate by `cd`-ing to `/`, and then `cd`-ing back into the directory with one command including tab completion.

### `touch`

1. create an `index.html` file in the file manager and a `style.css` file with `touch`.
2. Do an `ls` and compare with the file manager.
3. Open with VS Code and show that both files are empty. Leave the program open if you're doing the next part.

### One More Demo Of The Terminal's Power

1. Talk about how you can even edit files in the terminal.
2. Open the `index.html` file with Chrome to show how that's done.
3. Go back to the terminal and run `echo "h1 {color: green} p {color: blue} span {font-weight: 900}" > style.css`
4. Open `style.css` in VS Code (or switch to it if you left it open) to show that it's been edited.
5. Go back to the terminal and run `echo '<html><head><title>Terminal Demo</title><link href="style.css" rel="stylesheet" /></head><body><h1>Terminals Are Neat-o</h1><p>Yeah they <span>are</span>!</p></body></html>' > index.html`
6. Now look at the HTML file in VS Code to see how it's changed.
7. And reload the window in Chrome to see the HTML and CSS working together.


