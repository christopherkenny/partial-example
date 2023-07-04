# Short Example of Quarto Partials

To add a page break before (and optionally after) a Table of Contents

1. For an existing document with `format: pdf` and a table of contents, update the YAML to:

```yaml
format: 
  pdf: 
    toc: true
    template-partials: 
      - toc.tex
```

2. Create a file `toc.tex` with the contents of the Quarto default file `toc.tex`, available on [GitHub](https://github.com/quarto-dev/quarto-cli/blob/main/src/resources/formats/pdf/pandoc/toc.tex).

3. Add a `\newpage` to the start of `toc.tex`. (You can do the same to the bottom of the file to put a page break before and after the ToC.)
