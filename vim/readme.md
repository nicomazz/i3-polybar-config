
`:edit file` : open file

#### Splits
`:vsp` `:sp` : open this file also in a split

`ctrl-W _` : open current split full-screen

`ctrl-W =` : make all splits equal size

#### Folding
`zM` to increase foldlevel at max (fold everything) (z More)
`zm` to increase foldlevel by one
`zR` to unfold everything
`zr` to reduce foldlevel by one
`zo` open current fold
`zc` close current fold
`zi` enable/disable folding
`za` toggle a fold (mapped to <s-Tab>)

#### Spell check
`:set spell`/`:set nospell` to enable/disable

`z=` : when 'spellcheck' is on ('set spell') displays a list of correction for the actual word

#### Moving around 
`#` : previous occurrence

`*` : next occurrence

`ctrl-o` `ctrl-i` : jump backward and foreword in jump list (`:jump` to see the jump list)

#### Edit
`C` delete until the end of the line and enter in insert mode

#### Compile
`:make` : execute a make file

`:cw` : open the quickfix window (from which you can jump to compilation warning and errors)

#### Search
`:set hlsearch` to hilight the last search

#### vim-multiple-cursors (plugin)
`ctrl-n` to create a new cursor on the next occurrence of the actual word
	- `c` to change text
	- `I` to insert at start
	- `A` to insert at end 
