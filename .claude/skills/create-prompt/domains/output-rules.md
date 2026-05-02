# 出力規則（プロンプト合成の最上位ルール）

## メタデータ
- priority: 10
- conflicts: []

## ルール

### 対象エンジン
- nijijourney v7 / midjourney v7

### 基本姿勢
- プロンプトは語義・構造・視覚定義の粒度で忠実に解釈される前提で扱う
- 曖昧な雰囲気語・慣用的ジャンル語に依存しない
- 形・比率・線の役割・色層・質感・情報密度といった、視覚的に解釈可能な要素へ分解して記述する

### 優先順位（絶対）
1. 画風成立
2. 主役の視認性
3. 配色成立
4. 構造維持
5. 情報再現

入力情報よりも、画面としての成立を常に優先する。

### 概念語・ジャンル語の扱い
概念語は単体では使用しない。使用する場合：
```
[concept term], defined as [visual description]
または
[concept term], visually interpreted as [visual description]
```
概念語は補助であり、主役は必ず visual description 側とする。

### プロンプト出力形式
- プロンプトは英語で出力（主）
- 各文はカンマ区切りのフレーズ列
- 1フレーズ＝1視覚的意図
- 意味衝突・過剰形容を避ける
- 英語プロンプトの後に日本語訳を併記する

### プロンプト優先順（固定）
1. 主役物理定義
2. 焦点物体
3. 髪
4. 目
5. 肌
6. 衣装層
7. ポーズ＋カメラ位置
8. 光
9. 画材
10. 技法
11. 色面構造
12. 影色混合
13. 背景
14. 密度差
15. 線の役割
16. 禁止要素

### 禁止ブロック（統合プロンプト末尾に必ず付与）
- no photorealism
- no heavy outlines
- no pure black lines
- no uniform digital shading

### 空間の明示
- 具体的な空間タイプを必ず一つ指定する
- 時間帯または光条件を必ず一つ指定する
- 空間は色面と奥行きとして成立させる

### 表現全体の前提
- 写真、写実、フォトリアルな描写は明確に避ける
- 紙・キャンバスの物理的質感は出さない（色の効果は使ってよい）
- すべての出力は「最初から描かれたイラスト」として成立させる

## キーワード
- 使用禁止: photo, realistic, photorealistic, hyper-realistic, 3D render, digital art（単体）, paper texture, paper grain
- 推奨: illustration, painted, drawn, depicted
- 必須末尾: no photorealism, no heavy outlines, no pure black lines, no uniform digital shading

### 主語先頭安定テンプレ
```
[physical subject definition],
[focal object or material],
[hair description],
[eye description],
[skin description],
[layered clothing structure],
[pose + camera position],
[lighting definition],
[painting medium visually interpreted as …],
[technique defined as …],
[color-plane structure],
[shadow mixed with secondary hue],
[background space type],
[density contrast],
[line role clarification],
[color harmony block],
[prohibition block]
```
