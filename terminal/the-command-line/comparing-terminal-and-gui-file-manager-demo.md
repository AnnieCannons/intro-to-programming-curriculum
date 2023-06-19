# Demo - Comparing GUI File Manager And The Terminal

The purpose of this instructor demonstration is to show how a graphical file manager and a terminal are showing the same information.

## Opening The File Manager And The Terminal

Open the file manager ("Finder" on macOS) and the terminal ("Terminal" on macOS).

Ask your students to follow along _only_ in the file manager as you do this. You'll slow things down too much if they're using the terminal, _unless_ you combine this with learning terminal commands.

This demo could also work to repeat it later with the students once they're ready to learn some terminal commands.

## Show `ls` and `pwd`.

1. Enter `ls` in the terminal and show that it has the same files and folders as shown in the file manager.
2. Ask, "now what folder are we in?" The answer is "your home folder", but you can _also_ show that you can find it by command-clicking the title bar.
3. Now show that `pwd` shows the same thing.

## Show `mkdir` and `touch`.

### `mkdir`

1. Navigate to the Documents folder by double-clicking. `cd` into the directory in the terminal. Show `ls` and  `pwd` and that they still match the file manager's output.
2. Create a folder with the file manager and a different one with `mkdir`.  `ls` and show the file manager. `cd` into one directory and run `pwd`, showing the equivalent in the Finder.

### A Side Note On `..`And A Demo Of Terminal Speed.

1. `cd` up a level with `..` and discuss that `..`is a shortcut for "the current directory's parent".
2. `cd` up several levels, following along in the file manager.
3. Then `cd` down several levels, following along in the file manager, ending up in the _other_ directory you made with `mkdir`.
4. Finally, demonstrate the speed with which you can navigate by `cd`-ing to `/`, and then `cd`-ing back into the directory with one command including tab completion.

### `touch`

1. create an `index.html` file in the file manager and a `style.css` file with `touch`.
2. Do an `ls` and compare with the file manager.
3. Open with VS Code and install to show that you can see both 
