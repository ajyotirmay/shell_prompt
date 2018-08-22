# shell_prompt
This project provides a set of functions for shells (tested with BASH and ZSH) to modify their functionality without affecting the performance

## Why to use it over oh-my-zsh
'oh-my-zsh' can slow down zsh shell. I didn't like the lag that oh-my-zsh caused to the shell, but I liked how it can show when you are in a directory that's a git repo. I wanted the similar behaviour - natively - without depending on python or something similar.

The benefit of using this over oh-my-zsh is that you can have the same behaviour for BASH too.

## How to use this project?
It's very simple:
1. Download the the file on your system
2. Open your `.bashrc` or `.zshrc` (depending on the shell you use) and add the line `source ~/shell_prompt`. Be sure to give the full path for this file, or you'll find a weird behaviour.
3. Just add the functions from the file that you want to use. For example, if you want a git branch information on your prompt, just add `$(git_prompt)` to your `PS1` (for BASH), `PROMPT` or `RPROMPT` (for ZSH) shell variable.

You can use any other function the same way, just call the function from the file and it will work.
