## スマホナビ

## 概要
日本のフリマ市場で取引が行われているスマホの相場把握・比較・検索・自動査定が行える嬉しいサイトです。  
スマホを「高く売りたい！」または「安く買いたい！」人々にとって価値の高い情報を提供します。  

Vercelでサイト公開しています。**百聞は一見に如かず！** ぜひ一度ご覧ください。  
https://shindan-console.vercel.app/

* **スマホ機種別状態別にグラフ表示されます**
![image](https://user-images.githubusercontent.com/66734196/102046011-be24f980-3e1d-11eb-9b87-1be24ca28410.png)

* **フリマサイト横断で出品中の商品検索が可能です**
![image](https://user-images.githubusercontent.com/66734196/102046159-12c87480-3e1e-11eb-9b7d-92c8b849a637.png)


## 目的・プロダクト作成の背景
2020年3月にSIerを退職して以降にインプットした知識・技術をフル動員して「何か形にできないか」と考え作成したプロダクトです。  
ただ勉強した成果を形にして自己満足するのではなく、使い手にとって嬉しい・使いやすいプロダクト制作を心掛けました。  
このレポジトリを訪れた方へ、忌憚ないご意見をお待ちしております。  

## システムアーキテクチャ
* インフラはAWSで構築（VPC、 EC2、 RDS、 Lambda、 CroudWatch、 API Gateway）
* EC2インスタンス上でcronでPythonスクレイピングプログラムをスケジュール実行しRDS（MySQL）へデータ集積
* フロントエンドはReact.jsで開発

![アーキテクチャー](https://user-images.githubusercontent.com/66734196/102052767-efa3c200-3e29-11eb-8da9-b5eaa30b3606.png)

## 開発環境

フロントエンド
* React v17.0.1
* react-chartjs-2 v2.11.1

バックエンド
* python3.8

インフラ
* AWS lambda
* AWS API Gateway
* RDS（MySQL)

## 今後の拡張予定
* 機械学習による自動査定ロジックの追加 ★実装中 12月中リリース予定
* Reduxを用いたリファクタリング ★実装中 12月中リリース予定

* 検索項目の追加（金額、容量、SIMロック状態など）
* 昇順・降順の選択
* Amazon Forecastを用いた価格推移の未来予測

## ライセンス
MIT

