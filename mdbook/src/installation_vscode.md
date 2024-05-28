# VSCode

Install the [vscode extension](https://marketplace.visualstudio.com/items?itemName=FelixZeller.markdown-oxide) (called `Markdown Oxide`). As for how the extension uses uses the language server, there are two options
1. Recommended: the extension will download the server's binary and use that
2. The extension will use `markdown-oxide` from path. To install to your path, there are the following methods for VSCode:

    - <details>
         <summary>Cargo Install (from source)</summary>

        ```bash
        cargo install --locked --git https://github.com/Feel-ix-343/markdown-oxide.git markdown-oxide
        ```

    </details>

    - <details>
         <summary>Cargo binstall[1] (from hosted binary)</summary>

        ```bash
        cargo binstall --git 'https://github.com/feel-ix-343/markdown-oxide' markdown-oxide
        ```

    </details>

    - <details>
         <summary>AUR (from source)</summary>

        ```bash
        paru -S markdown-oxide-git
        ```

        ```bash
        yay -S markdown-oxide-git
        ```

    </details>

    - Nix Unstable: `pkgs.markdown-oxide`
