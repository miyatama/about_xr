# about_xr

xr関連の色々なものを置く場所

# 技術メモ

## ちょろいやつ

| やること | 操作 |
| :----- | :----- |
| オブジェクトを結合する | `Ctrl + J` |
| サブディビジョンサーフェイス追加 | `Ctrl + 2` |
| 回転リセット | `Alt + R` |
| loop tools導入 | 4.2はエクステンションから追加 |
| マテリアルリンクショートカット | `Crrl + L` |
| モディファイア適用 | モディファイア上で`Crrl + A` |
| 選択中のメッシュ以外非表示 | オブジェクトを選択して`Shift + H`。表示は`Alt + H` |

## メッシュに関する情報

+ 球体の面分割は4の倍数
+ ベベルに関しては奇数差し込み

## UV展開に関する情報


 + [【完全版】blender初心者はコレさえ見ればUV展開できます【お題：フグ】](https://youtu.be/mFJNdIKApPc?si=1c74L4tA2yzt3NAO)

## テクスチャに関する情報源

| 種類 | 概要 |
| :----- | :----- |
| デュフューズマップ | 色や模様をつける |
| ラフネスマップ | 画像の粗さをつける。色空間に注意 |
| ノーマルマップ | 凹凸をつける。RGBがXYZとして保存される。 |
| ディスプレイスメントマップ | モデルを変形させるマップ。画像の濃淡が高さに変換される。 |

Node Wranglerの`Ctrl + Shift + T`で一括ノード追加

![texture_01](./img/texture_01.png)

+ [実は簡単！テクスチャでリアルな質感を作る方法【Blender】](https://youtu.be/K1MMnQjvzZ8?si=0IOpBbRIHsu0aba3)

## SVG取り込み & 実体化

[IllustratorのパスをBlenderで立体化する](https://styly.cc/ja/tips/jp-illustrator-to-blender/)

## プレーンを貼り付ける

Modifier -> Shrinkwrapを利用する。

![shrinkwrap](./img/modifier_shrinkwrap.png)

[【Blenderチュートリアル】ステッカーの貼り方 曲面、球、角にも対応！](https://youtu.be/PG7zuOHJUS4?si=RKcdE839pjp0JSsL)

## ループ同士に面を張る

Ctrl + E -> Bridge Edge Loop

![bridge_edge_loop](./img/bridge_edge_loop.png)


