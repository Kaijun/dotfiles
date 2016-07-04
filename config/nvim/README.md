# neovim

My configuration file for Neovim. No deep shit.

I use Vim-Plug as my plugin manager.

## How to use

```
git clone https://github.com/shenchsh/neovim.git ~/.config/nvim
nvim ~/.config/nvim/init.vim
```

use `:PlugInstall` to install all plugins.

## Plugins

* Theme: [gruvbox](https://github.com/morhetz/gruvbox)
* [CtrlP](https://github.com/kien/ctrlp.vim)
* [Nerdtree](https://github.com/scrooloose/nerdtree)
* [Goyo](https://github.com/junegunn/goyo.vim)
* [Airline](https://github.com/vim-airline/vim-airline)(better with [powerline fonts](https://github.com/powerline/fonts))
* [Gitgutter](https://github.com/airblade/vim-gitgutter)
* [Tagbar](https://github.com/majutsushi/tagbar)([Exuberant Ctags](http://ctags.sourceforge.net) required)
* [Bufexplorer](https://github.com/jlanzarotta/bufexplorer)
* [Syntastic](https://github.com/scrooloose/syntastic)

## Shortcuts

```
map <leader>tn :tabnew<cr>
map <leader>be :BufExplorer<cr>
map <leader>nt :NERDTreeToggle<cr>
map <leader>tb :TagbarToggle<cr> 
map <leader>gy :Goyo<cr> 
let g:ctrlp_map='<c-f>'
```

For shortcuts details, please refer to init.vim.

## Tips

1. Should be fine on Mac OS and Linux.
2. If you are a Linux user, you may encounter "No clipboard tool available" warning, please use `apt-get install xsel` to install [xsel](http://www.vergenet.net/~conrad/software/xsel/). 
3. If your airline doesn't look like what you want, please change the terminal font to a certain powerline font. **It is highly recommended.**
4. When using tmux with Neovim, it may have slightly delay when you change from insert mode to normal mode, just add `set -sg escape-time 0` to `~/.tmux.conf`

## Reference

For detailed introduction to Neovim installation. Please refer to:
[Neovim official website](https://neovim.io)

For Neovim installation: [Installing Neovim](https://github.com/neovim/neovim/wiki/Installing-Neovim)
