# Session handling
- List all sessions: tmux ls
- Create new session: tmux new -s <session name>
- Rename existing session: tmux rename-session -t <current name> <new name>
- Re-connect to a session: tmux attach -t <session name>

# Window handling
- Create new window: <prefix> + c
- Move between windows: Alt + h/l
- Move to specific window: <prefix> + <window number>

# Pane handling
- Create new pane: 
    <prefix> + \ 
    <prefix> + -
- Delete current pane: Ctrl + d
- Move between panes: Ctrl + h/j/k/l

# Copy inside the terminal:
1. Now you can enter copy mode normally with <prefix> + [.
2. Navigate the copy mode with vi-like-key bindings
3. Hit v to start copying.
4. Press y or Enter to copy the text into the tmux buffer. This automatically cancels copy mode.
5. Paste into the buffer with <prefix> + P (make sure that it’s uppercase P).
