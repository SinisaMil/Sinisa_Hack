# Optimal and comprehensive WordStar keybindings for VS Code
# by Sinisa Milivojevic


## Introduction

This is a short description of my WordStar keybindings, written for Visual Studio Code. These combinations of keys are based 
on the original WordStar program. However, I have added all keybindings found in Borland and JOE  editors, as well as my full WS keybindings 
that I wrote for (X)Emacs. 

__Problem with (X)Emacs is that ELisp programmers are not disciplined. If they used keymaps, as they were designed, it would have been fine.__
__However, all add-ons contain full key-sequences, so you have to re-program all ELisp add-ons. On the latest (X)Emacs on macOS you also have to change its C source code !!!__

It is so much better with Visual Studio Code. Microsoft has done a terrific job and configuring is truly easy. I did have to add small routines 
in JavaScript, but that is OK. 

Why WordStar keybingings ???

The answer is simple. That is the only set that allows you to do anything, without moving your hands away from the alpha-numeric part of the 
keyboard. No function keys, no arrows, PgUp, PgDn or similar .......

To put it simply, ideal for the touchtypists like myself.

In short, this contribution of mine contains all the things that a spoiled WS coder can wish for.

Most of things I wanted to see working are in full function and perform quite well.

### Necessary remarks

First of all, all keybindings are a combination of the prefix, like CtrlX+... or CtrlQ+ as you can clearly see from the tables below.

There are two important things to notice. 

**First , I have made it easier for use, by adopting that, for example, CtrlX+A invokes to the same command as CtrlX+CtrlA. Hence, you do not have to pay much of the attention to how long do you have to keep Ctrl pressed.**

Furthermore, so many commands have been assigned to the Wordstar / Borland / **Sinisa** combos that you will find most of what you need in this setup. If you want to see more, write your comments, please ...

Using Ctrl- prefix is also very nice, since that way, you go around various variations of the keys that you can find in Linux / Windows / macOS. Nothing to unlearn or to learn.

Next, this paper groups all keybindings into their respective categories. But, please do not expect to find them in the same order in the accompanying keybindings.json file.

I hope you know how to install keybindings.json in your local (HOME) directory. If you do not know how, I suggest the following URL:

https://stackoverflow.com/questions/33791097/how-can-i-change-keyboard-shortcut-bindings-in-visual-studio-code

Next, navigation among the panes (tabs) ...... This is done already, but it is not working as it should ..... Any ideas are welcome !!!


### Where to report a problem ???

Write a comment on this page with a question ..... I am still quite busy, so be patient ... You can report a problem that you spotted in the JSON file or in this document.

### Few words about myself

I am MySQL Developer since 1997. which means that I am still happily employed at Oracle Inc. 

In my spare time, I am now mostly focused on researching and coding some basic algorithms and coding them in C 2017, while waiting on C 2023. Lot's of work remains to be done ....

### Required extensions

In order for all of this to work, you need __"MultiCommand Extension"__  and __"Numbered Bookmarks Extensions"__ ...... for the time being ......

## TODO

* "Duplicate a current line" command ...... I like it on F4, but I might come up with some Ctrl+Q-... combo .. It is not working yet !!

* Move the block ..... I plan to start  working on it ....

* Navigation throughout most of VS Code menus, windows, separate parts of the window by Ctrl+... sequences .... this will not be that easy nor that soon ......

*  MUCH simpler Makefile-mode ..... No, I do not want to mess with CMake ....

If you have any idea, feel free to add them and post your addition in the comments. 

I will definitely put it on my TODO list. BTW, this is one of my most favorite sayings ...... "It is on my TODO list" ..... it increases perpetually .....


## Keybindings

These are separated in several categories ....

Control key combinations are denoted by Ctrl+. So Ctrl+W-E, means you first hold Ctrl, press 'W', then again press 'E'. As we learned above, Ctrl+W-E is identical to Ctrl+W-Ctrl+E.



### Navigation keys

