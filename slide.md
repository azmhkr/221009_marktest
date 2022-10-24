---
header-includes:
    - \setmainfont{Hiragino Mincho ProN}
    - \setsansfont{Hiragino Maru Gothic ProN}
    # - \setmonofont{Osaka}
    - \setmonofont{Cica}

title: Pandoc & Markdownでスライド作成
author: azmhkr
---

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

# 見出しで次のページ

:::::: {.columns}
::: {.column width="33%"}
このように，段組みもでき
ます．
:::
::: {.column width="33%"}
数式も，
$$
e^{i\pi} = -1
$$
書けます．
:::
::: {.column width="33%"}
改行は自動ではされませんので，書きすぎると見切れます．
．
:::
::::::

# 画像の挿入
このように，サイズを指定して図を挿入できます．
<div style="piyopiyo">
![](figure.png){width=1.5cm}
</div>
代替テキストを書くとキャプションになります．
<div style="hogehoge">
![キャプション](figure.png){width=3cm}
</div>
