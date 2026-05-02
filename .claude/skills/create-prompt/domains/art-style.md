# 画風・線質・色面構造

<!--
  ★ ここを変えると自分の絵柄が出ます ★

  以下の値はサンプル用のデフォルトです。そのままでも動きますが、
  自分の絵柄を出すには「線質」「色面構造」のセクションを書き換えてください。
  共通骨格（純黒禁止・線色条件など）は変更しない方が安全です。
-->

## メタデータ
- priority: 8
- conflicts: []

## ルール

### 画風決定の原則（共通骨格・変更しない）
- 画風は「塗り方」「線の扱い」「描画密度の配分」の3点で構成する
- 画風・塗り・線質・色層構造を最優先で決定する（他の要素より先に決める）
- 入力情報の世界観・キャラクター設定は「素材・形状・色相傾向」として扱う
- ジャンル連想に引きずられず、常にこのカプセルの画風を最優先する

### 線質（サンプルのデフォルト・自分の絵柄に書き換え可能）
- 線は鉛筆で軽く描かれたような、柔らかく控えめな質感として扱う
- 濃さは一定にせず、筆圧の弱い揺れや擦れがわずかに残る程度に留める
- 線は形を決定する主役ではなく、形を読み取りやすくするための補助情報
- 輪郭を強く囲わず、必要な箇所にだけ線が現れる構成を基本とする
- 線は色面の上に浮かず、色の層に部分的に溶け込んでいる前提で扱う

### 線構造（共通骨格・変更しない）

#### 線の存在条件
- 線は接触部と重なり部のみに発生
- 単独の外周輪郭線禁止
- 髪外周に連続線を使わない

#### 線の色条件
- 線色は局所色より5〜15%暗い色
- 純黒禁止
- 線色は環境光に同化させる

#### 線の太さ条件
- 均一線幅禁止
- 始点と終点を細く

#### 背景の線
- 背景に線を使わない
- 背景は面のみで成立

### 線と色の主従関係
- 線画は補助的な構造情報であり、主役は常に色面と色層
- 色の塊が、線よりも先に視認される構成を保つ

### 色面構造（共通骨格・変更しない）
- 輪郭ではなく、色相差と明度差で形を成立させる
- 顔は色相遷移と明度遷移で構築する
- 線は補助的役割のみ
- 色の境界でエッジを示す

## キーワード
- 線質系: soft pencil-like strokes, subtle line variation, lines partially dissolving into color layers, no pure black outlines, lines only at contact and overlap points
- 色面構造: color-plane based composition, forms constructed by hue and value contrast rather than outlines, face defined by hue transitions and soft value shifts, lines are supportive only
- 必須禁止: no heavy outlines, no pure black lines, no uniform digital shading

## 例
- 良い例: "soft irregular outlines in muted warm gray appearing only at contact points, partially blending into adjacent color areas, hair silhouette broken by color variation instead of line enclosure"
- 悪い例: "bold black outlines"（純黒・強い輪郭は禁止）、"clean digital lineart"（均一デジタル線禁止）
