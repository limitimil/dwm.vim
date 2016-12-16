# dwm.vim : Tiled Window Management for Vim

dwm.vim adds tiled window management capabilities to Vim. It is highly inspired by [dwm](http://dwm.suckless.org/) (Dynamic Window Manager) tiled layout management.

Windows are always organised as follows:

```
===================================
|              |        S1        |
|              |===================
|      M       |        S2        |
|              |===================
|              |        S3        |
===================================
```

## Use

Use the following shortcuts and commands to create, browse and close windows:

- `C-N`, `:New` Creates a new window and place it in the master pane [M] & stacks all previous windows in the stacked pane [S].
- `C-P`, `:Split ` Open all files provided as argument. The last file is added to [M] and all existing and new windows are stacked in [S].
- `C-C` Close the current window if no unsaved changes.
- `C-J` Jumps to next window (clockwise).
- `C-K` Jumps to previous window (anti-clockwise).
- `C-Space` Focus the current window, that is, place it in the master pane [M] & stacks all other windows in the stacked pane [S].

## Installation

Install to `~/.vim/plugin/dwm.vim`.

Or, if you use Vundle, add the following line to your `.vimrc`

```
Bundle 'raphael-proust/dwm.vim'
```


### Options

- `g:dwm_map_keys`: if set to a falsey value, prevents key mapping.
- `g:dwm_make_commands`: if set to a falsey value, prevents commands creation.
- `g:dwm_master_pane_width`: set the width of the master pane (e.g., `g:dwm_master_pane_width=85`)

To use a mouse to select windows and resize panes:
- `set mouse=a`: enable the use of the mouse in all modes
- `set ttymouse=xterm2`: recognize mouse codes for the xterm2 terminal type


### Contributors

```
@dsapala (Dan Sapala)
@rhacker
@matze (Matthias Vogelgesang)
@mitnk
@tony (Tony Narlock)
@lmarburger (Larry Marburger)
@afriggeri (Adrien)
@n4kz (Alexander Nazarov)
```

