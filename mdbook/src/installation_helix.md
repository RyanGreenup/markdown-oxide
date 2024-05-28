# Helix

For Helix, all you must do is install the language server's binary to your path. The following installation methods are available:
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


> [!Note]
> There are some major issues with markdown oxide on helix as it does not fully implement the language server protocol. Most obtrusive is that helix does not implement `is_incomplete` for completions, and since completion filtering and sorting happens on the server (for performance), you must manually re-request completions after typing (one method I have found is to exit and re-enter insert mode)
