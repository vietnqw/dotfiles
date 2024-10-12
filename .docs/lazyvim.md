# Installation
- Neovim: `sudo snap install nvim --classic`
- lazygit: https://github.com/jesseduffield/lazygit
- ripgrep: https://github.com/BurntSushi/ripgrep
- fd: https://github.com/sharkdp/fd
- Starter template for LazyVim: 
  - `git clone https://github.com/LazyVim/starter ~/.config/nvim`
  - `rm -rf ~/.config/nvim/.git`

# Plugin manager
- Access
  - From dashboard: `l`
  - From Normal mode: <leader> + `l`
  - To perform sync (install, clean, and update at the same time, usually when "Plugin Updates" notification poped up): Shift + `s`
- Exit: `q`

# Getting help
- In Normal mode: `:help`

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
