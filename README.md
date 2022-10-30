# Pandoc Markdown Syntax

![](./icon.png)

[VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=garlicbreadcleric.pandoc-markdown-syntax) |
[Open VSX](https://open-vsx.org/extension/garlicbreadcleric/pandoc-markdown-syntax) |
[GitHub](https://github.com/garlicbreadcleric/vscode-pandoc-markdown)

Standard VSCode Markdown syntax with some modifications to support Pandoc Markdown extensions:

- Citations: `@citationKey`, `@{citationKey}`, `[see @citationKey1 p. 42; citationKey2 p. 24]`
- Fenced divs:

  ```markdown
  ::: {.float-right}
  ![figure 1](./figure1.png)
  :::
  ```
- Fenced spans: `[foo]{.mark}`
