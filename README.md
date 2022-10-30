## Requirements

- Tex Live 2022 or newer
- pandoc 2.19.2 or newr

## Getting started
markdownファイル（slide.md）からbeamerスライド（slide.pdf）を作成するコマンドは，
```
pandoc slide.md -o slide.pdf -t beamer -V theme:metropolis --pdf-engine=xelatex
```
日本語を使わないなら以下で良い．
```
pandoc slide.md -o slide.pdf -t beamer -V theme:metropolis
```
