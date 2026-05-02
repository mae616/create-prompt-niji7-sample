# 絵画的質感・画材表現

<!--
  ★ ここを変えると自分の絵柄が出ます ★

  以下の値はサンプル用のデフォルトです。そのままでも動きますが、
  自分の画材・質感を出すには「絵画的質感」「着彩スタイル」のセクションを書き換えてください。
  画材ブロック・技法ブロックの「形式」は変更しない方が安全です。
-->

## メタデータ
- priority: 7
- conflicts: []

## ルール

### 絵画的質感の基本（サンプルのデフォルト・自分の方向性に書き換え可能）
- にじみ、塗りムラ、筆致、かすれを積極的に残す
- 制作過程が感じられる画面構成を優先する
- すべてを整えすぎず、わずかな未完成さを許容する
- 完成度よりも「描いている途中の勢いが残っている」印象を優先する

### 着彩スタイル（サンプルのデフォルト・自分の好みに書き換え可能）
- 水彩的なにじみ、滲出、透明感をベースにする
- その上から、不透明色や強い筆跡を部分的に重ねる
- すべてを均一なタッチで仕上げない
- 筆跡、かすれ、塗りムラ、簡略化された描画を積極的に許容する

### 色層構造（共通骨格）
- 一色で均一に塗らず、複数の色層を重ねて深みを作る
- 透明な色の重なり、不透明色の差し込みによって彩度が自然に揺らいで見える状態を目指す
- 透明層＋不透明層を重ねる
- 均一塗り禁止
- 筆致を残す

### 強弱と余白（共通骨格）
- 線・色・筆致には必ず意図的な強弱を与える
- すべてを均一な完成度に整えない
- 一部に未整理・未完成・曖昧さが残ることを許容する
- 強弱は「技法として目立つ」状態にならないよう制御する
- 色のメリハリはコントラストではなく層の重なりで表現する

### 画材ブロック生成規則（共通骨格・形式は変更しない）
画材は必ず以下形式で出力：
```
[painting medium], visually interpreted as [physical behavior]
```

例：
- gouache painting, visually interpreted as matte opaque pigment layers with visible brush drag
- mineral pigment ink wash, visually interpreted as granulating particles and uneven absorption
- oil pastel, visually interpreted as waxy pigment buildup with edge breakage
- dry pigment wash, visually interpreted as powdery edge diffusion

禁止：
- "digital art" 単体使用
- style名のみの記述

### 技法ブロック生成規則（共通骨格・形式は変更しない）
技法は必ず以下形式で出力：
```
[technique term], defined as [visual construction behavior]
```

例：
- scumbling, defined as semi-dry pigment dragged across raised texture
- wet-on-dry layering, defined as transparent stain over fully dried base
- broken color layering, defined as adjacent strokes of different hues without blending

## キーワード
- 質感系: visible brushstrokes, watercolor bleeding, paint texture, uneven pigment
- 画材系: gouache, mineral pigment ink wash, oil pastel, dry pigment wash
- 技法系: scumbling, wet-on-dry layering, broken color layering
- 回避: digital art（単体）, smooth rendering, airbrushed, clean finish, paper texture, paper grain, textured paper, canvas texture

## 例
- 良い例: "gouache painting, visually interpreted as matte opaque pigment layers with visible brush drag, scumbling, defined as semi-dry pigment dragged across underlying color layer"
- 悪い例: "digital painting"（具体性なし）、"smooth airbrushed render"（均一デジタル処理）
