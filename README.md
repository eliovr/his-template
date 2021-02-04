This is a (more or less) mended version of the official Latex template found [here](https://www.his.se/forskning/utbildning-pa-forskarniva/avhandlingsmallar/).

## Requirements
- [TexLive](https://tug.org/texlive/).

## Useful commands
- Compile to pdf (using [latexmk](https://mg.readthedocs.io/latexmk.html)):
```bash
latexmk -pdflatex=lualatex -pdf example-thesis.tex
```
- Clean (delete some of the auxiliary files):
```bash
latexmk -c
```
- Make glossary (or this one you need to first compile, make the glossary, and then compile again):
```bash
makeglossaries example-thesis
```

- Install Microsoft fonts (if in Linux):
```bash
sudo apt install ttf-mscorefonts-installer
```
