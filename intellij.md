# Useful intellij features I discovered with time

### Remote command execution

You can configure a command to be executed on a remote server when you press a shortcut.
Sure, you can also run a local script that does the same.
Little tip: if you want file links in your workspace, even if remote files have another path (another prefix), just use sed.
Example:
go to `Edit configuration` -> `Before launch` -> `+` -> `Remote tool` to configure what to execute and where.
If, in the output, you have files paths, like `/your/remote/path/file.c`, but in your local system it is at `/your/local/path/file.c`, you can pipe the output of the command to somwthing like `sed -e 's/remote\/path/\/carlazz\/Projects/'` to replace.

### Bookmarks and favourite file list

- `ctrl+shift+ 0-9` to add a new bookmark
- `ctrl+ 0-9` to jump to that bookmark
- `Alt+shift+f` to add a file to a favourite list
