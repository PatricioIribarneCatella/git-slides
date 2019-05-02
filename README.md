# Pandoc commands

#### Dependencies

- [pandoc](https://pandoc.org/) 

  - ```bash
    sudo apt install pandoc
    ```

- [texlive](https://tug.org/texlive/)

  - ```bash
    sudo apt install texlive
    ```

- latex-engine

  - ```bash
    sudo apt install xelatex pdflatex
    ```

### PDF file

```bash
 $ pandoc FILE.md -o FILE.pdf
```

### PDF slides

```bash
 $ pandoc FILE.md -t beamer -o FILE.pdf
```

### HTML slides

```bash
 $ pandoc FILE.md -s -t dzslides -o FILE.html
```

