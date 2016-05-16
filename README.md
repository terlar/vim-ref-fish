# vim-ref-fish

A [vim-ref](https://github.com/thinca/vim-ref) source for fish.

This is to ensure the manpage gets executed in the fish context. This
allows you to have a different shell set than fish to avoid having
conflicts in vim scripts that requires a POSIX compatible shell.

## Usage

```vim
:Ref fish test
```

### Keyword program

To use with the `K` command you can put the following in your
`~/.vim/after/ftplugin/fish.vim`:

```vim
setlocal keywordprg=:Ref\ fish
```
