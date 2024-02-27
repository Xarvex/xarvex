# Vim

Insight into what I think is, while not for everyone, the best editor out there for development.


## Table of Contents

- [Introduction](#introduction)
- [Environment](#environment)
- [PDE](#pde)
- [Learning](#learning)


## Introduction

If you are reading this you likely already have at least some intrigue in Vim/Neovim.
Perhaps its the personal nature of it, or the raw feel of editing in a terminal.
This document will be about Vim-type editors in general, however my recommendation is Neovim and that is what I will be expanding on later.
Since Neovim is a fork of Vim, at the time of writing their general ideas are consistent,
so when I refer to Vim, Neovim will also apply in that aspect.

Want a quick introduction? Here are two great videos made by [Fireship](https://youtube.com/@Fireship):\
[Vim in 100 Seconds](https://youtu.be/-txKSRn0qeA)\
[Neovim in 100 Seconds](https://youtu.be/c4OyfL5o7DU)

For the longest time, I had been a Visual Studio Code user. Eventually, I switched to Neovim,
and have created a configuration suited exactly to my workflow.
While I don't think I can call myself an expert, here are several resources I find relevant in making the plunge, too.

Quick disclaimer though, is that while I do believe Vim-based editors are the very best around,
there is that one caviat in that it is not for everyone. This is namely because there is a steep learning curve.
Proper usage of Vim means minimal or no usage of the mouse, and using various keyboard shortcuts to perform actions,
added onto the overall comfortability with using the terminal the editor is home to.
It is for these reasons someone might be discouraged, which I myself was for very long.
However, when the effort and time is put in reaching benefits are made in productivity, flow, and understanding.

That being said, you can choose to learn strictly the keybinds/shortcuts and leverage Vim as a plugin in an alternative editor.
Perfectly okay and will still have lasting benefits! For that, maybe jump to [Learning](#learning).


## Environment

Again, part of using a terminal application is, quite obviously, the terminal.
But, what I mean by that is the usage and integration with other command-line tools on your system.
Using a terminal editor is not about pressing the green start button in your JetBrains IDE to somehow run your code in its magic.

One of the most important attributes is the understanding of your environment.
Don't press "play" on your Rust code; execute `cargo run`.
When you understand your environment, you understand how your code interacts with it,
and a terminal edtior is not detached from it as Visual Studio Code would be.
Content can be directed "piped" back and forth just as in typical CLI applications,
with an otherwise encouragement to open the terminal for other tasks.

I would recommend some sort of Unix-like system that gives access to essentials such as `cat`, `sed`, `awk`, `jq`, and others.
For Windows users, look into [WSL](https://learn.microsoft.com/windows/wsl).
Using an Ubuntu system would be my recommendation for those new to Linux,
and not very sure about what distribution to choose.
As for MacOS, install [brew](https://brew.sh) and [coreutils](https://formulae.brew.sh/formula/coreutils).


Speaking of environment...

## PDE

Looking at this acronym you might think I made it up on the spot.
Well, it is a little made up, but not by me! PDE stands for Personal Development Environment,
it is essentially an IDE tailored to your needs and workflow.

Both Vim and Neovim have scripting languages to configure them, called Vimscript.
This kind of freedom gives you, the user, the power of your imagination (and the imagination of others through plugins) to customize.
What's more, Neovim additionally has support for Lua, a popular and performant language that is easy to learn and has various other applications.

I will touch on actually creating these kinds of environments later on in this document.
Right now, I only want to instill the idea that its not just an editor we're talking about here.
It's *your* editor.


## Learning

If you are reading this, I guess you haven't been scared away yet,
and want to actually get into things after I've been teasing these past few sections.
I will be referring to Vim-motions, which is about the general navigation of Vim and its shortcuts.

There are three approaches I see to learning Vim-motions, in order of (opinionable) effectiveness:
1. Use a typical editor, but add a Vim plugin/extension
2. Go through Vim training modules
3. Edit simple files such as configs with Vim

Ideally, I would combine multiple if not all of these. Exposure will be the biggest driver,
even if it means starting at just a few minutes per day, and slowly building up from that.

Starting with plugins/extensions:
- Visual Studio Code ([related](https://youtu.be/aCgDs8Nv-jo), some concepts translate to other editors)
    - Vim emulation for Visual Studio Code
        - Is strictly about **emulating** Vim-motions/shortcuts
        - [Open VSX Registry](https://open-vsx.org/extension/vscodevim/vim)
        - [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim)
    - Vim mode for VSCode, powered by Neovim
        - Fully integrates with Neovim (see extension description for installation instructions)
        - [Open VSX Registry](https://open-vsx.org/extension/asvetliakov/vscode-neovim)
        - [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=asvetliakov.vscode-neovim)

Some people only want the motions in their already-preferred editor of choice, and that is entirely okay!
Once you are comfortable using it, you can be done, essentially!

Training modules:
- [vimtutor](https://linux.die.net/man/1/vimtutor) (comes with Vim)
- [vim-be-good](https://github.com/ThePrimeagen/vim-be-good) (Neovim plugin by [ThePrimeagen](https://github.com/ThePrimeagen))

Of course, some of the boring elements is reading documentation, and as tedious as it sounds there is a lot to read about:
- [Vim documentation](https://www.vim.org/docs.php) from the official [Vim organization](https://www.vim.org)
- [how2nvim](https://github.com/AlphaKeks/how2nvim) by [AlphaKeks](https://github.com/AlphaKeks)
- [Vim help.txt](https://vimhelp.org) (`:help` or `:h`)
- [Neovim help.txt](https://neo.vimhelp.org) (`:help` or `:h`)

Keep in mind those help commands! They can be used to search for help on most topics right within the editor,
such as `:h diff` to lookup help about Vim's diff feature.
Particularly `:h user-manual` provides in-depth usage information.
