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
- Make glossary (for this one you need to first compile, call the command below, and then compile again):
```bash
makeglossaries example-thesis
```

- Install Microsoft fonts (if in Linux):
```bash
sudo apt install ttf-mscorefonts-installer
```

- Install TexLive packages:
```bash
tlmgr install <package name>
```

## Notes

- Remove the extra margins and the cutting marks by adding `final` to the document class options:
```latex
\documentclass[english,final]{his-thesis}
```

- Change the colors of the pages separating parts in `hismetadata.sty`.
