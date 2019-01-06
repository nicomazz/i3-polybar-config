
`:edit file` : open file

#### Splits
`:vsp` `:sp` : open this file also in a split

`ctrl-W _` : open current split full-screen

`ctrl-W =` : make all splits equal size

#### Spell check
`:set spell`/`:set nospell` to enable/disable

`z=` : when 'spellcheck' is on ('set spell') displays a list of correction for the actual word

#### moving around 
`#` : previous occurrence

`*` : next occurrence

`ctrl-o` `ctrl-i` : jump backward and foreword in jump list (`:jump` to see the jump list)

#### compile
`:make` : execute a make file

`:cw` : open the quickfix window (from which you can jump to compilation warning and errors)

#### vim-multiple-cursors
`ctrl-n` to create a new cursor on the next occurrence of the actual word
	- `c` to change text
	- `I` to insert at start
	- `A` to insert at end 
