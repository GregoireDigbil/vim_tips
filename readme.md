Some useful vim tips and commands.

* `vi]:g/stuffIWantToDisapear/d`   - delete all lines matching a pattern in the currently selected range


* `:mksession /tmp/tmp_feature` and `:so /tmp/tmp_feature`
Vim sessions: you can save the state of all your buffer, window and register in a file
and then, source it, to reload all of it

* `G` go to end of file.
* `:r %` paste the current file after the cursor
* `:.,$v/pattern/d` delete all line without the pattern

* `:r! grep pattern %` will put the result of the grep after the cursor

* `vi}` selects what's inside the brackets
* `:'<,'>norm @c` apply macro c to the selection.
 A way to execute command as if you were in normal mode. This can be used on a selection (applied on every line of the selection) or with the global command, to apply the actions on all lines matching the given pattern

* `dt<character>` eg: `dt"` or `dt'`: delete until <character>
Similarly, see `f`, `T` and `F`, with the related move commands: `;` and `,`

* `gt/gT` - previous/next tabs int he window

