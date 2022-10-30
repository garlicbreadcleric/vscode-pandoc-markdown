# Pandoc Markdown Syntax

![](./icon.png)

Standard VSCode Markdown syntax with some modifications to support Pandoc Markdown extensions:

- Citations: `@citationKey`, `@{citationKey}`, `[see @citationKey1 p. 42; citationKey2 p. 24]`
- Fenced divs:

  ```markdown
  ::: {.float-right}
  ![figure 1](./figure1.png)
  :::
  ```
- Fenced spans: `[foo]{.mark}`
