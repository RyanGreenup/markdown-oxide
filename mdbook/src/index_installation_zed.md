# Zed

> [!Note]
> Zed does not implement some of the language server protocol that this LS uses. Namely, unindexed block completions do not work at all. There are also other issues with the language server unique to Zed (such as completions being unexpectedly hidden). Over time, these issues will be resolved; for now, Zed provides an interesting exhibition for a potential (beautiful + fast) note-taking experience provided by markdown oxide

Markdown Oxide is available as an extension titled `Markdown Oxide`. Similarly to VSCode, there are two methods for this extension to access the language server
1. Recommended: the extension will download the server's binary and use that
2. The extension will use `markdown-oxide` from path. To install to your path, there are the following methods for Zed:

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


