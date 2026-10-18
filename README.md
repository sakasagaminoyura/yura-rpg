# 逆髪の結羅

ブラウザで遊べるファンゲーム（個人用）。

- トップ（ゲーム選択）: https://sakasagaminoyura.github.io/yura-rpg/
- RPG「逆髪の結羅 〜鬼の美少女の四魂の欠片集め〜」: https://sakasagaminoyura.github.io/yura-rpg/rpg/
- 横スクロール「結羅のぼうけん」: https://sakasagaminoyura.github.io/yura-rpg/boken/

本編：犬夜叉・かごめ討伐後、四魂の玉の欠片狩り。名前有りキャラは遭遇・討伐対象。

## フォルダ構成（デプロイ）

- `index.html` … トップのポータル（2つのゲームへの入口）
- `assets/portal/` … ポータル用サムネイル
- `rpg/index.html` … RPG本体（/workspace/yura-rpg の build-all-in-one.py で作る play.html をコピー）
- `boken/index.html` … 結羅のぼうけん（/workspace/yura-platformer/yura-platformer.html をそのままコピー）
- `favicon.ico`, `assets/favicon.png` … ルート用（RPG用は rpg/ にも同じものあり）

RPGの更新手順：`cd /workspace/yura-rpg && python3 build-all-in-one.py --deploy` → このリポジトリで commit / push。
**ルートの index.html に play.html をコピーしないこと**（ポータルが消えます）。
