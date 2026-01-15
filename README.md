# dotfiles-tmux

My tmux configuration.

## Features

- Mouse support enabled
- Pane border at top showing: pane title, git repo:branch, current path
- Status bar at bottom with window list and time
- Auto-renumber windows when closed

## Installation

```bash
git clone https://github.com/matowang/dotfiles-tmux ~/Code/dotfiles-tmux
ln -sf ~/Code/dotfiles-tmux/.tmux.conf ~/.tmux.conf
tmux source ~/.tmux.conf
```

## Ghostty Setup

For proper color and terminal support with Ghostty, add to your Ghostty config (`~/.config/ghostty/config`):

```
term = xterm-256color
```

This ensures tmux receives correct terminal capabilities.

## Requirements

- tmux 3.0+
- git (for branch/repo display in pane border)
