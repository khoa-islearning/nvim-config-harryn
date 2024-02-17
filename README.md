# Start Guide

## Navigate the vanilla Neovim
- Use `%` to create file
- `d` to create folder
- `:Explore` to go back to file explorer


## Set up Lazy:
1. Create `init.lua`, where nvim will look for next instructions
2. Create `lua` folder
3. In `init.lua`, require the path to `core` folder. e.g. `require("harryn.core")`
4. In `lua`, create `harryn\core\` folder
5. In `core`, create file lazy.lua to bootstrap [lazy](https://github.com/folke/lazy.nvim)
6. Also create `init.lua` and require "harryn.core.lazy" to bootstrap the bootstrap file

## Setup remaps:
1. create remap.lua in core to remap leader character
2. Then we can create shortcut for commands (including plugins commands) in the plugins files

## Working with Lazy
`:Lazy` to open menu
`:Lazy load <plugin>` to load after install

## Install Plugins

- require `plugins` folder in `lazy.lua`
- add extensions in `plugins`
- after adding .lua files, remember to install and load plugins

### [nvim-tree](https://github.com/nvim-tree/nvim-tree.lua):
prereq: [nvim 0.8 or higher](https://github.com/neovim/neovim/releases)
- Extra instructions: Remember to download a [patched font](https://www.nerdfonts.com/font-downloads) and [configure](https://stackoverflow.com/questions/2054627/how-do-i-change-tab-size-in-vim) your terminal emulator to use the font.

### [editorconfig-vim](https://github.com/editorconfig/editorconfig-vim)
To manage indent size for different languages

### [which-key](https://github.com/folke/which-key.nvim)
Show which keybinding you are using

### [telescope](https://github.com/nvim-telescope/telescope.nvim)
Fast fuzzy finder

### colorscheme-picker
Easily switch between themes, fun.

### lualine, barbar 
vscode like visual, won't help much with workflow

### undotree
Show file history, not sure how useful.

### nvim treesitter
Install parser for different file type, use :TSInstall <filetype> to install parser. Treesitter parser is only for visualization.
To let nvim understand the syntax, you need LSP.

### LSP, Mason
This combo enable you to install languages server effortlessly. To summarize, LSP enable nvim to parse file and understand syntax.
These LSP must be installed outside of nvim, and each are installed differently. To overcome that complication, we can use Mason.

### trouble
use LSP to show error in your code.

### Conform
Also combo with Mason, allow nvim to format your code beautifully.

### Competitest
For competitive programming contest, which I need for school.

### Twilight, ZenMode, Pomo
For focus session.

### Obsidian, Markdown-viewer
For note taking

--TODO: add hyperlink
