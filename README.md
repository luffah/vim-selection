# vim selection : get visual selection text

Library to retrieve the selected text from visual mode (v, V, square).

```vim
" to get numerical details of the selection from statusline
set statusline+=%{selection#Status()}

" from anywhere, get the selected text
echo selection#getSelectedText()

" while in visual mode (limited use) return the text selected or under cursor
echo selection#vgetSelectedText()

```
I
# Example installation
```sh
mkdir -p ~/.vim/pack/ui/start/
cd ~/.vim/pack/ui/start

wget https://github.com/luffah/vim-selection/heads/main.zip
unzip main.zip
```

```vim
" init.vim
packloadall

set statusline+=%{selection#Status()}
```

License GPLv3.
