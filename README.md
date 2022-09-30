# Zshell autocompletions

## Setup

Create somewhere to place completion functions, eg `~/.zcomp`

On shell start, amend fpath and call `compinit`:

    if autoload compinit; then
      fpath+=(~/.zcomp)
      compinit -C
    fi

Note the use of `-C` to read cache instead of lengthy scanning

## Add a new completion

Place file in `~/.zcomp`

Note that file name must start with underscore

## Refresh a completion

Do a full `compinit` initialisation

Occassionally, you will to manually delete local cache in `~/.zcompdump`

## Reference

- A User's Guide to the Z-Shell, chapter 6: Completion, old and new

- The Z Shell Manual (SourceForge), chapter 20: Completion System

- Zsh Community Projects (GitHub), zsh-completions guide

- standard completers in /usr/share
