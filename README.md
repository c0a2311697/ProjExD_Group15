# 丸焼き豪華豚

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
主人公キャラクター豪華豚（ゴウカトン）をマウス操作により丸焼きにするゲームで，．．．

* 2人用のゲーム



## ゲームの遊び方
* 矢印キーで豪華豚を操作し，スペースキー押下によるバーナーで豪華豚を丸焼きにする
* 豪華豚が10秒以上バーナーにあぶられたら，ゲームオーバーとなる


* 

## ゲームの実装
### 共通基本機能
* 背景画像(コート)、プレイヤーの描画
* 2人用で実装
* ビームの発射
* 当たり判定：喜びエフェクト、捕まった時の
* （スタート画面）

### 担当追加機能
* CPUの参戦(担当：)：プレイヤー以外を描画するクラス
* バリアの追加(担当：)：指定キーを押下したときに自分の周りにバリアが発生
* チャージ切り札(担当：)：必殺技打つためのゲージと必殺技（玉が速くなる、相手コートに煙幕など）
* エネルギーの追加と表示(担当：)：ビームを打つためのエネルギーチャージ
* 体力の追加と体力ゲージの表示(担当：)

### ToDo
- [ ] ほげほげ機能
- [ ] ふがふが関数内の変数名の統一

### メモ
* クラス内の変数は，すべて，「get_変数名」という名前のメソッドを介してアクセスするように設計してある
* すべてのクラスに関係する関数は，クラスの外で定義してある


###  使うキー
####  プレイヤー1
* 矢印キー：移動
* 全矢印キーの同時押し：バリアの発動
* 右シフト：ビーム発射
* 右シフト長押しorビーム残量無し時の右シフト：ビームチャージ
* 右コントロール：必殺技


#### プレイヤー2
* WASD：移動
* WASDキーの同時押し：バリアの発動
* 左シフト：ビーム発射
* 左シフト長押しorビーム残量無し時の左シフト：ビームチャージ
* 左コントロール：必殺技
