# Neoterm

Simple neovim terminal plugin written in lua

# Usage

Neoterm provides both vim commands as well as a lua API

## Commands

Neoterm provides the following commands

| Command              | Description                                                                            |
| -------------------- | -------------------------------------------------------------------------------------- |
| `NeotermToggle`      | Toggle the neoterm window                                                              |
| `NeotermInteractive` | Jump to insert mode in the the neoterm window. If it doesn't exist, it will be created |
| `NeotermRun <args>`  | Run the given command in the neoterm window                                            |
| `NeotermRerun`       | Run the previous command again                                                         |
| `NeotermExit`        | Close the neoterm window and delete the terminal buffer                                |

## Lua API

The following functions are available on the neoterm module. They map directly to the commands above

```lua
local neoterm = require('neoterm')

neoterm.toggle()
neoterm.interactive()
neoterm.run('ls')
neoterm.rerun()
neoterm.exit()
```
