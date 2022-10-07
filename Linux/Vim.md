# ⌨️Vim

## What to study - resources I find helpful📚

Vim 

- [上古神器Vim：从恶言相向到爱不释手 - 终极Vim教程01](https://www.bilibili.com/video/BV164411P7tw?spm_id_from=333.999.0.0&vd_source=feba2df2be8d73a9f79885dece576693)
- [上古神器Vim：进阶使用/配置、必备插件介绍 - 终极Vim教程02](https://www.bilibili.com/video/BV1e4411V7AA?spm_id_from=333.999.0.0&vd_source=feba2df2be8d73a9f79885dece576693)
- [「妈妈不会告诉你的Vim技巧」 -Vim终极教程03](https://www.bilibili.com/video/BV1r4411G7de?spm_id_from=333.999.0.0&vd_source=feba2df2be8d73a9f79885dece576693)
- [Vim Tutorial for Beginners](https://www.youtube.com/watch?v=RZ4p-saaQkc)
- [Vim Tutorial](https://www.youtube.com/watch?v=IiwGbcd8S7I)
- [Editors (Vim)](https://missing.csail.mit.edu/2020/editors/)

Neo Vim

- [Neovim from Scratch](https://www.youtube.com/playlist?list=PLhoH5vyxr6Qq41NFL4GvhFp-WLd5xzIzZ)
- [21世纪最强代码编辑器：NeoVim](https://www.bilibili.com/video/BV1y4411C7pE?spm_id_from=333.999.0.0&vd_source=feba2df2be8d73a9f79885dece576693)
- [让你的vim像vscode一样强大](https://www.bilibili.com/video/BV1Ka4y1E7AM?spm_id_from=333.999.0.0&vd_source=feba2df2be8d73a9f79885dece576693)

Others' config

- https://github.com/jonhoo/configs/blob/master/editor/.config/nvim/init.vim
- https://github.com/anishathalye/dotfiles/blob/master/vimrc
- https://github.com/JJGO/dotfiles/blob/master/vim/.vimrc
- https://github.com/theniceboy/nvim
- https://gist.github.com/benawad/b768f5a5bbd92c8baabd363b7e79786f
- https://github.com/craftzdog/dotfiles-public
- https://github.com/NeuralNine/config-files/blob/master/init.vim

## Project  - what I do to study the topic⌨️



## Study Note ✍️

- [Fundamental](#Fundamental)

- [Config](#Config)

## Fundamental

### Modal editing

- **Normal**: for moving around a file and making edits
- **Insert**: for inserting text
- **Replace**: for replacing text
- **Visual** (plain, line, or block): for selecting blocks of text
- **Command-line**: for running a command

### Command-line

- `:q` quit (close window)
- `:w` save (“write”)
- `:wq` save and quit
- `:e {name of file}` open file for editing
- `:ls` show open buffers
- `:help {topic}` open help

### Movement

- Basic movement: `hjkl` (left, down, up, right)
- Words: `w` (next word), `b` (beginning of word), `e` (end of word)
- Lines: `0` (beginning of line), `^` (first non-blank character), `$` (end of line)
- Screen: `H` (top of screen), `M` (middle of screen), `L` (bottom of screen)
- Scroll: `Ctrl-u` (up), `Ctrl-d` (down)
- File: `gg` (beginning of file), `G` (end of file)
- Line numbers: `:{number}<CR>` or `{number}G` (line {number})
- Misc: `%` (corresponding item)
- Find: `f{character}`, `t{character}`, `F{character}`, `T{character}`
- Search: `/{regex}`, `n` / `N` for navigating matches

### Selection

- Visual: `v`
- Visual Line: `V`
- Visual Block: `Ctrl-v`

### Edit

- `i` enter Insert mode
- `o` / `O` insert line below / above
- `d{motion}` delete {motion}
  - e.g. `dw` is delete word, `d$` is delete to end of line, `d0` is delete to beginning of line
- `c{motion}` change {motion}
  - e.g. `cw` is change word
- `x` delete character (equal do `dl`)
- `s` substitute character (equal to `cl`)
- `u` to undo, `<C-r>` to redo
- `y` to copy / “yank” (some other commands like `d` also copy)
- `p` to paste

## Config

### Vimrc

- Vim is customized through a plain-text configuration file in `~/.vimrc`

### Plugins

- Coc
- Fzf
- Nerdtree