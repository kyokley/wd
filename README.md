warp
====

Warp lets jump to custom directories in zsh, without using cd. Why? Because cd seems ineffecient when the folder is for example frequently visited.

### Setup

Add `wd` alias (warp directory) to `.zshrc``:

    echo "alias wd='. /path/to/warp'" >> ~/.profile


### Usage

Add warp point to current working directory:

    wd add dev

If a previous warp point exists, use `add!` to overwrite it.

From other directory, warp to dev with:

    wd dev

Remove warp point dev point:

    wd rm dev

List all warp points (stored in `~/.warprc`):

    wd ls

Print usage with no opts.
