# newcode
The perfect code editor--not. It's a script to install my Neovim configuration on Linux.

My vim configuration can be found [here](https://github.com/elfry2/code).

![A screenshot of the latest version](screenshots/Screenshot%20from%202023-12-21%2003-11-51.png "A screenshot of the latest version")

## Installation
Be aware that installing newcode overwrites your current ```~/.config/nvim/init.vim```. To install newcode, execute 
```bash
git clone https://github.com/elfry2/newcode.git && cd newcode && ./main
```
The installation may take some time due to downloads, so you may want to skip them later after successfully running them once by appending ```--no-download```.

## Usage
Execute
```bash
nvim
```

To learn vim basics, read [this article](https://www.linuxfoundation.org/blog/blog/classic-sysadmin-vim-101-a-beginners-guide-to-vim).

To learn how to use plugins, read [this StackOverflow answer](https://stackoverflow.com/a/55846872).

## Configuration
Plugins are to be managed using [vim-plug](https://github.com/junegunn/vim-plug) and registered in ```~/.config/nvim/newcode/plugs.vim```. Configuration for plugins are to be placed in ```~.config/nvim/newcode/plugin-config.vim```. Configuration for built-in features are to be placed in ```~/.config/nvim/newcode/builtin-config.vim```.

## Remaps 
- ```<ESC>``` -> ```jk``` in insert and visual mode
- Toggle Neo-tree -> ```tr``` in normal mode. Other Neo-tree mappings can be read on [its documentation](https://github.com/nvim-neo-tree/neo-tree.nvim/blob/main/doc/neo-tree.txt)
- Expand snippets -> ```Ctrl``` + ```j```

## Troubleshooting
- **Lualine arrows not showing, only rectangles; missing icons, etc.** The script has installed Hack Nerd Font Mono on your system. Configure your terminal to use it or another nerd font of your choice.
