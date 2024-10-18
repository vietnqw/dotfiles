# Installation

- Neovim: `sudo snap install nvim --classic`
- lazygit: <https://github.com/jesseduffield/lazygit>
- ripgrep: <https://github.com/BurntSushi/ripgrep>
- fd: <https://github.com/sharkdp/fd>
- Starter template for LazyVim:
  - `git clone https://github.com/LazyVim/starter ~/.config/nvim`
  - `rm -rf ~/.config/nvim/.git`

# Plugin manager

- Access
  - From dashboard: `l`
  - From Normal mode: <leader> + `l`
  - To perform sync (install, clean, and update at the same time, usually when "Plugin Updates" notification poped up): Shift + `s`
- Exit: `q`
- `Neo-tree.nvim` plugin:
  - Turn on side-bar: <leader> + `e` (root dir)  or  <leader> + `E` (cwd)
  - Create new file (eg: `filename`) or folder (eg: `dir/`): `a`
  - Rename file/folder: `r`
  - Cut a file/folder: `x`
  - Copy a file/folder: `y`
  - Paste a file/folder: `p`
  - Navigate up directory: <backspace>
  - Set the directory to be root: `.`
- **LazyExtras**:
  - Open with: `:` + `LazyExtras`   or   `:` + `Dashboard` + `x`
  - It is recommended to install all packages named: `lang.*` for any languages you're using
  - Language Extras such as `venv-selector.nvim`:
    - <leader> + `c` + `s`
- `Mason.nvim`
  - Database of programming language support tooling, including: language servers, formatters, linters
  - Open Mason: `:` + `Mason`   or   <leader> + `c` + `m`
- Open the LazyVim configuration directory (`$HOME/.config/nvim/`): `c` (at the Dashboard)   or   <leader> + `f` + `c`
- LazyVim will first load the `init.lua` by default, and any Lua file under `lua/plugins/` subdirectory.
  - You can create a file `lua/plugins/disabled.lua` to disable all plugins that are loaded by default by LazyVim.

# Getting help

- In Normal mode: `:help`

# General commands

- Quit LazyVim: <leader> q q
- See cwd: `:` + `pwd`
- Change cwd: `:` + `cd`
- Change cwd locally (for current window only): `:lcd`
- Use Telescope picker:
  - Find file (with fuzzy search):
    - Keywords to search are separated by spaces
    - Open search: <leader> + <leader>
    - Jump to a search result with Seek: `s`

# Navigating

- Navigate n steps: <n> + h/j/k/l
- Jump by n words: <n> + w/b/e
  - Words separated by punctuations: w/b/e
  - Words separated by spaces: Shift + w/b/e
- Go inline:
  - Beginning of the line: `0`
  - Beginning of the line (first non-whitespace): `^`
  - The end of the line: `$`
- Go to line:
  - nth line: `:` + n
  - The nth line before: `:` + -n
  - The nth line after: `:` + +n
  - First line of the file: `g` + `g`
  - Last line of the file: Shift + `g`
- Jump history:
  - Jump backward in history: Ctrl + `o`
  - Jump forward in history: Ctrl + `i`

# Modal editing

- Insert at the beginning of line: Shift + `i`
- Append at the end of line: Shift + `a`
- Go to:
  - Previous editing location: `g` + `i`
  - The path under the cursor: `g` + `f`
- Scrolling:
  - Up 1 line: Ctrl + `y`
  - Down 1 line: Ctrl + `e`
  - Up 1/2 page: Ctrl + `u`
  - Down 1/2 page: Ctrl + `d`
  - Up n page: <n> + Ctrl + `b`
  - Down n page: <n> + Ctrl + `f`
- Find:
  - Find text with plugin (`flash.nvim`): `s` + <type_the_text>, then type the key masked with the position you want to move to
- Replace:
  - 1 character at current cursor: `r` + <character_to_replace>

## Command mode

- Enter this mode with: Shift + `;` --> `:`
- Tab completion: Use `Tab` and Shift + `Tab` to select different entries
- Open a file/directory: `e`
- To choose an option at current cursor (navigating with `Tab`): `Down` arrow key / Ctrl + `y`

## Z mode

- Bring the current cursor to the top of screen: `z` + `t`
- Bring the current cursor to the middle of screen: `z` + `z`
- Bring the current cursor to the bottom of screen: `z` + `b`
