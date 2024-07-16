# HADO★kokaton!!

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
* ドッジボールを基盤とした2人用の対戦ゲーム

## ゲームの遊び方
* 指定キーで操作し，ビームやバリアを駆使して相手を倒す
* 体力が0になったら，ゲームオーバーとなる

## ゲームの実装
### 共通基本機能
* 背景画像(コート)、プレイヤーの描画
* 2人用で実装
* ビームの発射
* 当たり判定：喜びエフェクト、捕まった時の
* （スタート画面）

### 担当追加機能
#### 【】内はブランチ名
* 【CPU】CPUの参戦(担当：宮島)：プレイヤー以外を描画するクラス
* 【barrier】バリアの追加(担当：古賀)：指定キーを押下したときに自分の周りにバリアが発生
* 【skill】チャージ切り札(担当：秦)：必殺技打つためのゲージと必殺技（玉が速くなる、相手コートに煙幕など）
* 【energy】エネルギーの追加と表示(担当：岩永)：ビームを打つためのエネルギーチャージ
* 【HP】体力の追加と体力ゲージの表示(担当：高野)

### ToDo
- [ ] 
- [ ] 全体の変数名の統一

### メモ
* プレイヤーそれぞれにビーム(Beamクラス)、コート内にいるかの判定(check_bound_playerクラス)、キャラクターの描画(Charaクラス)を作っているので確認してください！ 

  
### 使うキー
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