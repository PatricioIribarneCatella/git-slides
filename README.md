# git-slides

_Git_ slides using **pandoc**

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
 $ pandoc -i -t revealjs -s -o FILE.html FILE.md -V revealjs-url=https://revealjs.com -V theme=$theme -V transition=$transition
```

With `$theme`:

- Black
- White
- League
- Sky
- Beige
- Simple
- Serif
- Blood
- Night
- Moon
- Solarized

and `$transition`:

- None
- Fade
- Slide
- Convex
- Concave
- Zoom

