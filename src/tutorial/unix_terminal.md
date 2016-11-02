# Unix/Linux Terminal

This is going to be a tutorial on usage of a Linux/Unix based terminal. If you want a more in depth overview of Bash on the hand you may find [this](/tutorial/bash.html) useful.

The topics that are going to be covered are as follows:

* Moving around the system
* Basic commands
* Searching
* Editing
* Tunneling (SSH)

## Moving around the system

The most common thing you are going to need to do is move around the system and see where you are.

Commands that are going to be used here are (not including variations):

* `cd`
* `ls`
* `pwd`
* `cd ~`
* `cd ..`

The first thing you will see when opening a terminal will be something along the lines of:

```
merlin@machine ~ $
```

That line tells us 4 things:

1. `merlin` is your username
2. `machine` is your hostname
3. `~` is your current location (`~` means home directory)
4. `$` is your current access rights (`$` is normal, `#` is sudo)

From here there are many things we can do, some of which are seeing what is in this directory (`ls`), or going to a different directory (`cd`), or we could run a program.

Examples of each of those commands:

* `cd Music` - will switch to the "Music" directory
* `ls` - will list all the files and directories (that are not hidden)
* `ls -l` - will produce the above items in a list with more information.

There are some very useful arguments that can be passed into `ls`, a short list of them are:

* `-a` - show all files, including hidden files.
* `-l` - show detailed list
* `-1` - show in a list
* `-h` - show sizes in "human" readable format
* `--help` - will show all the available arguments

If you want to move up a directory then the special file `..` is available, which can be used like: `cd ..` or perhaps `cd ../Pictures`

You can always move around the system like that usually you know exactly where you want to go then you can go straight there like `cd Code/projects/site/src` or if the location is not in your current directory but you know the location from the root (`/`) of the drive then you can use `cd /usr/bin` to get there directly.

If you are ever lost then you can always use `pwd` to see where you are from the root or your home directory, depending on where you are.

And if you need to go to your home directory in a hurry then either of `cd ~` or `cd` will take you directly to your home directory.

## Basic commands

Now that we can see what files are where we would like to see some information regarding the files. There are many things you might want to know about a file. For example the size of a file, or the type of file it is. And quite often the contents of the file.

The various commands and an example of their usage would be:

* `file test.mp3` to see the type of file it is
* `file -I test.mp3` to print the mimetype
* `ls -lh test.mp3` to print the size of the file and other properties
* `wc test.txt` to check how many lines/words/characters are in a file
* `cat test.txt` to print the contents to the screen

## Searching

There are many times that searching for files is needed. This is going to be split into two sections. Searching by file/directory name and searching based on content.

### File/Folder name

### File content

## File Editing

## Tunnelling
