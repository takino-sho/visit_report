

# [visit_report]

## サービス概要
訪問あんまマッサージ事業を運営する事業所が患者情報や職員情報の管理を行うことができ、事業所と職員間でスムーズに情報共有を行うことができるアプリケーション。

##　想定されるユーザー層
訪問あんまマッサージ事業の新規参入層

## サービスコンセプト
実際に働いた経験をもとに下記のような不便さを感じ、事業主の意見などをヒアリングし、その問題を解消したいと思ったため。
・職員：職員が患者の自宅に訪問を行うため、事業所で管理している患者情報の確認が必要な際にタイムリーに行えない。
・事業主：既存のアプリケーションでは導入費や月額費用が発生するため未だ導入に至っておらず、患者のスケジュール管理や情報などを複数のアプリを使用して行っており業務が煩雑になっているため、一つのアプリに集約したい。

矢野経済研究所の2022年の調査によると柔道整復・鍼灸・マッサージ市場規模は9,680億円であり、近年の在宅医療やフレイル予防への取り組みが進んでいることもあり市場規模はコロナウイルスの発症年を除けば、年々増加傾向にある。そのため新規参入も増加傾向にあると予想する。
https://www.yano.co.jp/press-release/show/press_id/3062#:~:text=2021%E5%B9%B4%E3%81%AF%E6%82%A3%E8%80%85%E6%95%B0,%E5%84%84%E5%86%86%E3%81%A8%E6%8E%A8%E8%A8%88%E3%81%97%E3%81%9F%E3%80%82

新規参入において苦労するのが患者の獲得であり、事業開始から黒字化になるまでに期間を要することがほとんどである。現在でも高機能のアプリは存在しているが、それにかかる導入費や月額利用料は決して安くはない。そのため、このアプリケーションにおいては可能な限りの機能を削ぎ落とし必要最低限にすることで無料で使用できるサービスを提供し、新規参入層が導入しやすいようにする。

## 実装を予定している機能
### MVP
⚫︎管理者ログイン、登録
⚫︎管理者画面
　・職員アカウントの作成、修正、削除
　・患者情報の入力（施術部位、住所、負担割合）、修正、削除
　・スケジュールの作成、修正、削除
　・スケジュール変更時の職員への通知　LINE Messaging API
　・患者宅間の距離の計算　Google Maps Platform

⚫︎職員ログイン
⚫︎職員画面
　・患者情報の確認（施術部位、住所）
　・患者ごとの請求金額の確認、受け取り金額の入力
　・スケジュールの確認、修正依頼

### その後の機能
　日報入力
　レセプト作成