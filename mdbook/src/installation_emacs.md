# Emacs

## Eglot

Markdown-oxide is just an lsp server, so you can use it with any lsp client. Here is an example of how to use it with eglot [^1716875010]

[^1716875010]: [Eglot: Setting Up LSP Servers](https://joaotavora.github.io/eglot/#Setting-Up-LSP-Servers)

```elisp
;; assumes markdown-oxide is in $PATH

(with-eval-after-load 'eglot
  (add-to-list 'eglot-server-programs
               `(markdown-mode . ,(eglot-alternatives
                                   '(("markdown-oxide"))))))
```

After setting this in `init.el` [^1716875149], run open your notes vault and run `M-x eglot`. This has been tested on [Doom Emacs](https://github.com/doomemacs/doomemacs).

[^1716875149]: This would be `~/.config/doom/config.el` for [Doom Emacs](https://github.com/doomemacs/doomemacs).


## LSP Mode

Refer to the [LSP Mode documentation](https://emacs-lsp.github.io/lsp-mode/page/adding-new-language/).