-----------------------------------------------------------------
|*Key combo* | *Command or action * | Editing State     |      Comments |
|:--------   |:--------------------:| :-------: |--------------:|
|Ctrl+E      | CursorUp             | Editor    | Basic stuff               |
|Ctrl+E      | Previous Parameter   | Parameter  Hint | Depending on status |
|Ctrl+E      | Previous Quick Fix   | Quick Fix | Depending on status |
|Ctrl+E      | Previous Suggestion Fix   | Suggest Widget | Depending on status |
|Shift+Ctrl+E | SelectUp             | Select mode    | VS Code specific            |
|Ctrl+X      | CursorDown             | Editor    | Basic stuff               |
|Ctrl+X      | Next Parameter   | Param Hin | Depending on status |
|Ctrl+X      | Next Quick Fix   | Quick Fix | Depending on status |
|Ctrl+X      | Next Suggestion Fix   | Suggest Widget | Depending on status |
|Shift+Ctrl+X | SelectDown             | Select mode    | VS Code specific               |
|Ctrl+S      | CursorLeft             | Editor  | Basic stuff               |
|Ctrl+D      | CursorRight             | Editor    | Basic stuff             |
|Shift+Ctrl+S      | CursorLeftSelect             | Select Mode    | Code specific               |
|Shift+Ctrl+D      | CursorRightSelect             | Select Mode    | Code specific               |
|Ctrl+W      | Scroll Up              | Editor    | Basic stuff               |
|Ctrl+Z      | Scroll Down             | Editor    |  Basic stuff             |
|Ctrl+A      | WordLeft             | Editor    | Basic stuff               |
|Ctrl+F      | WordRight             | Editor    | Basic stuff               |
|Ctrl+Q-S      | Beginning of Line             | Editor    |  Basic stuff             |
|Ctrl+Q-D      | End of Line             | Editor    | Basic stuff               |
|Ctrl+K-J      | JumpToLineNo             | Editor    | from WordStar               |
|Ctrl+Q-I      | JumpToLineNo            | Editor    | from JOE               |
|Ctrl+R      | Page Up              | Editor    | Basic stuff               |
|Ctrl+C      | Page Down             | Editor    |  Basic stuff             |
|Ctrl+Q-R      | Top of the file              | Editor    | Basic stuff               |
|Ctrl+Q-C      | Bottom of the file             | Editor    |  Basic stuff             |



### File action keys

-----------------------------------------------------------------
|*Key combo* | *Command or action * | Editing State     |      Comments |
|:--------   |:--------------------:| :-------: |--------------:|
|Ctrl+K-S    | Save Current File    | Any       | Basic stuff              |
|Ctrl+K-E    | Open new File    | Any       |     Basic stuff          |
|Ctrl+K-Q    | Leave VS Code    | Any       |     Basic stuff          |
|Ctrl+Q-P    | Move to the left tab    | Any       |    Moves tab, but not file .... Advice required       |
|Ctrl+Q-N    | Move to the right tab    | Any       |   Moves tab, but not file .... Advice required            |


### Editing keys

-----------------------------------------------------------------
|*Key combo* | *Command or action * | Editing State     |      Comments |
|:--------   |:--------------------:| :-------: |--------------:|
|Ctrl+U      | Undo              | Editor    |    Basic stuff           |
|Ctrl+Q-F      | Find String            | Editor    | Basic stuff               |
|Ctrl+Q-A      | Replace String            | Editor    | Basic stuff               |
|Ctrl+L      | Next Find / Replace            | Editor    | Basic stuff               |
|Esc (Escape) | Abort Find / Replace            | Editor    | VS Code standard               |
|Ctrl+Q-F      | Find String            | Editor    | Basic stuff               |
|Ctrl+H      | Delete Char Left            | Editor    | Basic stuff               |
|Ctrl+G      | Delete Char Right            | Editor    | Basic stuff               |
|Ctrl+T      | Delete Word Right            | Editor    | Basic stuff               |
|Ctrl+Y      | Delete Entire Line  | Editor    | Basic Stuff   |
|Ctrl+Q-Y      | Delete Line to the Right   | Editor    |  Basic stuff             |
|Ctrl+N      |  Insert Line            | Editor    | Basic stuff               |
|Ctrl+M      | Break Current Line            | Editor    | Basic stuff               |
|Ctrl+I      | Insert Tab            | Editor    | Basic stuff               |
|Shift+Ctrl+I      |  UnTab            | Editor    | Basic stuff               |
|  F4      | Duplicate Current Line            | Editor    | Still on TODO list ... Recommend some CTRL sequence instead |

### Block Command keys

-----------------------------------------------------------------
|*Key combo* | *Command or action * | Editing State     |      Comments |
|:--------   |:--------------------:| :-------: |--------------:|
|Ctrl+K-B    | Begin Block    | Editor       | Basic stuff              |
|Ctrl+K-K    | End Block    | Editor       |     Basic stuff          |
|Ctrl+K-Y    | Delete Block    | Editor       |     Basic stuff          |
|Ctrl+K-C    | Copy Block    | Editor       |     Basic stuff          |
|Ctrl+K-V    | Move Block    | Editor       |     On TODO list ... or CtrlK-M or both ???   |


### Bookmark command keys .....  read above about the extensions ......

-----------------------------------------------------------------
|*Key combo* | *Command or action * | Editing State     |      Comments |
|:--------   |:--------------------:| :-------: |--------------:|
|Ctrl+K-1    | Set Bookmark No 1    | Editor       | Bookmarks              |
|Ctrl+K-N    | Set Bookmark N ... N = 2 to 9     | Editor       |     Bookmarks          |
|Ctrl+Q-N    | Go To Bookmark N ... N = 1 to 9     | Editor       |     Bookmarks          |
|Ctrl+O-C    | Clear Bookmarks in Current File     | Editor       |     Bookmarks          |
|Ctrl+O-Y    | Clear Bookmarks in All Files     | Editor       |     Bookmarks          |


## THE END


