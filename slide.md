---
header-includes:
    # フォントは任意で変更可
    - \setmainfont{Hiragino Mincho ProN}
    - \setsansfont{Hiragino Maru Gothic ProN}
    - \setmonofont{Osaka}

title: Pandoc & Markdownでスライド作成
---

# コードブロックと数式
詳細はpandocドキュメントを参照：https://pandoc.org/MANUAL.html

コードブロックが作れます．
```
pandoc slide.md -o slide.pdf -t beamer -V theme:metropolis --pdf-engine=xelatex
```
数式も書けます．
$$
e^{i\pi} = -1
$$

# 段組み

:::::: {.columns}
::: {.column width="33%"}
このように，段組みもでき
ます．
:::
::: {.column width="33%"}
- じゃがいも
- にんじん
- ぶたにく
- ばなな
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
