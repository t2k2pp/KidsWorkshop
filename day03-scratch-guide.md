# Day 3: 衝突を検知しよう！

## やあ、プログラマー！

2日間の冒険お疲れさま！今日はもっとワクワクする機能を学ぶよ。キャラクター同士が触れ合ったときに何かが起こる「衝突検知」だ！これができるとゲームの幅がグンと広がるよ！

## 今日のミッション
**ネコが何かに触れたら反応するようにしよう！**

## 準備しよう
1. [Scratch](https://scratch.mit.edu/)のウェブサイトにログインしよう → https://scratch.mit.edu/
2. 昨日のプロジェクトを開くか、「作る」から新しいプロジェクトを始めよう
3. まず、ネコと触れるためのものが必要だね。新しいスプライト（キャラクター）を追加しよう！

## やってみよう！

### Step 1: 新しいスプライトを追加しよう
1. 画面右下の「スプライトを選ぶ」ボタン（+マークのついたアイコン）をクリックしよう
2. いろいろなキャラクターが表示されるから、好きなものを選んでクリックしよう（例えば「Apple」リンゴなど）
3. 新しいスプライトが画面上に表示されたね！これでネコと触れ合うものができたよ

### Step 2: ネコが他のスプライトに触れたことを検知しよう
1. ネコのスプライトをクリックして選択しよう
2. 「制御」カテゴリー（オレンジ色）をクリックしよう
3. 「もし〜なら」ブロックをスクリプトエリアにドラッグしよう
4. 「調べる」カテゴリー（水色）をクリックして、「○○に触れた」ブロックを見つけよう
5. このブロックを「もし〜なら」ブロックの六角形の部分にはめ込もう
6. 「○○」の部分をクリックして、追加したスプライト（例えばリンゴ）を選ぼう

### Step 3: 触れたときの反応を追加しよう
1. 「見た目」カテゴリー（紫色）から「こんにちは！と2秒言う」ブロックを見つけよう
2. これを「もし〜なら」ブロックの中に入れよう
3. 「こんにちは！」の部分をクリックして、「いただきます！」や「おいしそう！」など好きな言葉に変えよう
4. 「イベント」カテゴリーから「緑の旗が押されたとき」ブロックを取って、一番上につなげよう
5. 「制御」カテゴリーから「ずっと」ブロックを取って、「緑の旗が押されたとき」の下につなげよう
6. 「もし〜なら」ブロックを「ずっと」ブロックの中に入れよう

### Step 4: プログラムを動かしてみよう
1. 緑の旗をクリックしてプログラムを開始しよう
2. 矢印キーを使ってネコをリンゴに近づけて触れてみよう
3. ネコがリンゴに触れると、吹き出しでメッセージが表示されるね！

### Step 5: スコアを追加しよう
1. 「変数」カテゴリー（オレンジ赤色）をクリックしよう
2. 「変数を作る」ボタンをクリックしよう
3. 変数の名前を「スコア」にして「OK」をクリックしよう
4. 「スコア」という変数ブロックが作られたよ！
5. 「変数」カテゴリーから「スコアを0にする」ブロックを取って、「緑の旗が押されたとき」の下につなげよう
6. 「変数」カテゴリーから「スコアを(　)ずつ変える」ブロックを取って、「もし〜なら」ブロックの中の「いただきます！と2秒言う」の下につなげよう
7. 「スコアを(　)ずつ変える」の数値を「1」にしておこう

### Step 6: 触れたらスプライトを移動させよう
1. リンゴのスプライトをクリックして選択しよう
2. 「イベント」カテゴリーから「このスプライトが押されたとき」ブロックを取ろう
3. 「動き」カテゴリーから「x座標を(　)、y座標を(　)にする」ブロックを下につなげよう
4. x座標とy座標をランダムな数値に変えよう（例：x座標を「-200から200の乱数」、y座標を「-150から150の乱数」）
5. 「演算」カテゴリー（緑色）にある「(　)から(　)までの乱数」ブロックを使って入力しよう

### Step 7: ネコとリンゴが触れたときにもリンゴが移動するようにしよう
1. ネコのスプライトに戻ろう
2. 「調べる」カテゴリーから「○○へメッセージを送る」ブロックを見つけよう
3. これを「もし〜なら」ブロックの中の一番下（「スコアを1ずつ変える」の下）につなげよう
4. 「○○」の部分をクリックして、「message1」を選び、「新しいメッセージ」をクリックして「ゲット」という名前を付けよう
5. 次にリンゴのスプライトをクリックして選択しよう
6. 「イベント」カテゴリーから「ゲットを受け取ったとき」ブロックを取ろう
7. 「動き」カテゴリーから「x座標を(　)、y座標を(　)にする」ブロックを下につなげよう
8. さっきと同じように乱数を使って位置をランダムにしよう

## 今日のチャレンジ！
基本のプログラムができたら、次のチャレンジに挑戦してみよう：

1. リンゴを3つくらい増やしてみよう（スプライトを右クリックして「複製」を選ぶと簡単だよ）
2. リンゴを取ると効果音が鳴るようにしてみよう（「音」カテゴリーを使おう）
3. タイムリミットを追加してみよう（「変数」で「タイム」を作り、「制御」カテゴリーの「(　)秒待つ」ブロックを使おう）

## 考えてみよう！
- スコアが増えていくと、どんなゲームになるだろう？
- 触れると逃げるスプライトと、触れると追いかけてくるスプライトがあったら、どんなゲームができるかな？
- 「○○に触れた」以外の条件を使うとしたら、どんな条件が考えられるだろう？

## 今日のミッション達成チェック
□ 新しいスプライトを追加できた  
□ ネコが他のスプライトに触れたことを検知できた  
□ 触れたときにメッセージが表示されるようになった  
□ スコアを追加して、触れるたびに増えるようにした  
□ 触れたらスプライトが別の場所に移動するようにした  

## 困ったときは？
- スプライト同士が触れても反応しないときは、「もし〜なら」ブロックがきちんと「ずっと」ブロックの中に入っているか確認しよう
- スコアが増えないときは、「スコアを(　)ずつ変える」ブロックが正しい場所にあるか確認しよう
- リンゴが移動しないときは、メッセージの送受信が正しく設定されているか確認しよう

**明日のヒント**: 明日は、タイマーの使い方を学んで、制限時間のあるゲームを作るよ！どれだけ早くたくさんのリンゴを集められるか挑戦してみよう！
