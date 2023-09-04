# Pandoc Markdown Syntax

[VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=garlicbreadcleric.pandoc-markdown-syntax) |
[Open VSX](https://open-vsx.org/extension/garlicbreadcleric/pandoc-markdown-syntax) |
[GitHub](https://github.com/garlicbreadcleric/vscode-pandoc-markdown)

Standard VSCode Markdown syntax with some modifications to support Pandoc Markdown extensions:

- [Citations](https://pandoc.org/MANUAL.html#extension-citations): `@citationKey`, `@{citationKey}`, `[see @citationKey1 p. 42; citationKey2 p. 24]`
- [Fenced divs](https://pandoc.org/MANUAL.html#extension-fenced_divs):

  ```markdown
  ::: {.float-right}
  ![figure 1](./figure1.png)
  :::
  ```
- [Bracketed spans](https://pandoc.org/MANUAL.html#extension-bracketed_spans): `[foo]{.mark}`

## Caveats

- Instead of injecting into the builtin Markdown grammar, this extension overrides it completely (even though the grammar is still mostly the same as the one built into VSCode, with a few tweaks). The reason for this is that I also use these grammar definitions for parsing Markdown in [Markane](https://github.com/garlicbreadcleric/markane) language server via [vscode-textmate](https://github.com/microsoft/vscode-textmate) library, and vscode-textmate doesn't support language injections.

## See also

- [Document Preview](https://github.com/garlicbreadcleric/vscode-document-preview) VSCode extension for previewing Markdown via Pandoc
- Markane ([language server](https://github.com/garlicbreadcleric/markane) and [VSCode extension](https://github.com/garlicbreadcleric/vscode-markane)) for templates, snippets, completion, citations and more
