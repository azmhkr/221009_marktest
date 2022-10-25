pandocを使ってMarkdownからbeamerスライドを作るためのテンプレート
# 環境

- Mac OS Monterey 12.6
- Tex Live 2022
- pandoc 2.19.2

Markdownをbeamerスライドに変換するコマンドは，
```
pandoc slide.md -o slide.pdf -t beamer -V theme:metropolis --pdf-engine=xelatex
```
日本語を使わないなら，
```
pandoc slide.md -o slide.pdf -t beamer -V theme:metropolis
```
