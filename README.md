# Emacs lll-mode

For editing programs written in LLL.

Mostly by Rob Myers: https://github.com/robmyers/lll-mode


## Installation

To install the Emacs major mode, add the file `lll-mode.el` to your Emacs
load path. You can then load it by typing the following in Emacs:

```
M-x lll-mode
```

Alternatively you can have Emacs load it automatically for files with an
`.lll` extension by adding the following to your `.emacs` file:
 
``` elisp
(autoload 'lll-mode "lll-mode.el" "Major mode for editing LLL files" t)
(setq auto-mode-alist (append '(("\\.lll$" . lll-mode)) auto-mode-alist))
```

## Electric Mode

`lll-mode` works well with `electric-pair` mode from Emacs 24.1.
To enable electric pair mode either:

```
M-x electric-pair-mode
```

or add the following to your .emacs file:

``` elisp
(add-hook 'lll-mode-hook 'electric-pair-mode)
```

## License

GPLv3. See [`COPYING`](COPYING).
