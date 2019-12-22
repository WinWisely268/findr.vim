# Findr.vim
An incremental file finder for neovim, inspired by [ivy](https://github.com/abo-abo/swiper) find-file
![Screenshot](screenshots/findr.gif)

## Requirements
* `nvim`: version > 0.4.0
* macos/linux

## Instalation
Using [vim-plug](https://github.com/junegunn/vim-plug):
```vim
Plug 'conweller/findr.vim'
```

## Usage
Launch with the command `:Findr`

Inside a findr buffer, filter subdirectories/files by entering in the desired
pattern

You can delimit multiple patterns you are searching for with a space.

The first matching file is selected by default, you can select a different
file using `<c-p>` (or `<up>` or  `<c-k>`) for the previous file, or `<c-n>`
(or `<down>` or  `<c-j>`) for the next file

Use `<cr>` to edit a file

Use `<tab>`, `/`, or `<c-l>` to change to the selected directory

Use `<c-h>` or use `<bs>` when the cursor is right of the prompt to got the
parent directory

## Configuration
Disable border around floating window (default 1):
```vim
let g:findr_enable_border = 0
```

For additional documentation see:
```vim
:h findr
```

## TODO
* Configuration
