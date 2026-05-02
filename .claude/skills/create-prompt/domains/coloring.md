# 色彩・配色

<!--
  ★ ここを変えると自分の絵柄が出ます ★

  以下の値はサンプル用のデフォルトです。そのままでも動きますが、
  自分の配色感覚を出すには「基本方針」「影色」のセクションを書き換えてください。
  色相バランスや「白背景禁止」などの構造ルールは変更しない方が安全です。
-->

## メタデータ
- priority: 7
- conflicts: []

## ルール

### 基本方針（サンプルのデフォルト・自分の配色感覚に書き換え可能）
- 彩度を意図的に抑えることは目的にしない
- 色は十分な存在感を持たせ、画面内で生きている状態を優先する
- 鮮やかさは「強弱」や「密度」で制御し、彩度そのものを一律に下げない
- 白飛びや過剰な発光表現による色抜けは避ける
- 色は整理されていても、無難にまとまりすぎない配色を許容する

### 色面による空間成立（共通骨格）
- 明度差だけでなく、色相差によって形が認識できること
- 線がなくても、色面だけで大まかな構造が読み取れること
- 配色が決まらない場合は、彩度を下げる方向ではなく色層を増やす方向で調整する
- 色面が先に認識され、その上に線が補助的に存在する構成を維持する

### 色相バランス（共通骨格）

#### 面積比
- 主色 約60%
- 隣接色 約25%
- 補色アクセント 10〜15%
- それ以上の分散禁止

#### 彩度
- 背景は主役より低彩度
- 最高彩度は焦点周辺のみ
- 全体高彩度禁止

### 影色（サンプルのデフォルト・自分の感覚に書き換え可能）
- 影は隣接または補色を微量混合
- 単色影禁止
- 影色は「その物の色を暗くしたもの」として扱わず、別の色相がわずかに混ざった状態として解釈してよい
- 髪の影に黄緑、灰紫、くすんだ青などが微量に混ざってよい
- 服や小物の影にも周囲の空気色が侵食することを許容する

### 配色語の解釈ルール
- 「落ち着いた」「穏やか」「暖色寄り」などの表現は、彩度を下げる・色数を減らす指示として解釈しない
- 落ち着きは「彩度の低下」ではなく、色相差・明度差・密度差の整理によって表現する
- 暖色寄りでも、寒色や中間色を補助色として必ず画面内に含める

### 禁止事項（共通骨格・変更しない）
- 無彩色のみの配色は禁止
- 白背景は禁止
- 色面で空間が成立する前提を保つ

### 統合プロンプトへの必須追加文
プロンプト生成時に以下を必ず含める：
- color harmony controlled by dominant hue with adjacent support and limited complementary accent
- dominant hue covering majority area
- secondary hue supporting without equal saturation
- small complementary accent restricted to focal zone
- background saturation lower than subject

## キーワード
- 推奨: layered colors, color-defined forms, chromatic depth, visible color planes, shadow mixed with secondary hue
- 回避: monochrome, desaturated, white background, flat color, uniform digital shading

## 例
- 良い例: "forms defined by overlapping warm and cool color planes, shadow mixed with muted orange into teal-based forms, color harmony controlled by dominant hue with adjacent support and limited complementary accent"
- 悪い例: "simple flat colors on white background"、"shadows are just darker versions of base color"
