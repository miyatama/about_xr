# Grimoire

+ サイズ: A5(148 × 210 ミリ)
+ ページの白: `#e7e2df`
+ ページの画像サイズ: 1024 x 1448
+ ベースの文字色: `#1e1d1c`

設定

+ 特別仮想空間防衛隊2課
  + 特仮隊
  + 特仮隊2課
+ 指南魔導書
+ 重要区分指定
+ 特仮隊2課行使魔道要綱
+ 章
  + 第1項: 索敵
    + 同一空間ノ遠距離索敵: 仮想空間ノ最大距離ヲ4分ノ1毎に分割シウル空間中点ニ拠点ヲ取リ、各拠点間ノ三点範囲内ヲ索敵ス
    + 三点範囲ノ索敵: 自身又ハ拠点ノ衝突反応ヲ以て是ヲ対象物有ト見做ス
    + 敵仮想個性体認識: 情報対交信二依リ敵性反応ト見做ス
    + 仮想空間内背景同化: 自身仮想個性体に情報記述を投入し敵仮想個性体からの検出を困難とす
  + 第2項: 攻勢
    + 膨大情報記述負荷攻撃: 敵仮想個性体に情報記述を投入し高負荷状態への遷移を促す
    + 仮想背景射影化: 仮想空間地形への情報記述を投入し敵仮想個性体資格への混乱を促す

```text
本誌目的: 仮想空間二於ケル索敵・攻勢・防衛ノ手段ヲ以テ敵ヲ制圧スル
```

```rust
use virtdefence::{
    ally::{search_ally, gen_token, refresh_token},
    call::{send_token, recv_token},
};

fn main() {
    let ally = search_ally();
    let token = gen_token();
    let ally_signals = search_ally
        .iter()
        .map(|ally| ally.signal)
        .collect::<Vec<_>>();
    for i in 0..ally_signals.len() {
        let signal = ally_signals.get(i);
        send_token(signal, token);
    }
    // do reciv
}
```

| file | description |
| :----- | :----- |
| grimoire1.blend ||
| grimoire2.blend ||
| grimoire3.blend | 表紙、本身、各ページ + 本を開くアニメーション |
| grimoire4.blend | 外観調整(マテリアル等) + 本身修正 |


参考サイト

+ [Flipping Pages: Animation In Blender | Easy Step By Step Tutorial | Books | Magazines | Diaries etc.](https://youtu.be/ijRabIP8GnA?si=WzjXNqFs5Id69RGn)